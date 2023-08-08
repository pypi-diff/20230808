# Comparing `tmp/geomancy-1.1.2.tar.gz` & `tmp/geomancy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-1.1.2.tar", last modified: Sat Aug  5 21:37:12 2023, max compression
+gzip compressed data, was "geomancy-1.1.3.tar", last modified: Tue Aug  8 18:39:37 2023, max compression
```

## Comparing `geomancy-1.1.2.tar` & `geomancy-1.1.3.tar`

### file list

```diff
@@ -1,150 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 21:37:01.000000 geomancy-1.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-05 21:37:01.000000 geomancy-1.1.2/.geomancy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.552366 geomancy-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-05 21:37:01.000000 geomancy-1.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-05 21:37:01.000000 geomancy-1.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-05 21:37:01.000000 geomancy-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-05 21:37:01.000000 geomancy-1.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 21:37:01.000000 geomancy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 21:37:12.568366 geomancy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-05 21:37:01.000000 geomancy-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-05 21:37:01.000000 geomancy-1.1.2/Taskfile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-05 21:37:01.000000 geomancy-1.1.2/changelog/48.bugfix.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-05 21:37:01.000000 geomancy-1.1.2/changelog/_template.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/geomancy_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/geomancy_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/about/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/about/api/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/about/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/about/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/guides/tips_and_tricks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/iam.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/s3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/aws/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/snippets/common_args.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/env.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/exec.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/path.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/platform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/python.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/snippets/common_args.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/cmd_checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/cmd_run.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/format.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/examples/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/aws/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/geomancy.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/geomancy/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/__description__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    19392 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/geomancy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/environment/dotenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 21:37:01.000000 geomancy-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 21:37:12.568366 geomancy-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.552366 geomancy-1.1.2/tests/checks/aws/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/config1.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/data/test.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/entrypoints/test_geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/environment/test_dotenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/utils/sleep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 18:39:26.000000 geomancy-1.1.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-08 18:39:26.000000 geomancy-1.1.3/.geomancy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.062754 geomancy-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.066754 geomancy-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 18:39:26.000000 geomancy-1.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 18:39:26.000000 geomancy-1.1.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-08 18:39:26.000000 geomancy-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-08 18:39:26.000000 geomancy-1.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-08 18:39:26.000000 geomancy-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-08-08 18:39:37.082756 geomancy-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-08-08 18:39:26.000000 geomancy-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-08 18:39:26.000000 geomancy-1.1.3/Taskfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.066754 geomancy-1.1.3/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-08 18:39:26.000000 geomancy-1.1.3/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/_static/geomancy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/_static/geomancy_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/about/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/about/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/about/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/about/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/guides/tips_and_tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/aws/iam.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/aws/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/aws/s3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/checks/aws/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/aws/snippets/common_args.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/checks/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/env.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/exec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/platform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/core/python.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/docs/usage/checks/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/checks/snippets/common_args.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/cmd_checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/cmd_run.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-08 18:39:26.000000 geomancy-1.1.3/docs/usage/format.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/examples/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 18:39:26.000000 geomancy-1.1.3/examples/aws/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-08 18:39:26.000000 geomancy-1.1.3/examples/geomancy.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-08 18:39:26.000000 geomancy-1.1.3/examples/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 18:39:26.000000 geomancy-1.1.3/examples/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.070755 geomancy-1.1.3/geomancy/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/__description__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.074755 geomancy-1.1.3/geomancy/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.074755 geomancy-1.1.3/geomancy/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/aws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19392 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/checks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.074755 geomancy-1.1.3/geomancy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.074755 geomancy-1.1.3/geomancy/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/geomancy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-08 18:39:26.000000 geomancy-1.1.3/geomancy/environment/dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.074755 geomancy-1.1.3/geomancy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 18:39:37.000000 geomancy-1.1.3/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-08 18:39:26.000000 geomancy-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:39:37.082756 geomancy-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/tests/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.066754 geomancy-1.1.3/tests/checks/aws/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/tests/checks/aws/cassettes/test_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.078755 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/aws/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/checks/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/config/config1.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/data/test.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/environment/test_dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:37.082756 geomancy-1.1.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-08 18:39:26.000000 geomancy-1.1.3/tests/utils/sleep.yaml
```

### Comparing `geomancy-1.1.2/.geomancy.yaml` & `geomancy-1.1.3/.geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/.github/workflows/publish-to-pypi.yml` & `geomancy-1.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/.github/workflows/tests.yml` & `geomancy-1.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/.gitignore` & `geomancy-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/LICENSE` & `geomancy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/PKG-INFO` & `geomancy-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
@@ -160,37 +160,44 @@
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables common to all development environments
 
     Path:
-      decs: Paths to search for executables
+      decs: Search paths for executables
       checkEnv: $PATH
 ```
 
 or [toml](https://toml.io/en/) (e.g. ``.geomancy.toml``)
 
 ```toml
 [checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
+or [toml](https://toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``)
+
+```toml
+[Checks.Environment]
+Path = {checkEnv = "$PATH", desc = "Search paths for executables"}
+```
+
 or [pyproject.toml](https://peps.python.org/pep-0621/)
 
 ```toml
 [tool.geomancy.checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [tool.geomancy.checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
 </details>
 </p>
 
 ### Available Checks
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.1.2 Summary: Geomancy validates
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.3 Summary: Geomancy validates
 deployment and development environments Author: Justin Lorieau Keywords:
 .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
@@ -57,23 +57,26 @@
 accessible using the [current credentials](https://docs.aws.amazon.com/cli/
 latest/userguide/cli-configure-files.html) and are secured. This example is in
 yaml format, and checks can be formatted in toml format as well. ```yaml AWS:
 TemplateS3: checkS3: myproject-cfn-templates StaticS3: checkS3: myproject-
 static MediaS3: checkS3: myproject-media ```
   Load_checks_in_multiple_formats  Including [yaml](https://yaml.org) (e.g.
 ``.geomancy.yaml``) ```yaml checks: Environment: desc: Check environment
-variables common to all development environments Path: decs: Paths to search
-for executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
+variables common to all development environments Path: decs: Search paths for
+executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
 ``.geomancy.toml``) ```toml [checks.Environment] desc = "Check environment
 variables common to all development environments" [checks.Environment.Path]
-desc = "Paths to search for executables" checkEnv = "$PATH" ``` or
-[pyproject.toml](https://peps.python.org/pep-0621/) ```toml
-[tool.geomancy.checks.Environment] desc = "Check environment variables common
-to all development environments" [tool.geomancy.checks.Environment.Path] desc =
-"Paths to search for executables" checkEnv = "$PATH" ```
+desc = "Search paths for executables" checkEnv = "$PATH" ``` or [toml](https://
+toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``) ```toml
+[Checks.Environment] Path = {checkEnv = "$PATH", desc = "Search paths for
+executables"} ``` or [pyproject.toml](https://peps.python.org/pep-0621/
+) ```toml [tool.geomancy.checks.Environment] desc = "Check environment
+variables common to all development environments"
+[tool.geomancy.checks.Environment.Path] desc = "Search paths for executables"
+checkEnv = "$PATH" ```
 ### Available Checks
  Operating_systems meet the minimum required versions (checkOS)  The following
 shows an example in yaml format. Checks can be formatted in toml format as
 well. ```yaml OperatingSystem: desc: Check the minimum operating system
 versions subchecks: any checkMacOS: desc: MacOS 10.9 or later (released 2013)
 checkOS: "macOS >= 10.9" checkLinuxOS: desc: Linux 4.0 or later (released 2015)
 checkOS: "Linux >= 3.0" checkWindows: desc: Windows 10 or later (released 2015)
```

### Comparing `geomancy-1.1.2/README.md` & `geomancy-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,37 +129,44 @@
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables common to all development environments
 
     Path:
-      decs: Paths to search for executables
+      decs: Search paths for executables
       checkEnv: $PATH
 ```
 
 or [toml](https://toml.io/en/) (e.g. ``.geomancy.toml``)
 
 ```toml
 [checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
+or [toml](https://toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``)
+
+```toml
+[Checks.Environment]
+Path = {checkEnv = "$PATH", desc = "Search paths for executables"}
+```
+
 or [pyproject.toml](https://peps.python.org/pep-0621/)
 
 ```toml
 [tool.geomancy.checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [tool.geomancy.checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
 </details>
 </p>
 
 ### Available Checks
```

#### html2text {}

```diff
@@ -41,23 +41,26 @@
 accessible using the [current credentials](https://docs.aws.amazon.com/cli/
 latest/userguide/cli-configure-files.html) and are secured. This example is in
 yaml format, and checks can be formatted in toml format as well. ```yaml AWS:
 TemplateS3: checkS3: myproject-cfn-templates StaticS3: checkS3: myproject-
 static MediaS3: checkS3: myproject-media ```
   Load_checks_in_multiple_formats  Including [yaml](https://yaml.org) (e.g.
 ``.geomancy.yaml``) ```yaml checks: Environment: desc: Check environment
-variables common to all development environments Path: decs: Paths to search
-for executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
+variables common to all development environments Path: decs: Search paths for
+executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
 ``.geomancy.toml``) ```toml [checks.Environment] desc = "Check environment
 variables common to all development environments" [checks.Environment.Path]
-desc = "Paths to search for executables" checkEnv = "$PATH" ``` or
-[pyproject.toml](https://peps.python.org/pep-0621/) ```toml
-[tool.geomancy.checks.Environment] desc = "Check environment variables common
-to all development environments" [tool.geomancy.checks.Environment.Path] desc =
-"Paths to search for executables" checkEnv = "$PATH" ```
+desc = "Search paths for executables" checkEnv = "$PATH" ``` or [toml](https://
+toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``) ```toml
+[Checks.Environment] Path = {checkEnv = "$PATH", desc = "Search paths for
+executables"} ``` or [pyproject.toml](https://peps.python.org/pep-0621/
+) ```toml [tool.geomancy.checks.Environment] desc = "Check environment
+variables common to all development environments"
+[tool.geomancy.checks.Environment.Path] desc = "Search paths for executables"
+checkEnv = "$PATH" ```
 ### Available Checks
  Operating_systems meet the minimum required versions (checkOS)  The following
 shows an example in yaml format. Checks can be formatted in toml format as
 well. ```yaml OperatingSystem: desc: Check the minimum operating system
 versions subchecks: any checkMacOS: desc: MacOS 10.9 or later (released 2013)
 checkOS: "macOS >= 10.9" checkLinuxOS: desc: Linux 4.0 or later (released 2015)
 checkOS: "Linux >= 3.0" checkWindows: desc: Windows 10 or later (released 2015)
```

### Comparing `geomancy-1.1.2/Taskfile.yaml` & `geomancy-1.1.3/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/changelog/_template.rst` & `geomancy-1.1.3/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/_static/custom.css` & `geomancy-1.1.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/_static/geomancy_logo.png` & `geomancy-1.1.3/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/_static/geomancy_logo.svg` & `geomancy-1.1.3/docs/_static/geomancy_logo.svg`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/about/api/index.rst` & `geomancy-1.1.3/docs/about/api/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/about/changelog.rst` & `geomancy-1.1.3/docs/about/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,32 @@
 (``<major>.<minor>.<patch>``).
 
 Changes in API will only be introduced in major versions with notes in the
 deprecations section.
 
 .. towncrier release notes start
 
+`geomancy 1.1.3 <https://github.com/jlorieau/geomancy/tree/1.1.3>`_ - 2023-08-08
+================================================================================
+
+Bug Fixes
+---------
+
+- `#48 <https://github.com/jlorieau/geomancy/issues/48>`_. Fixed bug that would disallow parentheses within parentheses in Result stasuses
+
+
+`gomancy 1.1.3 <https://github.com/jlorieau/geomancy/tree/1.1.3>`_ - 2023-08-08
+===============================================================================
+
+Bug Fixes
+---------
+
+- `#48 <https://github.com/jlorieau/geomancy/issues/48>`_. Fixed bug that would disallow parentheses within parentheses in Result stasuses
+
+
 `geomancy 1.1.1 <https://github.com/jlorieau/geomancy/tree/1.1.1>`_ - 2023-08-05
 ================================================================================
 
 Features
 --------
 
 - `#35 <https://github.com/jlorieau/geomancy/issues/35>`_. Added CheckAwsIam for checking AWS authentication and security settings
```

### Comparing `geomancy-1.1.2/docs/conf.py` & `geomancy-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/guides/tips_and_tricks.rst` & `geomancy-1.1.3/docs/usage/checks/core/base.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,78 @@
-.. _tips-and-tricks:
+.. _check:
 
-Tips and Tricks
-===============
-
-Unwanted environment substitution
----------------------------------
+Checks and Groups
+-----------------
 
-Environment variables are substituted by default in the values passed to
-checks. This can be avoided by setting ``substitute`` to False or by
-using a literal with single quotes.
+.. automodule:: geomancy.checks.python
+  :noindex:
 
-.. tab-set::
+.. card::
 
-    .. tab-item:: substitute (yaml)
+    Parameters
+    ^^^
 
-        .. code-block:: yaml
+    ``desc``: str (Optional)
+        | The description for the check group
+
+    ``subchecks``: str (Optional)
+        | The pass condition for the sub-checks of the group. Can be either ``'all'``
+          to require that all sub-checks pass or ``'any'`` to require that only one
+          sub-check passes.
+        | *default*: ``'all'``
+        | *aliases*: ``condition``
 
-            MyOddFilename:
-              checkPath: myfile$.txt
-              substitute: False
+.. tab-set::
 
-    .. tab-item:: literal string (yaml)
+    .. tab-item:: Example 1 (yaml)
 
-        Use triple (3) single quotes
+        The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+        ``Pyproject``.
 
         .. code-block:: yaml
 
-            MyOddFilename:
-              checkPath: '''myfile$.txt'''
-
-    .. tab-item:: substitute (toml)
+            checksFiles:
+              desc: Checks that at least one checks file exists
+              subchecks: any
+
+              Geomancy:
+                desc: Check for the 'geomancy.toml' file
+                checkPath: examples/geomancy.toml
+                type: file
+              Pyproject:
+                desc: Check for 'pyproject.toml' file
+                checkPath: examples/pyproject.toml
+                type: file
 
-        .. code-block:: toml
+    .. tab-item:: Example 2 (toml)
 
-            [MyOddFilename]
-            checkpath='myfile$.txt'
-            substitute=false
-
-    .. tab-item:: literal string (toml)
-
-        Use quadruple (4) single quotes
+        The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+        ``Pyproject``.
 
         .. code-block:: toml
 
-            [MyOddFilename]
-            checkpath=''''myfile$.txt''''
-
-Flat Checks Files
------------------
-
-Checks can be conveniently grouped by category, but this is not a strict
-requirement for checks files. For example, the following checks file
-includes checks at the root level.
+            [checks.ChecksFile]
+            desc = "Checks that at least one checks file exists"
+            subchecks = "any"
 
-.. tab-set::
-
-    .. tab-item:: example 1 (yaml)
+            [checks.ChecksFile.Geomancy]
+            desc = "Check for 'geomancy.toml' file"
+            checkPath = "examples/geomancy.toml"
+            type = "file"
 
-        .. code-block:: yaml
+            [checks.ChecksFile.Pyproject]
+            desc = "Check for 'pyproject.toml' file"
+            checkPath = "examples/pyproject.toml"
+            type = "file"
 
-            Geomancy:
-              desc: Check for the 'geomancy.toml' file
-              checkPath: examples/geomancy.toml
-              type: file
-
-            Pyproject:
-              desc: Check for 'pyproject.toml' file
-              checkPath: examples/pyproject.toml
-              type: file
+    .. tab-item:: Example 3 (toml)
 
-    .. tab-item:: example 2 (toml)
+        The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+        ``Pyproject``, in abbreviated format.
 
         .. code-block:: toml
 
-            [Geomancy]
-            desc = "Check for the 'geomancy.toml' file"
-            checkPath = "examples/geomancy.toml"
-            type = "file"
+            [checks.ChecksFile]
+            subchecks = "any"
 
-            [Pyproject]
-            desc = "Check for 'pyproject.toml' file"
-            checkPath = "examples/pyproject.toml"
-            type = "file"
+            Geomancy = { checkPath = "examples/geomancy.toml", type = "file" }
+            Pyproject = { checkPath = "examples/pyproject.toml", type = "file" }
```

### Comparing `geomancy-1.1.2/docs/index.rst` & `geomancy-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/aws/iam.rst` & `geomancy-1.1.3/docs/usage/checks/aws/iam.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .. _checkAwsIam:
 
-checkAwsIam
+checkIam
 -----------
 
 .. automodule:: geomancy.checks.aws.iam
   :noindex:
 
 .. card::
 
     Parameters
     ^^^
 
     ``checkAwsIam``:
         | Check the IAM account
-        | *aliases*: ``checkIAM``, ``CheckIAM``, ``checkAWSIAM``, ``checkAwsIAM``,
+        | *aliases*: ``CheckIAM``, ``checkAwsIam``, ``checkAWSIAM``, ``checkAwsIAM``,
           ``CheckAwsIAM``,
 
     ``root``: bool (Optional)
         | Security check for root access key and signing certificate availability
         | *aliases*: ``root_access``
         | *default*: True
```

### Comparing `geomancy-1.1.2/docs/usage/checks/aws/index.rst` & `geomancy-1.1.3/docs/usage/checks/aws/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/aws/s3.rst` & `geomancy-1.1.3/docs/usage/checks/aws/s3.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .. _checkAwsS3:
 
-checkAwsS3
-----------
+checkS3
+-------
 
 .. automodule:: geomancy.checks.aws.s3
   :noindex:
 
 .. card::
 
     Parameters
     ^^^
 
     ``checkAwsS3``: str
         | Check the given S3 bucket
-        | *aliases*: ``checkS3``, ``CheckS3``, ``checkAWSS3``, ``checkAwsS3``,
+        | *aliases*: ``CheckS3``, ``checkAWSS3``, ``checkAwsS3``,
           ``CheckAwsS3``
 
     ``private``: bool
         | Security check the public availability of the bucket
         | *default*: True
 
     .. include:: snippets/common_args.rst
```

### Comparing `geomancy-1.1.2/docs/usage/checks/core/env.rst` & `geomancy-1.1.3/docs/usage/checks/core/env.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/core/exec.rst` & `geomancy-1.1.3/docs/usage/checks/core/exec.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/core/index.rst` & `geomancy-1.1.3/docs/usage/checks/core/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/core/path.rst` & `geomancy-1.1.3/docs/usage/checks/core/path.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/core/platform.rst` & `geomancy-1.1.3/docs/usage/checks/core/platform.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/checks/core/python.rst` & `geomancy-1.1.3/docs/usage/checks/core/python.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/cmd_checks.rst` & `geomancy-1.1.3/docs/usage/cmd_checks.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/cmd_run.rst` & `geomancy-1.1.3/docs/usage/cmd_run.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/docs/usage/format.rst` & `geomancy-1.1.3/docs/usage/format.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/examples/geomancy.toml` & `geomancy-1.1.3/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/examples/geomancy.yaml` & `geomancy-1.1.3/examples/geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/aws/base.py` & `geomancy-1.1.3/geomancy/checks/aws/base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/aws/iam.py` & `geomancy-1.1.3/geomancy/checks/aws/iam.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/aws/s3.py` & `geomancy-1.1.3/geomancy/checks/aws/s3.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/base.py` & `geomancy-1.1.3/geomancy/checks/base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/env.py` & `geomancy-1.1.3/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/exec.py` & `geomancy-1.1.3/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/path.py` & `geomancy-1.1.3/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/platform.py` & `geomancy-1.1.3/geomancy/checks/platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/python.py` & `geomancy-1.1.3/geomancy/checks/python.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/test.py` & `geomancy-1.1.3/geomancy/checks/test.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/utils.py` & `geomancy-1.1.3/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/checks/version.py` & `geomancy-1.1.3/geomancy/checks/version.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/config/config.py` & `geomancy-1.1.3/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/entrypoints/check.py` & `geomancy-1.1.3/geomancy/entrypoints/check.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/entrypoints/config.py` & `geomancy-1.1.3/geomancy/entrypoints/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/entrypoints/environment.py` & `geomancy-1.1.3/geomancy/entrypoints/environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/entrypoints/geo.py` & `geomancy-1.1.3/geomancy/entrypoints/geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/entrypoints/utils.py` & `geomancy-1.1.3/geomancy/entrypoints/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy/environment/dotenv.py` & `geomancy-1.1.3/geomancy/environment/dotenv.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/geomancy.egg-info/PKG-INFO` & `geomancy-1.1.3/geomancy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
@@ -160,37 +160,44 @@
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables common to all development environments
 
     Path:
-      decs: Paths to search for executables
+      decs: Search paths for executables
       checkEnv: $PATH
 ```
 
 or [toml](https://toml.io/en/) (e.g. ``.geomancy.toml``)
 
 ```toml
 [checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
+or [toml](https://toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``)
+
+```toml
+[Checks.Environment]
+Path = {checkEnv = "$PATH", desc = "Search paths for executables"}
+```
+
 or [pyproject.toml](https://peps.python.org/pep-0621/)
 
 ```toml
 [tool.geomancy.checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [tool.geomancy.checks.Environment.Path]
-    desc = "Paths to search for executables"
+    desc = "Search paths for executables"
     checkEnv = "$PATH"
 ```
 
 </details>
 </p>
 
 ### Available Checks
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.1.2 Summary: Geomancy validates
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.3 Summary: Geomancy validates
 deployment and development environments Author: Justin Lorieau Keywords:
 .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
@@ -57,23 +57,26 @@
 accessible using the [current credentials](https://docs.aws.amazon.com/cli/
 latest/userguide/cli-configure-files.html) and are secured. This example is in
 yaml format, and checks can be formatted in toml format as well. ```yaml AWS:
 TemplateS3: checkS3: myproject-cfn-templates StaticS3: checkS3: myproject-
 static MediaS3: checkS3: myproject-media ```
   Load_checks_in_multiple_formats  Including [yaml](https://yaml.org) (e.g.
 ``.geomancy.yaml``) ```yaml checks: Environment: desc: Check environment
-variables common to all development environments Path: decs: Paths to search
-for executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
+variables common to all development environments Path: decs: Search paths for
+executables checkEnv: $PATH ``` or [toml](https://toml.io/en/) (e.g.
 ``.geomancy.toml``) ```toml [checks.Environment] desc = "Check environment
 variables common to all development environments" [checks.Environment.Path]
-desc = "Paths to search for executables" checkEnv = "$PATH" ``` or
-[pyproject.toml](https://peps.python.org/pep-0621/) ```toml
-[tool.geomancy.checks.Environment] desc = "Check environment variables common
-to all development environments" [tool.geomancy.checks.Environment.Path] desc =
-"Paths to search for executables" checkEnv = "$PATH" ```
+desc = "Search paths for executables" checkEnv = "$PATH" ``` or [toml](https://
+toml.io/en/) with each check on 1 line (e.g. ``.geomancy.toml``) ```toml
+[Checks.Environment] Path = {checkEnv = "$PATH", desc = "Search paths for
+executables"} ``` or [pyproject.toml](https://peps.python.org/pep-0621/
+) ```toml [tool.geomancy.checks.Environment] desc = "Check environment
+variables common to all development environments"
+[tool.geomancy.checks.Environment.Path] desc = "Search paths for executables"
+checkEnv = "$PATH" ```
 ### Available Checks
  Operating_systems meet the minimum required versions (checkOS)  The following
 shows an example in yaml format. Checks can be formatted in toml format as
 well. ```yaml OperatingSystem: desc: Check the minimum operating system
 versions subchecks: any checkMacOS: desc: MacOS 10.9 or later (released 2013)
 checkOS: "macOS >= 10.9" checkLinuxOS: desc: Linux 4.0 or later (released 2015)
 checkOS: "Linux >= 3.0" checkWindows: desc: Windows 10 or later (released 2015)
```

### Comparing `geomancy-1.1.2/geomancy.egg-info/SOURCES.txt` & `geomancy-1.1.3/geomancy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .readthedocs.yaml
 LICENSE
 README.md
 Taskfile.yaml
 pyproject.toml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
-changelog/48.bugfix.rst
 changelog/_template.rst
 docs/conf.py
 docs/index.rst
 docs/quickstart.rst
 docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
```

### Comparing `geomancy-1.1.2/pyproject.toml` & `geomancy-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml` & `geomancy-1.1.3/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/conftest.py` & `geomancy-1.1.3/tests/checks/aws/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/test_base.py` & `geomancy-1.1.3/tests/checks/aws/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/test_iam.py` & `geomancy-1.1.3/tests/checks/aws/test_iam.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/aws/test_s3.py` & `geomancy-1.1.3/tests/checks/aws/test_s3.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_base.py` & `geomancy-1.1.3/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_env.py` & `geomancy-1.1.3/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_exec.py` & `geomancy-1.1.3/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_path.py` & `geomancy-1.1.3/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_platform.py` & `geomancy-1.1.3/tests/checks/test_platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/checks/test_python.py` & `geomancy-1.1.3/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/config/test_config.py` & `geomancy-1.1.3/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/conftest.py` & `geomancy-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/entrypoints/test_geo.py` & `geomancy-1.1.3/tests/entrypoints/test_geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.2/tests/environment/test_dotenv.py` & `geomancy-1.1.3/tests/environment/test_dotenv.py`

 * *Files identical despite different names*

