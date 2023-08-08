# Comparing `tmp/vcorelib-2.4.3.tar.gz` & `tmp/vcorelib-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-2.4.3.tar", last modified: Sun Aug  6 05:50:23 2023, max compression
+gzip compressed data, was "vcorelib-2.4.4.tar", last modified: Tue Aug  8 05:53:53 2023, max compression
```

## Comparing `vcorelib-2.4.3.tar` & `vcorelib-2.4.4.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 05:48:45.000000 vcorelib-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-06 05:50:23.138630 vcorelib-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-06 05:48:45.000000 vcorelib-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-06 05:48:45.000000 vcorelib-2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 05:50:23.138630 vcorelib-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-06 05:48:45.000000 vcorelib-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.130630 vcorelib-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-06 05:48:45.000000 vcorelib-2.4.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-06 05:48:45.000000 vcorelib-2.4.3/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-06 05:48:45.000000 vcorelib-2.4.3/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-06 05:48:45.000000 vcorelib-2.4.3/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.130630 vcorelib-2.4.3/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.130630 vcorelib-2.4.3/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.130630 vcorelib-2.4.3/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.134630 vcorelib-2.4.3/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/analysis/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/math/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/python.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.138630 vcorelib-2.4.3/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-06 05:48:45.000000 vcorelib-2.4.3/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:50:23.130630 vcorelib-2.4.3/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-06 05:50:23.000000 vcorelib-2.4.3/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-06 05:50:23.000000 vcorelib-2.4.3/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:50:23.000000 vcorelib-2.4.3/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-06 05:50:23.000000 vcorelib-2.4.3/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 05:50:23.000000 vcorelib-2.4.3/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 05:52:09.000000 vcorelib-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-08 05:53:53.319524 vcorelib-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-08 05:52:09.000000 vcorelib-2.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-08 05:52:09.000000 vcorelib-2.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 05:53:53.319524 vcorelib-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-08 05:52:09.000000 vcorelib-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.295524 vcorelib-2.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-08 05:52:09.000000 vcorelib-2.4.4/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 05:52:09.000000 vcorelib-2.4.4/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-08 05:52:09.000000 vcorelib-2.4.4/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 05:52:09.000000 vcorelib-2.4.4/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.299524 vcorelib-2.4.4/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.303524 vcorelib-2.4.4/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.303524 vcorelib-2.4.4/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.303524 vcorelib-2.4.4/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.307524 vcorelib-2.4.4/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.307524 vcorelib-2.4.4/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.311524 vcorelib-2.4.4/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.311524 vcorelib-2.4.4/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.311524 vcorelib-2.4.4/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.311524 vcorelib-2.4.4/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.311524 vcorelib-2.4.4/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/analysis/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.315524 vcorelib-2.4.4/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.315524 vcorelib-2.4.4/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.315524 vcorelib-2.4.4/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.315524 vcorelib-2.4.4/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.319524 vcorelib-2.4.4/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-08 05:52:09.000000 vcorelib-2.4.4/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:53:53.299524 vcorelib-2.4.4/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-08 05:53:53.000000 vcorelib-2.4.4/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 05:53:53.000000 vcorelib-2.4.4/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:53:53.000000 vcorelib-2.4.4/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 05:53:53.000000 vcorelib-2.4.4/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 05:53:53.000000 vcorelib-2.4.4/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-2.4.3/LICENSE` & `vcorelib-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/PKG-INFO` & `vcorelib-2.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.4.3
+Version: 2.4.4
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3b4ebfecfc843a3b928bad2dfa380bbd
+    hash=f407494d736c466d1d8497a1326cf9ae
     =====================================
 -->
 
-# vcorelib ([2.4.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.4.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.4.3/README.md` & `vcorelib-2.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3b4ebfecfc843a3b928bad2dfa380bbd
+    hash=f407494d736c466d1d8497a1326cf9ae
     =====================================
 -->
 
-# vcorelib ([2.4.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.4.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.4.3/pyproject.toml` & `vcorelib-2.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "2.4.3"
+version = "2.4.4"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-2.4.3/setup.py` & `vcorelib-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/tests/test_logging.py` & `vcorelib-2.4.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/tests/test_names.py` & `vcorelib-2.4.4/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/tests/test_namespace.py` & `vcorelib-2.4.4/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/args/__init__.py` & `vcorelib-2.4.4/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/args/newline.py` & `vcorelib-2.4.4/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/asyncio/__init__.py` & `vcorelib-2.4.4/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/asyncio/cli.py` & `vcorelib-2.4.4/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/asyncio/subprocess.py` & `vcorelib-2.4.4/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/dict/__init__.py` & `vcorelib-2.4.4/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/dict/cache.py` & `vcorelib-2.4.4/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/dict/codec.py` & `vcorelib-2.4.4/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/dict/config.py` & `vcorelib-2.4.4/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/dict/env.py` & `vcorelib-2.4.4/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/graph/__init__.py` & `vcorelib-2.4.4/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/graph/abc.py` & `vcorelib-2.4.4/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/graph/edge.py` & `vcorelib-2.4.4/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/graph/node.py` & `vcorelib-2.4.4/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/graph/port.py` & `vcorelib-2.4.4/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/__init__.py` & `vcorelib-2.4.4/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/abc.py` & `vcorelib-2.4.4/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/arbiter/base.py` & `vcorelib-2.4.4/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/arbiter/context.py` & `vcorelib-2.4.4/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/arbiter/directory.py` & `vcorelib-2.4.4/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/archive/__init__.py` & `vcorelib-2.4.4/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/cache.py` & `vcorelib-2.4.4/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/decode.py` & `vcorelib-2.4.4/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/encode.py` & `vcorelib-2.4.4/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/mapping.py` & `vcorelib-2.4.4/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/io/types.py` & `vcorelib-2.4.4/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/logging.py` & `vcorelib-2.4.4/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/__init__.py` & `vcorelib-2.4.4/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/analysis/average.py` & `vcorelib-2.4.4/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/analysis/buffer.py` & `vcorelib-2.4.4/vcorelib/math/analysis/buffer.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-2.4.4/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-2.4.4/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/analysis/weighted.py` & `vcorelib-2.4.4/vcorelib/math/analysis/weighted.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/time.py` & `vcorelib-2.4.4/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/math/unit.py` & `vcorelib-2.4.4/vcorelib/math/unit.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/names.py` & `vcorelib-2.4.4/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/namespace.py` & `vcorelib-2.4.4/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/__init__.py` & `vcorelib-2.4.4/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/base.py` & `vcorelib-2.4.4/vcorelib/paths/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/context.py` & `vcorelib-2.4.4/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/hashing.py` & `vcorelib-2.4.4/vcorelib/paths/hashing.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/info.py` & `vcorelib-2.4.4/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/paths/info_cache.py` & `vcorelib-2.4.4/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/platform/__init__.py` & `vcorelib-2.4.4/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/python.py` & `vcorelib-2.4.4/vcorelib/python.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/schemas/__init__.py` & `vcorelib-2.4.4/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/schemas/base.py` & `vcorelib-2.4.4/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/schemas/json.py` & `vcorelib-2.4.4/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/schemas/mixins.py` & `vcorelib-2.4.4/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/script/__init__.py` & `vcorelib-2.4.4/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/target/__init__.py` & `vcorelib-2.4.4/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/target/evaluation.py` & `vcorelib-2.4.4/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/target/expression.py` & `vcorelib-2.4.4/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/target/resolver.py` & `vcorelib-2.4.4/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/task/__init__.py` & `vcorelib-2.4.4/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/task/dict/melder.py` & `vcorelib-2.4.4/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/task/manager.py` & `vcorelib-2.4.4/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/task/subprocess/run.py` & `vcorelib-2.4.4/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib/task/time/sleep.py` & `vcorelib-2.4.4/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.4.3/vcorelib.egg-info/PKG-INFO` & `vcorelib-2.4.4/vcorelib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.4.3
+Version: 2.4.4
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3b4ebfecfc843a3b928bad2dfa380bbd
+    hash=f407494d736c466d1d8497a1326cf9ae
     =====================================
 -->
 
-# vcorelib ([2.4.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.4.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.4.3/vcorelib.egg-info/SOURCES.txt` & `vcorelib-2.4.4/vcorelib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 vcorelib/graph/node.py
 vcorelib/graph/port.py
 vcorelib/io/__init__.py
 vcorelib/io/abc.py
 vcorelib/io/cache.py
 vcorelib/io/decode.py
 vcorelib/io/encode.py
+vcorelib/io/file_writer.py
 vcorelib/io/mapping.py
 vcorelib/io/types.py
 vcorelib/io/arbiter/__init__.py
 vcorelib/io/arbiter/base.py
 vcorelib/io/arbiter/context.py
 vcorelib/io/arbiter/directory.py
 vcorelib/io/archive/__init__.py
```

