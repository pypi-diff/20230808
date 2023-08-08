# Comparing `tmp/valorant.py-1.0.0.dev0.tar.gz` & `tmp/valorant.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valorant.py-1.0.0.dev0.tar", last modified: Sat Aug 27 06:54:31 2022, max compression
+gzip compressed data, was "valorant.py-1.0.1.tar", last modified: Tue Aug  8 10:40:57 2023, max compression
```

## Comparing `valorant.py-1.0.0.dev0.tar` & `valorant.py-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,79 @@
-drwxrwxrwx   0        0        0        0 2022-08-27 06:54:31.898205 valorant.py-1.0.0.dev0/
--rw-rw-rw-   0        0        0     1084 2022-08-27 06:26:16.000000 valorant.py-1.0.0.dev0/LICENSE
--rw-rw-rw-   0        0        0     2204 2022-08-27 06:54:31.896206 valorant.py-1.0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2022-08-27 06:45:03.000000 valorant.py-1.0.0.dev0/README.md
--rw-rw-rw-   0        0        0     1031 2022-08-27 06:33:33.000000 valorant.py-1.0.0.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-27 06:54:31.900204 valorant.py-1.0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1414 2022-08-27 06:52:49.000000 valorant.py-1.0.0.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-27 06:54:31.877705 valorant.py-1.0.0.dev0/valorant/
--rw-rw-rw-   0        0        0      328 2022-08-27 06:35:10.000000 valorant.py-1.0.0.dev0/valorant/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-27 06:54:31.891203 valorant.py-1.0.0.dev0/valorant.py.egg-info/
--rw-rw-rw-   0        0        0     2204 2022-08-27 06:54:31.000000 valorant.py-1.0.0.dev0/valorant.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-08-27 06:54:31.000000 valorant.py-1.0.0.dev0/valorant.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-27 06:54:31.000000 valorant.py-1.0.0.dev0/valorant.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-08-27 06:54:31.000000 valorant.py-1.0.0.dev0/valorant.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-27 06:54:31.000000 valorant.py-1.0.0.dev0/valorant.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.449462 valorant.py-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-08 10:40:46.000000 valorant.py-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 10:40:46.000000 valorant.py-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-08 10:40:57.449462 valorant.py-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 10:40:46.000000 valorant.py-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 10:40:46.000000 valorant.py-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 10:40:46.000000 valorant.py-1.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 10:40:46.000000 valorant.py-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:40:57.449462 valorant.py-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 10:40:46.000000 valorant.py-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.437461 valorant.py-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 10:40:46.000000 valorant.py-1.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-08-08 10:40:46.000000 valorant.py-1.0.1/tests/test_valorant_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.441461 valorant.py-1.0.1/valorant/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17875 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/localization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.445461 valorant.py-1.0.1/valorant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/buddies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/ceremonies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/competitive_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/content_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/gear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/level_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/player_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/player_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/sprays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/weapons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.449462 valorant.py-1.0.1/valorant/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/buddies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/ceremonies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/competitive_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/content_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/gear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/level_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/player_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/player_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/sprays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/weapons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.441461 valorant.py-1.0.1/valorant.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/top_level.txt
```

### Comparing `valorant.py-1.0.0.dev0/LICENSE` & `valorant.py-1.0.1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 xSTACIA
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 STACIA
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

