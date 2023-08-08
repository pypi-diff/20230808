# Comparing `tmp/hdx_python_utilities-3.6.1.tar.gz` & `tmp/hdx_python_utilities-3.6.2.tar.gz`

## Comparing `hdx_python_utilities-3.6.1.tar` & `hdx_python_utilities-3.6.2.tar`

### file list

```diff
@@ -1,122 +1,123 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0    35309 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/main.md
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/_version.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/compare.py
--rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0        0        0    61802 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/downloader.py
--rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0        0        0     8056 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/email.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/encoding.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0        0        0     2968 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/html.py
--rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/loader.py
--rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/path.py
--rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/retriever.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/saver.py
--rwxr-xr-x   0        0        0     7648 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/session.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/state.py
--rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/text.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/typehint.py
--rwxr-xr-x   0        0        0     7151 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/useragent.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/uuid.py
--rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/compare/test_csv_processing2.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_email_configuration.yaml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/json_csv.yaml
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/smtp_config.yaml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/basicauth.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params.yaml
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params_tree.yaml
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xlsx_processing.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/html/response.html
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/loader/empty.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/loader/empty.yaml
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test_hxl.csv
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out2.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out2.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out5.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out6.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out7.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out8.csv
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out8.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0        0        0    47756 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0        0        0     5657 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0        0        0    10274 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0        0        0     3541 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/utils.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/LICENSE
--rwxr-xr-x   0        0        0     1727 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/README.md
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/pyproject.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4074 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    36050 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/documentation/main.md
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/_version.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/compare.py
+-rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0        0        0    61802 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0        0        0     8028 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/email.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/encoding.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0        0        0     2968 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/html.py
+-rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/loader.py
+-rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/path.py
+-rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/retriever.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/saver.py
+-rwxr-xr-x   0        0        0     7648 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/session.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/state.py
+-rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/text.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0        0        0     7151 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/useragent.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/src/hdx/utilities/uuid.py
+-rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/compare/test_csv_processing2.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/hdx_email_configuration.yaml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/json_csv.yaml
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/logging_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/smtp_config.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/basicauth.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/extra_params.yaml
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/extra_params_tree.yaml
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_data.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_xlsx_processing.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/html/response.html
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/loader/empty.yaml
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/test.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/test_hxl.csv
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/retriever/fallbacks/test.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out2.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out2.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out5.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out6.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out7.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out8.csv
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/out8.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/state/analysis_dates.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0        0        0    47758 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0        0        0     5657 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0        0        0    10274 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0        0        0     2941 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0        0        0     3541 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/tests/hdx/utilities/utils.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/LICENSE
+-rwxr-xr-x   0        0        0     1727 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/README.md
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.2/PKG-INFO
```

### Comparing `hdx_python_utilities-3.6.1/CONTRIBUTING.md` & `hdx_python_utilities-3.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/requirements.txt` & `hdx_python_utilities-3.6.2/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
+annotated-types==0.5.0
+    # via pydantic
 attrs==23.1.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
 beautifulsoup4==4.12.2
     # via hdx-python-utilities (pyproject.toml)
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cfgv==3.3.1
     # via pre-commit
-chardet==5.1.0
+chardet==5.2.0
     # via frictionless
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via typer
 colorama==0.4.6
     # via typer
 coverage[toml]==7.2.7
     # via pytest-cov
 decorator==5.1.1
     # via validators
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.1
     # via email-validator
 email-validator==2.0.0.post2
     # via hdx-python-utilities (pyproject.toml)
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
-frictionless==5.13.1
+frictionless==5.15.10
     # via hdx-python-utilities (pyproject.toml)
 html5lib==1.1
     # via hdx-python-utilities (pyproject.toml)
-humanize==4.6.0
+humanize==4.7.0
     # via frictionless
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   email-validator
     #   requests
-ijson==3.2.2
+ijson==3.2.3
     # via hdx-python-utilities (pyproject.toml)
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.2
     # via frictionless
@@ -79,57 +81,59 @@
     # via pre-commit
 openpyxl==3.1.2
     # via hdx-python-utilities (pyproject.toml)
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.7.0
+platformdirs==3.10.0
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via hdx-python-utilities (pyproject.toml)
-pydantic==1.10.9
+pydantic==2.1.1
     # via frictionless
-pygments==2.15.1
+pydantic-core==2.4.0
+    # via pydantic
+pygments==2.16.1
     # via rich
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   hdx-python-utilities (pyproject.toml)
     #   pytest-cov
     #   pytest-loguru
 pytest-cov==4.1.0
     # via hdx-python-utilities (pyproject.toml)
 pytest-loguru==0.2.0
     # via hdx-python-utilities (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   frictionless
     #   hdx-python-utilities (pyproject.toml)
 python-slugify==8.0.1
     # via frictionless
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 ratelimit==2.2.1
     # via hdx-python-utilities (pyproject.toml)
 requests==2.31.0
     # via
     #   frictionless
     #   requests-file
 requests-file==1.5.1
     # via hdx-python-utilities (pyproject.toml)
 rfc3986==2.0.0
     # via frictionless
-rich==13.4.2
+rich==13.5.2
     # via typer
 ruamel-yaml==0.17.32
     # via hdx-python-utilities (pyproject.toml)
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 shellingham==1.5.0.post1
     # via typer
@@ -149,24 +153,25 @@
     # via hdx-python-utilities (pyproject.toml)
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
 typer[all]==0.9.0
     # via frictionless
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   frictionless
     #   pydantic
+    #   pydantic-core
     #   typer
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 validators==0.20.0
     # via frictionless
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via pre-commit
 webencodings==0.5.1
     # via html5lib
 xlrd==2.0.1
     # via hdx-python-utilities (pyproject.toml)
 xlsxwriter==3.1.2
     # via tableschema-to-template
```

### Comparing `hdx_python_utilities-3.6.1/.config/pre-commit-config.yaml` & `hdx_python_utilities-3.6.2/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/.github/workflows/publish.yaml` & `hdx_python_utilities-3.6.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/.github/workflows/run-python-tests.yaml` & `hdx_python_utilities-3.6.2/.github/workflows/run-python-tests.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This workflow will install Python dependencies, lint and run tests
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run tests
 
 on:
+  workflow_dispatch: # add run button in github
   push:
     branches-ignore:
       - gh-pages
   pull_request:
     branches-ignore:
       - gh-pages
```

### Comparing `hdx_python_utilities-3.6.1/documentation/main.md` & `hdx_python_utilities-3.6.2/documentation/main.md`

 * *Files 2% similar despite different names*

```diff
@@ -675,14 +675,35 @@
                 assert state.get() == date1
                 state.set(date2)
             with State(
                 statepath, parse_date, iso_string_from_datetime
             ) as state:
                 assert state.get() == date2.replace(hour=0, minute=0)
 
+            with State(
+                statepath,
+                State.dates_str_to_country_date_dict,
+                State.country_date_dict_to_dates_str,
+            ) as state:
+                state_dict = state.get()
+                assert state_dict == {"DEFAULT": date1}
+                state_dict["AFG"] = date2
+                state.set(state_dict)
+            with State(
+                statepath,
+                State.dates_str_to_country_date_dict,
+                State.country_date_dict_to_dates_str,
+            ) as state:
+                state_dict = state.get()
+                assert state_dict == {
+                    "DEFAULT": date1,
+                    "AFG": date2.replace(hour=0, minute=0),
+                }
+
+
 If run inside a GitHub Action, the saved state file could be committed to 
 GitHub so that on the next run the state is available in the repository.
 
 ## Path utilities
 
 Examples:
```

### Comparing `hdx_python_utilities-3.6.1/documentation/pydoc-markdown.yaml` & `hdx_python_utilities-3.6.2/documentation/pydoc-markdown.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.utilities
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Utilities
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-python-utilities"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-utilities
   pages:
     - title: Home
```

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/base_downloader.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/compare.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/dateparse.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/dictandlist.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/downloader.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/easy_logging.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/email.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             return recipients
         normalised_recipients = []
         for recipient in recipients:
             v = validate_email(
                 recipient, check_deliverability=True
             )  # validate and get info
             normalised_recipients.append(
-                v["email"]
+                v.normalized
             )  # replace with normalized form
         return normalised_recipients
 
     def send(
         self,
         to: Union[str, ListTuple[str]],
         subject: str,
@@ -205,15 +205,15 @@
             None
         """
         if sender is None:
             sender = self.sender
         v = validate_email(
             sender, check_deliverability=False
         )  # validate and get info
-        sender = v["email"]  # replace with normalized form
+        sender = v.normalized
 
         if html_body is not None:
             msg = MIMEMultipart("alternative")
             part1 = MIMEText(text_body, "plain")
             part2 = MIMEText(html_body, "html")
             msg.attach(part1)
             msg.attach(part2)
```

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/encoding.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/errors_onexit.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/frictionless_wrapper.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/frictionless_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/html.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/loader.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/path.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/retriever.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/saver.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/session.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/session.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/text.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/useragent.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/src/hdx/utilities/uuid.py` & `hdx_python_utilities-3.6.2/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/test_data.csv` & `hdx_python_utilities-3.6.2/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/config/json_csv.yaml` & `hdx_python_utilities-3.6.2/tests/fixtures/config/json_csv.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.json` & `hdx_python_utilities-3.6.2/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.yaml` & `hdx_python_utilities-3.6.2/tests/fixtures/config/logging_config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.xlsx` & `hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xls_processing.xls` & `hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx_python_utilities-3.6.2/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/fixtures/html/response.html` & `hdx_python_utilities-3.6.2/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/conftest.py` & `hdx_python_utilities-3.6.2/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_compare.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dateparse.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dictandlist.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_downloader.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
     @pytest.fixture(scope="class")
     def fixtureurlexcel(self):
         return "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-utilities/main/tests/fixtures/downloader/test_data.xlsx"
 
     @pytest.fixture(scope="class")
     def getfixtureurl(self):
-        return "http://httpbin.org/get"
+        return "https://httpbin.org/get"
 
     @pytest.fixture(scope="class")
     def postfixtureurl(self):
-        return "http://httpbin.org/post"
+        return "https://httpbin.org/post"
 
     @pytest.fixture(scope="class")
     def fixturenotexistsurl(self):
         return "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-utilities/main/tests/fixtures/NOTEXIST.csv"
 
     @pytest.fixture(scope="class")
     def fixtureprocessurl(self):
```

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_easy_logging.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_email.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_email.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_encoding.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_errors_onexit.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_html.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_loader.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_path.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_retriever.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_saver.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_text.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_useragent.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/test_useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/tests/hdx/utilities/utils.py` & `hdx_python_utilities-3.6.2/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/.gitignore` & `hdx_python_utilities-3.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/LICENSE` & `hdx_python_utilities-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/README.md` & `hdx_python_utilities-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/pyproject.toml` & `hdx_python_utilities-3.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.1/PKG-INFO` & `hdx_python_utilities-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-utilities
-Version: 3.6.1
+Version: 3.6.2
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-utilities
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,date,datetime,dict,json,library,list,streaming,tabular data,time,timezone,utilities,yaml
 Classifier: Development Status :: 5 - Production/Stable
```

