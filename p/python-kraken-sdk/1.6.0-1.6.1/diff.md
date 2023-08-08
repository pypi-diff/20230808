# Comparing `tmp/python-kraken-sdk-1.6.0.tar.gz` & `tmp/python-kraken-sdk-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kraken-sdk-1.6.0.tar", last modified: Tue Aug  1 18:14:49 2023, max compression
+gzip compressed data, was "python-kraken-sdk-1.6.1.tar", last modified: Tue Aug  8 05:49:35 2023, max compression
```

## Comparing `python-kraken-sdk-1.6.0.tar` & `python-kraken-sdk-1.6.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/self-review.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_futures_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_futures_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_spot_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_spot_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_test_futures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_test_spot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    33064 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/about/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/about/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/base_api/base_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/futures_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/futures_ws_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_bot_templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_orderbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_ws_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/trading_bot_templates.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/futures/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/futures/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/issues.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/krakenexceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/krakenexceptions/krakenexceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/spot/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/spot/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_ws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/market_client_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_ws_examples_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_ws_examples_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/kraken/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/base_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/futures/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    29168 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    41526 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/spot/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/spot/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)   204293 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/fixture/orderbook.json
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_internals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27928 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.562582 python-kraken-sdk-1.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.562582 python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/self-review.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.566582 python-kraken-sdk-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_test_futures_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_test_futures_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_test_spot_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/_test_spot_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/manual_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/manual_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/manual_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/manual_test_futures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/manual_test_spot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33064 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.566582 python-kraken-sdk-1.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.566582 python-kraken-sdk-1.6.1/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.566582 python-kraken-sdk-1.6.1/docs/src/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/about/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.566582 python-kraken-sdk-1.6.1/docs/src/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/base_api/base_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/docs/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/futures_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/futures_ws_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/spot_bot_templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/spot_orderbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/spot_ws_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/examples/trading_bot_templates.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/docs/src/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/futures/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/futures/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/docs/src/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/issues.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/docs/src/krakenexceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/krakenexceptions/krakenexceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/docs/src/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/spot/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/docs/src/spot/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/futures_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/futures_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/futures_ws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/market_client_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_trading_bot_template_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_trading_bot_template_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_ws_examples_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/examples/spot_ws_examples_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/kraken/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/kraken/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/base_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.570582 python-kraken-sdk-1.6.1/kraken/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/kraken/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/kraken/futures/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/futures/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/kraken/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29168 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41526 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/kraken/spot/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/websocket/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/websocket_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/kraken/spot/websocket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 05:49:35.000000 python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.574582 python-kraken-sdk-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/tests/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/futures/test_futures_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/tests/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:49:35.578582 python-kraken-sdk-1.6.1/tests/spot/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)   204293 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/fixture/orderbook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27928 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-08-08 05:49:25.000000 python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_v2.py
```

### Comparing `python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `python-kraken-sdk-1.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/codecov.yml` & `python-kraken-sdk-1.6.1/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/pull_request_template.md` & `python-kraken-sdk-1.6.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/release.yaml` & `python-kraken-sdk-1.6.1/.github/release.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/self-review.md` & `python-kraken-sdk-1.6.1/.github/self-review.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_build.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_build_doc.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_build_doc.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_codecov.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_codecov.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_codeql.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_codeql.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_pypi_publish.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_test_futures_private.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_test_futures_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_test_futures_public.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_test_futures_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_test_spot_private.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_test_spot_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/_test_spot_public.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/_test_spot_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/cicd.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/manual_build.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/manual_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/manual_test_futures.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/manual_test_futures.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/manual_test_spot.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/manual_test_spot.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.github/workflows/release.yaml` & `python-kraken-sdk-1.6.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.gitignore` & `python-kraken-sdk-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/.pre-commit-config.yaml` & `python-kraken-sdk-1.6.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -45,14 +45,24 @@
     rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - --select=E9,F63,F7,F82
           - --show-source
           - --statistics
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.0
+    hooks:
+      - id: pylint
+        name: pylint
+        types: [python]
+        exclude: ^examples/|^tests/|^setup.py$
+        args:
+          - --rcfile=pyproject.toml
+          - -d=R0801 # ignore duplicate code
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.0.282
     hooks:
       - id: ruff
         args:
           - --fix
           - --exit-non-zero-on-fix
```

### Comparing `python-kraken-sdk-1.6.0/.readthedocs.yaml` & `python-kraken-sdk-1.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/CHANGELOG.md` & `python-kraken-sdk-1.6.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/CODE_OF_CONDUCT.md` & `python-kraken-sdk-1.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/CONTRIBUTING.md` & `python-kraken-sdk-1.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/LICENSE` & `python-kraken-sdk-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/Makefile` & `python-kraken-sdk-1.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/PKG-INFO` & `python-kraken-sdk-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.6.0
+Version: 1.6.1
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `python-kraken-sdk-1.6.0/README.md` & `python-kraken-sdk-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/Makefile` & `python-kraken-sdk-1.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/conf.py` & `python-kraken-sdk-1.6.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 import sys
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "python-kraken-sdk"
-copyright = "2023, Benjamin Thomas Schwertfeger"  # noqa: A001
+copyright = "2023, Benjamin Thomas Schwertfeger"  # noqa: A001 # pylint: disable=redefined-builtin
 author = "Benjamin Thomas Schwertfeger"
 
 # to import the package
 sys.path.insert(0, os.path.abspath(".."))
 
 rst_epilog = ""
 # Read link all targets from file
```

### Comparing `python-kraken-sdk-1.6.0/docs/index.rst` & `python-kraken-sdk-1.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/links.rst` & `python-kraken-sdk-1.6.1/docs/links.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/make.bat` & `python-kraken-sdk-1.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/base_api/base_api.rst` & `python-kraken-sdk-1.6.1/docs/src/base_api/base_api.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/futures_bot_template.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/futures_bot_template.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/futures_ws_examples.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/futures_ws_examples.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/spot_bot_templates.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/spot_bot_templates.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/spot_orderbook.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/spot_orderbook.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/spot_ws_examples.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/spot_ws_examples.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/examples/trading_bot_templates.rst` & `python-kraken-sdk-1.6.1/docs/src/examples/trading_bot_templates.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/futures/rest.rst` & `python-kraken-sdk-1.6.1/docs/src/futures/rest.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/getting_started/getting_started.rst` & `python-kraken-sdk-1.6.1/docs/src/getting_started/getting_started.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/introduction.rst` & `python-kraken-sdk-1.6.1/docs/src/introduction.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/issues.rst` & `python-kraken-sdk-1.6.1/docs/src/issues.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/docs/src/spot/rest.rst` & `python-kraken-sdk-1.6.1/docs/src/spot/rest.rst`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/futures_examples.py` & `python-kraken-sdk-1.6.1/examples/futures_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/futures_trading_bot_template.py` & `python-kraken-sdk-1.6.1/examples/futures_trading_bot_template.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/futures_ws_examples.py` & `python-kraken-sdk-1.6.1/examples/futures_ws_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,38 +63,39 @@
     time.sleep(2)  # in case subscribe is not done yet
     # await client.unsubscribe(feed='ticker', products=['PI_XBTUSD'])
     await client.unsubscribe(feed="ticker", products=["PF_XBTUSD"])
     await client.unsubscribe(feed="book", products=products)
     # ...
 
     # _____Private_Websocket_Feeds_________________
-    client_auth = Client(key=key, secret=secret)
-    # print(client_auth.get_available_private_subscription_feeds())
+    if key and secret:
+        client_auth = Client(key=key, secret=secret)
+        # print(client_auth.get_available_private_subscription_feeds())
+
+        # subscribe to a private/authenticated websocket feed
+        await client_auth.subscribe(feed="fills")
+        await client_auth.subscribe(feed="open_positions")
+        # await client_auth.subscribe(feed='open_orders')
+        # await client_auth.subscribe(feed='open_orders_verbose')
+        # await client_auth.subscribe(feed='deposits_withdrawals')
+        # await client_auth.subscribe(feed='account_balances_and_margins')
+        # await client_auth.subscribe(feed='balances')
+        # await client_auth.subscribe(feed='account_log')
+        # await client_auth.subscribe(feed='notifications_auth')
+
+        # authenticated clients can also subscribe to public feeds
+        # await client_auth.subscribe(feed='ticker', products=['PI_XBTUSD', 'PF_ETHUSD'])
+
+        # time.sleep(1)
+        # unsubscribe from a private/authenticated websocket feed
+        await client_auth.unsubscribe(feed="fills")
+        await client_auth.unsubscribe(feed="open_positions")
+        # ...
 
-    # subscribe to a private/authenticated websocket feed
-    await client_auth.subscribe(feed="fills")
-    await client_auth.subscribe(feed="open_positions")
-    # await client_auth.subscribe(feed='open_orders')
-    # await client_auth.subscribe(feed='open_orders_verbose')
-    # await client_auth.subscribe(feed='deposits_withdrawals')
-    # await client_auth.subscribe(feed='account_balances_and_margins')
-    # await client_auth.subscribe(feed='balances')
-    # await client_auth.subscribe(feed='account_log')
-    # await client_auth.subscribe(feed='notifications_auth')
-
-    # authenticated clients can also subscribe to public feeds
-    # await client_auth.subscribe(feed='ticker', products=['PI_XBTUSD', 'PF_ETHUSD'])
-
-    # time.sleep(1)
-    # unsubscribe from a private/authenticated websocket feed
-    await client_auth.unsubscribe(feed="fills")
-    await client_auth.unsubscribe(feed="open_positions")
-    # ...
-
-    while not client.exception_occur and not client_auth.exception_occur:
+    while not client.exception_occur:  # and not client_auth.exception_occur:
         await asyncio.sleep(6)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
     # the websocket client will send {'event': 'asyncio.CancelledError'} via on_message
```

### Comparing `python-kraken-sdk-1.6.0/examples/market_client_example.ipynb` & `python-kraken-sdk-1.6.1/examples/market_client_example.ipynb`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/spot_examples.py` & `python-kraken-sdk-1.6.1/examples/spot_examples.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/spot_orderbook.py` & `python-kraken-sdk-1.6.1/examples/spot_orderbook.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v1.py` & `python-kraken-sdk-1.6.1/examples/spot_trading_bot_template_v1.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v2.py` & `python-kraken-sdk-1.6.1/examples/spot_trading_bot_template_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 """
 Module that provides a template to build a Spot trading algorithm using the
-python-kraken-sdk and Kraken Spot websocket API v1.
+python-kraken-sdk and Kraken Spot websocket API v2.
 """
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import logging.config
```

### Comparing `python-kraken-sdk-1.6.0/examples/spot_ws_examples_v1.py` & `python-kraken-sdk-1.6.1/examples/spot_ws_examples_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,26 +78,27 @@
         subscription={"name": "ticker"},
         pair=["XBT/USD", "DOT/USD"],
     )
     await client.unsubscribe(subscription={"name": "spread"}, pair=["XBT/USD"])
     await client.unsubscribe(subscription={"name": "spread"}, pair=["DOT/USD"])
     # ...
 
-    client_auth = Client(key=key, secret=secret)
-    # print(client_auth.active_private_subscriptions)
-    # print(client_auth.private_channel_names) # list private channel names
-    # when using the authenticated client, you can also subscribe to public feeds
-    await client_auth.subscribe(subscription={"name": "ownTrades"})
-    await client_auth.subscribe(subscription={"name": "openOrders"})
+    if key and secret:
+        client_auth = Client(key=key, secret=secret)
+        # print(client_auth.active_private_subscriptions)
+        # print(client_auth.private_channel_names) # list private channel names
+        # when using the authenticated client, you can also subscribe to public feeds
+        await client_auth.subscribe(subscription={"name": "ownTrades"})
+        await client_auth.subscribe(subscription={"name": "openOrders"})
 
-    await asyncio.sleep(2)
-    await client_auth.unsubscribe(subscription={"name": "ownTrades"})
-    await client_auth.unsubscribe(subscription={"name": "openOrders"})
+        await asyncio.sleep(2)
+        await client_auth.unsubscribe(subscription={"name": "ownTrades"})
+        await client_auth.unsubscribe(subscription={"name": "openOrders"})
 
-    while not client.exception_occur and not client_auth.exception_occur:
+    while not client.exception_occur:  # and not client_auth.exception_occur:
         await asyncio.sleep(6)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
     # The websocket client will send {'event': 'asyncio.CancelledError'}
```

### Comparing `python-kraken-sdk-1.6.0/examples/spot_ws_examples_v2.py` & `python-kraken-sdk-1.6.1/examples/spot_ws_examples_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,27 +86,28 @@
     await asyncio.sleep(3)
     # print(client.active_public_subscriptions) # … to list active subscriptions
     await client.unsubscribe(
         params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]},
     )
     # ...
 
-    # Per default, the authenticated client starts two websocket connections,
-    # one for authenticated and one for public messages. If there is no need
-    # for a public connection, it can be disabled using the ``no_public``
-    # parameter.
-    client_auth = Client(key=key, secret=secret, no_public=True)
-    # print(client_auth.private_channel_names)  # … list private channel names
-    # when using the authenticated client, you can also subscribe to public feeds
-    await client_auth.subscribe(params={"channel": "executions"})
+    if key and secret:
+        # Per default, the authenticated client starts two websocket connections,
+        # one for authenticated and one for public messages. If there is no need
+        # for a public connection, it can be disabled using the ``no_public``
+        # parameter.
+        client_auth = Client(key=key, secret=secret, no_public=True)
+        # print(client_auth.private_channel_names)  # … list private channel names
+        # when using the authenticated client, you can also subscribe to public feeds
+        await client_auth.subscribe(params={"channel": "executions"})
 
-    await asyncio.sleep(5)
-    await client_auth.unsubscribe(params={"channel": "executions"})
+        await asyncio.sleep(5)
+        await client_auth.unsubscribe(params={"channel": "executions"})
 
-    while not client.exception_occur and not client_auth.exception_occur:
+    while not client.exception_occur:  # and not client_auth.exception_occur:
         await asyncio.sleep(6)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
     # The websocket client will send {'event': 'asyncio.CancelledError'}
```

### Comparing `python-kraken-sdk-1.6.0/kraken/base_api/__init__.py` & `python-kraken-sdk-1.6.1/kraken/base_api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/exceptions/__init__.py` & `python-kraken-sdk-1.6.1/kraken/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/__init__.py` & `python-kraken-sdk-1.6.1/kraken/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/funding.py` & `python-kraken-sdk-1.6.1/kraken/futures/funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/market.py` & `python-kraken-sdk-1.6.1/kraken/futures/market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/trade.py` & `python-kraken-sdk-1.6.1/kraken/futures/trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/user.py` & `python-kraken-sdk-1.6.1/kraken/futures/user.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 """Module that implements the Kraken Futures user client"""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Union
 
+from kraken.base_api import KrakenBaseFuturesAPI, defined
+
 if TYPE_CHECKING:
     import requests
 
-from kraken.base_api import KrakenBaseFuturesAPI, defined
-
 
 class User(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures user client
 
     If the sandbox environment is chosen, the keys must be generated from here:
     https://demo-futures.kraken.com/settings/api
```

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/websocket/__init__.py` & `python-kraken-sdk-1.6.1/kraken/futures/websocket/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import TYPE_CHECKING, Any, List, Optional
 
 import websockets
 
 from kraken.exceptions import KrakenException
 
 if TYPE_CHECKING:
-    # to avoid circular import for type checking
     from kraken.futures import KrakenFuturesWSClient
 
 
 class ConnectFuturesWebsocket:
     """
     This class is only called by the :class:`kraken.futures.KrakenFuturesWSClient`
     to establish the websocket connection.
@@ -85,18 +84,18 @@
                 event.set()
             self.__reconnect_num = 0
 
             while keep_alive:
                 try:
                     _msg = await asyncio.wait_for(self.__socket.recv(), timeout=15)
                 except asyncio.TimeoutError:
-                    logging.debug(
-                        "Timeout error in {endpoint}",
-                        extra={"endpoint": self.__ws_endpoint},
-                    )  # important
+                    logging.debug(  # important
+                        "Timeout error in %s",
+                        self.__ws_endpoint,
+                    )
                 except asyncio.CancelledError:
                     logging.exception("asyncio.CancelledError")
                     keep_alive = False
                     await self.__callback({"error": "asyncio.CancelledError"})
                 else:
                     try:
                         message: dict = json.loads(_msg)
@@ -134,16 +133,17 @@
 
         self.__reconnect_num += 1
         if self.__reconnect_num >= self.MAX_RECONNECT_NUM:
             raise KrakenException.MaxReconnectError
 
         reconnect_wait: float = self.__get_reconnect_wait(self.__reconnect_num)
         logging.debug(
-            "asyncio sleep reconnect_wait={wait} s reconnect_num={num}",
-            extra={"wait": reconnect_wait, "num": self.__reconnect_num},
+            "asyncio sleep reconnect_wait=%f s reconnect_num=%d",
+            reconnect_wait,
+            self.__reconnect_num,
         )
         await asyncio.sleep(reconnect_wait)
         logging.debug("asyncio sleep done")
         event: asyncio.Event = asyncio.Event()
 
         tasks: dict = {
             asyncio.ensure_future(
@@ -161,15 +161,15 @@
             for task in finished:
                 if task.exception():
                     exception_occur = True
                     traceback.print_stack()
                     message = f"{task} got an exception {task.exception()}\n {task.get_stack()}"
                     logging.warning(message)
                     for process in pending:
-                        logging.warning("pending {proc}", extra={"proc": process})
+                        logging.warning("pending %s", process)
                         try:
                             process.cancel()
                         except asyncio.CancelledError:
                             logging.exception("CancelledError")
                         logging.warning("cancel ok")
                     await self.__callback({"error": message})
             if exception_occur:
@@ -177,29 +177,29 @@
         logging.warning("reconnect over")
 
     async def __recover_subscription_req_msg(
         self: ConnectFuturesWebsocket,
         event: asyncio.Event,
     ) -> None:
         logging.info(
-            "Recover subscriptions {subscriptions} waiting.",
-            extra={"subscriptions": self.__subscriptions},
+            "Recover subscriptions %s waiting.",
+            self.__subscriptions,
         )
         await event.wait()
 
         for sub in self.__subscriptions:
             if sub["feed"] in self.__client.get_available_private_subscription_feeds():
                 await self.send_message(deepcopy(sub), private=True)
             elif sub["feed"] in self.__client.get_available_public_subscription_feeds():
                 await self.send_message(deepcopy(sub), private=False)
-            logging.info("{sub}: OK", extra={"sub": sub})
+            logging.info("%s: OK", sub)
 
         logging.info(
-            "Recover subscriptions {subscriptions} done.",
-            extra={"subscriptions": self.__subscriptions},
+            "Recover subscriptions %s done.",
+            self.__subscriptions,
         )
 
     async def send_message(
         self: ConnectFuturesWebsocket,
         msg: dict,
         private: bool = False,
     ) -> None:
```

### Comparing `python-kraken-sdk-1.6.0/kraken/futures/ws_client.py` & `python-kraken-sdk-1.6.1/kraken/futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/__init__.py` & `python-kraken-sdk-1.6.1/kraken/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/funding.py` & `python-kraken-sdk-1.6.1/kraken/spot/funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/market.py` & `python-kraken-sdk-1.6.1/kraken/spot/market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/orderbook.py` & `python-kraken-sdk-1.6.1/kraken/spot/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,16 +302,16 @@
 
                 async def on_book_update(
                     self: "Orderbook",
                     pair: str,
                     message: list
                 ) -> None:
                     book: Dict[str, Any] = self.get(pair="XBT/USD")
-                    ask: List[Tuple[str, str]] = list(book["ask"].items())
-                    bid: List[Tuple[str, str]] = list(book["bid"].items())
+                    ask: list[Tuple[str, str]] = list(book["ask"].items())
+                    bid: list[Tuple[str, str]] = list(book["bid"].items())
                     # ask and bid are now in format [price, (volume, timestamp)]
                     # … and include the whole orderbook
         """
         return self.__book.get(pair)
 
     def __update_book(
         self: OrderbookClient,
```

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/staking.py` & `python-kraken-sdk-1.6.1/kraken/spot/staking.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/trade.py` & `python-kraken-sdk-1.6.1/kraken/spot/trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/user.py` & `python-kraken-sdk-1.6.1/kraken/spot/user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/websocket/__init__.py` & `python-kraken-sdk-1.6.1/kraken/spot/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/websocket/connectors.py` & `python-kraken-sdk-1.6.1/kraken/spot/websocket/connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
         """
         keep_alive: bool = True
         self._last_ping = time()
         self.ws_conn_details = (
             None if not self.__is_auth else self.__client.get_ws_token()
         )
         self.LOG.debug(
-            "Websocket token: {details}",
-            extra={"details": self.ws_conn_details},
+            "Websocket token: %s",
+            self.ws_conn_details,
         )
 
         async with websockets.connect(  # pylint: disable=no-member
             f"wss://{self.__ws_endpoint}",
             ping_interval=30,
         ) as socket:
             self.LOG.info("Websocket connected!")
@@ -158,16 +158,17 @@
         except KrakenException.MaxReconnectError:
             await self.__callback(
                 {"error": "kraken.exceptions.KrakenException.MaxReconnectError"},
             )
         except Exception as exc:
             traceback_: str = traceback.format_exc()
             logging.exception(
-                "{exc}: {traceback}",
-                extra={"exc": exc, "traceback": traceback_},
+                "%s: %s",
+                exc,
+                traceback_,
             )
             await self.__callback({"error": traceback_})
         finally:
             await self.__callback(
                 {"error": "Exception stopped the Kraken Spot Websocket Client!"},
             )
             self.__client.exception_occur = True
@@ -211,15 +212,15 @@
             for task in finished:
                 if task.exception():
                     exception_occur = True
                     traceback.print_stack()
                     message: str = f"{task} got an exception {task.exception()}\n {task.get_stack()}"
                     self.LOG.warning(message)
                     for process in pending:
-                        self.LOG.warning("pending {proc}", extra={"proc": process})
+                        self.LOG.warning("pending %s", process)
                         try:
                             process.cancel()
                         except asyncio.CancelledError:
                             self.LOG.exception("asyncio.CancelledError")
                     await self.__callback({"error": message})
             if exception_occur:
                 break
@@ -351,15 +352,15 @@
                 and "name" in sub["subscription"]
                 and sub["subscription"]["name"] in self.client.private_channel_names
             ):
                 cpy["subscription"]["token"] = self.ws_conn_details["token"]
                 private = True
 
             await self.client.send_message(cpy, private=private)
-            self.LOG.info("{sub} OK", extra={"sub": sub})
+            self.LOG.info("%s: OK", sub)
 
         self.LOG.info("%s done.", log_msg)
 
     def _manage_subscriptions(
         self: ConnectSpotWebsocketV1,
         message: Union[dict, list],
     ) -> None:
@@ -496,15 +497,15 @@
         """
         log_msg: str = f'Recover {"authenticated" if self.is_auth else "public"} subscriptions {self._subscriptions}'
         self.LOG.info("%s waiting.", log_msg)
         await event.wait()
 
         for subscription in self._subscriptions:
             await self.client.subscribe(params=subscription)
-            self.LOG.info("{subscription} OK", extra={"subscription": subscription})
+            self.LOG.info("%s: OK", subscription)
 
         self.LOG.info("%s done.", log_msg)
 
     def _manage_subscriptions(self: ConnectSpotWebsocketV2, message: dict) -> None:  # type: ignore[override]
         """
         Checks if the message contains events about un-/subscriptions
         to add or remove these from the list of current tracked subscriptions.
```

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/websocket_v1.py` & `python-kraken-sdk-1.6.1/kraken/spot/websocket_v1.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/kraken/spot/websocket_v2.py` & `python-kraken-sdk-1.6.1/kraken/spot/websocket_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             secret=secret,
             callback=callback,
             no_public=no_public,
             beta=beta,
             api_version="v2",
         )
 
-    async def send_message(  # noqa: PLR0912
+    async def send_message(  # noqa: PLR0912 # pylint: disable=arguments-differ
         self: KrakenSpotWSClientV2,
         message: dict,
         raw: bool = False,
     ) -> None:
         """
         Sends a message via the websocket connection. For private messages
         the authentication token will be assigned automatically if
```

### Comparing `python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/PKG-INFO` & `python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.6.0
+Version: 1.6.1
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/SOURCES.txt` & `python-kraken-sdk-1.6.1/python_kraken_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/conftest.py` & `python-kraken-sdk-1.6.1/tests/futures/conftest.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/helper.py` & `python-kraken-sdk-1.6.1/tests/futures/helper.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_base_api.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_base_api.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_funding.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_market.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_trade.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_user.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/futures/test_futures_websocket.py` & `python-kraken-sdk-1.6.1/tests/futures/test_futures_websocket.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/conftest.py` & `python-kraken-sdk-1.6.1/tests/spot/conftest.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/fixture/orderbook.json` & `python-kraken-sdk-1.6.1/tests/spot/fixture/orderbook.json`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/helper.py` & `python-kraken-sdk-1.6.1/tests/spot/helper.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_base_api.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_base_api.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_funding.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_funding.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_market.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_market.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_orderbook.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_orderbook.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_staking.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_staking.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_trade.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_trade.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_user.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_user.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_internals.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_internals.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v1.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_v1.py`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v2.py` & `python-kraken-sdk-1.6.1/tests/spot/test_spot_websocket_v2.py`

 * *Files identical despite different names*

