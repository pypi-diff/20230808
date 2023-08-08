# Comparing `tmp/causal_testing_framework-5.1.0.tar.gz` & `tmp/causal_testing_framework-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-5.1.0.tar", last modified: Fri Aug  4 13:19:01 2023, max compression
+gzip compressed data, was "causal_testing_framework-5.1.1.tar", last modified: Tue Aug  8 15:53:54 2023, max compression
```

## Comparing `causal_testing_framework-5.1.0.tar` & `causal_testing_framework-5.1.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20352 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_adequacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    28237 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/intervention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/actions_and_webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/version_release.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.842663 causal_testing_framework-5.1.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.842663 causal_testing_framework-5.1.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data_with_categorical.csv
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_adequacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.870738 causal_testing_framework-5.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.870738 causal_testing_framework-5.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20352 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28237 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/testing/intervention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.874738 causal_testing_framework-5.1.1/causal_testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/causal_testing/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-08 15:53:54.000000 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-08-08 15:53:54.000000 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:53:54.000000 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-08 15:53:54.000000 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 15:53:54.000000 causal_testing_framework-5.1.1/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/dev/actions_and_webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/dev/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/dev/version_release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.870738 causal_testing_framework-5.1.1/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.878738 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.882738 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.882738 causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.882738 causal_testing_framework-5.1.1/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.882738 causal_testing_framework-5.1.1/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.882738 causal_testing_framework-5.1.1/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.870738 causal_testing_framework-5.1.1/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.886738 causal_testing_framework-5.1.1/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.870738 causal_testing_framework-5.1.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/resources/data/data_with_categorical.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:54.890738 causal_testing_framework-5.1.1/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-08 15:53:03.000000 causal_testing_framework-5.1.1/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-5.1.0/.github/CONTRIBUTING.md` & `causal_testing_framework-5.1.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-5.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-5.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-5.1.1/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-5.1.1/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-5.1.1/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.gitignore` & `causal_testing_framework-5.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.pylintrc` & `causal_testing_framework-5.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/.readthedocs.yaml` & `causal_testing_framework-5.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/LICENSE` & `causal_testing_framework-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/PKG-INFO` & `causal_testing_framework-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 5.1.0
+Version: 5.1.1
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-5.1.0/README.md` & `causal_testing_framework-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-5.1.1/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-5.1.1/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/generation/enum_gen.py` & `causal_testing_framework-5.1.1/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-5.1.1/causal_testing/json_front/json_class.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-5.1.1/causal_testing/specification/causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/specification/causal_specification.py` & `causal_testing_framework-5.1.1/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-5.1.1/causal_testing/specification/metamorphic_relation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/specification/scenario.py` & `causal_testing_framework-5.1.1/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/specification/variable.py` & `causal_testing_framework-5.1.1/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-5.1.1/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_adequacy.py` & `causal_testing_framework-5.1.1/causal_testing/testing/causal_test_adequacy.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,34 +22,44 @@
         causal_dag: CausalDAG,
         test_suite: CausalTestSuite,
     ):
         self.causal_dag = causal_dag
         self.test_suite = test_suite
         self.tested_pairs = None
         self.pairs_to_test = None
-        self.untested_edges = None
+        self.untested_pairs = None
         self.dag_adequacy = None
 
     def measure_adequacy(self):
         """
-        Calculate the adequacy measurement, and populate the `dat_adequacy` field.
+        Calculate the adequacy measurement, and populate the `dag_adequacy` field.
         """
-        self.tested_pairs = {(t.treatment_variable, t.outcome_variable) for t in self.test_suite}
-        self.pairs_to_test = set(combinations(self.causal_dag.graph.nodes, 2))
-        self.untested_edges = self.pairs_to_test.difference(self.tested_pairs)
+        self.pairs_to_test = set(combinations(self.causal_dag.graph.nodes(), 2))
+        self.tested_pairs = set()
+
+        for n1, n2 in self.pairs_to_test:
+            if (n1, n2) in self.causal_dag.graph.edges():
+                if any((t.treatment_variable, t.outcome_variable) == (n1, n2) for t in self.test_suite):
+                    self.tested_pairs.add((n1, n2))
+            else:
+                # Causal independences are not order dependent
+                if any((t.treatment_variable, t.outcome_variable) in {(n1, n2), (n2, n1)} for t in self.test_suite):
+                    self.tested_pairs.add((n1, n2))
+
+        self.untested_pairs = self.pairs_to_test.difference(self.tested_pairs)
         self.dag_adequacy = len(self.tested_pairs) / len(self.pairs_to_test)
 
     def to_dict(self):
         "Returns the adequacy object as a dictionary."
         return {
             "causal_dag": self.causal_dag,
             "test_suite": self.test_suite,
             "tested_pairs": self.tested_pairs,
             "pairs_to_test": self.pairs_to_test,
-            "untested_edges": self.untested_edges,
+            "untested_pairs": self.untested_pairs,
             "dag_adequacy": self.dag_adequacy,
         }
 
 
 class DataAdequacy:
     """
     Measures the adequacy of a given test according to the Fisher kurtosis of the bootstrapped result.
```

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-5.1.1/causal_testing/testing/causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-5.1.1/causal_testing/testing/causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-5.1.1/causal_testing/testing/causal_test_result.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-5.1.1/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/estimators.py` & `causal_testing_framework-5.1.1/causal_testing/testing/estimators.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/testing/intervention.py` & `causal_testing_framework-5.1.1/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing/utils/validation.py` & `causal_testing_framework-5.1.1/causal_testing/utils/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-5.1.1/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 5.1.0
+Version: 5.1.1
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-5.1.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-5.1.1/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/Makefile` & `causal_testing_framework-5.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/README.md` & `causal_testing_framework-5.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/make.bat` & `causal_testing_framework-5.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/conf.py` & `causal_testing_framework-5.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/description.rst` & `causal_testing_framework-5.1.1/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/dev/actions_and_webhooks.rst` & `causal_testing_framework-5.1.1/docs/source/dev/actions_and_webhooks.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/dev/documentation.rst` & `causal_testing_framework-5.1.1/docs/source/dev/documentation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/dev/version_release.rst` & `causal_testing_framework-5.1.1/docs/source/dev/version_release.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-5.1.1/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-5.1.1/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/images/workflow.png` & `causal_testing_framework-5.1.1/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/index.rst` & `causal_testing_framework-5.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/installation.rst` & `causal_testing_framework-5.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-5.1.1/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-5.1.1/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-5.1.1/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/docs/source/usage.rst` & `causal_testing_framework-5.1.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-5.1.1/examples/covasim_/doubling_beta/example_beta.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-5.1.1/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/README.md` & `causal_testing_framework-5.1.1/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/dag.dot` & `causal_testing_framework-5.1.1/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/dag.png` & `causal_testing_framework-5.1.1/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-5.1.1/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/data/results.csv` & `causal_testing_framework-5.1.1/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-5.1.1/examples/lr91/example_max_conductances.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-5.1.1/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson/README.md` & `causal_testing_framework-5.1.1/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson/causal_tests.json` & `causal_testing_framework-5.1.1/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson/dag.dot` & `causal_testing_framework-5.1.1/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson/data.csv` & `causal_testing_framework-5.1.1/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-5.1.1/examples/poisson/example_run_causal_tests.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/README.md` & `causal_testing_framework-5.1.1/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-5.1.1/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-5.1.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-5.1.1/examples/poisson-line-process/example_poisson_process.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/images/workflow.png` & `causal_testing_framework-5.1.1/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/pyproject.toml` & `causal_testing_framework-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/data/nhefs.csv` & `causal_testing_framework-5.1.1/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-5.1.1/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-5.1.1/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-5.1.1/tests/json_front_tests/test_json_class.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-5.1.1/tests/specification_tests/test_causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-5.1.1/tests/specification_tests/test_metamorphic_relations.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-5.1.1/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/test_helpers.py` & `causal_testing_framework-5.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_adequacy.py` & `causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_suite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,118 @@
 import unittest
-from pathlib import Path
-from statistics import StatisticsError
-import scipy
 import os
-
-from causal_testing.testing.estimators import LinearRegressionEstimator
-from causal_testing.testing.base_test_case import BaseTestCase
-from causal_testing.testing.causal_test_case import CausalTestCase
+import numpy as np
+import pandas as pd
 from causal_testing.testing.causal_test_suite import CausalTestSuite
-from causal_testing.testing.causal_test_adequacy import DAGAdequacy
-from causal_testing.testing.causal_test_outcome import NoEffect, Positive
-from tests.test_helpers import remove_temp_dir_if_existent
-from causal_testing.json_front.json_class import JsonUtility, CausalVariables
-from causal_testing.specification.variable import Input, Output, Meta
-from causal_testing.specification.scenario import Scenario
-from causal_testing.specification.causal_specification import CausalSpecification
+from causal_testing.testing.causal_test_case import CausalTestCase
+from causal_testing.testing.base_test_case import BaseTestCase
+from causal_testing.specification.variable import Input, Output
+from causal_testing.testing.causal_test_outcome import ExactValue
+from causal_testing.testing.estimators import CausalForestEstimator, LinearRegressionEstimator
+from causal_testing.specification.causal_specification import CausalSpecification, Scenario
+from causal_testing.data_collection.data_collector import ObservationalDataCollector
+from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
+from causal_testing.specification.causal_dag import CausalDAG
 
 
-class TestCausalTestAdequacy(unittest.TestCase):
-    """
-    Test the causal test adequacy metrics. These provide metrics determine how comprehensive a test set is and,
-    ultimately whether we can stop testing.
-    """
+class TestCausalTestSuite(unittest.TestCase):
+    """Test the Test Suite object and it's implementation in the test engine using dummy data."""
 
     def setUp(self) -> None:
-        json_file_name = "tests.json"
-        dag_file_name = "dag.dot"
-        data_file_name = "data_with_categorical.csv"
-        test_data_dir_path = Path("tests/resources/data")
-        self.json_path = str(test_data_dir_path / json_file_name)
-        self.dag_path = str(test_data_dir_path / dag_file_name)
-        self.data_path = [str(test_data_dir_path / data_file_name)]
-        self.json_class = JsonUtility("temp_out.txt", True)
-        self.example_distribution = scipy.stats.uniform(1, 10)
-        self.input_dict_list = [
-            {"name": "test_input", "datatype": float, "distribution": self.example_distribution},
-            {"name": "test_input_no_dist", "datatype": float},
+        # 1. Create dummy Scenario and BaseTestCase
+        A = Input("A", float)
+        self.A = A
+        C = Output("C", float)
+        self.C = C
+        D = Output("D", float)
+        self.D = D
+        self.base_test_case = BaseTestCase(A, C)
+        self.scenario = Scenario({A, C, D})
+
+        # 2. Create DAG and dummy data and write to csvs
+        temp_dir_path = create_temp_dir_if_non_existent()
+        dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        dag_dot = """digraph G { A -> C; D -> A; D -> C}"""
+        with open(dag_dot_path, "w") as file:
+            file.write(dag_dot)
+
+        np.random.seed(1)
+        df = pd.DataFrame({"D": list(np.random.normal(60, 10, 1000))})  # D = exogenous
+        df["A"] = [1 if d > 50 else 0 for d in df["D"]]
+        df["C"] = df["D"] + (4 * (df["A"] + 2))  # C = (4*(A+2)) + D
+        self.df = df
+        self.causal_dag = CausalDAG(dag_dot_path)
+
+        # 3. Specify data structures required for test suite
+        self.expected_causal_effect = ExactValue(4)
+        test_list = [
+            CausalTestCase(
+                self.base_test_case,
+                self.expected_causal_effect,
+                0,
+                1,
+            ),
+            CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 2),
         ]
-        self.output_dict_list = [{"name": "test_output", "datatype": float}]
-        variables = CausalVariables(inputs=self.input_dict_list, outputs=self.output_dict_list, metas=[])
-        self.scenario = Scenario(variables=variables, constraints=None)
-        self.json_class.set_paths(self.json_path, self.dag_path, self.data_path)
-        self.json_class.setup(self.scenario)
-
-    def test_data_adequacy_numeric(self):
-        example_test = {
-            "tests": [
-                {
-                    "name": "test1",
-                    "mutations": {"test_input": "Increase"},
-                    "estimator": "LinearRegressionEstimator",
-                    "estimate_type": "coefficient",
-                    "effect_modifiers": [],
-                    "expected_effect": {"test_output": "NoEffect"},
-                    "coverage": True,
-                    "skip": False,
-                }
-            ]
-        }
-        self.json_class.test_plan = example_test
-        effects = {"NoEffect": NoEffect()}
-        mutates = {
-            "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
-        }
-        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+        self.estimators = [LinearRegressionEstimator]
 
-        test_results = self.json_class.run_json_tests(
-            effects=effects, estimators=estimators, f_flag=False, mutates=mutates
-        )
-        self.assertEqual(
-            test_results[0]["result"].adequacy.to_dict(),
-            {"kurtosis": {"test_input": 0.0}, "bootstrap_size": 100, "passing": 100},
+        # 3. Create test_suite and add a test
+        self.test_suite = CausalTestSuite()
+        self.test_suite.add_test_object(
+            base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=self.estimators
         )
+        self.causal_specification = CausalSpecification(self.scenario, self.causal_dag)
 
-    def test_data_adequacy_cateogorical(self):
-        example_test = {
-            "tests": [
-                {
-                    "name": "test1",
-                    "mutations": ["test_input_no_dist"],
-                    "estimator": "LinearRegressionEstimator",
-                    "estimate_type": "coefficient",
-                    "effect_modifiers": [],
-                    "expected_effect": {"test_output": "NoEffect"},
-                    "coverage": True,
-                    "skip": False,
-                }
-            ]
-        }
-        self.json_class.test_plan = example_test
-        effects = {"NoEffect": NoEffect()}
-        mutates = {
-            "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
-        }
-        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
-
-        test_results = self.json_class.run_json_tests(
-            effects=effects, estimators=estimators, f_flag=False, mutates=mutates
-        )
-        print("RESULT")
-        print(test_results[0]["result"])
-        self.assertEqual(
-            test_results[0]["result"].adequacy.to_dict(),
-            {"kurtosis": {"test_input_no_dist[T.b]": 0.0}, "bootstrap_size": 100, "passing": 100},
-        )
+        self.data_collector = ObservationalDataCollector(self.scenario, self.df)
 
-    def test_dag_adequacy(self):
-        base_test_case = BaseTestCase(
-            treatment_variable="test_input",
-            outcome_variable="test_output",
-            effect=None,
-        )
-        causal_test_case = CausalTestCase(
-            base_test_case=base_test_case,
-            expected_causal_effect=None,
-            estimate_type=None,
-        )
+    def test_adding_test_object(self):
+        "test an object can be added to the test_suite using the add_test_object function"
         test_suite = CausalTestSuite()
-        test_suite.add_test_object(base_test_case, causal_test_case, None, None)
-        dag_adequacy = DAGAdequacy(self.json_class.causal_specification.causal_dag, test_suite)
-        dag_adequacy.measure_adequacy()
-        print(dag_adequacy.to_dict())
-        self.assertEqual(
-            dag_adequacy.to_dict(),
-            {
-                "causal_dag": self.json_class.causal_specification.causal_dag,
-                "test_suite": test_suite,
-                "tested_pairs": {("test_input", "test_output")},
-                "pairs_to_test": {
-                    ("test_input_no_dist", "test_input"),
-                    ("test_input", "B"),
-                    ("test_input_no_dist", "C"),
-                    ("test_input_no_dist", "B"),
-                    ("test_input", "C"),
-                    ("B", "C"),
-                    ("test_input_no_dist", "test_output"),
-                    ("test_input", "test_output"),
-                    ("C", "test_output"),
-                    ("B", "test_output"),
-                },
-                "untested_edges": {
-                    ("test_input_no_dist", "test_input"),
-                    ("test_input", "B"),
-                    ("test_input_no_dist", "C"),
-                    ("test_input_no_dist", "B"),
-                    ("test_input", "C"),
-                    ("B", "C"),
-                    ("test_input_no_dist", "test_output"),
-                    ("C", "test_output"),
-                    ("B", "test_output"),
-                },
-                "dag_adequacy": 0.1,
-            },
+        test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
+        estimators = [LinearRegressionEstimator]
+        test_suite.add_test_object(
+            base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
         )
+        manual_test_object = {
+            self.base_test_case: {"tests": test_list, "estimators": estimators, "estimate_type": "ate"}
+        }
+        self.assertEqual(test_suite, manual_test_object)
 
-    def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
-        if os.path.exists("temp_out.txt"):
-            os.remove("temp_out.txt")
+    def test_return_single_test_object(self):
+        """Test that a single test case can be returned from the test_suite"""
+        base_test_case = BaseTestCase(self.A, self.D)
+
+        test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
+        estimators = [LinearRegressionEstimator]
+        self.test_suite.add_test_object(
+            base_test_case=base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
+        )
+
+        manual_test_case = {"tests": test_list, "estimators": estimators, "estimate_type": "ate"}
+
+        test_case = self.test_suite[base_test_case]
+
+        self.assertEqual(test_case, manual_test_case)
+
+    def test_execute_test_suite_single_base_test_case(self):
+        """Check that the test suite can return the correct results from dummy data for a single base_test-case"""
+
+        causal_test_results = self.test_suite.execute_test_suite(self.data_collector, self.causal_specification)
+        causal_test_case_result = causal_test_results[self.base_test_case]
+        self.assertAlmostEqual(causal_test_case_result["LinearRegressionEstimator"][0].test_value.value, 4, delta=1e-10)
+
+    def test_execute_test_suite_multiple_estimators(self):
+        """Check that executing a test suite with multiple estimators returns correct results for the dummy data
+        for each estimator
+        """
+        estimators = [LinearRegressionEstimator, CausalForestEstimator]
+        test_suite_2_estimators = CausalTestSuite()
+        test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
+        test_suite_2_estimators.add_test_object(
+            base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
+        )
+        causal_test_results = test_suite_2_estimators.execute_test_suite(self.data_collector, self.causal_specification)
+        causal_test_case_result = causal_test_results[self.base_test_case]
+        linear_regression_result = causal_test_case_result["LinearRegressionEstimator"][0]
+        causal_forrest_result = causal_test_case_result["CausalForestEstimator"][0]
+        self.assertAlmostEqual(linear_regression_result.test_value.value, 4, delta=1e-1)
+        self.assertAlmostEqual(causal_forrest_result.test_value.value, 4, delta=1e-1)
```

### Comparing `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-5.1.1/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-5.1.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-5.1.1/tests/testing_tests/test_estimators.py`

 * *Files identical despite different names*

