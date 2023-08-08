# Comparing `tmp/asreview-1.3a1.tar.gz` & `tmp/asreview-1.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-1.3a1.tar", last modified: Tue Jul 18 11:21:02 2023, max compression
+gzip compressed data, was "asreview-1.3rc0.tar", last modified: Tue Aug  8 12:57:30 2023, max compression
```

## Comparing `asreview-1.3a1.tar` & `asreview-1.3rc0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-18 11:18:58.000000 asreview-1.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 11:18:58.000000 asreview-1.3a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-18 11:21:02.004891 asreview-1.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-18 11:18:58.000000 asreview-1.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.008891 asreview-1.3a1/asreview/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 11:21:02.008891 asreview-1.3a1/asreview/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:01.996891 asreview-1.3a1/asreview/data/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:01.996891 asreview-1.3a1/asreview/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/auth_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/entry_points/state_inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:01.996891 asreview-1.3a1/asreview/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/paper_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/ris_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/ris_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/tsv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:01.996891 asreview-1.3a1/asreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/models/balance/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/triple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/undersample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/balance/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/models/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/logistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/lstm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/lstm_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/nb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/nn_2_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/rf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/classifiers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/models/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/embedding_idf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/embedding_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/sbert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/feature_extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/models/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/models/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/review/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/review/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/review/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/state/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.000891 asreview-1.3a1/asreview/state/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/sql_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    42551 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/state/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/api/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    50917 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/api/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/authentication/login_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/authentication/oauth_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4561 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/run_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/start_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/integration_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18164 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_api/test_webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_collaboration_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_database_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_project_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_user_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/test_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/test_extensions/test_auth_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:02.004891 asreview-1.3a1/asreview/webapp/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/utils/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/utils/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-18 11:18:58.000000 asreview-1.3a1/asreview/webapp/tests/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:21:01.996891 asreview-1.3a1/asreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 11:21:01.000000 asreview-1.3a1/asreview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 11:21:02.008891 asreview-1.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-18 11:18:58.000000 asreview-1.3a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68752 2023-07-18 11:18:58.000000 asreview-1.3a1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-08 12:55:04.000000 asreview-1.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-08 12:55:04.000000 asreview-1.3rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-08-08 12:57:30.174348 asreview-1.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-08-08 12:55:04.000000 asreview-1.3rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.162347 asreview-1.3rc0/asreview/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.162347 asreview-1.3rc0/asreview/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/auth_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/entry_points/state_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.162347 asreview-1.3rc0/asreview/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/paper_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/ris_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/ris_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/tsv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.166348 asreview-1.3rc0/asreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.166348 asreview-1.3rc0/asreview/models/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/triple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/undersample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/balance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.166348 asreview-1.3rc0/asreview/models/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/lstm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/lstm_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/nn_2_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/classifiers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.166348 asreview-1.3rc0/asreview/models/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/embedding_idf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/embedding_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/feature_extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/models/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/models/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/review/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/review/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/review/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/state/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/sql_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42551 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/state/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/webapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50833 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/api/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.170348 asreview-1.3rc0/asreview/webapp/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/authentication/login_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/authentication/oauth_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4561 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/start_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18164 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_api/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_collaboration_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_database_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_project_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/test_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/test_extensions/test_auth_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.174348 asreview-1.3rc0/asreview/webapp/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/utils/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/utils/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-08 12:55:04.000000 asreview-1.3rc0/asreview/webapp/tests/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:57:30.162347 asreview-1.3rc0/asreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 12:57:30.000000 asreview-1.3rc0/asreview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 12:57:30.174348 asreview-1.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-08-08 12:55:04.000000 asreview-1.3rc0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68752 2023-08-08 12:55:04.000000 asreview-1.3rc0/versioneer.py
```

### Comparing `asreview-1.3a1/LICENSE` & `asreview-1.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/PKG-INFO` & `asreview-1.3rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview
-Version: 1.3a1
+Version: 1.3rc0
 Summary: ASReview LAB - A tool for AI-assisted systematic reviews
 Home-page: https://github.com/asreview/asreview
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
 Project-URL: Source, https://github.com/asreview/asreview/
 Keywords: systematic review,machine-learning
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.3a1 Summary: ASReview LAB - A
+Metadata-Version: 2.1 Name: asreview Version: 1.3rc0 Summary: ASReview LAB - A
 tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
 asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
 URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
 Source, https://github.com/asreview/asreview/ Keywords: systematic
 review,machine-learning Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `asreview-1.3a1/README.md` & `asreview-1.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/__init__.py` & `asreview-1.3rc0/asreview/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/__main__.py` & `asreview-1.3rc0/asreview/__main__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/_deprecated.py` & `asreview-1.3rc0/asreview/_deprecated.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/compat.py` & `asreview-1.3rc0/asreview/compat.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/config.py` & `asreview-1.3rc0/asreview/config.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/data/__init__.py` & `asreview-1.3rc0/asreview/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/data/base.py` & `asreview-1.3rc0/asreview/data/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
+from io import StringIO
 from pathlib import Path
-from urllib.error import HTTPError
-from urllib.parse import urlparse
-from urllib.request import urlopen
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from asreview.config import COLUMN_DEFINITIONS
@@ -28,14 +26,15 @@
 from asreview.datasets import DatasetManager
 from asreview.datasets import DatasetNotFoundError
 from asreview.exceptions import BadFileFormatError
 from asreview.io import PaperRecord
 from asreview.io.utils import convert_keywords
 from asreview.io.utils import type_from_column
 from asreview.utils import _entry_points
+from asreview.utils import _get_filename_from_url
 from asreview.utils import is_iterable
 from asreview.utils import is_url
 
 
 def load_data(name, *args, **kwargs):
     """Load data from file, URL, or plugin.
 
@@ -50,43 +49,24 @@
         Inititalized ASReview data object.
     """
 
     # check is file or URL
     if is_url(name) or Path(name).exists():
         return ASReviewData.from_file(name, *args, **kwargs)
 
-    # check if dataset is plugin dataset\
+    # check if dataset is plugin dataset
     try:
-        dataset_path = DatasetManager().find(name).filepath
-        return ASReviewData.from_file(dataset_path, *args, **kwargs)
+        return ASReviewData.from_extension(name, *args, **kwargs)
     except DatasetNotFoundError:
         pass
 
     # Could not find dataset, return None.
     raise FileNotFoundError(f"File, URL, or dataset does not exist: '{name}'")
 
 
-def _get_filename_from_url(url):
-    if not is_url(url):
-        raise ValueError(f"'{url}' is not a valid URL.")
-
-    if Path(urlparse(url).path).suffix:
-        return Path(urlparse(url).path).name, url
-    else:
-        try:
-            return urlopen(url).headers.get_filename(), url
-        except HTTPError as err:
-            # 308 (Permanent Redirect) not supported
-            # See https://bugs.python.org/issue40321
-            if err.code == 308:
-                return _get_filename_from_url(err.headers.get("Location"))
-            else:
-                raise err
-
-
 class ASReviewData:
     """Data object to the dataset with texts, labels, DOIs etc.
 
     Arguments
     ---------
     df: pandas.DataFrame
         Dataframe containing the data for the ASReview data object.
@@ -125,15 +105,14 @@
         Identical to included.
 
     """
 
     def __init__(self, df=None, column_spec=None):
         self.df = df
         self.prior_idx = np.array([], dtype=int)
-
         self.max_idx = max(df.index.values) + 1
 
         # Infer column specifications if it is not given.
         if column_spec is None:
             self.column_spec = {}
             for col_name in list(df):
                 data_type = type_from_column(col_name, COLUMN_DEFINITIONS)
@@ -185,28 +164,66 @@
         """
 
         if reader is not None:
             return cls(reader.read_data(fp))
 
         # get the filename from a url else file path
         if is_url(fp):
-            fn, fp = _get_filename_from_url(fp)
+            fn = _get_filename_from_url(fp)
         else:
             fn = Path(fp).name
 
         try:
             reader = _entry_points(
                 group="asreview.readers")[Path(fn).suffix].load()
         except Exception:
             raise BadFileFormatError(f"Importing file {fp} not possible.")
 
         df, column_spec = reader.read_data(fp)
 
         return cls(df, column_spec=column_spec)
 
+    @classmethod
+    def from_extension(cls, name, reader=None):
+        """Load a dataset from extension.
+
+        Arguments
+        ---------
+        fp: str, pathlib.Path
+            Read the data from this file or url.
+        reader: class
+            Reader to import the file.
+        """
+
+        dataset = DatasetManager().find(name)
+
+        if dataset.filepath:
+            fp = dataset.filepath
+        else:
+            # build dataset to temporary file
+            reader = dataset.reader()
+            fp = StringIO(dataset.to_file())
+
+        if reader is None:
+            # get the filename from a url else file path
+            if is_url(fp):
+                fn = _get_filename_from_url(fp)
+            else:
+                fn = Path(fp).name
+
+            try:
+                reader = _entry_points(
+                    group="asreview.readers")[Path(fn).suffix].load()
+            except Exception:
+                raise BadFileFormatError(f"Importing file {fp} not possible.")
+
+        df, column_spec = reader.read_data(fp)
+
+        return cls(df, column_spec=column_spec)
+
     def record(self, i, by_index=True):
         """Create a record from an index.
 
         Arguments
         ---------
         i: int, iterable
             Index of the record, or list of indices.
```

### Comparing `asreview-1.3a1/asreview/data/statistics.py` & `asreview-1.3rc0/asreview/data/statistics.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/__init__.py` & `asreview-1.3rc0/asreview/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/algorithms.py` & `asreview-1.3rc0/asreview/entry_points/algorithms.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/auth_tool.py` & `asreview-1.3rc0/asreview/entry_points/auth_tool.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/base.py` & `asreview-1.3rc0/asreview/entry_points/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/lab.py` & `asreview-1.3rc0/asreview/entry_points/lab.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/simulate.py` & `asreview-1.3rc0/asreview/entry_points/simulate.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/entry_points/state_inspect.py` & `asreview-1.3rc0/asreview/entry_points/state_inspect.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/exceptions.py` & `asreview-1.3rc0/asreview/exceptions.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/__init__.py` & `asreview-1.3rc0/asreview/io/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/csv_reader.py` & `asreview-1.3rc0/asreview/io/csv_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/csv_writer.py` & `asreview-1.3rc0/asreview/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/excel_reader.py` & `asreview-1.3rc0/asreview/io/excel_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/excel_writer.py` & `asreview-1.3rc0/asreview/io/excel_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/paper_record.py` & `asreview-1.3rc0/asreview/io/paper_record.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/ris_reader.py` & `asreview-1.3rc0/asreview/io/ris_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/ris_writer.py` & `asreview-1.3rc0/asreview/io/ris_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/tsv_writer.py` & `asreview-1.3rc0/asreview/io/tsv_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/io/utils.py` & `asreview-1.3rc0/asreview/io/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/__init__.py` & `asreview-1.3rc0/asreview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/__init__.py` & `asreview-1.3rc0/asreview/models/balance/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/base.py` & `asreview-1.3rc0/asreview/models/balance/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/double.py` & `asreview-1.3rc0/asreview/models/balance/double.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/simple.py` & `asreview-1.3rc0/asreview/models/balance/simple.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/triple.py` & `asreview-1.3rc0/asreview/models/balance/triple.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/undersample.py` & `asreview-1.3rc0/asreview/models/balance/undersample.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/balance/utils.py` & `asreview-1.3rc0/asreview/models/balance/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/base.py` & `asreview-1.3rc0/asreview/models/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/__init__.py` & `asreview-1.3rc0/asreview/models/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/base.py` & `asreview-1.3rc0/asreview/models/classifiers/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/logistic.py` & `asreview-1.3rc0/asreview/models/classifiers/logistic.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/lstm_base.py` & `asreview-1.3rc0/asreview/models/classifiers/lstm_base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/lstm_pool.py` & `asreview-1.3rc0/asreview/models/classifiers/lstm_pool.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/nb.py` & `asreview-1.3rc0/asreview/models/classifiers/nb.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/nn_2_layer.py` & `asreview-1.3rc0/asreview/models/classifiers/nn_2_layer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/rf.py` & `asreview-1.3rc0/asreview/models/classifiers/rf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/svm.py` & `asreview-1.3rc0/asreview/models/classifiers/svm.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/classifiers/utils.py` & `asreview-1.3rc0/asreview/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/__init__.py` & `asreview-1.3rc0/asreview/models/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/base.py` & `asreview-1.3rc0/asreview/models/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/doc2vec.py` & `asreview-1.3rc0/asreview/models/feature_extraction/doc2vec.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/embedding_idf.py` & `asreview-1.3rc0/asreview/models/feature_extraction/embedding_idf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/embedding_lstm.py` & `asreview-1.3rc0/asreview/models/feature_extraction/embedding_lstm.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/sbert.py` & `asreview-1.3rc0/asreview/models/feature_extraction/sbert.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/tfidf.py` & `asreview-1.3rc0/asreview/models/feature_extraction/tfidf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/feature_extraction/utils.py` & `asreview-1.3rc0/asreview/models/feature_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/__init__.py` & `asreview-1.3rc0/asreview/models/query/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/base.py` & `asreview-1.3rc0/asreview/models/query/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/cluster.py` & `asreview-1.3rc0/asreview/models/query/cluster.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/max.py` & `asreview-1.3rc0/asreview/models/query/max.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/mixed.py` & `asreview-1.3rc0/asreview/models/query/mixed.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/random.py` & `asreview-1.3rc0/asreview/models/query/random.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/uncertainty.py` & `asreview-1.3rc0/asreview/models/query/uncertainty.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/models/query/utils.py` & `asreview-1.3rc0/asreview/models/query/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/project.py` & `asreview-1.3rc0/asreview/project.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/review/__init__.py` & `asreview-1.3rc0/asreview/review/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/review/base.py` & `asreview-1.3rc0/asreview/review/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/review/simulate.py` & `asreview-1.3rc0/asreview/review/simulate.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/search.py` & `asreview-1.3rc0/asreview/search.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/settings.py` & `asreview-1.3rc0/asreview/settings.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/__init__.py` & `asreview-1.3rc0/asreview/state/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/base.py` & `asreview-1.3rc0/asreview/state/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/errors.py` & `asreview-1.3rc0/asreview/state/errors.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/legacy/base.py` & `asreview-1.3rc0/asreview/state/legacy/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/legacy/dict.py` & `asreview-1.3rc0/asreview/state/legacy/dict.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/legacy/hdf5.py` & `asreview-1.3rc0/asreview/state/legacy/hdf5.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/legacy/json.py` & `asreview-1.3rc0/asreview/state/legacy/json.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/legacy/utils.py` & `asreview-1.3rc0/asreview/state/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/sql_converter.py` & `asreview-1.3rc0/asreview/state/sql_converter.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/sqlstate.py` & `asreview-1.3rc0/asreview/state/sqlstate.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/state/utils.py` & `asreview-1.3rc0/asreview/state/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/types.py` & `asreview-1.3rc0/asreview/types.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/utils.py` & `asreview-1.3rc0/asreview/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 # limitations under the License.
 
 import functools
 import os
 import sys
 import warnings
 from pathlib import Path
+from urllib.error import HTTPError
 from urllib.parse import urlparse
+from urllib.request import urlopen
 
 import numpy as np
 
 from asreview._deprecated import _deprecated_func
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import entry_points as _entry_points
@@ -119,14 +121,32 @@
                     warnings.warn(f"Keyword argument '{k}' is deprecated. Use '{kwarg_map[k]}' instead.", DeprecationWarning)  # noqa
                 new_kwargs[kwarg_map.get(k, k)] = v
             return func(*args, **new_kwargs)
         return wrapper
     return dec
 
 
+def _get_filename_from_url(url):
+    if not is_url(url):
+        raise ValueError(f"'{url}' is not a valid URL.")
+
+    if Path(urlparse(url).path).suffix:
+        return Path(urlparse(url).path).name
+    else:
+        try:
+            return urlopen(url).headers.get_filename()
+        except HTTPError as err:
+            # 308 (Permanent Redirect) not supported
+            # See https://bugs.python.org/issue40321
+            if err.code == 308:
+                return _get_filename_from_url(err.headers.get("Location"))
+            else:
+                raise err
+
+
 def asreview_path():
     """Get the location where projects are stored.
 
     Overwrite this location by specifying the ASREVIEW_PATH enviroment
     variable.
     """
     if os.environ.get("ASREVIEW_PATH", None):
@@ -240,15 +260,16 @@
     return {entry.name: entry for entry in _entry_points(group=entry_name)}
 
 
 def is_url(url):
     """Check if object is a valid url."""
     try:
         result = urlparse(url)
-        return all(getattr(result, x) != "" for x in ["scheme", "netloc", "path"])
+        return all(
+            getattr(result, x) not in [b"", ""] for x in ["scheme", "netloc", "path"])
     except Exception:
         return False
 
 
 def get_random_state(random_state):
     """Create a RandomState instance.
```

### Comparing `asreview-1.3a1/asreview/webapp/__init__.py` & `asreview-1.3rc0/asreview/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/api/__init__.py` & `asreview-1.3rc0/asreview/webapp/api/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/api/auth.py` & `asreview-1.3rc0/asreview/webapp/api/auth.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/api/projects.py` & `asreview-1.3rc0/asreview/webapp/api/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from asreview.config import DEFAULT_BALANCE_STRATEGY
 from asreview.config import DEFAULT_FEATURE_EXTRACTION
 from asreview.config import DEFAULT_MODEL
 from asreview.config import DEFAULT_QUERY_STRATEGY
 from asreview.config import PROJECT_MODE_EXPLORE
 from asreview.config import PROJECT_MODE_SIMULATE
 from asreview.data import ASReviewData
-from asreview.data.base import _get_filename_from_url
 from asreview.data.statistics import n_duplicates
 from asreview.datasets import DatasetManager
 from asreview.exceptions import BadFileFormatError
 from asreview.io import list_readers
 from asreview.io import list_writers
 from asreview.models.balance import get_balance_model
 from asreview.models.balance import list_balance_strategies
@@ -67,14 +66,15 @@
 from asreview.search import fuzzy_find
 from asreview.settings import ASReviewSettings
 from asreview.state.errors import StateError
 from asreview.state.errors import StateNotFoundError
 from asreview.state.sql_converter import upgrade_asreview_project_file
 from asreview.state.sql_converter import upgrade_project_config
 from asreview.utils import _get_executable
+from asreview.utils import _get_filename_from_url
 from asreview.utils import asreview_path
 from asreview.utils import list_reader_names
 from asreview.webapp import DB
 from asreview.webapp.authentication.login_required import app_is_authenticated
 from asreview.webapp.authentication.login_required import asreview_login_required
 from asreview.webapp.authentication.login_required import project_authorization
 from asreview.webapp.authentication.models import Project
@@ -311,15 +311,15 @@
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to load plugin datasets."), 500
 
     elif subset == "benchmark":
         try:
             # collect the datasets metadata
-            result_datasets = manager.list(include=["benchmark-nature", "benchmark"])
+            result_datasets = manager.list(include=["synergy", "benchmark-nature"])
 
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to load benchmark datasets."), 500
 
     else:
         response = jsonify(message="demo-data-loading-failed")
@@ -346,29 +346,31 @@
         logging.warning("Removing old dataset and adding new dataset.")
         project.remove_dataset()
 
     # create dataset folder if not present
     Path(project.project_path, "data").mkdir(exist_ok=True)
 
     if request.form.get("plugin", None):
-        url = DatasetManager().find(request.form["plugin"]).filepath
-        filename, url = _get_filename_from_url(url)
+        ds = DatasetManager().find(request.form["plugin"])
+        filename = ds.filename
+        ds.to_file(Path(project.project_path, "data", filename))
+
+    elif request.form.get("benchmark", None):
+        ds = DatasetManager().find(request.form["benchmark"])
+        filename = ds.filename
+        ds.to_file(Path(project.project_path, "data", filename))
 
-    if request.form.get("benchmark", None):
-        url = DatasetManager().find(request.form["benchmark"]).filepath
-        filename, url = _get_filename_from_url(url)
-
-    if request.form.get("url", None):
+    elif request.form.get("url", None):
         url = request.form.get("url")
 
         # check if url value is actually DOI without netloc
         if url.startswith("10."):
             url = f"https://doi.org/{url}"
 
-        filename, url = _get_filename_from_url(url)
+        filename = _get_filename_from_url(url)
 
         if bool(request.form.get("validate", None)):
             reader_keys = list_reader_names()
 
             if (
                 filename
                 and Path(filename).suffix
@@ -388,19 +390,14 @@
                             Path(files[i]["name"]).suffix not in reader_keys
                         )
 
                     return jsonify(files=files), 201
                 except Exception:
                     raise BadFileFormatError("Can't retrieve files.")
 
-    if (
-        request.form.get("plugin", None)
-        or request.form.get("benchmark", None)
-        or request.form.get("url", None)
-    ):
         try:
             urlretrieve(url, Path(project.project_path, "data") / filename)
         except Exception as err:
             logging.error(err)
             message = f"Can't retrieve data from URL {url}."
 
             return jsonify(message=message), 400
```

### Comparing `asreview-1.3a1/asreview/webapp/api/team.py` & `asreview-1.3rc0/asreview/webapp/api/team.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/authentication/__init__.py` & `asreview-1.3rc0/asreview/webapp/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/authentication/login_required.py` & `asreview-1.3rc0/asreview/webapp/authentication/login_required.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/authentication/models.py` & `asreview-1.3rc0/asreview/webapp/authentication/models.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/authentication/oauth_handler.py` & `asreview-1.3rc0/asreview/webapp/authentication/oauth_handler.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/io.py` & `asreview-1.3rc0/asreview/webapp/io.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/run_model.py` & `asreview-1.3rc0/asreview/webapp/run_model.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/start_flask.py` & `asreview-1.3rc0/asreview/webapp/start_flask.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
-import json
 import logging
 import os
 import socket
 import webbrowser
 from pathlib import Path
 from threading import Timer
 
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
+
 from flask import Flask
 from flask import send_from_directory
 from flask.json import jsonify
 from flask.templating import render_template
 from flask_cors import CORS
 from flask_login import LoginManager
 from gevent.pywsgi import WSGIServer
@@ -108,20 +112,19 @@
         f"Start browser at {start_url}"
         "\n\n\n\nIf your browser doesn't open. "
         f"Please navigate to '{start_url}'\n\n\n\n"
     )
 
 
 def _lab_parser():
-
     # parse arguments if available
     parser = argparse.ArgumentParser(
         prog="lab",
         description="""ASReview LAB - Active learning for Systematic Reviews.""",  # noqa
-        formatter_class=argparse.RawTextHelpFormatter
+        formatter_class=argparse.RawTextHelpFormatter,
     )
 
     parser.add_argument(
         "--clean-project",
         dest="clean_project",
         default=None,
         type=str,
@@ -179,15 +182,15 @@
         help="When using authentication, a salt code is needed" "for hasing passwords.",
     )
 
     parser.add_argument(
         "--flask-configfile",
         default="",
         type=str,
-        help="Full path to a JSON file containing Flask parameters"
+        help="Full path to a TOML file containing Flask parameters"
         "for authentication.",
     )
 
     parser.add_argument(
         "--no-browser",
         dest="no_browser",
         action="store_true",
@@ -260,15 +263,21 @@
     app.config["HOST"] = kwargs.get("host")
 
     # Read config parameters if possible, this overrides
     # the previous assignments.
     config_file_path = kwargs.get("flask_configfile", "").strip()
     # Use absolute path, because otherwise it is relative to the config root.
     if config_file_path != "":
-        app.config.from_file(Path(config_file_path).absolute(), load=json.load)
+        config_file_path = Path(config_file_path)
+        if config_file_path.suffix == ".toml":
+            app.config.from_file(
+                config_file_path.absolute(), load=tomllib.load, text=False
+            )
+        else:
+            raise ValueError("'flask_configfile' should have a .toml extension")
 
     # If the frontend runs on a different port, or even on a different
     # URL, then allowed-origins must be set to avoid CORS issues. You can
     # set the allowed-origins in the config file. In the previous lines
     # the config file has been read.
     # If the allowed-origins are not set by now, they are set to
     # False, which will bypass setting any CORS parameters!
@@ -357,19 +366,15 @@
         pass
 
     # We only need CORS if they are necessary: when the frontend is
     # running on a different port, or even url, we need to set the
     # allowed origins to avoid CORS problems. The allowed-origins
     # can be set in the config file.
     if app.config.get("ALLOWED_ORIGINS", False):
-        CORS(
-            app,
-            origins=app.config.get("ALLOWED_ORIGINS"),
-            supports_credentials=True
-        )
+        CORS(app, origins=app.config.get("ALLOWED_ORIGINS"), supports_credentials=True)
 
     with app.app_context():
         app.register_blueprint(projects.bp)
         app.register_blueprint(auth.bp)
         app.register_blueprint(team.bp)
 
     @app.errorhandler(InternalServerError)
```

### Comparing `asreview-1.3a1/asreview/webapp/tests/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/config/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/config/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/conftest.py` & `asreview-1.3rc0/asreview/webapp/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 def _get_app(app_type="auth-basic", path=None):
     """Create and returns test flask app based on app_type"""
     # set asreview path
     os.environ.update({"ASREVIEW_PATH": path})
     # get path of appropriate flask config
     base_dir = Path(__file__).resolve().parent / "config"
     if app_type == "auth-basic":
-        config_path = str(base_dir / "auth_basic_config.json")
+        config_path = str(base_dir / "auth_basic_config.toml")
     elif app_type == "auth-no-creation":
-        config_path = str(base_dir / "auth_no_creation.json")
+        config_path = str(base_dir / "auth_no_creation.toml")
     elif app_type == "auth-verified":
-        config_path = str(base_dir / "auth_verified_config.json")
+        config_path = str(base_dir / "auth_verified_config.toml")
     elif app_type == "no-auth":
-        config_path = str(base_dir / "no_auth_config.json")
+        config_path = str(base_dir / "no_auth_config.toml")
     else:
         raise ValueError(f"Unknown config {app_type}")
     # create app
     app = create_app(flask_configfile=config_path)
     # and return it
     return app
```

### Comparing `asreview-1.3a1/asreview/webapp/tests/data/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/integration_tests/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/conftest.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/conftest.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/test_auth.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/test_auth.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/test_projects.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/test_projects.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/test_teams.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/test_teams.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_api/test_webapp.py` & `asreview-1.3rc0/asreview/webapp/tests/test_api/test_webapp.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/conftest.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/conftest.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_collaboration_models.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_collaboration_models.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_database_creation.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_database_creation.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_project_model.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_project_model.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_database_and_models/test_user_model.py` & `asreview-1.3rc0/asreview/webapp/tests/test_database_and_models/test_user_model.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_extensions/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/test_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/test_extensions/test_auth_tool.py` & `asreview-1.3rc0/asreview/webapp/tests/test_extensions/test_auth_tool.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/utils/__init__.py` & `asreview-1.3rc0/asreview/webapp/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/utils/api_utils.py` & `asreview-1.3rc0/asreview/webapp/tests/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/utils/config_parser.py` & `asreview-1.3rc0/asreview/webapp/tests/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/utils/crud.py` & `asreview-1.3rc0/asreview/webapp/tests/utils/crud.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview/webapp/tests/utils/misc.py` & `asreview-1.3rc0/asreview/webapp/tests/utils/misc.py`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview.egg-info/PKG-INFO` & `asreview-1.3rc0/asreview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview
-Version: 1.3a1
+Version: 1.3rc0
 Summary: ASReview LAB - A tool for AI-assisted systematic reviews
 Home-page: https://github.com/asreview/asreview
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
 Project-URL: Source, https://github.com/asreview/asreview/
 Keywords: systematic review,machine-learning
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.3a1 Summary: ASReview LAB - A
+Metadata-Version: 2.1 Name: asreview Version: 1.3rc0 Summary: ASReview LAB - A
 tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
 asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
 URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
 Source, https://github.com/asreview/asreview/ Keywords: systematic
 review,machine-learning Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `asreview-1.3a1/asreview.egg-info/SOURCES.txt` & `asreview-1.3rc0/asreview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asreview-1.3a1/asreview.egg-info/entry_points.txt` & `asreview-1.3rc0/asreview.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [asreview.datasets]
 benchmark = asreview.datasets:BenchmarkDataGroup
 benchmark-nature = asreview.datasets:NaturePublicationDataGroup
+synergy = asreview.datasets:SynergyDataGroup
 
 [asreview.entry_points]
 algorithms = asreview.entry_points:AlgorithmsEntryPoint
 auth-tool = asreview.entry_points:AuthTool
 lab = asreview.entry_points:LABEntryPoint
 simulate = asreview.entry_points:SimulateEntryPoint
 state-inspect = asreview.entry_points:StateInspectEntryPoint
```

### Comparing `asreview-1.3a1/setup.py` & `asreview-1.3rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,33 @@
 REQUIRES = [
     "numpy",
     "pandas>=1,<3",
     "scikit-learn",
     "rispy~=0.7.0",
     "xlrd>=1.0.0",
     "setuptools",
-    "flask>=2.0",
+    "flask>=2.3.0",
     "flask_cors",
     "flask-login",
     "flask-mail",
     "openpyxl",
     "jsonschema",
     "filelock",
     "Flask-SQLAlchemy>=3.0.2",
     "requests",
     "tqdm",
     "gevent>=20",
     "datahugger>=0.2",
+    "synergy_dataset"
 ]
 
+if sys.version_info < (3, 11):
+    REQUIRES += ["tomli"]
+
+
 if sys.version_info < (3, 10):
     REQUIRES += ["importlib_metadata>=3.6"]
 
 
 DEPS = {
     "sbert": ["sentence_transformers"],
     "doc2vec": ["gensim"],
@@ -181,14 +186,15 @@
             ".ris = asreview.io:RISWriter",
             ".txt = asreview.io:RISWriter",
             ".xlsx = asreview.io:ExcelWriter",
         ],
         "asreview.datasets": [
             "benchmark = asreview.datasets:BenchmarkDataGroup",
             "benchmark-nature = asreview.datasets:NaturePublicationDataGroup",
+            "synergy = asreview.datasets:SynergyDataGroup"
         ],
         "asreview.models.classifiers": [
             "svm = asreview.models.classifiers:SVMClassifier",
             "nb = asreview.models.classifiers:NaiveBayesClassifier",
             "rf = asreview.models.classifiers:RandomForestClassifier",
             "nn-2-layer = asreview.models.classifiers:NN2LayerClassifier",
             "logistic = asreview.models.classifiers:LogisticClassifier",
```

### Comparing `asreview-1.3a1/versioneer.py` & `asreview-1.3rc0/versioneer.py`

 * *Files identical despite different names*

