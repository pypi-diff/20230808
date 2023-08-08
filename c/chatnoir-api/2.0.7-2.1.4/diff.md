# Comparing `tmp/chatnoir-api-2.0.7.tar.gz` & `tmp/chatnoir-api-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatnoir-api-2.0.7.tar", last modified: Thu Feb 23 13:00:07 2023, max compression
+gzip compressed data, was "chatnoir-api-2.1.4.tar", last modified: Tue Aug  8 13:37:23 2023, max compression
```

## Comparing `chatnoir-api-2.0.7.tar` & `chatnoir-api-2.1.4.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.037841 chatnoir-api-2.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.037841 chatnoir-api-2.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.037841 chatnoir-api-2.0.7/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/chatnoir-api.iml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/discord.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.037841 chatnoir-api-2.0.7/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/php.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-02-23 13:00:07.045842 chatnoir-api-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.037841 chatnoir-api-2.0.7/chatnoir_api/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/chatnoir_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/model/highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/chatnoir_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/search_phrases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/chatnoir_api/v1/search_phrases.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/chatnoir_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-02-23 13:00:06.000000 chatnoir-api-2.0.7/chatnoir_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 13:00:07.000000 chatnoir-api-2.0.7/chatnoir_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 13:00:06.000000 chatnoir-api-2.0.7/chatnoir_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-23 13:00:07.000000 chatnoir-api-2.0.7/chatnoir_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 13:00:07.000000 chatnoir-api-2.0.7/chatnoir_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/search_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/search_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/examples/search_single.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-02-23 13:00:07.045842 chatnoir-api-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:00:07.041842 chatnoir-api-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/test_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-02-23 12:59:44.000000 chatnoir-api-2.0.7/tests/test_search_phrases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.445990 chatnoir-api-2.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.445990 chatnoir-api-2.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.449991 chatnoir-api-2.1.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/chatnoir-api.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/discord.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.449991 chatnoir-api-2.1.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/php.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.449991 chatnoir-api-2.1.4/chatnoir_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.449991 chatnoir-api-2.1.4/chatnoir_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/model/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/chatnoir_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/search_phrases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/chatnoir_api/v1/search_phrases.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.449991 chatnoir-api-2.1.4/chatnoir_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-08-08 13:37:23.000000 chatnoir-api-2.1.4/chatnoir_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-08 13:37:23.000000 chatnoir-api-2.1.4/chatnoir_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:37:23.000000 chatnoir-api-2.1.4/chatnoir_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-08 13:37:23.000000 chatnoir-api-2.1.4/chatnoir_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:37:23.000000 chatnoir-api-2.1.4/chatnoir_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/search_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/search_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/examples/search_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:23.453991 chatnoir-api-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-08-08 13:37:03.000000 chatnoir-api-2.1.4/tests/test_search_phrases.py
```

### Comparing `chatnoir-api-2.0.7/.github/workflows/ci.yml` & `chatnoir-api-2.1.4/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - name: "📥 Check-out"
         uses: actions/checkout@v2
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip build twine
           pip install -e .
       - name: "🏗️ Build Python wheel"
         run: python -m build
       - name: "🧪 Check package bundles"
@@ -49,15 +49,15 @@
       - name: "📥 Check-out"
         uses: actions/checkout@v2
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip
           pip install -e .
           pip install -e .[test]
       - name: "🔍 Check Python code format"
         run: flake8 chatnoir_api examples tests
@@ -77,15 +77,15 @@
       - name: "📥 Check-out"
         uses: actions/checkout@v2
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip
           pip install -e .
           pip install -e .[test]
       - name: "🔍 Lint Python code"
         run: pylint -E chatnoir_api examples tests
@@ -105,24 +105,25 @@
       - name: "📥 Check-out"
         uses: actions/checkout@v2
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip
           pip install -e .
           pip install -e .[test]
       - name: "🧪 Test Python code"
         env:
           CHATNOIR_API_KEY: ${{ secrets.CHATNOIR_API_KEY }}
           CHATNOIR_API_KEY_STAGING: ${{ secrets.CHATNOIR_API_KEY_STAGING }}
+          CHATNOIR_API_KEY_CHAT: ${{ secrets.CHATNOIR_API_KEY_CHAT }}
         run: pytest chatnoir_api examples tests --cov --cov-report=term --cov-report=xml
       - name: "📤 Upload test coverage"
         uses: actions/upload-artifact@v2
         with:
           path: coverage.xml
           name: Python test coverage
       - name: "📤 Publish test coverage"
@@ -139,15 +140,15 @@
       - name: "📥 Check-out"
         uses: actions/checkout@v2
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip build
           pip install -e .
       - name: "🏗️ Build Python wheel"
         run: python -m build
       - name: "🚀 Publish Python package"
@@ -170,15 +171,15 @@
         id: get-version
         run: echo ::set-output name=tag::${GITHUB_REF/refs\/tags\//}
       - name: "🧰 Install Python"
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
       - name: "🧰 Install dependencies"
         run: |
           python -m pip install --upgrade pip build
           pip install -e .
       - name: "🏗️ Build Python wheel"
         run: python -m build
       - name: "🚀 Create GitHub release"
```

### Comparing `chatnoir-api-2.0.7/.github/workflows/codeql-analysis.yml` & `chatnoir-api-2.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/.gitignore` & `chatnoir-api-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/.idea/chatnoir-api.iml` & `chatnoir-api-2.1.4/.idea/chatnoir-api.iml`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/LICENSE` & `chatnoir-api-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/PKG-INFO` & `chatnoir-api-2.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: chatnoir-api
-Version: 2.0.7
+Version: 2.1.4
 Summary: Simple, type-safe access to the ChatNoir search API.
-Home-page: https://github.com/chatnoir-eu/chatnoir-api
-Author: Jan Heinrich Reimer
-Author-email: jan.reimer@student.uni-halle.de
-Maintainer: Jan Heinrich Reimer
+Author-email: Jan Heinrich Reimer <heinrich.reimer@uni-jena.de>, Maik Fröbe <maik.froebe@uni-jena.de>
+Project-URL: Homepage, https://github.com/chatnoir-eu/chatnoir-api
 Project-URL: Bug Tracker, https://github.com/chatnoir-eu/chatnoir-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -81,18 +81,29 @@
 #### Phrase Search
 To search for phrases, use the `search_phrases` method in the same way as normal `search`:
 
 ```python
 from chatnoir_api.v1 import search_phrases
 
 api_key: str = "<API_KEY>"
-results = search_phrases(api_key, "python library", staging=True)
+response = search_phrases(api_key, "python library", staging=True)
 ```
 
-### Retrieve Document Content
+### Chat
+To generate text with the ChatNoir Chat API you need to request an API key from the [admins](mailto:maik.froebe@uni-jena.de).
+With your API key, you can chat with the cat, like this:
+
+```python
+from chatnoir_api.chat import chat
+
+api_key: str = "<API_KEY>"
+answer = chat(api_key, "how are you?")
+```
+
+### Retrieve Document Contents
 Often the title and ID of a document is not enough to effectively re-rank a list of search results.
 To retrieve the full content or plain text for a given document you can use the `html_contents` helper function.
 The `html_contents` function expects a ChatNoir-internal UUID, shorthand UUID, or a TREC ID 
 and the index from which to retrieve the document.
 
 #### Retrieve by TREC ID
 You can retrieve a document by its TREC ID like this:
```

### Comparing `chatnoir-api-2.0.7/README.md` & `chatnoir-api-2.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,18 +58,29 @@
 #### Phrase Search
 To search for phrases, use the `search_phrases` method in the same way as normal `search`:
 
 ```python
 from chatnoir_api.v1 import search_phrases
 
 api_key: str = "<API_KEY>"
-results = search_phrases(api_key, "python library", staging=True)
+response = search_phrases(api_key, "python library", staging=True)
 ```
 
-### Retrieve Document Content
+### Chat
+To generate text with the ChatNoir Chat API you need to request an API key from the [admins](mailto:maik.froebe@uni-jena.de).
+With your API key, you can chat with the cat, like this:
+
+```python
+from chatnoir_api.chat import chat
+
+api_key: str = "<API_KEY>"
+answer = chat(api_key, "how are you?")
+```
+
+### Retrieve Document Contents
 Often the title and ID of a document is not enough to effectively re-rank a list of search results.
 To retrieve the full content or plain text for a given document you can use the `html_contents` helper function.
 The `html_contents` function expects a ChatNoir-internal UUID, shorthand UUID, or a TREC ID 
 and the index from which to retrieve the document.
 
 #### Retrieve by TREC ID
 You can retrieve a document by its TREC ID like this:
```

### Comparing `chatnoir-api-2.0.7/chatnoir_api/__init__.py` & `chatnoir-api-2.1.4/chatnoir_api/__init__.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/cache.py` & `chatnoir-api-2.1.4/chatnoir_api/cache.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/lazy.py` & `chatnoir-api-2.1.4/chatnoir_api/lazy.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/model/__init__.py` & `chatnoir-api-2.1.4/chatnoir_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/model/highlight.py` & `chatnoir-api-2.1.4/chatnoir_api/model/highlight.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/model/result.py` & `chatnoir-api-2.1.4/chatnoir_api/model/result.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/model.py` & `chatnoir-api-2.1.4/chatnoir_api/v1/model.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/requests.py` & `chatnoir-api-2.1.4/chatnoir_api/v1/requests.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/search.py` & `chatnoir-api-2.1.4/chatnoir_api/v1/search.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/search.pyi` & `chatnoir-api-2.1.4/chatnoir_api/v1/search.pyi`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/search_phrases.py` & `chatnoir-api-2.1.4/chatnoir_api/v1/search_phrases.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api/v1/search_phrases.pyi` & `chatnoir-api-2.1.4/chatnoir_api/v1/search_phrases.pyi`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/chatnoir_api.egg-info/PKG-INFO` & `chatnoir-api-2.1.4/chatnoir_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: chatnoir-api
-Version: 2.0.7
+Version: 2.1.4
 Summary: Simple, type-safe access to the ChatNoir search API.
-Home-page: https://github.com/chatnoir-eu/chatnoir-api
-Author: Jan Heinrich Reimer
-Author-email: jan.reimer@student.uni-halle.de
-Maintainer: Jan Heinrich Reimer
+Author-email: Jan Heinrich Reimer <heinrich.reimer@uni-jena.de>, Maik Fröbe <maik.froebe@uni-jena.de>
+Project-URL: Homepage, https://github.com/chatnoir-eu/chatnoir-api
 Project-URL: Bug Tracker, https://github.com/chatnoir-eu/chatnoir-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -81,18 +81,29 @@
 #### Phrase Search
 To search for phrases, use the `search_phrases` method in the same way as normal `search`:
 
 ```python
 from chatnoir_api.v1 import search_phrases
 
 api_key: str = "<API_KEY>"
-results = search_phrases(api_key, "python library", staging=True)
+response = search_phrases(api_key, "python library", staging=True)
 ```
 
-### Retrieve Document Content
+### Chat
+To generate text with the ChatNoir Chat API you need to request an API key from the [admins](mailto:maik.froebe@uni-jena.de).
+With your API key, you can chat with the cat, like this:
+
+```python
+from chatnoir_api.chat import chat
+
+api_key: str = "<API_KEY>"
+answer = chat(api_key, "how are you?")
+```
+
+### Retrieve Document Contents
 Often the title and ID of a document is not enough to effectively re-rank a list of search results.
 To retrieve the full content or plain text for a given document you can use the `html_contents` helper function.
 The `html_contents` function expects a ChatNoir-internal UUID, shorthand UUID, or a TREC ID 
 and the index from which to retrieve the document.
 
 #### Retrieve by TREC ID
 You can retrieve a document by its TREC ID like this:
```

### Comparing `chatnoir-api-2.0.7/chatnoir_api.egg-info/SOURCES.txt` & `chatnoir-api-2.1.4/chatnoir_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 .github/release.yml
 .github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
 .idea/.gitignore
 .idea/chatnoir-api.iml
 .idea/discord.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/php.xml
 .idea/vcs.xml
 .idea/inspectionProfiles/profiles_settings.xml
 chatnoir_api/__init__.py
 chatnoir_api/cache.py
+chatnoir_api/chat.py
 chatnoir_api/constants.py
 chatnoir_api/lazy.py
 chatnoir_api/logger.py
 chatnoir_api/types.py
 chatnoir_api.egg-info/PKG-INFO
 chatnoir_api.egg-info/SOURCES.txt
 chatnoir_api.egg-info/dependency_links.txt
@@ -35,18 +34,20 @@
 chatnoir_api/v1/requests.py
 chatnoir_api/v1/search.py
 chatnoir_api/v1/search.pyi
 chatnoir_api/v1/search_phrases.py
 chatnoir_api/v1/search_phrases.pyi
 examples/__init__.py
 examples/cache.py
+examples/chat.py
 examples/search.py
 examples/search_iterator.py
 examples/search_page.py
 examples/search_single.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cache.py
+tests/test_chat.py
 tests/test_highlight.py
 tests/test_model.py
 tests/test_search.py
 tests/test_search_phrases.py
```

### Comparing `chatnoir-api-2.0.7/examples/cache.py` & `chatnoir-api-2.1.4/examples/cache.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/examples/search.py` & `chatnoir-api-2.1.4/examples/search.py`

 * *Files identical despite different names*

### Comparing `chatnoir-api-2.0.7/tests/conftest.py` & `chatnoir-api-2.1.4/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,27 @@
     key: str
     if staging:
         key = "CHATNOIR_API_KEY_STAGING"
     else:
         key = "CHATNOIR_API_KEY"
     if key not in environ:
         raise RuntimeError(
-            f"Must specify ChatNoir api key "
+            f"Must specify ChatNoir API key "
+            f"in the {key} environment variable "
+            f"to run this test."
+        )
+    return environ[key]
+
+
+@fixture(scope="module")
+def api_key_chat() -> str:
+    key = "CHATNOIR_API_KEY_CHAT"
+    if key not in environ:
+        raise RuntimeError(
+            f"Must specify ChatNoir Chat API key "
             f"in the {key} environment variable "
             f"to run this test."
         )
     return environ[key]
 
 
 @fixture(scope="module", params=["python library", "search engine"])
```

### Comparing `chatnoir-api-2.0.7/tests/test_cache.py` & `chatnoir-api-2.1.4/tests/test_cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 from uuid import UUID
 
 from chatnoir_api import cache_contents, Index, ShortUUID
 
 
-def test_html_contents_trec_id():
+def test_html_contents_trec_id() -> None:
     contents = cache_contents(
         "clueweb09-en0051-90-00849",
         Index.ClueWeb09,
     )
 
     assert contents is not None
     assert isinstance(contents, str)
     assert "<title>Test, test, test</title>" in contents
 
 
-def test_html_contents_plain_trec_id():
+def test_html_contents_plain_trec_id() -> None:
     contents = cache_contents(
         "clueweb09-en0051-90-00849",
         Index.ClueWeb09,
         plain=True
     )
 
     assert contents is not None
     assert isinstance(contents, str)
     assert "<title>Test, test, test</title>" in contents
 
 
-def test_html_contents_uuid():
+def test_html_contents_uuid() -> None:
     contents = cache_contents(
         UUID("e635baa8-7341-596a-b3cf-b33c05954361"),
         Index.CommonCrawl1511,
     )
 
     assert contents is not None
     assert isinstance(contents, str)
     assert "<title>hello world</title>" in contents
 
 
-def test_html_contents_plain_uuid():
+def test_html_contents_plain_uuid() -> None:
     contents = cache_contents(
         UUID("e635baa8-7341-596a-b3cf-b33c05954361"),
         Index.CommonCrawl1511,
         plain=True,
     )
 
     assert contents is not None
     assert isinstance(contents, str)
     assert "<title>hello world</title>" in contents
 
 
-def test_html_contents_short_uuid():
+def test_html_contents_short_uuid() -> None:
     contents = cache_contents(
         ShortUUID("f6J0lMPmVfWs19jJNQkHKA"),
         Index.ClueWeb22,
         staging=True,
     )
 
     assert contents is not None
     assert isinstance(contents, str)
     assert "<title data-dcnode-id=\"1108\">" \
            "Hello World | Codecademy</title>" in contents
 
 
-def test_html_contents_plain_short_uuid():
+def test_html_contents_plain_short_uuid() -> None:
     contents = cache_contents(
         ShortUUID("f6J0lMPmVfWs19jJNQkHKA"),
         Index.ClueWeb22,
         plain=True,
         staging=True,
     )
```

### Comparing `chatnoir-api-2.0.7/tests/test_search.py` & `chatnoir-api-2.1.4/tests/test_search_phrases.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Sequence
 
-from pytest import fixture, skip
+from pytest import fixture
 
-from chatnoir_api import Index, Meta, Results, MinimalResult, \
-    Result, ExplainedMinimalResult, ExtendedMeta
-from chatnoir_api.v1 import search_page, search
+from chatnoir_api import (
+    Index, Results, Meta, MinimalResult, Result, ExtendedMeta,
+    ExplainedMinimalResult
+)
+from chatnoir_api.v1 import search_phrases_page, search_phrases
 
 
 @fixture(params=[True, False])
-def minimal(request, staging: bool) -> bool:
-    if not staging and request.param:
-        skip("Minimal response is not available on the production API.")
+def minimal(request) -> bool:
     return request.param
 
 
-def test_page(api_key: str, query: str, staging: bool):
-    results = search_page(
+def test_page(api_key: str, query: str, staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         staging=staging,
     )
     meta = results.meta
 
     assert meta is not None
@@ -38,51 +38,56 @@
     assert len(results) > 0
     assert len(results) <= meta.total_results
 
     assert results[0] is not None
     assert isinstance(results[0], MinimalResult)
 
 
-def test_page_size(api_key: str, query: str, page_size: int, staging: bool):
-    results = search_page(
+def test_page_size(api_key: str, query: str, page_size: int,
+                   staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         size=page_size,
         staging=staging,
     )
     assert len(results) == page_size
 
 
-def test_page_index(api_key: str, query: str, index: Index, staging: bool):
-    results = search_page(
+def test_page_index(api_key: str, query: str, index: Index,
+                    staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         size=1,
         index=index,
+        minimal=False,
         staging=staging,
     )
     assert results[0].index == index
 
 
-def test_page_minimal(api_key: str, query: str, minimal: bool, staging: bool):
-    results = search_page(
+def test_page_minimal(api_key: str, query: str, minimal: bool,
+                      staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         size=1,
         minimal=minimal,
         staging=staging,
     )
     if minimal:
         assert isinstance(results[0], MinimalResult)
     else:
         assert isinstance(results[0], Result)
 
 
-def test_page_explain(api_key: str, query: str, explain: bool, staging: bool):
-    results = search_page(
+def test_page_explain(api_key: str, query: str, explain: bool,
+                      staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         size=1,
         explain=explain,
         staging=staging,
     )
     if explain:
@@ -94,32 +99,32 @@
         assert results[0].explanation.description is not None
         assert isinstance(results[0].explanation.description, str)
     else:
         assert isinstance(results[0], MinimalResult)
 
 
 def test_page_meta(api_key: str, query: str, extended_meta: bool,
-                   staging: bool):
-    results = search_page(
+                   staging: bool) -> None:
+    results = search_phrases_page(
         api_key=api_key,
         query=query,
         size=1,
         extended_meta=extended_meta,
         staging=staging,
     )
     meta = results.meta
 
     if extended_meta:
         assert isinstance(meta, ExtendedMeta)
     else:
         assert isinstance(meta, Meta)
 
 
-def test_iterable(api_key: str, query: str, staging: bool):
-    results = search(
+def test_iterable(api_key: str, query: str, staging: bool) -> None:
+    results = search_phrases(
         api_key=api_key,
         query=query,
         page_size=1,
         staging=staging,
     )
     assert results is not None
     assert isinstance(results, Results)
@@ -142,44 +147,45 @@
     assert isinstance(first_result, MinimalResult)
 
     second_result = next(result_iterator, None)
     assert second_result is not None
     assert isinstance(second_result, MinimalResult)
 
 
-def test_iterable_index(api_key: str, query: str, index: Index, staging: bool):
-    results = search(
+def test_iterable_index(api_key: str, query: str, index: Index,
+                        staging: bool) -> None:
+    results = search_phrases(
         api_key=api_key,
         query=query,
         page_size=1,
         index=index,
         minimal=False,
         staging=staging,
     )
     assert results[0].index == index
 
 
 def test_iterable_minimal(api_key: str, query: str, minimal: bool,
-                          staging: bool):
-    results = search(
+                          staging: bool) -> None:
+    results = search_phrases(
         api_key=api_key,
         query=query,
         page_size=1,
         minimal=minimal,
         staging=staging,
     )
     if minimal:
         assert isinstance(results[0], MinimalResult)
     else:
         assert isinstance(results[0], Result)
 
 
 def test_iterable_explain(api_key: str, query: str, explain: bool,
-                          staging: bool):
-    results = search(
+                          staging: bool) -> None:
+    results = search_phrases(
         api_key=api_key,
         query=query,
         page_size=1,
         explain=explain,
         staging=staging,
     )
 
@@ -192,16 +198,16 @@
         assert results[0].explanation.description is not None
         assert isinstance(results[0].explanation.description, str)
     else:
         assert isinstance(results[0], MinimalResult)
 
 
 def test_iterable_meta(api_key: str, query: str, extended_meta: bool,
-                       staging: bool):
-    results = search(
+                       staging: bool) -> None:
+    results = search_phrases(
         api_key=api_key,
         query=query,
         page_size=1,
         extended_meta=extended_meta,
         staging=staging,
     )
```

### Comparing `chatnoir-api-2.0.7/tests/test_search_phrases.py` & `chatnoir-api-2.1.4/tests/test_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Sequence
 
-from pytest import fixture
+from pytest import fixture, skip
 
-from chatnoir_api import (
-    Index, Results, Meta, MinimalResult, Result, ExtendedMeta,
-    ExplainedMinimalResult
-)
-from chatnoir_api.v1 import search_phrases_page, search_phrases
+from chatnoir_api import Index, Meta, Results, MinimalResult, \
+    Result, ExplainedMinimalResult, ExtendedMeta
+from chatnoir_api.v1 import search_page, search
 
 
 @fixture(params=[True, False])
-def minimal(request) -> bool:
+def minimal(request, staging: bool) -> bool:
+    if not staging and request.param:
+        skip("Minimal response is not available on the production API.")
     return request.param
 
 
-def test_page(api_key: str, query: str, staging: bool):
-    results = search_phrases_page(
+def test_page(api_key: str, query: str, staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         staging=staging,
     )
     meta = results.meta
 
     assert meta is not None
@@ -38,52 +38,55 @@
     assert len(results) > 0
     assert len(results) <= meta.total_results
 
     assert results[0] is not None
     assert isinstance(results[0], MinimalResult)
 
 
-def test_page_size(api_key: str, query: str, page_size: int, staging: bool):
-    results = search_phrases_page(
+def test_page_size(api_key: str, query: str, page_size: int,
+                   staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         size=page_size,
         staging=staging,
     )
     assert len(results) == page_size
 
 
-def test_page_index(api_key: str, query: str, index: Index, staging: bool):
-    results = search_phrases_page(
+def test_page_index(api_key: str, query: str, index: Index,
+                    staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         size=1,
         index=index,
-        minimal=False,
         staging=staging,
     )
     assert results[0].index == index
 
 
-def test_page_minimal(api_key: str, query: str, minimal: bool, staging: bool):
-    results = search_phrases_page(
+def test_page_minimal(api_key: str, query: str, minimal: bool,
+                      staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         size=1,
         minimal=minimal,
         staging=staging,
     )
     if minimal:
         assert isinstance(results[0], MinimalResult)
     else:
         assert isinstance(results[0], Result)
 
 
-def test_page_explain(api_key: str, query: str, explain: bool, staging: bool):
-    results = search_phrases_page(
+def test_page_explain(api_key: str, query: str, explain: bool,
+                      staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         size=1,
         explain=explain,
         staging=staging,
     )
     if explain:
@@ -95,32 +98,32 @@
         assert results[0].explanation.description is not None
         assert isinstance(results[0].explanation.description, str)
     else:
         assert isinstance(results[0], MinimalResult)
 
 
 def test_page_meta(api_key: str, query: str, extended_meta: bool,
-                   staging: bool):
-    results = search_phrases_page(
+                   staging: bool) -> None:
+    results = search_page(
         api_key=api_key,
         query=query,
         size=1,
         extended_meta=extended_meta,
         staging=staging,
     )
     meta = results.meta
 
     if extended_meta:
         assert isinstance(meta, ExtendedMeta)
     else:
         assert isinstance(meta, Meta)
 
 
-def test_iterable(api_key: str, query: str, staging: bool):
-    results = search_phrases(
+def test_iterable(api_key: str, query: str, staging: bool) -> None:
+    results = search(
         api_key=api_key,
         query=query,
         page_size=1,
         staging=staging,
     )
     assert results is not None
     assert isinstance(results, Results)
@@ -143,44 +146,45 @@
     assert isinstance(first_result, MinimalResult)
 
     second_result = next(result_iterator, None)
     assert second_result is not None
     assert isinstance(second_result, MinimalResult)
 
 
-def test_iterable_index(api_key: str, query: str, index: Index, staging: bool):
-    results = search_phrases(
+def test_iterable_index(api_key: str, query: str, index: Index,
+                        staging: bool) -> None:
+    results = search(
         api_key=api_key,
         query=query,
         page_size=1,
         index=index,
         minimal=False,
         staging=staging,
     )
     assert results[0].index == index
 
 
 def test_iterable_minimal(api_key: str, query: str, minimal: bool,
-                          staging: bool):
-    results = search_phrases(
+                          staging: bool) -> None:
+    results = search(
         api_key=api_key,
         query=query,
         page_size=1,
         minimal=minimal,
         staging=staging,
     )
     if minimal:
         assert isinstance(results[0], MinimalResult)
     else:
         assert isinstance(results[0], Result)
 
 
 def test_iterable_explain(api_key: str, query: str, explain: bool,
-                          staging: bool):
-    results = search_phrases(
+                          staging: bool) -> None:
+    results = search(
         api_key=api_key,
         query=query,
         page_size=1,
         explain=explain,
         staging=staging,
     )
 
@@ -193,16 +197,16 @@
         assert results[0].explanation.description is not None
         assert isinstance(results[0].explanation.description, str)
     else:
         assert isinstance(results[0], MinimalResult)
 
 
 def test_iterable_meta(api_key: str, query: str, extended_meta: bool,
-                       staging: bool):
-    results = search_phrases(
+                       staging: bool) -> None:
+    results = search(
         api_key=api_key,
         query=query,
         page_size=1,
         extended_meta=extended_meta,
         staging=staging,
     )
```

