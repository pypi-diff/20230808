# Comparing `tmp/spekk-1.0.1.tar.gz` & `tmp/spekk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spekk-1.0.1.tar", last modified: Fri Jul 21 18:32:36 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `spekk-1.0.1.tar` & `spekk-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,716 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.856966 spekk-1.0.1/
--rw-r--r--   0 magnus     (501) staff       (20)    11356 2023-07-21 15:08:01.000000 spekk-1.0.1/LICENSE
--rw-r--r--   0 magnus     (501) staff       (20)     7896 2023-07-21 18:32:36.856439 spekk-1.0.1/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     7351 2023-07-21 15:03:13.000000 spekk-1.0.1/README.md
--rw-r--r--   0 magnus     (501) staff       (20)      581 2023-07-21 18:32:17.000000 spekk-1.0.1/pyproject.toml
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-07-21 18:32:36.857106 spekk-1.0.1/setup.cfg
--rw-r--r--   0 magnus     (501) staff       (20)      302 2023-07-21 18:32:20.000000 spekk-1.0.1/setup.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.819606 spekk-1.0.1/spekk/
--rw-r--r--   0 magnus     (501) staff       (20)       77 2023-07-21 18:32:25.000000 spekk-1.0.1/spekk/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    12630 2023-07-19 08:18:35.000000 spekk-1.0.1/spekk/spec.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.839609 spekk-1.0.1/spekk/transformations/
--rw-r--r--   0 magnus     (501) staff       (20)     6475 2023-07-21 14:41:00.000000 spekk-1.0.1/spekk/transformations/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2151 2023-07-18 12:37:43.000000 spekk-1.0.1/spekk/transformations/apply.py
--rw-r--r--   0 magnus     (501) staff       (20)     3619 2023-07-18 13:20:36.000000 spekk-1.0.1/spekk/transformations/axis.py
--rw-r--r--   0 magnus     (501) staff       (20)    15523 2023-07-19 07:38:43.000000 spekk-1.0.1/spekk/transformations/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2965 2023-07-19 08:22:04.000000 spekk-1.0.1/spekk/transformations/common.py
--rw-r--r--   0 magnus     (501) staff       (20)     3784 2023-07-21 14:42:27.000000 spekk-1.0.1/spekk/transformations/for_all.py
--rw-r--r--   0 magnus     (501) staff       (20)     5805 2023-07-18 13:45:41.000000 spekk-1.0.1/spekk/transformations/reduce.py
--rw-r--r--   0 magnus     (501) staff       (20)     1970 2023-07-18 13:46:06.000000 spekk-1.0.1/spekk/transformations/wrap.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.847224 spekk-1.0.1/spekk/trees/
--rw-r--r--   0 magnus     (501) staff       (20)      663 2023-07-19 08:08:29.000000 spekk-1.0.1/spekk/trees/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     7070 2023-07-18 13:09:43.000000 spekk-1.0.1/spekk/trees/core.py
--rw-r--r--   0 magnus     (501) staff       (20)     5672 2023-07-21 13:57:38.000000 spekk-1.0.1/spekk/trees/registry.py
--rw-r--r--   0 magnus     (501) staff       (20)     5109 2023-07-18 13:00:44.000000 spekk-1.0.1/spekk/trees/treelens.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.854656 spekk-1.0.1/spekk/util/
--rw-r--r--   0 magnus     (501) staff       (20)      342 2023-07-18 13:53:37.000000 spekk-1.0.1/spekk/util/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5165 2023-07-18 13:46:46.000000 spekk-1.0.1/spekk/util/flatten.py
--rw-r--r--   0 magnus     (501) staff       (20)      712 2023-07-21 13:59:51.000000 spekk-1.0.1/spekk/util/shape.py
--rw-r--r--   0 magnus     (501) staff       (20)     3110 2023-07-18 13:49:24.000000 spekk-1.0.1/spekk/util/slicing.py
--rw-r--r--   0 magnus     (501) staff       (20)     8012 2023-07-18 13:58:57.000000 spekk-1.0.1/spekk/util/validation.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.823484 spekk-1.0.1/spekk.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     7896 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      673 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/top_level.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 spekk-1.0.3/.env
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 spekk-1.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 spekk-1.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/tmp9m1yugmy.tar.gz
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 spekk-1.0.3/tmpsoogpd87cacert.pem
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/Activate.ps1
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/activate
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/activate.csh
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/activate.fish
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/hatchling
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/pip
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/pip3
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/pip3.9
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/python3 -> /home/magnusk/miniconda3/envs/vbeam/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/bin/python3.9 -> python3
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables/py.typed
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables/redirector.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables-0.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables-0.5.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables-0.5.dist-info/METADATA
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables-0.5.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/editables-0.5.dist-info/WHEEL
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/__main__.py
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/build.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/ouroboros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/bridge/__init__.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/bridge/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/__init__.py
+-rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/app.py
+-rw-r--r--   0        0        0    39377 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/constants.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/custom.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/sdist.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/utils.py
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/custom.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/plugin/__init__.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/plugin/hooks.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/hooks/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/plugin/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/plugin/hooks.py
+-rw-r--r--   0        0        0    15682 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/builders/plugin/interface.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/cli/__init__.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/cli/build/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/cli/dep/__init__.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/cli/metadata/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/cli/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/dep/__init__.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/dep/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/licenses/__init__.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/licenses/parse.py
+-rw-r--r--   0        0        0    35020 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/licenses/supported.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/__init__.py
+-rw-r--r--   0        0        0    59933 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/core.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/custom.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/spec.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/plugin/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/plugin/hooks.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/metadata/plugin/interface.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/plugin/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/plugin/exceptions.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/plugin/manager.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/plugin/specs.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/plugin/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/utils/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/utils/constants.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/utils/context.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/utils/fs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/__init__.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/scheme/__init__.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/scheme/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/scheme/plugin/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/scheme/plugin/hooks.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/scheme/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/__init__.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/code.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/env.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/plugin/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/plugin/hooks.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling/version/source/plugin/interface.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/hatchling-1.18.0.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/packaging-23.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/__init__.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/_meta.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/gitignore.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/pathspec.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/pattern.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/py.typed
+-rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/util.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/patterns/__init__.py
+-rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec/patterns/gitwildmatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec-0.11.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec-0.11.2.dist-info/LICENSE
+-rw-r--r--   0        0        0    19563 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec-0.11.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec-0.11.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pathspec-0.11.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    24244 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    16507 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35763 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    97992 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    37414 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45686 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    26070 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14298 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0    76671 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pip-23.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_callers.py
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_hooks.py
+-rw-r--r--   0        0        0    17944 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_manager.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_result.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_tracing.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy/_version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0    40186 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/METADATA
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 spekk-1.0.3/build-env-ldszqng8/lib/python3.9/site-packages/trove_classifiers-2023.8.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/make.bat
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/_static/spekk_logo.png
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/_templates/class-template.rst
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 spekk-1.0.3/docs/_templates/module-template.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/__init__.py
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/spec.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/apply.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/axis.py
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/base.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/common.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/for_all.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/reduce.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/transformations/wrap.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/trees/__init__.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/trees/core.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/trees/registry.py
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/trees/treelens.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/util/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/util/flatten.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/util/shape.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/util/slicing.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 spekk-1.0.3/spekk/util/validation.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/test_spec.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/test_transformations.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/test_helpers/mock_data.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/test_helpers/generators/spec.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/transformations/test_for_all.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/transformations/test_partial_transformations.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/transformations/test_reduce.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 spekk-1.0.3/tests/util/test_flatten.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spekk-1.0.3/tmpaai92nfe/input.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spekk-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 spekk-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 spekk-1.0.3/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 spekk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 spekk-1.0.3/PKG-INFO
```

### Comparing `spekk-1.0.1/LICENSE` & `spekk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/README.md` & `spekk-1.0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,131 @@
 # spekk is a tool for working with named dimensions for arrays
-`spekk` lets you declare specifications of the shapes of your arrays.
-
-A common problem with array programming (i.e. working with libraries such as NumPy or JAX) is that an array can have many dimensions, and it can be easy to get them wrong. Additionally, dimensions may be "shared" across different arrays, for example a `"batch"` dimension may exist both for a set of images and their corresponding label tokens — each element in the `"batch"` dimension consist of one image and one label. `spekk` attempts to solve this by providing a way to declare the dimensions of arrays using a class called `Spec`.
+![spekk logo](docs/_static/spekk_logo.png)
 
-`spekk` exists independently of the underlying arrays and can thus be used to specify the dimensions of both NumPy and JAX arrays (or anything else that has a `shape` property).
+`spekk` lets you declare specifications of the shapes of your arrays.
 
+A common problem with multidimensional arrays is that it can be hard to keep track of the dimensions of the data over time. Additionally, dimensions may be "shared" across different arrays. For example, two different arguments to a function may share a dimension, like the positions of receiving elements in an ultrasound array and their corresponding recorded signals.
 
-# How does it work
-Anything that can be represented as a (nested) tree of arrays _(see `spekk.trees.registry.TreeDef`)_ can be specced. This means that we can easily spec custom classes, dictionaries, or the arguments to a function:
+`spekk` attempts to solve this by providing a way to declare the dimensions of arrays using a class called `Spec`:
 
 ```python
+import numpy as np
 from spekk import Spec
-import numpy.random as random
 
-def foo(images, labels):
-    ...
+# Anything that is a collection of key-value pairs can be used as a container of arrays:
+spec = Spec({
+    "receiving_element": { # <- You could also use your own custom class instead of dict
+        "position": ["receivers", "xyz"],
+        "weight": ["receivers"],
+    },
+    "signal": ["transmits", "receivers", "samples"],
+})
+# my_fn = lambda signal, receiving_element: ...
+```
 
-spec = Spec(
-    {
-        "images": ["batch", "width", "height"],  # <-  Dimensions are always a sequence of strings
-        "labels": ["batch", "label_tokens"],  # <- "labels" also have a "batch" dimension
-        # Since both "images" and "labels" have a "batch" dimension, they should be iterated over together
-    }
-)
-# The data could look like this:
-data = {
-    # batch-size = 32
-    # width = height = 128 pixels
-    # Number of tokens per label = 10
-    "images": random.normal(size=(32, 128, 128)),
-    "labels": random.normal(size=(32, 10)),
-}
-spec.validate(data)  # <- This is OK!
+`spekk` exists independently of the underlying arrays and can thus be used to specify the dimensions of both NumPy and JAX arrays (or anything else that has a `shape` property). This is useful when working with code that need to support multiple array backends.
+
+See [an overview of spekk](#overview) below. [Read the documentation](https://spekk.readthedocs.io/) for more details.
+
+
+# Installation
+```bash
+python3 -m pip install spekk
+```
+
+
+# Overview
+`spekk` lets you name the dimensions of an array as a sequence of strings:
+
+```python
+import numpy as np
+from spekk import Spec
 
-# We can get the indices in the data for a given dimension:
-assert spec.index_for("batch") == {"images": 0, "labels": 0}
-assert spec.index_for("width") == {"images": 1, "labels": None}
-assert spec.index_for("height") == {"images": 2, "labels": None}
+data = np.ones([4, 5, 6])  # A 3D array with shape [4, 5, 6].
+spec = Spec(["transmits", "receivers", "samples"])  # <- The names of the dimensions, 
+                                                    #    each name corresponding to an 
+                                                    #    axis in the array ([4, 5, 6]).
 ```
 
-We can also spec more complex nested data structures:
+It also lets you specify the dimensions of nested data structures of arrays:
 
 ```python
 data = {
-    "particles": {
-        # The last dimension (with size = 2) represent the x- and y-components of the position and velocity.
-        "position": random.random(size=(3, 2)),
-        "velocity": random.random(size=(4, 3, 2)),
+    "receiving_element": {
+        "position": np.ones([5, 3]),
+        "weight": np.ones([5]),
     },
-    "attractors": {
-        "position": random.random(size=(5, 2)),
-        "strength": random.random(size=(5,)),
-    },
-}
-spec = Spec(
-    {
-        "particles": {
-            # We can ignore trailing dimensions such as the x- and y-components above
-            "position": ["particles"],
-            "velocity": ["starting_velocities", "particles"],
-        },
-        "attractors": {
-            "position": ["attractors"],
-            "strength": ["attractors"],
-        },
-    }
-)
-spec.validate(data)
-assert spec.index_for("particles") == {
-    "particles": {"position": 0, "velocity": 1},
-    "attractors": {"position": None, "strength": None},
+    "signal": np.ones([4, 5, 6]),
 }
+# Note that the structure is the same as the data:
+spec = Spec({
+    "receiving_element": {
+        "position": ["receivers", "xyz"],
+        "weight": ["receivers"],
+    },
+    "signal": ["transmits", "receivers", "samples"],
+})
 ```
 
-
-## Building up more complex specced functions using function transformations
-`spekk` is quite verbose, but it gets more useful when used as a building block for describing what happens to data when it is passed as arguments to a function.
-
-Let's say we have a function that takes a point at position (`x`, `y`) and a scalar value `c` and returns the value of a circle and a hyperbola at that point:
+You can spec what happens to data when you apply some function to it:
 
 ```python
+from spekk.transformations import Specced
+
 def f(x, y, c):
-    "Return a dictionary of a circle and a hyperbola evaluated at point (x, y)."
+    """Return a dictionary of a circle and two hyperbolas (one for each axis) evaluated 
+    at point (x, y) with radius/axis-width c."""
     return {
-        "circle":    x**2 + y**2 - c**2,
-        "hyperbola": x**2 - y**2 - c**2,
+        "circle": x**2 + y**2 - c**2,
+        "hyperbola": [
+            x**2 - y**2 - c**2,
+            x**2 - y**2 + c**2
+        ],
     }
-```
 
-We can spec this function by wrapping it in a `Specced` object. The `Specced` function acts the same as the original function when called, but it additionally describes what happens to the `input_spec` (aka the spec of the arguments to the function) after it has been called. In this case we assume (without actually checking) that all input arguments are scalars, and we return a dictionary with two numbers, one for the circle and one for the hyperbola:
-
-```python
-from spekk.transformations import Specced
+# Ignore input_spec and just return the output_spec:
+specced_f = Specced(f, lambda input_spec: {"circle": [], "hyperbola": ["axes"]})
+specced_f = specced_f.build(spec) # <- Let the function know about the spec
 
-specced_f = Specced(f, lambda input_spec: {"circle": (), "hyperbola": ()})  # An empty dimensions-sequence represent a 0-dimensional array, also called a scalar
-
-# The returned values are the same before and after speccing the function:
 assert f(x=1, y=2, c=3) == specced_f(x=1, y=2, c=3)
+assert specced_f.output_spec == Spec({"circle": [], "hyperbola": ["axes"]})
 ```
 
-But what if we want a function that takes a list of `x`-values and a list of `y`-values and evaluate `f` on all the points in the grid? It would be nice if we could write it like this:
+You can describe what happens to the spec of a function when you transform the function, for example when transforming it to loop over the arguments:
 
 ```python
 from spekk.transformations import ForAll, compose
+from spekk.util import shape
+
+# The following spec represent the input kwargs to the function f:
+spec = Spec({"x": ["x-values"], "y": ["y-values"], "c": ["c-values"]})
 
-f_for_grid = compose(
+tf = compose(
     specced_f,
     ForAll("y-values"),  # Run it for all the y-values (all rows)
-    ForAll("x-values"),  # Run it for all the x-values (all columns)
-)
-```
-
-This is valid `spekk` code. `compose` wraps each function in the previous step with a transformation, so starting with `specced_f`, `ForAll("y-values")` transforms it into a function that automatically runs it for all the `"y-values"` (defined by a spec as shown below). `ForAll("x-values")` then takes the result of the function transformation and transforms it again to run for all the `"x-values"`.
-
-Let's create some example data and define the corresponding spec:
+    ForAll("x-values"),  # Run that for all the x-values (all columns)
+    ForAll("c-values"),  # And then run that for all values of c
+).build(spec)  # <- Building the transformed function lets it know the spec of the data
+               #    so that it also knows how to loop over it.
+result = tf(x=np.linspace(-5, 5, 10), y=np.linspace(-5, 5, 11), c=np.arange(1, 6))
 
-```python
-import numpy as np
-
-# A grid of points with shape (20, 30)
-x = np.linspace(-5, 5, 20)  # 20 columns
-y = np.linspace(-5, 5, 30)  # 30 rows
-c = 2
-
-# The corresponding spec may look like this:
-spec = Spec({"x": ["x-values"], "y": ["y-values"]})
+assert shape(result["circle"]) == (5, 10, 11)
+assert tf.output_spec == Spec({
+    "circle":    ["c-values", "x-values", "y-values"],
+    "hyperbola": ["c-values", "x-values", "y-values", "axes"],
+})
 ```
 
-We let the transformed function know about the dimensions of the data by building it with the spec:
+You may use more powerful frameworks when transforming functions using `ForAll`:
 
 ```python
-f_for_grid = f_for_grid.build(spec)  # Now it knows how to loop over the data :)
+from functools import partial
+import jax
 
-# We can call it now with the lists of x- and y-values:
-result = f_for_grid(x=x, y=y, c=c)
-# result is a dictionary with keys "circle" and "hyperbola", each value is a 2D list 
-# with shape (20, 30), corresponding to the output_spec:
-assert f_for_grid.output_spec == Spec({
-    "circle":    ["x-values", "y-values"],
-    "hyperbola": ["x-values", "y-values"],
-})
+# Use JAX's vmap to vectorize the function in order to run in parallel on GPUs:
+ForAll_jax = partial(ForAll, vmap_impl=jax.vmap)
 ```
 
-We can further transform the function over arbitrary dimensions, as long as we also update the spec:
+In most cases, Numpy broadcasting will be enough to get the desired result when working with multidimensional data. However, broadcasting can sometimes be difficult or inefficient to get right, and it can be hard to keep track of the dimensions of the arrays over time. `ForAll` makes it easier to write code that loops over arbitrary dimensions and — if used in conjunction with for example JAX and `jax.vmap` — it can be very efficient as well.
 
-```python
-f_for_all_xyc = compose(
-    f_for_grid,
-    ForAll("c-values"),
-).build(spec.replace({"c": ["c-values"]}))  # <- Update the spec to include the "c-values" dimension for the c argument.
-
-# We can now call it with multiple values for "c" as well:
-result = f_for_grid(x=x, y=y, c=np.arange(0, 6))  # <- 6 values for "c"
-# result is a dictionary with keys "circle" and "hyperbola", each value is a 2D list 
-# with shape (20, 30), corresponding to the output_spec:
-assert f_for_all_xyc.output_spec == Spec({
-    "circle":    ["c-values", "x-values", "y-values"],
-    "hyperbola": ["c-values", "x-values", "y-values"],
-})
-
-from spekk.util import shape
-assert shape(result["circle"]) == (6, 20, 30)  # <- 6 values for "c"
-```
+[Read the documentation](https://spekk.readthedocs.io/) for more details.
 
-In many cases, broadcasting in Numpy will be enough to get the desired result. However, broadcasting can sometimes be difficult or inefficient to get right, and it can be hard to keep track of the dimensions of the arrays. `ForAll` makes it easier to write code that loops over arbitrary dimensions, and if used in conjunction with JAX and `jax.vmap` it can be very efficient as well.
```

### Comparing `spekk-1.0.1/spekk/spec.py` & `spekk-1.0.3/spekk/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,38 @@
                 return _is_spec_leaf(self.tree)
             else:
                 # is_leaf was called as a static method
                 return _is_spec_leaf(self)
         else:
             return _is_spec_leaf(tree)
 
-    def remove_dimension(self, dimension: str, path: Sequence = ()) -> "Spec":
+    def remove_dimension(
+        self,
+        dimension: Union[str, Sequence[str]],
+        path: Sequence = (),
+    ) -> "Spec":
         """Remove the given dimension from everywhere in the spec.
 
         >>> spec = Spec({"signal": ["transmits", "receivers"],
         ...              "receiver": {"position": ["receivers"], "direction": []}})
         >>> spec.remove_dimension("receivers")
         Spec({'signal': ['transmits'], 'receiver': {'position': [], 'direction': []}})
+
+        You can also remove multiple dimensions at once:
+
+        >>> spec.remove_dimension(["transmits", "receivers"])
+        Spec({'signal': [], 'receiver': {'position': [], 'direction': []}})
         """
         state = self.get(path)
+
+        if isinstance(dimension, (list, tuple, set)):
+            for dim in dimension:
+                state = state.remove_dimension(dim, path)
+            return state
+
         for leaf in leaves(state.tree, self.is_leaf):
             if dimension in leaf.value:
                 state = state.set([x for x in leaf.value if x != dimension], leaf.path)
         return state
 
     def index_for(self, dimension: str, path: Sequence = ()) -> Tree:
         """Return the indices of the given dimension in the spec with the same
@@ -121,15 +136,15 @@
         >>> spec = Spec({"signal": ["transmits", "receivers"],
         ...              "receiver": {"position": ["receivers"], "direction": []},
         ...              "point_position": ["transmits", "points"]})
         >>> sorted(spec.dimensions)
         ['points', 'receivers', 'transmits']
         """
         return reduce(
-            lambda dims, leaf: dims.union(leaf.value),
+            lambda dims, leaf: dims.union(leaf.value if leaf.value is not None else []),
             leaves(self.tree, self.is_leaf),
             set(),
         )
 
     def has_dimension(self, *dimensions: str) -> bool:
         """Return True if the spec has the given dimension(s).
 
@@ -202,15 +217,15 @@
         Spec({'foo': {'baz': ['c']}, 'bar': ['b']})
         """
         state = self.tree
         for replacement in traverse(replacements, self.is_leaf):
             if replacement.value is None:
                 state = trees.remove(state, replacement.path)
             elif replacement.is_leaf or self.is_leaf(
-                trees.get(state, replacement.path)
+                trees.get(state, replacement.path, None)
             ):
                 state = trees.set(state, replacement.value, replacement.path)
             else:
                 replacement_value = trees.filter(
                     replacement.value,
                     self.is_leaf,
                     lambda tree: tree is not None,
```

### Comparing `spekk-1.0.1/spekk/transformations/__init__.py` & `spekk-1.0.3/spekk/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/transformations/apply.py` & `spekk-1.0.3/spekk/transformations/apply.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/transformations/axis.py` & `spekk-1.0.3/spekk/transformations/axis.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/transformations/base.py` & `spekk-1.0.3/spekk/transformations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The base classes and abstract classes for working with :class:`Transformation`s."""
+"""The base classes and abstract classes for working with :class:`Transformation`."""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Callable, Optional, Sequence, TypeVar, Union
 
 from spekk import Spec
 from spekk.transformations.common import get_fn_name
@@ -209,15 +209,15 @@
                 e.original_exception, self, e.error_step
             ) from e.original_exception
         except Exception as e:
             # An exception was raised in this step.
             raise TransformedFunctionError(e, self, self) from e
 
     def traverse(self, *, depth_first: bool = False):
-        """Recursively yield the potentially nested :class:`TransformedFunction`s.
+        """Recursively yield the potentially nested :class:`TransformedFunction`.
 
         >>> from spekk.transformations import ForAll, compose, TransformedFunction
         >>> tf = compose(abs, ForAll("x"), ForAll("y"))
         >>> for t in tf.traverse():
         ...     if isinstance(t, TransformedFunction):
         ...         t = t.transformation  # Print transformation, not TransformedFunction
         ...     print(repr(t))
@@ -259,15 +259,17 @@
             the wrapped function after the transformation has been applied.
         transform_output_spec: A function that returns the final returned spec of the
             transformed function.
     """
 
     def __call__(self, wrapped_fn: callable) -> TransformedFunction:
         "Transform the wrapped function."
-        if isinstance(wrapped_fn, Transformation):
+        if isinstance(wrapped_fn, PartialTransformation):
+            return PartialTransformation([*wrapped_fn.partial_transformations, self])
+        elif isinstance(wrapped_fn, Transformation):
             # Handle partial application of transformations.
             return PartialTransformation([wrapped_fn, self])
         return TransformedFunction(wrapped_fn, self)
 
     @abstractmethod
     def transform_function(
         self, wrapped_fn: callable, input_spec: Spec, output_spec: Spec
@@ -297,15 +299,15 @@
         """
 
 
 @dataclass
 class PartialTransformation(Transformation):
     """A partially applied transformation.
 
-    :class:`PartialTransformation`s lets us compose transformations such that they can
+    :class:`PartialTransformation` lets us compose transformations such that they can
     be re-used as building blocks. For example, in the below code, ``tf_partial`` and
     ``tf_full`` are equivalent:
 
     >>> import numpy as np
     >>> from spekk.transformations import ForAll, compose
 
     Let's create an example kernel function along with some data and a spec:
```

### Comparing `spekk-1.0.1/spekk/transformations/common.py` & `spekk-1.0.3/spekk/transformations/common.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/transformations/for_all.py` & `spekk-1.0.3/spekk/transformations/for_all.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,85 @@
 """:class:`ForAll` transforms a function that works on scalar inputs such that it works 
 on arrays instead (vectorization), and can be used with :func:`jax.vmap`."""
 
-from dataclasses import dataclass
 from typing import Callable, Optional, Sequence
 
 from spekk import Spec, trees, util
 from spekk.transformations import Transformation, common
 
 T_in_axes = Sequence[Optional[int]]
 T_vmap = Callable[[callable, T_in_axes], callable]
 
 
-@dataclass
 class ForAll(Transformation):
     """Vectorize/"make looped" a function such that it works on arrays instead of
     scalars.
-    """
 
-    dimension: str  #: The dimension to vectorize/loop over.
-    vmap_impl: Optional[
-        T_vmap
-    ] = None  #: The ``vmap`` implementation to use. Defaults to a simple Python implementation, but can also (for example) be set to :func:`jax.vmap`.
+    >>> from spekk.transformations import ForAll, compose
+    >>> f = lambda x, y: x + y
+    >>> data =       {"x": range(2), "y": range(3)}
+    >>> spec = Spec( {"x": ["dim1"], "y": ["dim2"]} )
+
+    Transform f to run on a grid defined by the "dim1" and "dim2" dimensions:
+
+    >>> tf = compose(f, ForAll("dim2"), ForAll("dim1")).build(spec)
+    >>> tf.output_spec
+    Spec(['dim1', 'dim2'])
+    >>> result = tf(**data)
+    >>> util.shape(result)
+    (2, 3)
+    >>> result
+    [[0, 1, 2], [1, 2, 3]]
+
+    You can also use vmap over multiple dimensions at once. Note that the order of the 
+    dimensions in ``ForAll("dim2"), ForAll("dim1")`` and ``ForAll("dim1", "dim2")`` is 
+    reversed:
+
+    >>> tf = compose(f, ForAll("dim1", "dim2")).build(spec)
+    >>> tf(**data)  # This results in the same as in the previous example
+    [[0, 1, 2], [1, 2, 3]]"""
+
+    def __init__(
+        self,
+        dimension: str,
+        *additional_dimensions: str,
+        vmap_impl: Optional[T_vmap] = None,
+    ):
+        self.dimensions = [dimension, *additional_dimensions]
+        self.vmap_impl = vmap_impl
 
     def transform_function(
         self, to_be_transformed: callable, input_spec: Spec, output_spec: Spec
     ) -> callable:
-        if not input_spec.has_dimension(self.dimension):
-            raise ValueError(f"Spec does not contain the dimension {self.dimension}.")
-        return specced_vmap(
-            to_be_transformed, input_spec, self.dimension, self.vmap_impl
-        )
+        transformed = to_be_transformed
+        remaining_dimensions = set(self.dimensions)
+        for dimension in reversed(self.dimensions):
+            if not input_spec.has_dimension(dimension):
+                raise ValueError(f"Spec does not contain the dimension {dimension}.")
+            remaining_dimensions.remove(dimension)
+            transformed = specced_vmap(
+                transformed,
+                input_spec.remove_dimension(remaining_dimensions),
+                dimension,
+                self.vmap_impl,
+            )
+        return transformed
 
     def transform_input_spec(self, spec: Spec) -> Spec:
         # The returned function works on 1 element of the dimension at a time, so it has
         # one less dimension.
-        return spec.remove_dimension(self.dimension)
+        return spec.remove_dimension(self.dimensions)
 
     def transform_output_spec(self, spec: Spec) -> Spec:
-        # We re-add the dimension after the function has been applied to each element.
-        return spec.update_leaves(lambda dimensions: [self.dimension, *dimensions])
+        # The dimensions are re-added after vmapping the wrapped function.
+        return spec.update_leaves(lambda dimensions: [*self.dimensions, *dimensions])
 
     def __repr__(self) -> str:
-        return f'ForAll("{self.dimension}")'
+        dimensions_str = ", ".join([repr(dim) for dim in self.dimensions])
+        return f"ForAll({dimensions_str})"
 
 
 def specced_vmap(
     f: callable,
     spec: Spec,
     dimension: str,
     vmap_impl: Optional[T_vmap] = None,
@@ -99,7 +133,13 @@
             result0, lambda x: isinstance(x, list) or not trees.has_treedef(x)
         ):
             values = [trees.get(_result, leaf.path) for _result in all_results]
             combined_result = trees.set(combined_result, values, leaf.path)
         return combined_result
 
     return wrapped
+
+
+if __name__ == "__main__":
+    import doctest
+
+    doctest.testmod()
```

### Comparing `spekk-1.0.1/spekk/transformations/reduce.py` & `spekk-1.0.3/spekk/transformations/reduce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """:class:`Reduce` transforms a function that works on scalar inputs such that it works 
 on arrays instead and iteratively reduces the values of a dimension. For example, 
 ``Reduce.Sum("dimension")`` produces equivalent results as a ``ForAll("dimension")`` 
 followed by an ``Apply(np.sum, "dimension")`` transformation, but will potentially use 
 less memory because it sums the partial results iteratively isntead of trying to 
 parallelize over the dimension first (in the case of using GPU-backends such as JAX).
 """
-
 import operator
-from dataclasses import dataclass
-from typing import Any, Callable, Iterable, Optional, TypeVar
+from dataclasses import dataclass, field
+from typing import Any, Callable, Dict, Iterable, Optional, Sequence, TypeVar
 
-from spekk import Spec, util
+from spekk import Spec, trees, util
 from spekk.transformations import Transformation, common
+from spekk.transformations.axis import Axis, concretize_axes
 
+T_reduce_cls = TypeVar("T_reduce_cls", bound="Reduce")
 T_f_result = TypeVar("T_f_result")
 T_reduction_result = TypeVar("T_reduction_result")
 T_reduce_fn = Callable[[T_reduction_result, T_f_result], T_reduction_result]
 T_reduce = Callable[[T_reduce_fn, Iterable, T_reduction_result], T_reduction_result]
 
 
 @dataclass
@@ -34,84 +35,109 @@
     """
 
     dimension: str  #: The dimension to reduce over.
     reduce_fn: T_reduce_fn  #: The function to reduce with. For example operator.add for summation.
     initial_value: Optional[
         T_reduction_result
     ] = None  #: The initial value for the reduction. For example 0 for summation.
+    enumerate: bool = False  #: If True, each item is a tuple of (index, value), similar to Python's built-in :func:`enumerate`.
+    extra_args: Sequence[Any] = field(
+        default_factory=tuple
+    )  #: Extra arguments to pass to the reduce function.
+    extra_kwargs: Dict[str, Any] = field(
+        default_factory=dict
+    )  #: Extra keyword arguments to pass to the reduce function.
     reduce_impl: Optional[
         T_reduce
     ] = None  #: The ``reduce`` implementation to use. Defaults to Python's built-in :func:`functools.reduce`.
 
     def __post_init__(self):
-        if self.reduce_impl is None:
-            import functools
-
-            self.reduce_impl = functools.reduce
+        "Sub-classes may override this method to perform additional initialization."
 
     def transform_function(
         self, to_be_transformed: callable, input_spec: Spec, output_spec: Spec
     ) -> callable:
         if not input_spec.has_dimension(self.dimension):
             raise ValueError(f"Spec does not contain the dimension {self.dimension}.")
 
         def wrapped(*_unsupported_positional_args, **kwargs):
             if _unsupported_positional_args:
                 raise ValueError(
                     "Positional arguments are not supported when using Reduce. Use keyword arguments when calling the transformed function instead."
                 )
+            extra_args, extra_kwargs = concretize_axes(
+                output_spec, self.extra_args, self.extra_kwargs
+            )
+            reduce_fn = lambda *args, **kwargs: self.reduce_fn(
+                *args, *extra_args, **kwargs, **extra_kwargs
+            )
             return specced_map_reduce(
                 to_be_transformed,
-                self.reduce_fn,
+                reduce_fn,
                 kwargs,
                 input_spec,
                 self.dimension,
                 self.initial_value,
+                self.enumerate,
                 self.reduce_impl,
             )
 
         return wrapped
 
     def transform_input_spec(self, spec: Spec) -> Spec:
         return spec.remove_dimension(self.dimension)
 
     def transform_output_spec(self, spec: Spec) -> Spec:
+        tree = (self.extra_args, self.extra_kwargs)
+        for leaf in trees.leaves(
+            tree, lambda x: isinstance(x, Axis) or not trees.has_treedef(x)
+        ):
+            if isinstance(leaf.value, Axis):
+                spec = spec.update_leaves(leaf.value.new_dimensions)
         return spec
 
     def __repr__(self) -> str:
-        return f'Reduce("{self.dimension}", {self.reduce_fn}, {self.initial_value})'
+        return (
+            f"{self.__class__.__name__}("
+            + f'"{self.dimension}", '
+            + f"{self.reduce_fn}, "
+            + f"{self.initial_value})"
+        )
 
-    @staticmethod
+    @classmethod
     def Sum(
+        cls: T_reduce_cls,
         dimension: str,
         initial_value: Optional[T_reduction_result] = None,
         reduce_impl: T_reduce = None,
-    ) -> "Reduce":
-        """Transformation that iteratively adds the results of the wrapped function for 
+    ) -> T_reduce_cls:
+        """Transformation that iteratively adds the results of the wrapped function for
         each item in the given dimension."""
-        return Reduce(dimension, operator.add, initial_value, reduce_impl)
+        return cls(dimension, operator.add, initial_value, reduce_impl=reduce_impl)
 
-    @staticmethod
+    @classmethod
     def Product(
+        cls: T_reduce_cls,
         dimension: str,
         initial_value: Optional[T_reduction_result] = None,
         reduce_impl: T_reduce = None,
-    ) -> "Reduce":
-        """Transformation that iteratively multiplies the results of the wrapped 
+    ) -> T_reduce_cls:
+        """Transformation that iteratively multiplies the results of the wrapped
         function for each item in the given dimension."""
-        return Reduce(dimension, operator.mul, initial_value, reduce_impl)
+        return cls(dimension, operator.mul, initial_value, reduce_impl=reduce_impl)
 
 
 def specced_map_reduce(
     map_f: Callable[[Any], Any],
     reduce_f: T_reduce_fn,
     data: Any,
     spec: Spec,
     dimension: str,
     initial_value: Optional[Any] = None,
+    enumerate: bool = False,
     reduce_impl: Optional[T_reduce] = None,
 ):
     # Flatten the data so that we can iterate over it without worrying about the
     # potentially nested structure of the data.
     flattened_args, in_axes, unflatten = util.flatten(data, spec, dimension)
 
     # Get the size of the dimension that we are reducing over.
@@ -119,21 +145,23 @@
     if size == 0:  # Return early if there are no elements to reduce over.
         return initial_value
 
     # Get the first mapped value.
     carry = common.map_1_flattened(map_f, flattened_args, in_axes, unflatten, 0)
     # Use the first mapped value as the initial value if no initial value was given.
     if initial_value is not None:
-        carry = reduce_f(initial_value, carry)
+        x = (0, carry) if enumerate else carry
+        carry = reduce_f(initial_value, x)
 
     # `wrapped` puts everything together and makes it work with `reduce_impl`.
     # It gets the arguments indexed at `i` for the given dimension, and applies the
     # mapping function to them before performing a reduction step.
     def wrapped(carry, i):
         x = common.map_1_flattened(map_f, flattened_args, in_axes, unflatten, i)
+        x = (i, x) if enumerate else x
         return reduce_f(carry, x)
 
     # Default `reduce_impl` is Python's built-in `functools.reduce`.
     if reduce_impl is None:
         import functools
 
         reduce_impl = functools.reduce
```

### Comparing `spekk-1.0.1/spekk/transformations/wrap.py` & `spekk-1.0.3/spekk/transformations/wrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Example:
         >>> import jax
         >>> my_fn = lambda x: x**2
         >>> wrapped_fn1 = Wrap(jax.jit)(my_fn)
         >>> wrapped_fn2 = jax.jit(my_fn)
 
-        wrapped_fn1 and wrapped_fn2 are equivalent, but wrapped_fn1 will propagate 
+        `wrapped_fn1` and `wrapped_fn2` are equivalent, but `wrapped_fn1` will propagate 
         information about the spec (if applicable) to nested :class:`Transformation`.
     """
     def __init__(self, f: callable, *args, **kwargs):
         self.f = f
         self.args = args
         self.kwargs = kwargs
```

### Comparing `spekk-1.0.1/spekk/trees/__init__.py` & `spekk-1.0.3/spekk/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/trees/core.py` & `spekk-1.0.3/spekk/trees/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import operator
 from dataclasses import dataclass
 from typing import Any, Callable, Generator, Sequence
 
 from spekk.trees.registry import Tree, treedef
 
+_NO_DEFAULT = object()
+
 
 def update(tree: Tree, f: Callable[[Tree], Tree], path: tuple):
     """Update the subtree at the given path.
 
     >>> tree = {"a": [1, {"b": 2}, 3], "c": 4}
     >>> update(tree, lambda x: x + 10, ("a", 1, "b"))
     {'a': [1, {'b': 12}, 3], 'c': 4}
@@ -22,26 +24,29 @@
     values = [
         update(td.get(k), f, remaining_path) if k == key else td.get(k)
         for k in td.keys()
     ]
     return td.create(td.keys(), values)
 
 
-def get(tree: Tree, path: tuple):
+def get(tree: Tree, path: tuple, default: Any = _NO_DEFAULT):
     """Get the subtree at the given path.
 
     >>> tree = {"a": [1, {"b": 2}, 3], "c": 4}
     >>> get(tree, ("a", 1, "b"))
     2
     """
     if not path:
         return tree
 
     key, *remaining_path = path
     td = treedef(tree)
+    if default is not _NO_DEFAULT:
+        if key not in td.keys():
+            return default
     return get(td.get(key), remaining_path)
 
 
 def set(tree: Tree, value: Any, path: tuple):
     """Set the value of the subtree at the given path.
 
     >>> tree = {"a": [1, {"b": 2}, 3], "c": 4}
@@ -117,15 +122,15 @@
 
 
 def traverse(
     tree: Tree,
     is_leaf: Callable[[Tree], bool],
     path: tuple = (),
 ) -> Generator[TraversalItem, None, None]:
-    """Traverse a tree and yield all nodes (subtrees and leaves) as 
+    """Traverse a tree and yield all nodes (subtrees and leaves) as
     :class:`TraversalItem` objects. The traversal is depth-first, left-to-right.
 
     >>> tree = {"a": [1, {"b": 2}, 3], "c": 4}
     >>> for item in traverse(tree, is_leaf=lambda x: isinstance(x, int)):
     ...     print(item.value)
     1
     2
@@ -149,15 +154,15 @@
 
 
 def leaves(
     tree: Tree,
     is_leaf: Callable[[Tree], bool],
     path: tuple = (),
 ) -> Generator[TraversalItem, None, None]:
-    """Traverse a tree and yield all leaves as :class:`TraversalItem` objects. The 
+    """Traverse a tree and yield all leaves as :class:`TraversalItem` objects. The
     traversal is depth-first, left-to-right.
 
     >>> tree = {"a": [1, {"b": 2}, 3], "c": 4}
     >>> for item in leaves(tree, is_leaf=lambda x: isinstance(x, int)):
     ...     print(item.value)
     1
     2
```

### Comparing `spekk-1.0.1/spekk/trees/registry.py` & `spekk-1.0.3/spekk/trees/registry.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/trees/treelens.py` & `spekk-1.0.3/spekk/trees/treelens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 ":class:`TreeLens` is a functional interface to a tree-like data structure."
 
-from functools import reduce
 from typing import Any, Callable, Optional, Sequence, Tuple, TypeVar, Union
 
-from spekk.trees.core import filter, remove, set, update, update_leaves
+from spekk.trees.core import filter, remove, set, traverse, update, update_leaves
 from spekk.trees.registry import Tree, treedef
 
 TSelf = TypeVar("TSelf", bound="TreeLens")
 
 
 class TreeLens:
     """A functional interface to a Tree.
 
     A lens is an object in functional programming (FP) that allows you to access and
     modify a value in a nested structure in an immutable way.
     """
 
     def __init__(self, tree: Tree = ()):
+        # Ensure that there are no nested TreeLens objects:
+        for t in traverse(tree, self.is_leaf):
+            if isinstance(t.value, TreeLens):
+                tree = set(tree, t.value.tree, t.path)
         self.tree = tree
 
     def __getitem__(self: TSelf, path: Union[Any, Tuple[Any]]) -> TSelf:
         """Get the value or subtree at the given path.
 
         If you want to index by a single tuple, e.g. you have a dict with tuples as
         keys, then you should use get(…) instead. This is because there is no way of
@@ -46,30 +49,37 @@
 
         >>> tree = TreeLens({"a": {"b": [1, 2, 3]}, "d": [3]})
         >>> tree.get(["a", "b"])
         TreeLens([1, 2, 3])
         >>> tree.get(["a", "b", 1])
         TreeLens(2)
         """
-        return self.copy_with(reduce(lambda tree, k: tree[k], path, self.tree))
+        tree = self.tree
+        for k in path:
+            if k not in treedef(tree).keys():
+                return self.copy_with(None)  # Return with None tree
+            tree = tree[k]
+        return self.copy_with(tree)
 
     def has_subtree(self, path: Sequence[Any]) -> bool:
         """Return True if the given path exists in the tree.
 
         >>> tree = TreeLens({"a": {"b": [1, 2, 3]}})
         >>> tree.has_subtree(["a", "b", 1])
         True
         >>> tree.has_subtree(["a", "c"])
         False
         """
-        try:
-            self.get(path)
-            return True
-        except (KeyError, TypeError):
-            return False
+        tree = self.tree
+        for k in path:
+            if k in treedef(tree).keys():
+                tree = tree[k]
+            else:
+                return False
+        return True
 
     def set(self: TSelf, value: Any, path: Sequence[Any]) -> TSelf:
         """Set the value or subtree at the given path.
 
         >>> tree = TreeLens({"a": {"b": [1, 2, 3]}, "d": [3]})
         >>> tree.set(5, ["a", "b", 1])
         TreeLens({'a': {'b': [1, 5, 3]}, 'd': [3]})
@@ -121,14 +131,17 @@
         tree = self.tree if isinstance(self, TreeLens) else self
         not_empty = lambda tree: is_leaf(tree) or len(tree) > 0
         pruned_tree = filter(tree, is_leaf, not_empty)
         if isinstance(self, TreeLens):
             pruned_tree = self.copy_with(pruned_tree)
         return pruned_tree
 
+    def __iter__(self):
+        return iter([self.copy_with(t) for t in self.tree])
+
     def copy_with(self: TSelf, tree: Tree) -> TSelf:
         "Return a copy of this object with the given tree."
         return self.__class__(tree)
 
     def __repr__(self):
         return f"TreeLens({self.tree})"
```

### Comparing `spekk-1.0.1/spekk/util/flatten.py` & `spekk-1.0.3/spekk/util/flatten.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.1/spekk/util/shape.py` & `spekk-1.0.3/spekk/util/shape.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"Generalized :func:`np.shape` that works on nested Python sequences."
+
 from typing import Sequence
 
 
 def shape(x) -> Sequence[int]:
     """Get the shape of an array, number, or a nested sequence of numbers.
 
     >>> shape(1.0)
@@ -15,15 +17,15 @@
     >>> shape(np.ones((2, 3)))
     (2, 3)
     """
     if isinstance(x, (int, float, complex)):
         return ()
     elif hasattr(x, "shape"):
         return x.shape
-    elif isinstance(x, (list, tuple)):
+    elif isinstance(x, (list, tuple, range)):
         # Assume each item in x has the same shape.
         return (len(x), *shape(x[0]))
     raise ValueError(f"Cannot get shape of object with type {type(x)}")
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `spekk-1.0.1/spekk/util/slicing.py` & `spekk-1.0.3/spekk/util/slicing.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,18 @@
     data: Tree, spec: Spec, slice_definitions: Sequence[Union[str, IndicesT]]
 ):
     """Slice the data given a spec and a dict (kwargs) of slice definitions. The keys
     of ``slice_definitions`` are the names of the dimensions to slice, and the values 
     are the indices to slice along that dimension. Returns the sliced data and the
     (possibly modified) spec.
 
-    The data may have an arbitrary tree-like shape (nested ``dict``, `list`, `tuple`, 
-    etc.), but the leaves must support numpy indexing. The returned sliced data has the 
-    same shape as the input data. The spec argument describes the shape of the data.
+    The data may have an arbitrary tree-like shape (nested ``dict``, ``list``, 
+    ``tuple``, etc.), but the leaves must support numpy indexing. The returned sliced 
+    data has the same shape as the input data. The spec argument describes the shape of 
+    the data.
 
     If the indices for a dimension in ``slice_definitions`` is just an integer, said
     dimension is removed from the returned spec.
 
     >>> import numpy as np
     >>> data = {"foo": ({"bar": np.ones((4,5))},)}
     >>> spec = Spec({"foo": ({"bar": ["a", "b"]},)})
```

### Comparing `spekk-1.0.1/spekk/util/validation.py` & `spekk-1.0.3/spekk/util/validation.py`

 * *Files identical despite different names*

