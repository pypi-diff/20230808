# Comparing `tmp/thipster-0.23.7.tar.gz` & `tmp/thipster-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.7.tar", last modified: Mon Aug  7 06:48:34 2023, max compression
+gzip compressed data, was "thipster-0.23.8.tar", last modified: Tue Aug  8 12:10:24 2023, max compression
```

## Comparing `thipster-0.23.7.tar` & `thipster-0.23.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-07 06:48:16.000000 thipster-0.23.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 06:48:16.000000 thipster-0.23.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-07 06:48:34.552600 thipster-0.23.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-07 06:48:16.000000 thipster-0.23.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 06:48:16.000000 thipster-0.23.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 06:48:16.000000 thipster-0.23.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:48:34.552600 thipster-0.23.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-07 06:48:17.000000 thipster-0.23.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_parsedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_parserfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_github_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_local_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_resourcemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/thipster/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/auth/google.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/parsed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/parser_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/cdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/thipster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-08 12:10:04.000000 thipster-0.23.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 12:10:04.000000 thipster-0.23.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:10:24.930824 thipster-0.23.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-08 12:10:04.000000 thipster-0.23.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 12:10:04.000000 thipster-0.23.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 12:10:04.000000 thipster-0.23.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:10:24.934824 thipster-0.23.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 12:10:05.000000 thipster-0.23.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.918823 thipster-0.23.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_parsedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_parserfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_github_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/thipster/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/auth/google.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/parsed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/cdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.7/LICENSE` & `thipster-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/PKG-INFO` & `thipster-0.23.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.7
+Version: 0.23.8
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,17 @@
   </a>
   <a href="https://pypi.org/project/thipster/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipster?color=brightgreen" alt="Supported Python versions">
   </a>
   <a href="https://github.com/astral-sh/ruff">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
   </a>
+  <a href='https://coveralls.io/github/THipster/THipster'>
+    <img src='https://coveralls.io/repos/github/THipster/THipster/badge.svg' alt='Coverage Status' />
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
 THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.8 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -11,15 +11,15 @@
 doc Provides-Extra: google Provides-Extra: dev License-File: LICENSE # THipster
 THipster is a tool dedicated to simplifying the difficulty associated with
 writing Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                               versions] [Ruff]
+                      versions] [Ruff] [Coverage_Status]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
 more details. ## Dependencies In order to user THipster, you will need to have
 the following installed: - [Python](https://www.python.org/downloads/) (3.11+)
```

### Comparing `thipster-0.23.7/README.md` & `thipster-0.23.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
   </a>
   <a href="https://pypi.org/project/thipster/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipster?color=brightgreen" alt="Supported Python versions">
   </a>
   <a href="https://github.com/astral-sh/ruff">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
   </a>
+  <a href='https://coveralls.io/github/THipster/THipster'>
+    <img src='https://coveralls.io/repos/github/THipster/THipster/badge.svg' alt='Coverage Status' />
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
 THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # THipster THipster is a tool dedicated to simplifying the difficulty
 associated with writing Terraform files. It allows users to write
 infrastructure as code in a simplified format, using either YAML (with JINJA)
 or the dedicated Thipster DSL. Written entirely in Python, it leverages the
 Python CDK for Terraform to create Terraform files and apply them to the chosen
 provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                               versions] [Ruff]
+                      versions] [Ruff] [Coverage_Status]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
 more details. ## Dependencies In order to user THipster, you will need to have
 the following installed: - [Python](https://www.python.org/downloads/) (3.11+)
```

### Comparing `thipster-0.23.7/pyproject.toml` & `thipster-0.23.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/setup.py` & `thipster-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.7'
+__version__ = '0.23.8'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.7/tests/engine/test_engine.py` & `thipster-0.23.8/tests/engine/test_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Basic tests for the engine module functions."""
 
 import pytest
 
 import thipster.engine as eng
+from thipster.engine.exceptions import BadPortError
 from thipster.engine.parsed_file import ParsedFile
 from thipster.engine.resource_model import ResourceModel
 
 test_file = 'test.file'
 
 
 def logger(name: str):
@@ -136,7 +137,39 @@
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
 
     with pytest.raises(MockError):
         engine = eng.Engine(parser, repository, auth, terraform)
         engine.run(test_file)
+
+
+def test_engine_setters():
+    """Test the behavior of the engine setters when they fail."""
+    parser = MockParser()
+    repository = MockRepository()
+    auth = MockAuth()
+    terraform = MockTerraform()
+
+    with pytest.raises(BadPortError) as exc_info:
+        eng.Engine(None, repository, auth, terraform)
+
+    assert str(exc_info.value) == 'Error while setting THipster port : got NoneType, \
+expected ParserPort'
+
+    with pytest.raises(BadPortError) as exc_info:
+        eng.Engine(parser, None, auth, terraform)
+
+    assert str(exc_info.value) == 'Error while setting THipster port : got NoneType, \
+expected RepositoryPort'
+
+    with pytest.raises(BadPortError) as exc_info:
+        eng.Engine(parser, repository, None, terraform)
+
+    assert str(exc_info.value) == 'Error while setting THipster port : got NoneType, \
+expected AuthPort'
+
+    with pytest.raises(BadPortError) as exc_info:
+        eng.Engine(parser, repository, auth, None)
+
+    assert str(exc_info.value) == 'Error while setting THipster port : got NoneType, \
+expected TerraformPort'
```

### Comparing `thipster-0.23.7/tests/engine/test_generation.py` & `thipster-0.23.8/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.8/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.8/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.8/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.8/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.8/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/test_parsedfile.py` & `thipster-0.23.8/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/test_parserfactory.py` & `thipster-0.23.8/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/parser/test_yamlparser.py` & `thipster-0.23.8/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/repository/test_github_repository.py` & `thipster-0.23.8/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/repository/test_local_repository.py` & `thipster-0.23.8/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/repository/test_resourcemodel.py` & `thipster-0.23.8/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/test_e2e.py` & `thipster-0.23.8/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/tests/test_tools.py` & `thipster-0.23.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/auth/google.py` & `thipster-0.23.8/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/engine/engine.py` & `thipster-0.23.8/thipster/engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Engine.py module."""
 from pathlib import Path
 
 import thipster.engine.parsed_file as pf
 
+from .exceptions import BadPortError
 from .i_auth import AuthPort
 from .i_parser import ParserPort
 from .i_repository import RepositoryPort
 from .i_terraform import TerraformPort
 from .resource_model import ResourceModel
 
 terraform_plan_file = 'thipster.tfplan'
@@ -16,18 +17,18 @@
     """THipster's Engine.
 
     The core of the application, it is used to call and link all
     interfaces together.
     """
 
     def __init__(
-            self, parser: ParserPort,
-            repository: RepositoryPort,
-            auth: AuthPort,
-            terraform:  TerraformPort,
+            self, parser: ParserPort = None,
+            repository: RepositoryPort = None,
+            auth: AuthPort = None,
+            terraform:  TerraformPort = None,
     ):
         """THipster's Engine.
 
         The core of the application, it is used to call and link all
         interfaces together.
 
         Parameters
@@ -37,64 +38,72 @@
         repository : RepositoryPort
             Instance of a Respository class
         auth : AuthPort
             Instance of an Auth class
         terraform : TerraformPort
             Instance of a Terraform class
         """
-        self.__parser = parser
-        self.__repository = repository
-        self.__auth = auth
-        self.__terraform = terraform
+        self.parser = parser
+        self.repository = repository
+        self.auth = auth
+        self.terraform = terraform
 
     @property
     def parser(self):
         """Get the parser."""
-        return self.__parser
+        if self.__parser:
+            return self.__parser
+        raise NotImplementedError
 
     @parser.setter
     def parser(self, value):
         if not isinstance(value, ParserPort):
-            raise Exception
+            raise BadPortError(value.__class__, ParserPort)
 
         self.__parser = value
 
     @property
     def repository(self):
         """Get the repository."""
-        return self.__repository
+        if self.__repository:
+            return self.__repository
+        raise NotImplementedError
 
     @repository.setter
     def repository(self, value):
         if not isinstance(value, RepositoryPort):
-            raise Exception
+            raise BadPortError(value.__class__, RepositoryPort)
 
         self.__repository = value
 
     @property
     def auth(self):
         """Get the authentification module."""
-        return self.__auth
+        if self.__auth:
+            return self.__auth
+        raise NotImplementedError
 
     @auth.setter
     def auth(self, value):
         if not isinstance(value, AuthPort):
-            raise Exception
+            raise BadPortError(value.__class__, AuthPort)
 
         self.__auth = value
 
     @property
     def terraform(self):
         """Get the Terraform module."""
-        return self.__terraform
+        if self.__terraform:
+            return self.__terraform
+        raise NotImplementedError
 
     @terraform.setter
     def terraform(self, value):
         if not isinstance(value, TerraformPort):
-            raise Exception
+            raise BadPortError(value.__class__, TerraformPort)
 
         self.__terraform = value
 
     def run(self, path: str) -> str:
         """Return json Terraform files from the input file name.
 
         Calls the different run methods of the parser, repository,
@@ -140,15 +149,15 @@
             The path of the files to be processed
 
         Returns
         -------
         pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         """
-        parsed_file = self.__parser.run(path)
+        parsed_file = self.parser.run(path)
         assert type(parsed_file) == pf.ParsedFile
 
         return parsed_file
 
     def get_models(
         self, file: pf.ParsedFile,
     ) -> dict[str, ResourceModel]:
@@ -161,29 +170,29 @@
 
         Returns
         -------
         dict[str, ResourceModel]
             The dictionary of models
         """
         types = [r.resource_type for r in file.resources]
-        return self.__repository.get(types)
+        return self.repository.get(types)
 
     def generate_tf_files(
         self, file: pf.ParsedFile, models: dict[str, ResourceModel],
     ) -> None:
         """Generate Terraform files.
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         models : dict[str, ResourceModel]
             The dictionary of models
         """
-        self.__terraform.generate(file, models, self.__auth)
+        self.terraform.generate(file, models, self.__auth)
 
     def init_terraform(
         self,
         working_dir: Path = Path.cwd(),
         upgrade: bool = False,
     ) -> tuple[int, str]:
         """Initialize Terraform.
@@ -196,15 +205,15 @@
             Whether to upgrade the Terraform providers, by default False
 
         Returns
         -------
         tuple[int, str]
             The terraform init exit code and output
         """
-        return self.__terraform.init(working_dir, upgrade)
+        return self.terraform.init(working_dir, upgrade)
 
     def plan_terraform(
         self,
         working_dir: Path = Path.cwd(),
         plan_file_path: str = terraform_plan_file,
     ) -> tuple[int, str]:
         """Plan Terraform.
@@ -217,15 +226,15 @@
             The path of the plan file, by default thipster.tfplan
 
         Returns
         -------
         tuple[int, str]
             The terraform plan exit code and output
         """
-        return self.__terraform.plan(working_dir, plan_file_path)
+        return self.terraform.plan(working_dir, plan_file_path)
 
     def apply_terraform(
         self,
         working_dir: Path = Path.cwd(),
         plan_file_path: str = terraform_plan_file,
     ) -> tuple[int, str]:
         """Apply Terraform.
@@ -238,8 +247,8 @@
             The path of the plan file, by default thipster.tfplan
 
         Returns
         -------
         tuple[int, str]
             The terraform apply exit code and output
         """
-        return self.__terraform.apply(working_dir, plan_file_path)
+        return self.terraform.apply(working_dir, plan_file_path)
```

### Comparing `thipster-0.23.7/thipster/engine/i_parser.py` & `thipster-0.23.8/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/engine/i_repository.py` & `thipster-0.23.8/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/engine/i_terraform.py` & `thipster-0.23.8/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/engine/parsed_file.py` & `thipster-0.23.8/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/engine/resource_model.py` & `thipster-0.23.8/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/helpers.py` & `thipster-0.23.8/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.8/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.8/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.8/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.8/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.8/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.8/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/token.py` & `thipster-0.23.8/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.8/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/exceptions.py` & `thipster-0.23.8/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/parser_factory.py` & `thipster-0.23.8/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/parser/yaml_parser.py` & `thipster-0.23.8/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/repository/exceptions.py` & `thipster-0.23.8/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/repository/github.py` & `thipster-0.23.8/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/repository/json.py` & `thipster-0.23.8/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/repository/local.py` & `thipster-0.23.8/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/terraform/cdk.py` & `thipster-0.23.8/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster/terraform/exceptions.py` & `thipster-0.23.8/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.7/thipster.egg-info/PKG-INFO` & `thipster-0.23.8/thipster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.7
+Version: 0.23.8
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,17 @@
   </a>
   <a href="https://pypi.org/project/thipster/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipster?color=brightgreen" alt="Supported Python versions">
   </a>
   <a href="https://github.com/astral-sh/ruff">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
   </a>
+  <a href='https://coveralls.io/github/THipster/THipster'>
+    <img src='https://coveralls.io/repos/github/THipster/THipster/badge.svg' alt='Coverage Status' />
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
 THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.8 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -11,15 +11,15 @@
 doc Provides-Extra: google Provides-Extra: dev License-File: LICENSE # THipster
 THipster is a tool dedicated to simplifying the difficulty associated with
 writing Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                               versions] [Ruff]
+                      versions] [Ruff] [Coverage_Status]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
 more details. ## Dependencies In order to user THipster, you will need to have
 the following installed: - [Python](https://www.python.org/downloads/) (3.11+)
```

### Comparing `thipster-0.23.7/thipster.egg-info/SOURCES.txt` & `thipster-0.23.8/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

