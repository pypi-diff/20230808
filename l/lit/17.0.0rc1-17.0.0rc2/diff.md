# Comparing `tmp/lit-17.0.0rc1.tar.gz` & `tmp/lit-17.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit-17.0.0rc1.tar", last modified: Sat Jul 29 14:13:58 2023, max compression
+gzip compressed data, was "lit-17.0.0rc2.tar", last modified: Tue Aug  8 11:12:41 2023, max compression
```

## Comparing `lit-17.0.0rc1.tar` & `lit-17.0.0rc2.tar`

### file list

```diff
@@ -1,611 +1,611 @@
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    15141 2022-05-20 05:53:51.000000 lit-17.0.0rc1/LICENSE.TXT
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      242 2022-05-20 05:53:51.000000 lit-17.0.0rc1/MANIFEST.in
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2519 2023-07-29 14:13:58.786108 lit-17.0.0rc1/PKG-INFO
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1874 2023-05-13 06:19:19.000000 lit-17.0.0rc1/README.rst
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.763108 lit-17.0.0rc1/examples/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc1/examples/README.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.763108 lit-17.0.0rc1/examples/many-tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      549 2023-07-06 03:21:05.000000 lit-17.0.0rc1/examples/many-tests/ManyTests.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      382 2022-05-20 05:53:51.000000 lit-17.0.0rc1/examples/many-tests/README.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2023-07-06 00:01:13.000000 lit-17.0.0rc1/examples/many-tests/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)    12039 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/BooleanExpression.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     7871 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/LitConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/LitTestCase.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    11087 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ProgressBar.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3242 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ShCommands.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8811 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13734 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/Test.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    78657 2023-07-06 00:02:35.000000 lit-17.0.0rc1/lit/TestRunner.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1629 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/TestTimes.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8659 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/TestingConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      199 2023-07-29 14:11:55.000000 lit-17.0.0rc1/lit/__init__.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit/builtin_commands/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/lit/builtin_commands/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1892 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/builtin_commands/cat.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9817 2023-07-06 00:02:35.000000 lit-17.0.0rc1/lit/builtin_commands/diff.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    10608 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/cl_arguments.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9564 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/discovery.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5987 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/display.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.765108 lit-17.0.0rc1/lit/formats/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 03:21:05.000000 lit-17.0.0rc1/lit/formats/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2299 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/formats/base.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13602 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/formats/googletest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      992 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/formats/shtest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.765108 lit-17.0.0rc1/lit/llvm/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-05-20 05:53:51.000000 lit-17.0.0rc1/lit/llvm/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    31158 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/llvm/config.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5430 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/llvm/subst.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11652 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/main.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11056 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/reports.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4692 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/run.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    15927 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/util.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/worker.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit.egg-info/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2519 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/PKG-INFO
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    21372 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/SOURCES.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/dependency_links.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/entry_points.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-17.0.0rc1/lit.egg-info/not-zip-safe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/top_level.txt
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2023-04-28 22:43:05.000000 lit-17.0.0rc1/pyproject.toml
--rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2023-07-29 14:13:58.786108 lit-17.0.0rc1/setup.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1295 2023-07-06 00:01:13.000000 lit-17.0.0rc1/setup.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      152 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/.coveragerc
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/allow-retries/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       51 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       45 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/not-a-valid-integer.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/succeeds-within-limit.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      444 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/driver.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/invalid-test.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      281 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/lit.alt.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/main-config/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/main-config/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/custom-result-category/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      762 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/subdir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/subdir/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subdir/test-three.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      175 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/test-two.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test-two.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test.not-txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/custom_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      270 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/x.test
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      292 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery/lit.site.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/obj/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      205 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/fake-externals/
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/cd
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/diff
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/env
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/export
--rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/fake_external.py
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/mkdir
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/rm
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1267 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      189 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-crash/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1424 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-crash/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1350 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      131 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/subdir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       80 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2741 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2742 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1506 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/googletest-timeout/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1685 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      397 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-timeout/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/ignore-fail/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/unresolved.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/lit-opts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/lit-opts/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/lit-opts/test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/lld-features/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       31 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      714 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/max-failures/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/max-failures/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/max-time/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-time/fast.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/max-time/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-time/slow.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/parallelism-groups/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      474 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/progress-bar/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-4.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/py-config-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      299 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/py-config-discovery/lit.site.cfg.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/reorder/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/aaa.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/bbb.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/reorder/fff.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      173 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/reorder/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       78 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/reorder/lit_test_times
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/new-test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/reorder/subdir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/subdir/ccc.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/show-result-codes/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       36 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/unsupported.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/show-used-features/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      184 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      267 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/mixed.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       35 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/requires.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       42 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/unsupported.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       30 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/shtest-define/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.773108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/before-name.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      259 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      507 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      244 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      490 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      196 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/no-name.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      222 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      329 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      420 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      289 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      427 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      229 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      254 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      268 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      319 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      318 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      324 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      409 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      436 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      333 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      322 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      399 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      611 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      408 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      397 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/location-range.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/no-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/examples/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1772 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/examples/param-subst.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1683 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/expansion-order.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1224 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/line-number-substitutions.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2668 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      662 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/name-chars.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      265 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      886 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/value-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      509 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/value-escaped.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3926 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/ws-and-continuations.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.775108 lit-17.0.0rc1/tests/Inputs/shtest-env/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-assign.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       14 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-u.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-cd.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-colon.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-echo.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      875 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-env.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-export.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-mkdir.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      198 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-not-builtin.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-rm.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      687 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-u.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      465 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      310 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/mixed.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      107 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      191 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/utf8_command.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      138 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      146 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/write-control-chars.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      104 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      414 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/no-test-line.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-missing.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      122 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-present.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       49 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-star.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      114 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-triple.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      218 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-expr-false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      174 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-expr-true.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       52 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-star.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      147 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-expr-false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      151 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-expr-true.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       40 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-feature.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-target.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      320 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/argv0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      233 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-if-else/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       93 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3294 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-inject/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      109 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      183 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-many.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      133 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       44 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       29 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-not/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      211 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-calls-external.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/fail.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/fail2.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-last-is-crash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       85 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-cd.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-colon.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      252 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      413 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-diff.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-echo.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-env-builtin.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       97 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-export.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1933 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-external.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      142 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-fail2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       59 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-mkdir.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       46 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-rm.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/pass.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      159 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/basic.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      150 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      145 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/popd-args.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       16 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.762108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      340 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       28 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      372 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      125 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.780108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      221 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       84 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/shtest-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       75 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      269 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat_nonprinting.bin
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/check_args.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/check_path.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/colon-error.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      373 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/continuations.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      513 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/dev-null.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-I.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-b.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      622 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-encodings.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      141 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-5.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-6.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.bin
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       55 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.dos
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       50 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.unix
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.utf16
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.utf8
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      734 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-pipes.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      274 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      346 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      251 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      282 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-5.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      271 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-6.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-7.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-8.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      675 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      358 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      976 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-unified.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-w.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       71 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      248 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       74 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1215 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/redirects.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      120 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-unicode-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      738 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      157 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/stdout-encoding.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     7169 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/valid-shell.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/write-to-stderr.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      153 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/shtest-timeout/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/infinite_loop.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       82 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/short.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/standalone-tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      154 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test-data/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1172 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/test-data/metrics.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test-data-micro/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1907 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      220 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/micro-tests.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      387 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/test-two.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/unparsed-requirements/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unparsed-requirements/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case10
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case10.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case2
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case2.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case3
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case3.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case6
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case6.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case7
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case7.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case9.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/env-case1
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/env-case6
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1403 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case10
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case10.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case4
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case4.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case5
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case5.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case6
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case6.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case7
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case7.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search1/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search1/empty
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/case9.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/case9.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/found
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/found.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      451 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/test-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/test-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/false2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/true-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/tests/Inputs/xunit-output/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/bad&name.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/dummy_format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       69 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/excluded.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/missing_feature.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       65 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/pass.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/unsupported.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1954 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/allow-retries.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/boolean-parsing.py
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)      199 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/check-tested-lit-timeout-ability
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      484 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/custom-result-category.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9769 2023-07-29 14:11:39.000000 lit-17.0.0rc1/tests/discovery.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-cmd-wrapper.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1009 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-crash.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      502 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-detect-duplicate.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      337 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/googletest-discovery-failed.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      800 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-format-respect-gtest-sharding-env-vars.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1432 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1234 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-sanitizer-error.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2561 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-timeout.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      640 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/ignore-fail.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1096 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/lit-opts.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5298 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      410 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/lit.site.cfg.in
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/lld-features.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1001 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/max-failures.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/max-time.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      558 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/parallelism-groups.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      538 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/progress-bar.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      732 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/reorder.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6440 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/selecting.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       67 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shell-parsing.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      847 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/show-result-codes.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      512 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/show-used-features.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6636 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-define.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shtest-encoding.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     4015 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-env.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      588 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-format-argv0.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6916 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      699 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/shtest-if-else.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1228 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-inject.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      581 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-keyword-parse-errors.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     5363 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-not.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      979 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-output-printing.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      636 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/shtest-pushd-popd.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1615 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-recursive-substitution.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2221 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-run-at-line.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    17367 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-shell.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3498 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shtest-timeout.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      679 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-data-micro.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      353 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-data.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2380 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-output-micro-resultdb.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1624 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/test-output-micro.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1546 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/test-output-resultdb.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      552 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/test-output.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/tests/unit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4360 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/unit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13421 2023-07-29 14:11:39.000000 lit-17.0.0rc1/tests/unit/TestRunner.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      460 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/unittest-adaptor.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      816 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/unparsed-requirements.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/usage.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2077 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/use-llvm-tool.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1860 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/xfail-cl.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1486 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/xunit-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.194285 lit-17.0.0rc2/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    15141 2022-05-20 05:53:51.000000 lit-17.0.0rc2/LICENSE.TXT
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      242 2022-05-20 05:53:51.000000 lit-17.0.0rc2/MANIFEST.in
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2519 2023-08-08 11:12:41.194285 lit-17.0.0rc2/PKG-INFO
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1874 2023-05-13 06:19:19.000000 lit-17.0.0rc2/README.rst
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.172285 lit-17.0.0rc2/examples/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc2/examples/README.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.172285 lit-17.0.0rc2/examples/many-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      549 2023-07-06 03:21:05.000000 lit-17.0.0rc2/examples/many-tests/ManyTests.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      382 2022-05-20 05:53:51.000000 lit-17.0.0rc2/examples/many-tests/README.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2023-07-06 00:01:13.000000 lit-17.0.0rc2/examples/many-tests/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.173285 lit-17.0.0rc2/lit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    12039 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/BooleanExpression.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     7871 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/LitConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2023-08-01 20:33:24.000000 lit-17.0.0rc2/lit/LitTestCase.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    11087 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/ProgressBar.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3242 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/ShCommands.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8811 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13734 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/Test.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    78657 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/TestRunner.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1629 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/TestTimes.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8659 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/TestingConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      199 2023-08-08 11:12:32.000000 lit-17.0.0rc2/lit/__init__.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.173285 lit-17.0.0rc2/lit/builtin_commands/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc2/lit/builtin_commands/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1892 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/builtin_commands/cat.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9817 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/builtin_commands/diff.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    10608 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/cl_arguments.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9564 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/discovery.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5987 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/display.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.173285 lit-17.0.0rc2/lit/formats/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 03:21:05.000000 lit-17.0.0rc2/lit/formats/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2299 2023-08-01 20:33:24.000000 lit-17.0.0rc2/lit/formats/base.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13602 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/formats/googletest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      992 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/formats/shtest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.173285 lit-17.0.0rc2/lit/llvm/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-05-20 05:53:51.000000 lit-17.0.0rc2/lit/llvm/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    31158 2023-08-01 20:33:24.000000 lit-17.0.0rc2/lit/llvm/config.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5430 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/llvm/subst.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11652 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/main.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11056 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/reports.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4692 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/run.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    15927 2023-08-02 17:47:38.000000 lit-17.0.0rc2/lit/util.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit/worker.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.173285 lit-17.0.0rc2/lit.egg-info/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2519 2023-08-08 11:12:41.000000 lit-17.0.0rc2/lit.egg-info/PKG-INFO
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    21372 2023-08-08 11:12:41.000000 lit-17.0.0rc2/lit.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-08-08 11:12:41.000000 lit-17.0.0rc2/lit.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-08-08 11:12:41.000000 lit-17.0.0rc2/lit.egg-info/entry_points.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-17.0.0rc2/lit.egg-info/not-zip-safe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2023-08-08 11:12:41.000000 lit-17.0.0rc2/lit.egg-info/top_level.txt
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2023-07-06 00:01:13.000000 lit-17.0.0rc2/lit.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2023-04-28 22:43:05.000000 lit-17.0.0rc2/pyproject.toml
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2023-08-08 11:12:41.194285 lit-17.0.0rc2/setup.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1295 2023-07-06 00:01:13.000000 lit-17.0.0rc2/setup.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      152 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/.coveragerc
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/allow-retries/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/allow-retries/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       51 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       45 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/allow-retries/not-a-valid-integer.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/allow-retries/succeeds-within-limit.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/config-map-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      444 2023-08-02 17:47:38.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/driver.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/invalid-test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      281 2023-08-02 17:47:38.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/lit.alt.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/config-map-discovery/main-config/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/main-config/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/config-map-discovery/tests/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/tests/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/config-map-discovery/tests/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.176285 lit-17.0.0rc2/tests/Inputs/custom-result-category/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/custom-result-category/format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/custom-result-category/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/custom-result-category/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/custom-result-category/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      762 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/discovery/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/discovery/subdir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/discovery/subdir/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/subdir/test-three.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/discovery/subsuite/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      175 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/discovery/subsuite/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/subsuite/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/subsuite/test-two.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/test-two.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/discovery/test.not-txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/discovery-getTestsForPath/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2023-07-06 03:21:05.000000 lit-17.0.0rc2/tests/Inputs/discovery-getTestsForPath/custom_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      270 2023-07-06 03:21:05.000000 lit-17.0.0rc2/tests/Inputs/discovery-getTestsForPath/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2023-07-06 03:21:05.000000 lit-17.0.0rc2/tests/Inputs/discovery-getTestsForPath/x.test
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/exec-discovery/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      292 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/exec-discovery/lit.site.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/exec-discovery-in-tree/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/exec-discovery-in-tree/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/exec-discovery-in-tree/obj/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      205 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/exec-discovery-in-tree/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.177285 lit-17.0.0rc2/tests/Inputs/fake-externals/
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/cd
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/diff
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/env
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/export
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/fake_external.py
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/mkdir
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/fake-externals/rm
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-cmd-wrapper/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1267 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      189 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-cmd-wrapper/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-crash/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-crash/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1424 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-crash/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-detect-duplicate/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-detect-duplicate/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1350 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      131 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-detect-duplicate/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-discovery-failed/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-discovery-failed/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-discovery-failed/subdir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       80 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-format/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2741 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-format/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-format/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2742 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-sanitizer-error/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-sanitizer-error/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1506 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-sanitizer-error/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-timeout/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.178285 lit-17.0.0rc2/tests/Inputs/googletest-timeout/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1685 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      397 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/googletest-timeout/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.179285 lit-17.0.0rc2/tests/Inputs/ignore-fail/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/ignore-fail/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/ignore-fail/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/ignore-fail/unresolved.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/ignore-fail/xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/ignore-fail/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.179285 lit-17.0.0rc2/tests/Inputs/lit-opts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/lit-opts/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/lit-opts/test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.179285 lit-17.0.0rc2/tests/Inputs/lld-features/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld.lld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld.lld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       31 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld.lld.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld64.lld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld64.lld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/ld64.lld.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      714 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/lld-features/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/lld-link
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/lld-link.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/lld-link.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/wasm-ld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/wasm-ld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/lld-features/wasm-ld.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.179285 lit-17.0.0rc2/tests/Inputs/max-failures/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/max-failures/fail1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/max-failures/fail2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/max-failures/fail3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/max-failures/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.179285 lit-17.0.0rc2/tests/Inputs/max-time/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/max-time/fast.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/max-time/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/max-time/slow.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/parallelism-groups/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      474 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/parallelism-groups/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/parallelism-groups/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/parallelism-groups/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/progress-bar/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/progress-bar/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/progress-bar/test-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/progress-bar/test-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/progress-bar/test-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/progress-bar/test-4.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/py-config-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      299 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/py-config-discovery/lit.site.cfg.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/reorder/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/reorder/aaa.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/reorder/bbb.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/reorder/fff.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      173 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/reorder/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       78 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/reorder/lit_test_times
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/reorder/new-test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/reorder/subdir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/reorder/subdir/ccc.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.180285 lit-17.0.0rc2/tests/Inputs/show-result-codes/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-result-codes/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/show-result-codes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-result-codes/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       36 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-result-codes/unsupported.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-result-codes/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.181285 lit-17.0.0rc2/tests/Inputs/show-used-features/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      184 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/show-used-features/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      267 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/show-used-features/mixed.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       35 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-used-features/requires.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       42 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-used-features/unsupported.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       30 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/show-used-features/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.181285 lit-17.0.0rc2/tests/Inputs/shtest-define/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.181285 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.182285 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/before-name.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      259 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      507 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      244 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      490 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      196 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/no-name.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      222 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.182285 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      329 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      420 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      289 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      427 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      229 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      254 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      268 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.183285 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      319 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      318 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      324 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      409 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      436 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      333 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      322 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      399 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      611 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      408 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      397 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/location-range.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/errors/no-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.183285 lit-17.0.0rc2/tests/Inputs/shtest-define/examples/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1772 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/examples/param-subst.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1683 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/expansion-order.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1224 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/line-number-substitutions.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2668 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      662 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/name-chars.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      265 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/shared-substs-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/shared-substs-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      886 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/value-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      509 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/value-escaped.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3926 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-define/ws-and-continuations.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.184285 lit-17.0.0rc2/tests/Inputs/shtest-env/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-args-last-is-assign.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       14 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-args-last-is-u.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-cd.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-colon.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-echo.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      875 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-env.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-export.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-mkdir.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      198 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-not-builtin.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-rm.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      687 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env-u.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      465 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/env.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      310 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/mixed.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-env/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.184285 lit-17.0.0rc2/tests/Inputs/shtest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.185285 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/fail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      107 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      191 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/utf8_command.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      138 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      146 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/external_shell/write-control-chars.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      104 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      414 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/no-test-line.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/requires-missing.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      122 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/requires-present.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       49 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/requires-star.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      114 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/requires-triple.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      218 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported-expr-false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      174 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported-expr-true.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       52 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported-star.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.185285 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported_dir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      147 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xfail-expr-false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      151 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xfail-expr-true.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       40 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xfail-feature.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xfail-target.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-format/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.185285 lit-17.0.0rc2/tests/Inputs/shtest-format-argv0/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      320 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-format-argv0/argv0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      233 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-format-argv0/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.185285 lit-17.0.0rc2/tests/Inputs/shtest-if-else/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       93 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/test-neg1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/test-neg2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/test-neg3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/test-neg4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3294 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-if-else/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.185285 lit-17.0.0rc2/tests/Inputs/shtest-inject/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-inject/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      109 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-inject/test-empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      183 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-inject/test-many.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-inject/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.186285 lit-17.0.0rc2/tests/Inputs/shtest-keyword-parse-errors/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-keyword-parse-errors/empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      133 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       44 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       29 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-not/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/exclamation-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      211 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/exclamation-calls-external.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/fail.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/fail2.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-args-last-is-crash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       85 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-cd.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-colon.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      252 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      413 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-diff.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-echo.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-env-builtin.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       97 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-export.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1933 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-external.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      142 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-fail2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       59 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-mkdir.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       46 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-rm.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/pass.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      159 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-not/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-output-printing/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-output-printing/basic.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      150 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-output-printing/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      145 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/popd-args.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       16 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.171285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      340 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/escaping/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       28 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/escaping/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/negative-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/not-an-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.187285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/set-to-none/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.188285 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      372 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.188285 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.188285 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/external-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      125 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.188285 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/internal-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      221 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       84 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-run-at-line/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.190285 lit-17.0.0rc2/tests/Inputs/shtest-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       75 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/cat-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/cat-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      269 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/cat_nonprinting.bin
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/check_args.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/check_path.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/colon-error.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      373 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/continuations.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      513 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/dev-null.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-I.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-b.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      622 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-encodings.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      141 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-5.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-error-6.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-in.bin
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       55 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-in.dos
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       50 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-in.unix
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-in.utf16
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-in.utf8
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      734 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-pipes.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      274 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      346 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      251 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      282 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-5.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      271 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-6.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-7.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r-error-8.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      675 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      358 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      976 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-unified.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-w.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       71 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      248 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/mkdir-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/mkdir-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       74 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/mkdir-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1215 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/redirects.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/rm-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/rm-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/rm-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      120 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/rm-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/rm-unicode-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      738 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/sequencing-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/sequencing-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      157 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/stdout-encoding.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     7169 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/valid-shell.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/write-to-stderr.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      153 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.190285 lit-17.0.0rc2/tests/Inputs/shtest-timeout/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-timeout/infinite_loop.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/shtest-timeout/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       82 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/shtest-timeout/short.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.190285 lit-17.0.0rc2/tests/Inputs/standalone-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-excludes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      154 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-excludes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-excludes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-suffixes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/standalone-tests-with-suffixes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/test-data/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1172 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test-data/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test-data/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/test-data/metrics.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/test-data-micro/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1907 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test-data-micro/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test-data-micro/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      220 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/test-data-micro/micro-tests.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/test_retry_attempts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test_retry_attempts/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/test_retry_attempts/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/testrunner-custom-parsers/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/testrunner-custom-parsers/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      387 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/Inputs/testrunner-custom-parsers/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/unittest-adaptor/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/unittest-adaptor/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/unittest-adaptor/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/unittest-adaptor/test-two.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/unparsed-requirements/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/unparsed-requirements/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.191285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.192285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case10
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case10.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case2
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case2.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case3
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case3.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case6
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case6.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case7
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case7.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/build/case9.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/env-case1
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/env-case6
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1403 2023-08-02 17:47:38.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.192285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case10
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case10.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case4
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case4.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case5
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case5.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case6
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case6.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case7
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/path/case7.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.192285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search1/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search1/empty
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search2/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search2/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search2/case9.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search3/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search3/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/search3/case9.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.192285 lit-17.0.0rc2/tests/Inputs/use-llvm-tool-required/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool-required/found
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool-required/found.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      451 2023-08-02 17:47:38.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool-required/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/use-llvm-tool-required/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/xfail-cl/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/xfail-cl/a/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/a/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/a/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/a/test-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/a/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/xfail-cl/b/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/b/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/b/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/b/test-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/b/test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/false2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/true-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/Inputs/xfail-cl/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.193285 lit-17.0.0rc2/tests/Inputs/xunit-output/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/bad&name.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/dummy_format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       69 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/excluded.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/missing_feature.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       65 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/pass.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/Inputs/xunit-output/unsupported.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1954 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/allow-retries.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/boolean-parsing.py
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)      199 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/check-tested-lit-timeout-ability
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      484 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/custom-result-category.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9769 2023-08-01 20:33:24.000000 lit-17.0.0rc2/tests/discovery.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/googletest-cmd-wrapper.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1009 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/googletest-crash.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      502 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/googletest-detect-duplicate.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      337 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/googletest-discovery-failed.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      800 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/googletest-format-respect-gtest-sharding-env-vars.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1432 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/googletest-format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1234 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/googletest-sanitizer-error.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2561 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/googletest-timeout.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      640 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/ignore-fail.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1096 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/lit-opts.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5298 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      410 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/lit.site.cfg.in
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/lld-features.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1001 2023-07-06 03:21:05.000000 lit-17.0.0rc2/tests/max-failures.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/max-time.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      558 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/parallelism-groups.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      538 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/progress-bar.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      732 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/reorder.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6440 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/selecting.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       67 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/shell-parsing.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      847 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/show-result-codes.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      512 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/show-used-features.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6636 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/shtest-define.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/shtest-encoding.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     4015 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-env.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      588 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-format-argv0.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6916 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/shtest-format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      699 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/shtest-if-else.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1228 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-inject.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      581 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/shtest-keyword-parse-errors.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     5363 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-not.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      979 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-output-printing.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      636 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/shtest-pushd-popd.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1615 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-recursive-substitution.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2221 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/shtest-run-at-line.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    17367 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/shtest-shell.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3498 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/shtest-timeout.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      679 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/test-data-micro.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      353 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/test-data.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2380 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/test-output-micro-resultdb.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1624 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/test-output-micro.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1546 2023-03-31 08:26:53.000000 lit-17.0.0rc2/tests/test-output-resultdb.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      552 2023-04-28 22:43:05.000000 lit-17.0.0rc2/tests/test-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-08-08 11:12:41.194285 lit-17.0.0rc2/tests/unit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4360 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/unit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13421 2023-08-01 20:33:24.000000 lit-17.0.0rc2/tests/unit/TestRunner.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      460 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/unittest-adaptor.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      816 2023-07-06 00:01:13.000000 lit-17.0.0rc2/tests/unparsed-requirements.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/usage.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2077 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/use-llvm-tool.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1860 2022-08-02 09:00:57.000000 lit-17.0.0rc2/tests/xfail-cl.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1486 2022-05-20 05:53:51.000000 lit-17.0.0rc2/tests/xunit-output.py
```

### Comparing `lit-17.0.0rc1/LICENSE.TXT` & `lit-17.0.0rc2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/PKG-INFO` & `lit-17.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 17.0.0rc1
+Version: 17.0.0rc2
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-17.0.0rc1/README.rst` & `lit-17.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/examples/many-tests/ManyTests.py` & `lit-17.0.0rc2/examples/many-tests/ManyTests.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/BooleanExpression.py` & `lit-17.0.0rc2/lit/BooleanExpression.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/LitConfig.py` & `lit-17.0.0rc2/lit/LitConfig.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/LitTestCase.py` & `lit-17.0.0rc2/lit/LitTestCase.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/ProgressBar.py` & `lit-17.0.0rc2/lit/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/ShCommands.py` & `lit-17.0.0rc2/lit/ShCommands.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/ShUtil.py` & `lit-17.0.0rc2/lit/ShUtil.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/Test.py` & `lit-17.0.0rc2/lit/Test.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/TestRunner.py` & `lit-17.0.0rc2/lit/TestRunner.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/TestTimes.py` & `lit-17.0.0rc2/lit/TestTimes.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/TestingConfig.py` & `lit-17.0.0rc2/lit/TestingConfig.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/builtin_commands/cat.py` & `lit-17.0.0rc2/lit/builtin_commands/cat.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/builtin_commands/diff.py` & `lit-17.0.0rc2/lit/builtin_commands/diff.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/cl_arguments.py` & `lit-17.0.0rc2/lit/cl_arguments.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/discovery.py` & `lit-17.0.0rc2/lit/discovery.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/display.py` & `lit-17.0.0rc2/lit/display.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/formats/base.py` & `lit-17.0.0rc2/lit/formats/base.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/formats/googletest.py` & `lit-17.0.0rc2/lit/formats/googletest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/formats/shtest.py` & `lit-17.0.0rc2/lit/formats/shtest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/llvm/config.py` & `lit-17.0.0rc2/lit/llvm/config.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/llvm/subst.py` & `lit-17.0.0rc2/lit/llvm/subst.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/main.py` & `lit-17.0.0rc2/lit/main.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/reports.py` & `lit-17.0.0rc2/lit/reports.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/run.py` & `lit-17.0.0rc2/lit/run.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/util.py` & `lit-17.0.0rc2/lit/util.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit/worker.py` & `lit-17.0.0rc2/lit/worker.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/lit.egg-info/PKG-INFO` & `lit-17.0.0rc2/lit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 17.0.0rc1
+Version: 17.0.0rc2
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-17.0.0rc1/lit.egg-info/SOURCES.txt` & `lit-17.0.0rc2/lit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/setup.py` & `lit-17.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/allow-retries/succeeds-within-limit.py` & `lit-17.0.0rc2/tests/Inputs/allow-retries/succeeds-within-limit.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/discovery/lit.cfg` & `lit-17.0.0rc2/tests/Inputs/discovery/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/custom_format.py` & `lit-17.0.0rc2/tests/Inputs/discovery-getTestsForPath/custom_format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe` & `lit-17.0.0rc2/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-crash/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-format/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py` & `lit-17.0.0rc2/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/lld-features/lit.cfg` & `lit-17.0.0rc2/tests/Inputs/lld-features/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/examples/param-subst.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/examples/param-subst.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/expansion-order.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/expansion-order.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/line-number-substitutions.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/line-number-substitutions.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/lit.cfg` & `lit-17.0.0rc2/tests/Inputs/shtest-define/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/name-chars.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/name-chars.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-0.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/shared-substs-0.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-1.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/shared-substs-1.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/value-equals.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/value-equals.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-define/ws-and-continuations.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-define/ws-and-continuations.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-env.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-env/env-calls-env.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-env/env-u.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-env/env-u.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-env/mixed.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-env/mixed.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-if-else/test.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-if-else/test.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-external.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-not/not-calls-external.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/check_path.py` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/check_path.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/dev-null.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/dev-null.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-encodings.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-encodings.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-pipes.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-pipes.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-r.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-unified.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/diff-unified.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/redirects.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/redirects.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-0.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/sequencing-0.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-shell/valid-shell.txt` & `lit-17.0.0rc2/tests/Inputs/shtest-shell/valid-shell.txt`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/shtest-timeout/lit.cfg` & `lit-17.0.0rc2/tests/Inputs/shtest-timeout/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/test-data/dummy_format.py` & `lit-17.0.0rc2/tests/Inputs/test-data/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/test-data-micro/dummy_format.py` & `lit-17.0.0rc2/tests/Inputs/test-data-micro/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/test_retry_attempts/test.py` & `lit-17.0.0rc2/tests/Inputs/test_retry_attempts/test.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/use-llvm-tool/lit.cfg` & `lit-17.0.0rc2/tests/Inputs/use-llvm-tool/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/Inputs/xunit-output/dummy_format.py` & `lit-17.0.0rc2/tests/Inputs/xunit-output/dummy_format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/allow-retries.py` & `lit-17.0.0rc2/tests/allow-retries.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/discovery.py` & `lit-17.0.0rc2/tests/discovery.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/googletest-crash.py` & `lit-17.0.0rc2/tests/googletest-crash.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/googletest-format-respect-gtest-sharding-env-vars.py` & `lit-17.0.0rc2/tests/googletest-format-respect-gtest-sharding-env-vars.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/googletest-format.py` & `lit-17.0.0rc2/tests/googletest-format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/googletest-sanitizer-error.py` & `lit-17.0.0rc2/tests/googletest-sanitizer-error.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/googletest-timeout.py` & `lit-17.0.0rc2/tests/googletest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/ignore-fail.py` & `lit-17.0.0rc2/tests/ignore-fail.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/lit-opts.py` & `lit-17.0.0rc2/tests/lit-opts.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/lit.cfg` & `lit-17.0.0rc2/tests/lit.cfg`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/max-failures.py` & `lit-17.0.0rc2/tests/max-failures.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/parallelism-groups.py` & `lit-17.0.0rc2/tests/parallelism-groups.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/progress-bar.py` & `lit-17.0.0rc2/tests/progress-bar.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/reorder.py` & `lit-17.0.0rc2/tests/reorder.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/selecting.py` & `lit-17.0.0rc2/tests/selecting.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/show-result-codes.py` & `lit-17.0.0rc2/tests/show-result-codes.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/show-used-features.py` & `lit-17.0.0rc2/tests/show-used-features.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-define.py` & `lit-17.0.0rc2/tests/shtest-define.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-env.py` & `lit-17.0.0rc2/tests/shtest-env.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-format-argv0.py` & `lit-17.0.0rc2/tests/shtest-format-argv0.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-format.py` & `lit-17.0.0rc2/tests/shtest-format.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-if-else.py` & `lit-17.0.0rc2/tests/shtest-if-else.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-inject.py` & `lit-17.0.0rc2/tests/shtest-inject.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-keyword-parse-errors.py` & `lit-17.0.0rc2/tests/shtest-keyword-parse-errors.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-not.py` & `lit-17.0.0rc2/tests/shtest-not.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-output-printing.py` & `lit-17.0.0rc2/tests/shtest-output-printing.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-pushd-popd.py` & `lit-17.0.0rc2/tests/shtest-pushd-popd.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-recursive-substitution.py` & `lit-17.0.0rc2/tests/shtest-recursive-substitution.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-run-at-line.py` & `lit-17.0.0rc2/tests/shtest-run-at-line.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-shell.py` & `lit-17.0.0rc2/tests/shtest-shell.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/shtest-timeout.py` & `lit-17.0.0rc2/tests/shtest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/test-data-micro.py` & `lit-17.0.0rc2/tests/test-data-micro.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/test-output-micro-resultdb.py` & `lit-17.0.0rc2/tests/test-output-micro-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/test-output-micro.py` & `lit-17.0.0rc2/tests/test-output-micro.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/test-output-resultdb.py` & `lit-17.0.0rc2/tests/test-output-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/test-output.py` & `lit-17.0.0rc2/tests/test-output.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/unit/ShUtil.py` & `lit-17.0.0rc2/tests/unit/ShUtil.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/unit/TestRunner.py` & `lit-17.0.0rc2/tests/unit/TestRunner.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/unparsed-requirements.py` & `lit-17.0.0rc2/tests/unparsed-requirements.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/use-llvm-tool.py` & `lit-17.0.0rc2/tests/use-llvm-tool.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/xfail-cl.py` & `lit-17.0.0rc2/tests/xfail-cl.py`

 * *Files identical despite different names*

### Comparing `lit-17.0.0rc1/tests/xunit-output.py` & `lit-17.0.0rc2/tests/xunit-output.py`

 * *Files identical despite different names*

