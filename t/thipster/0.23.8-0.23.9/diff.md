# Comparing `tmp/thipster-0.23.8.tar.gz` & `tmp/thipster-0.23.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.8.tar", last modified: Tue Aug  8 12:10:24 2023, max compression
+gzip compressed data, was "thipster-0.23.9.tar", last modified: Tue Aug  8 12:27:18 2023, max compression
```

## Comparing `thipster-0.23.8.tar` & `thipster-0.23.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-08 12:10:04.000000 thipster-0.23.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 12:10:04.000000 thipster-0.23.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:10:24.930824 thipster-0.23.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-08 12:10:04.000000 thipster-0.23.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 12:10:04.000000 thipster-0.23.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 12:10:04.000000 thipster-0.23.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:10:24.934824 thipster-0.23.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 12:10:05.000000 thipster-0.23.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.918823 thipster-0.23.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/engine/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_parsedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_parserfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_github_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_local_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/repository/test_resourcemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-08 12:10:04.000000 thipster-0.23.8/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.922824 thipster-0.23.8/thipster/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/auth/google.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/i_terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/parsed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/engine/resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/parser_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/repository/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.930824 thipster-0.23.8/thipster/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/cdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-08 12:10:04.000000 thipster-0.23.8/thipster/terraform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:24.926823 thipster-0.23.8/thipster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 12:10:24.000000 thipster-0.23.8/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.590634 thipster-0.23.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-08 12:27:02.000000 thipster-0.23.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 12:27:02.000000 thipster-0.23.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:27:18.590634 thipster-0.23.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-08 12:27:02.000000 thipster-0.23.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 12:27:02.000000 thipster-0.23.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 12:27:02.000000 thipster-0.23.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:27:18.590634 thipster-0.23.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 12:27:03.000000 thipster-0.23.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.570634 thipster-0.23.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.574634 thipster-0.23.9/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/engine/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.574634 thipster-0.23.9/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.574634 thipster-0.23.9/tests/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/test_parsedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/test_parserfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.574634 thipster-0.23.9/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/repository/test_github_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/repository/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-08 12:27:02.000000 thipster-0.23.9/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.574634 thipster-0.23.9/thipster/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.578634 thipster-0.23.9/thipster/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/auth/google.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.582634 thipster-0.23.9/thipster/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/i_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/i_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/i_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/i_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/parsed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/engine/resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.582634 thipster-0.23.9/thipster/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.586634 thipster-0.23.9/thipster/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24358 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.586634 thipster-0.23.9/thipster/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/repository/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/repository/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/repository/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.590634 thipster-0.23.9/thipster/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/terraform/cdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-08 12:27:02.000000 thipster-0.23.9/thipster/terraform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:18.578634 thipster-0.23.9/thipster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 12:27:18.000000 thipster-0.23.9/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-08 12:27:18.000000 thipster-0.23.9/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:27:18.000000 thipster-0.23.9/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-08 12:27:18.000000 thipster-0.23.9/thipster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 12:27:18.000000 thipster-0.23.9/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.8/LICENSE` & `thipster-0.23.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/PKG-INFO` & `thipster-0.23.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.8
+Version: 0.23.9
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.8 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.9 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.8/README.md` & `thipster-0.23.9/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/pyproject.toml` & `thipster-0.23.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/setup.py` & `thipster-0.23.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.8'
+__version__ = '0.23.9'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.8/tests/engine/test_engine.py` & `thipster-0.23.9/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/engine/test_generation.py` & `thipster-0.23.9/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.9/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.9/tests/parser/dsl_parser/test_dslparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,25 +100,24 @@
 
 
 def test_parse_simple_file_with_newlines():
     """Test the parsing of a simple file with newlines."""
     out = __test_file(
         file="""
 
-bucket my-bucket:
+bucket    my-bucket:
 
-
-\tregion: euw
+\tregion:   euw
 
 bucket my-bucket2:
 \tregion: euw
 
 
 
-""",
+   """,
     )
     assert len(out.resources) == 2
     for bucket in out.resources:
         assert bucket.resource_type == 'bucket'
         assert 'my-bucket' in bucket.name
         assert len(bucket.attributes) == 1
```

### Comparing `thipster-0.23.8/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.9/tests/parser/dsl_parser/test_lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,16 @@
     line_value, column_value = 1, len(input_string)+1
     if is_newline:
         line_value, column_value = 2, 1
     expected_output = [
         __get_token_string(test_file_name, 1, 1, token, token_value),
         __get_token_string(
             test_file_name, line_value,
-            column_value, TT.NEWLINE,
+            column_value, TT.EOF,
         ),
-        __get_token_string(test_file_name, line_value+1, 1, TT.EOF),
     ]
     lexer = Lexer({test_file_name: input_string})
     lexer.run()
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -102,16 +101,15 @@
     """Test the lexing of brackets."""
     lexer = Lexer({'': ''})
     input_string = '[toto]'
     expected_output = [
         __get_token_string('file', 1, 1, TT.BRACKETS_START),
         __get_token_string('file', 1, 2, TT.STRING, 'toto'),
         __get_token_string('file', 1, 6, TT.BRACKETS_END),
-        __get_token_string('file', 1, 7, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 7, TT.EOF),
     ]
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
@@ -121,58 +119,54 @@
     """Test the lexing of quoted strings."""
     lexer = Lexer({'': ''})
 
     input_string = '"bucket number 21""bucket number 22"'
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number 21'),
         __get_token_string('file', 1, 20, TT.STRING, 'bucket number 22'),
-        __get_token_string('file', 1, 37, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 37, TT.EOF),
     ]
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
     input_string = "'bucket number 21'"
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number 21'),
-        __get_token_string('file', 1, 19, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 19, TT.EOF),
     ]
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
     input_string = "'bucket number \"21\"'"
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number "21"'),
-        __get_token_string('file', 1, 21, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 21, TT.EOF),
     ]
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
     input_string = '"bucket number \'21\'"'
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, "bucket number '21'"),
-        __get_token_string('file', 1, 21, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 21, TT.EOF),
     ]
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
@@ -194,16 +188,15 @@
         'file': 'bucket nom\\\ntest:',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nomtest'),
         __get_token_string('file', 2, 5, TT.COLON),
-        __get_token_string('file', 2, 6, TT.NEWLINE),
-        __get_token_string('file', 3, 1, TT.EOF),
+        __get_token_string('file', 2, 6, TT.EOF),
     ]
     lexer = Lexer(input_file)
     lexer.run()
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -211,16 +204,15 @@
 
 
 def test_lex_var():
     """Test the lexing of a variable."""
     input_string = '#variable'
     expected_output = [
         __get_token_string('file', 1, 2, TT.VAR, 'variable'),
-        __get_token_string('file', 1, 10, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 10, TT.EOF),
     ]
     lexer = Lexer({'': ''})
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -237,16 +229,15 @@
     input_file = {
         'file': '  \n\t',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.TAB),
         __get_token_string('file', 1, 3, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
-        __get_token_string('file', 2, 2, TT.NEWLINE),
-        __get_token_string('file', 3, 1, TT.EOF),
+        __get_token_string('file', 2, 2, TT.EOF),
     ]
     lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
@@ -258,16 +249,15 @@
         'file': '    \n\t',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.TAB),
         __get_token_string('file', 1, 3, TT.TAB),
         __get_token_string('file', 1, 5, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
-        __get_token_string('file', 2, 2, TT.NEWLINE),
-        __get_token_string('file', 3, 1, TT.EOF),
+        __get_token_string('file', 2, 2, TT.EOF),
     ]
     lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
@@ -275,16 +265,15 @@
 
 def test_lex_amount():
     """Test the lexing of an amount."""
     input_string = 'amount '
     expected_output = [
         __get_token_string('file', 1, 1, TT.AMOUNT),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
-        __get_token_string('file', 1, 8, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 8, TT.EOF),
     ]
     lexer = Lexer({'': ''})
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -298,16 +287,15 @@
         __get_token_string('file', 1, 1, TT.IF),
         __get_token_string('file', 1, 3, TT.WHITESPACE),
         __get_token_string('file', 1, 4, TT.STRING, 'condition'),
         __get_token_string('file', 1, 13, TT.WHITESPACE),
         __get_token_string('file', 1, 14, TT.ELSE),
         __get_token_string('file', 1, 18, TT.WHITESPACE),
         __get_token_string('file', 1, 19, TT.STRING, 'something'),
-        __get_token_string('file', 1, 28, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 28, TT.EOF),
     ]
     lexer = Lexer({'': ''})
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -319,16 +307,15 @@
     input_string = 'bucket nom-8'
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nom'),
         __get_token_string('file', 1, 11, TT.MINUS),
         __get_token_string('file', 1, 12, TT.INT, 8),
-        __get_token_string('file', 1, 13, TT.NEWLINE),
-        __get_token_string('file', 2, 1, TT.EOF),
+        __get_token_string('file', 1, 13, TT.EOF),
     ]
     lexer = Lexer({'': ''})
     lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
@@ -352,16 +339,15 @@
         __get_token_string('file', 1, 15, TT.AMOUNT),
         __get_token_string('file', 1, 21, TT.COLON),
         __get_token_string('file', 1, 22, TT.WHITESPACE),
         __get_token_string('file', 1, 23, TT.INT, '5'),
         __get_token_string('file', 1, 24, TT.WHITESPACE),
         __get_token_string('file', 1, 25, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
-        __get_token_string('file', 2, 2, TT.NEWLINE),
-        __get_token_string('file', 3, 1, TT.EOF),
+        __get_token_string('file', 2, 2, TT.EOF),
 
         __get_token_string('file2', 1, 1, TT.STRING, 'network'),
         __get_token_string('file2', 1, 8, TT.WHITESPACE),
         __get_token_string('file2', 1, 9, TT.STRING, 'aaaa'),
         __get_token_string('file2', 1, 13, TT.MINUS),
         __get_token_string('file2', 1, 15, TT.VAR, 'i'),
         __get_token_string('file2', 1, 16, TT.COLON),
@@ -373,16 +359,15 @@
         __get_token_string('file2', 1, 27, TT.WHITESPACE),
         __get_token_string('file2', 1, 28, TT.FLOAT, '4.5'),
         __get_token_string('file2', 1, 31, TT.NEWLINE),
         __get_token_string('file2', 2, 1, TT.TAB),
         __get_token_string('file2', 2, 2, TT.MINUS),
         __get_token_string('file2', 2, 3, TT.WHITESPACE),
         __get_token_string('file2', 2, 4, TT.STRING, 'property'),
-        __get_token_string('file2', 2, 12, TT.NEWLINE),
-        __get_token_string('file2', 3, 1, TT.EOF),
+        __get_token_string('file2', 2, 12, TT.EOF),
     ]
     lexer = Lexer(input_files)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
@@ -403,16 +388,15 @@
         __get_token_string('file', 1, 18, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
         __get_token_string('file', 2, 2, TT.WHITESPACE),
         __get_token_string('file', 2, 3, TT.STRING, 'toto'),
         __get_token_string('file', 2, 7, TT.COLON),
         __get_token_string('file', 2, 8, TT.WHITESPACE),
         __get_token_string('file', 2, 9, TT.STRING, 'tata'),
-        __get_token_string('file', 2, 13, TT.NEWLINE),
-        __get_token_string('file', 3, 1, TT.EOF),
+        __get_token_string('file', 2, 13, TT.EOF),
     ]
     lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
```

### Comparing `thipster-0.23.8/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.9/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.9/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/test_parsedfile.py` & `thipster-0.23.9/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/test_parserfactory.py` & `thipster-0.23.9/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/parser/test_yamlparser.py` & `thipster-0.23.9/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/repository/test_github_repository.py` & `thipster-0.23.9/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/repository/test_local_repository.py` & `thipster-0.23.9/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/repository/test_resourcemodel.py` & `thipster-0.23.9/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/test_e2e.py` & `thipster-0.23.9/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/tests/test_tools.py` & `thipster-0.23.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/auth/google.py` & `thipster-0.23.9/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/engine.py` & `thipster-0.23.9/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/exceptions.py` & `thipster-0.23.9/thipster/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/i_parser.py` & `thipster-0.23.9/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/i_repository.py` & `thipster-0.23.9/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/i_terraform.py` & `thipster-0.23.9/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/parsed_file.py` & `thipster-0.23.9/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/engine/resource_model.py` & `thipster-0.23.9/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/helpers.py` & `thipster-0.23.9/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.9/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.9/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.9/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.9/thipster/parser/dsl_parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         }
 
         single_char_tokens.get(self.__currentChar, self.__add_next_char)()
 
     def __handle_current_token(self) -> None:
         """Process the current stored token.
 
-        Check if the current token is a keyword, calls the cprresponding function, or
+        Check if the current token is a keyword, calls the corresponding function, or
         the '__handleLiteralsAndVariables' otherwise.
         """
         current_token = self.__lexerPosition.currentToken.lower()
 
         keywords = {
             '': self.__handle_empty_token,
             'amount': self.__handle_word_token(TT.AMOUNT),
@@ -414,15 +414,14 @@
     def __end_file(self) -> None:
         """Add a NEWLINE and an EOF token at the end of each file."""
         if len(self.__lexerPosition.currentToken.strip()) > 0:
             self.__handle_current_token()
             self.__lexerPosition.reset_current_token()
 
         self.__lexerPosition.isMultiLine = False
-        self.__handle_newline_token()
         self.__handle_eof_token()
 
     def __isfloat(self, num: str) -> bool:
         """Check if the string is a float.
 
         Parameters
         ----------
```

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.9/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.9/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/token.py` & `thipster-0.23.9/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.9/thipster/parser/dsl_parser/token_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
             match self.__get_next_type():
                 case TT.VAR:
                     file_node.variables.append(
                         self.__get_assignment(),
                     )
                 case TT.STRING:
-                    file_node.resources.append(self.__create_resource())
+                    file_node.resources.append(self.__get_resource())
                 case TT.OUTPUT:
                     self.__get_outputs(file_node)
                 case _:
                     raise DSLSyntaxError(
                         self.__next(), [TT.VAR, TT.STRING, TT.OUTPUT],
                     )
             self.__trim_newlines()
@@ -58,47 +58,50 @@
             Expected token type(s), by default None
 
         Returns
         -------
         Token
             The next token
         """
-        next_token_type = self.__get_next_type()
+        if not expected:
+            return self.__tokens.pop(0)
 
-        if expected:
-            if type(expected) is list:
-                if next_token_type not in expected:
-                    raise DSLSyntaxError(self.__tokens[0], expected)
-            elif next_token_type != expected:
-                raise DSLSyntaxError(self.__tokens[0], expected)
-        return self.__tokens.pop(0)
+        next_token = self.__check(expected)
+
+        if not next_token:
+            raise DSLSyntaxError(self.__tokens[0], expected)
+        return next_token
 
-    def __check(self, expected: TT, index: int = 0) -> Token | None:
+    def __check(self, expected: TT | list[TT], index: int = 0) -> Token | None:
         """Check if the next token is the expected one.
 
         If the type of the next token is equal to the expected parameter, it is popped
         from the list.
 
         Parameters
         ----------
-        expected : TT
-            Expected token type
+        expected : TT | list[TT]
+            Expected token type(s)
         index : int, optional
             Index of the token to check, by default 0
 
         Returns
         -------
         Token | None
             The next token if it is the expected one, None otherwise
         """
-        token = self.__get_next_type(index=index)
-        if token != expected:
-            return None
+        next_token_type = self.__get_next_type(index)
 
-        return self.__next(expected)
+        if expected:
+            if type(expected) is list:
+                if next_token_type not in expected:
+                    return None
+            elif next_token_type != expected:
+                return None
+        return self.__tokens.pop(0)
 
     def __get_next_type(self, index: int = 0) -> TT:
         """Get the type of the next token.
 
         Parameters
         ----------
         index : int, optional
@@ -120,45 +123,58 @@
 
     def __rm_empty_lines(self):
         # Detect empty line
         empty_types = [TT.TAB, TT.WHITESPACE]
         end = 0
         while end < len(self.__tokens):
             begin = end
+            next_token_type = self.__get_next_type(end)
             while self.__get_next_type(end) in empty_types:
                 end += 1
+                next_token_type = self.__get_next_type(end)
+
+            if next_token_type == TT.NEWLINE:
+                for _ in range(begin, end + 1):
+                    self.__tokens.pop(begin)
+                end = begin
 
-            if self.__get_next_type(index=end) == TT.NEWLINE:
+            elif next_token_type == TT.EOF:
                 for _ in range(begin, end):
                     self.__tokens.pop(begin)
-            end += 1
+                end += 1
+
+            else:
+                while next_token_type != TT.NEWLINE:
+                    end += 1
+                    next_token_type = self.__get_next_type(end)
+                end += 1
 
     def __get_newline(self):
         newline = self.__next(TT.NEWLINE)
         self.__trim_newlines()
 
         return newline
 
     def __get_whitespaces(self):
-        while self.__check(TT.WHITESPACE):
+        while self.__check([TT.WHITESPACE, TT.TAB]):
             pass
 
     def __get_tabs(self, indent: int) -> bool:
         """Check if the number of tabs is correct/ if it is the end of the block."""
         if self.__get_next_type() == TT.EOF:
             return False
         if indent == 0:
             return True
         if self.__get_next_type(indent-1) == TT.TAB:
             for _ in range(indent):
                 self.__next(TT.TAB)
             return True
         return False
 
-    def __create_resource(
+    def __get_resource(
         self,
         indent=0,
     ) -> ast.ResourceNode | ast.IfNode | ast.AmountNode:
         r"""Create an AST Resouce, If or Amount node.
 
         Format: type, name, ":", [amt_ctrl], [if_ctrl] ,"\\n"
         (list | dict | {parameter, "\\n"}).
```

### Comparing `thipster-0.23.8/thipster/parser/exceptions.py` & `thipster-0.23.9/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/parser_factory.py` & `thipster-0.23.9/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/parser/yaml_parser.py` & `thipster-0.23.9/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/repository/exceptions.py` & `thipster-0.23.9/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/repository/github.py` & `thipster-0.23.9/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/repository/json.py` & `thipster-0.23.9/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/repository/local.py` & `thipster-0.23.9/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/terraform/cdk.py` & `thipster-0.23.9/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster/terraform/exceptions.py` & `thipster-0.23.9/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.8/thipster.egg-info/PKG-INFO` & `thipster-0.23.9/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.8
+Version: 0.23.9
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.8 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.9 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.8/thipster.egg-info/SOURCES.txt` & `thipster-0.23.9/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

