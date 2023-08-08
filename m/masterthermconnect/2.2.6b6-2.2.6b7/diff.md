# Comparing `tmp/masterthermconnect-2.2.6b6.tar.gz` & `tmp/masterthermconnect-2.2.6b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterthermconnect-2.2.6b6.tar", last modified: Tue Aug  8 15:07:30 2023, max compression
+gzip compressed data, was "masterthermconnect-2.2.6b7.tar", last modified: Tue Aug  8 15:14:55 2023, max compression
```

## Comparing `masterthermconnect-2.2.6b6.tar` & `masterthermconnect-2.2.6b7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.049394 masterthermconnect-2.2.6b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.devcontainer-template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.021393 masterthermconnect-2.2.6b6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.025394 masterthermconnect-2.2.6b6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/ISSUE_TEMPLATE/issue.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.025394 masterthermconnect-2.2.6b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/workflows/push-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/workflows/push-prerelease.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.github/workflows/push-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/DEV_README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-08 15:07:30.049394 masterthermconnect-2.2.6b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.029394 masterthermconnect-2.2.6b6/masterthermconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/datamapread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/datamapwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/masterthermconnect/special.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.033394 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-08 15:07:29.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-08 15:07:30.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:07:29.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:07:29.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:07:29.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 15:07:29.000000 masterthermconnect-2.2.6b6/masterthermconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-08 15:07:30.049394 masterthermconnect-2.2.6b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.037394 masterthermconnect-2.2.6b6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.041394 masterthermconnect-2.2.6b6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/login_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/login_success.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.045394 masterthermconnect-2.2.6b6/tests/fixtures/mt/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/login_success.json
--rw-r--r--   0 runner    (1001) docker     (123)    46282 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0001_1_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    46238 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0002_1_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    46226 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_1_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    46218 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_2_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    46225 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    46224 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_4_0.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0001_1.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0002_1.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_1.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_3.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:07:30.049394 masterthermconnect-2.2.6b6/tests/fixtures/newapi/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/error_authorization.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/error_unavailable.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/login_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/login_success.json
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/modules.json
--rw-r--r--   0 runner    (1001) docker     (123)    46248 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_1_0.json
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_1_1668796652.json
--rw-r--r--   0 runner    (1001) docker     (123)    46267 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_2_0.json
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_2_1668796652.json
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpinfo_10021_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpinfo_10021_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpwrite_success.json
--rw-r--r--   0 runner    (1001) docker     (123)    46263 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_0.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_1614501746.json
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_1614763054.json
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_unavailable.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpinfo_1234_1.json
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpinfo_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpwrite_error.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/fixtures/pumpwrite_success.json
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/test_api_new.py
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/test_api_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/test_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29313 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 15:06:49.000000 masterthermconnect-2.2.6b6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.515253 masterthermconnect-2.2.6b7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.devcontainer-template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.487253 masterthermconnect-2.2.6b7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.491253 masterthermconnect-2.2.6b7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/ISSUE_TEMPLATE/issue.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.495253 masterthermconnect-2.2.6b7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/workflows/push-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/workflows/push-prerelease.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.github/workflows/push-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/DEV_README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-08 15:14:55.515253 masterthermconnect-2.2.6b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.499253 masterthermconnect-2.2.6b7/masterthermconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/datamapread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/datamapwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/masterthermconnect/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.499253 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 15:14:55.000000 masterthermconnect-2.2.6b7/masterthermconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-08 15:14:55.515253 masterthermconnect-2.2.6b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.503253 masterthermconnect-2.2.6b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.507253 masterthermconnect-2.2.6b7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/login_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/login_success.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.511253 masterthermconnect-2.2.6b7/tests/fixtures/mt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/login_success.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46282 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0001_1_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46238 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0002_1_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46226 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_1_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46218 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46225 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46224 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_4_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0001_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0002_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:14:55.515253 masterthermconnect-2.2.6b7/tests/fixtures/newapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/error_authorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/error_unavailable.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/login_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/login_success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/modules.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46248 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_1_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_1_1668796652.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46267 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_2_1668796652.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpinfo_10021_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpinfo_10021_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpwrite_success.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46263 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_1614501746.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_1614763054.json
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_unavailable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpinfo_1234_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpinfo_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpwrite_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/fixtures/pumpwrite_success.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/test_api_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/test_api_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/test_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29313 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 15:14:22.000000 masterthermconnect-2.2.6b7/tox.ini
```

### Comparing `masterthermconnect-2.2.6b6/.devcontainer-template.json` & `masterthermconnect-2.2.6b7/.devcontainer-template.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.github/ISSUE_TEMPLATE/feature_request.md` & `masterthermconnect-2.2.6b7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.github/ISSUE_TEMPLATE/issue.md` & `masterthermconnect-2.2.6b7/.github/ISSUE_TEMPLATE/issue.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.github/workflows/lint.yaml` & `masterthermconnect-2.2.6b7/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.github/workflows/push-main.yml` & `masterthermconnect-2.2.6b7/.github/workflows/push-main.yml`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.github/workflows/push-prerelease.yml` & `masterthermconnect-2.2.6b7/.github/workflows/push-prerelease.yml`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.gitignore` & `masterthermconnect-2.2.6b7/.gitignore`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.pre-commit-config.yaml` & `masterthermconnect-2.2.6b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/.ruff.toml` & `masterthermconnect-2.2.6b7/.ruff.toml`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/DEV_README.md` & `masterthermconnect-2.2.6b7/DEV_README.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/LICENSE` & `masterthermconnect-2.2.6b7/LICENSE`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/PKG-INFO` & `masterthermconnect-2.2.6b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.6b6
+Version: 2.2.6b7
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.6b6 Summary: Python
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.6b7 Summary: Python
 3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.6b6/README.md` & `masterthermconnect-2.2.6b7/README.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/__init__.py` & `masterthermconnect-2.2.6b7/masterthermconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/__main__.py` & `masterthermconnect-2.2.6b7/masterthermconnect/__main__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/api.py` & `masterthermconnect-2.2.6b7/masterthermconnect/api.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/const.py` & `masterthermconnect-2.2.6b7/masterthermconnect/const.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/controller.py` & `masterthermconnect-2.2.6b7/masterthermconnect/controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/datamapread.py` & `masterthermconnect-2.2.6b7/masterthermconnect/datamapread.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/datamapwrite.py` & `masterthermconnect-2.2.6b7/masterthermconnect/datamapwrite.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/exceptions.py` & `masterthermconnect-2.2.6b7/masterthermconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect/special.py` & `masterthermconnect-2.2.6b7/masterthermconnect/special.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect.egg-info/PKG-INFO` & `masterthermconnect-2.2.6b7/masterthermconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.6b6
+Version: 2.2.6b7
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.6b6 Summary: Python
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.6b7 Summary: Python
 3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.6b6/masterthermconnect.egg-info/SOURCES.txt` & `masterthermconnect-2.2.6b7/masterthermconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/pyproject.toml` & `masterthermconnect-2.2.6b7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools-scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masterthermconnect"
-version = "2.2.6b6"
+version = "2.2.6b7"
 description = "Python 3 API wrapper for Mastertherm API"
 readme = "README.md"
 authors = [{ name = "Richard Holmes", email = "richard@shedc.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,15 +24,15 @@
 [project.urls]
 Homepage = "https://github.com/sHedC/python-masterthermconnect"
 
 [project.scripts]
 masterthermconnect = "masterthermconnect.__main__:main"
 
 [tool.bumpver]
-current_version = "2.2.6-b6"
+current_version = "2.2.6-b7"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `masterthermconnect-2.2.6b6/setup.cfg` & `masterthermconnect-2.2.6b7/setup.cfg`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/conftest.py` & `masterthermconnect-2.2.6b7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/login_success.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/login_success.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0001_1_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0001_1_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0002_1_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0002_1_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_1_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_1_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_2_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_2_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_3_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_3_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpdata_0524_4_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpdata_0524_4_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0001_1.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0001_1.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0002_1.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0002_1.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_1.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_1.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_2.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_2.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_3.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_3.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/mt/pumpinfo_0524_4.json` & `masterthermconnect-2.2.6b7/tests/fixtures/mt/pumpinfo_0524_4.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/modules.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/modules.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_1_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_1_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_1_1668796652.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_1_1668796652.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_2_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_2_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpdata_10021_2_1668796652.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpdata_10021_2_1668796652.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpinfo_10021_1.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpinfo_10021_1.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/newapi/pumpinfo_10021_2.json` & `masterthermconnect-2.2.6b7/tests/fixtures/newapi/pumpinfo_10021_2.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_0.json` & `masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_0.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_1614501746.json` & `masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_1614501746.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/pumpdata_1234_1_1614763054.json` & `masterthermconnect-2.2.6b7/tests/fixtures/pumpdata_1234_1_1614763054.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/fixtures/pumpinfo_1234_1.json` & `masterthermconnect-2.2.6b7/tests/fixtures/pumpinfo_1234_1.json`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/test_api_new.py` & `masterthermconnect-2.2.6b7/tests/test_api_new.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/test_api_old.py` & `masterthermconnect-2.2.6b7/tests/test_api_old.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/test_config_data.py` & `masterthermconnect-2.2.6b7/tests/test_config_data.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/test_controller.py` & `masterthermconnect-2.2.6b7/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.6b6/tests/test_main.py` & `masterthermconnect-2.2.6b7/tests/test_main.py`

 * *Files identical despite different names*

