# Comparing `tmp/sextant-0.4.0.tar.gz` & `tmp/sextant-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sextant-0.4.0.tar", last modified: Wed Jun  7 06:12:28 2023, max compression
+gzip compressed data, was "sextant-0.5.0.tar", last modified: Tue Aug  8 13:03:22 2023, max compression
```

## Comparing `sextant-0.4.0.tar` & `sextant-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/
--rw-r--r--   0 joe       (1000) joe       (1000)      120 2022-10-17 14:22:50.000000 sextant-0.4.0/.gitignore
--rw-r--r--   0 joe       (1000) joe       (1000)      982 2022-11-10 15:31:15.000000 sextant-0.4.0/.gitlab-ci.yml
--rw-r--r--   0 joe       (1000) joe       (1000)      111 2022-11-10 15:31:15.000000 sextant-0.4.0/.pylintrc
--rw-r--r--   0 joe       (1000) joe       (1000)      281 2023-04-19 10:15:58.000000 sextant-0.4.0/CHANGELOG
--rw-r--r--   0 joe       (1000) joe       (1000)      785 2022-10-17 05:06:58.000000 sextant-0.4.0/LICENSE
--rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-06-07 06:12:28.563573 sextant-0.4.0/PKG-INFO
--rw-r--r--   0 joe       (1000) joe       (1000)     8459 2023-06-07 06:09:53.000000 sextant-0.4.0/README.md
--rw-r--r--   0 joe       (1000) joe       (1000)      337 2023-06-06 05:38:31.000000 sextant-0.4.0/pyproject.toml
--rw-r--r--   0 joe       (1000) joe       (1000)       38 2023-06-07 06:12:28.563573 sextant-0.4.0/setup.cfg
--rw-r--r--   0 joe       (1000) joe       (1000)     1008 2023-04-19 10:15:44.000000 sextant-0.4.0/setup.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/sextant/
--rw-r--r--   0 joe       (1000) joe       (1000)      224 2023-06-06 05:38:31.000000 sextant-0.4.0/sextant/__init__.py
--rw-r--r--   0 joe       (1000) joe       (1000)    12923 2023-06-07 06:09:42.000000 sextant-0.4.0/sextant/cli.py
--rw-r--r--   0 joe       (1000) joe       (1000)     8706 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/dependency.py
--rw-r--r--   0 joe       (1000) joe       (1000)     4672 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/module.py
--rw-r--r--   0 joe       (1000) joe       (1000)    13379 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/scaffold.py
--rw-r--r--   0 joe       (1000) joe       (1000)     1493 2023-01-12 14:50:29.000000 sextant-0.4.0/sextant/semver.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/sextant.egg-info/
--rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/PKG-INFO
--rw-r--r--   0 joe       (1000) joe       (1000)     1979 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/SOURCES.txt
--rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/dependency_links.txt
--rw-r--r--   0 joe       (1000) joe       (1000)       45 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/entry_points.txt
--rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/not-zip-safe
--rw-r--r--   0 joe       (1000) joe       (1000)       78 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/requires.txt
--rw-r--r--   0 joe       (1000) joe       (1000)       14 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/top_level.txt
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/
--rw-r--r--   0 joe       (1000) joe       (1000)       93 2022-10-17 06:53:02.000000 sextant-0.4.0/tests/__init__.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.555573 sextant-0.4.0/tests/fixtures/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/bar/
--rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:39:51.000000 sextant-0.4.0/tests/fixtures/bar/beer_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:40:01.000000 sextant-0.4.0/tests/fixtures/bar/beer_2.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)      563 2022-10-12 05:38:33.000000 sextant-0.4.0/tests/fixtures/bar/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:15.000000 sextant-0.4.0/tests/fixtures/bar/stool_0.5.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:27.000000 sextant-0.4.0/tests/fixtures/bar/stool_0.5.1.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:38.000000 sextant-0.4.0/tests/fixtures/bar/stool_1.0.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/baz/
--rw-r--r--   0 joe       (1000) joe       (1000)       20 2022-10-12 05:40:51.000000 sextant-0.4.0/tests/fixtures/baz/drunk-unicorn_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)      437 2022-10-17 14:10:38.000000 sextant-0.4.0/tests/fixtures/baz/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       23 2022-10-12 05:41:00.000000 sextant-0.4.0/tests/fixtures/baz/sitting-pangolin_1.0.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.555573 sextant-0.4.0/tests/fixtures/charts/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/bad/
--rw-r--r--   0 joe       (1000) joe       (1000)       59 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/bad/package.json
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/bad/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/bad/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/good/
--rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-06-06 11:36:44.000000 sextant-0.4.0/tests/fixtures/charts/good/Chart.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)       50 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/good/package.json
--rw-r--r--   0 joe       (1000) joe       (1000)      395 2023-06-07 05:33:18.000000 sextant-0.4.0/tests/fixtures/charts/good/package.lock
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/good/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/good/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/other/
--rw-r--r--   0 joe       (1000) joe       (1000)       43 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/package.json
--rw-r--r--   0 joe       (1000) joe       (1000)      248 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/package.lock
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/other/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/foo/
--rw-r--r--   0 joe       (1000) joe       (1000)      418 2022-10-12 05:43:41.000000 sextant-0.4.0/tests/fixtures/foo/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       16 2022-10-12 05:41:58.000000 sextant-0.4.0/tests/fixtures/foo/pangolin_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       15 2022-10-12 05:41:43.000000 sextant-0.4.0/tests/fixtures/foo/unicorn_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       14 2022-10-12 05:41:53.000000 sextant-0.4.0/tests/fixtures/foo/unicorn_1.1.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_skel/
--rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/Chart.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)       44 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/package.json
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)       20 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/configmap.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)      523 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)       18 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/service.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)       28 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/spurious.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)      151 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/values.yaml
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_wizard/
--rw-r--r--   0 joe       (1000) joe       (1000)      427 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/ingress.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)      287 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/ingress_nginx.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)     1061 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/scaffold.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)       77 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/presets.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)      177 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/questions.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)     3269 2023-06-07 06:09:42.000000 sextant-0.4.0/tests/test_cli.py
--rw-r--r--   0 joe       (1000) joe       (1000)     1120 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_dependency.py
--rw-r--r--   0 joe       (1000) joe       (1000)     2167 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_module.py
--rw-r--r--   0 joe       (1000) joe       (1000)     3049 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_package.py
--rw-r--r--   0 joe       (1000) joe       (1000)     8969 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_scaffold.py
--rw-r--r--   0 joe       (1000) joe       (1000)      814 2023-06-06 05:38:31.000000 sextant-0.4.0/tox.ini
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.193998 sextant-0.5.0/
+-rw-r--r--   0 joe       (1000) joe       (1000)      120 2022-10-17 14:22:50.000000 sextant-0.5.0/.gitignore
+-rw-r--r--   0 joe       (1000) joe       (1000)      982 2022-11-10 15:31:15.000000 sextant-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0 joe       (1000) joe       (1000)      111 2022-11-10 15:31:15.000000 sextant-0.5.0/.pylintrc
+-rw-r--r--   0 joe       (1000) joe       (1000)      476 2023-08-08 13:01:30.000000 sextant-0.5.0/CHANGELOG
+-rw-r--r--   0 joe       (1000) joe       (1000)      785 2022-10-17 05:06:58.000000 sextant-0.5.0/LICENSE
+-rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-08-08 13:03:22.193998 sextant-0.5.0/PKG-INFO
+-rw-r--r--   0 joe       (1000) joe       (1000)     8459 2023-06-07 06:09:53.000000 sextant-0.5.0/README.md
+-rw-r--r--   0 joe       (1000) joe       (1000)      337 2023-06-06 05:38:31.000000 sextant-0.5.0/pyproject.toml
+-rw-r--r--   0 joe       (1000) joe       (1000)       38 2023-08-08 13:03:22.193998 sextant-0.5.0/setup.cfg
+-rw-r--r--   0 joe       (1000) joe       (1000)     1008 2023-08-04 07:47:36.000000 sextant-0.5.0/setup.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.181998 sextant-0.5.0/sextant/
+-rw-r--r--   0 joe       (1000) joe       (1000)      224 2023-06-06 05:38:31.000000 sextant-0.5.0/sextant/__init__.py
+-rw-r--r--   0 joe       (1000) joe       (1000)    13959 2023-08-04 08:15:13.000000 sextant-0.5.0/sextant/cli.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     8662 2023-08-08 12:59:13.000000 sextant-0.5.0/sextant/dependency.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     4672 2023-04-19 10:15:44.000000 sextant-0.5.0/sextant/module.py
+-rw-r--r--   0 joe       (1000) joe       (1000)    13379 2023-04-19 10:15:44.000000 sextant-0.5.0/sextant/scaffold.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     1701 2023-08-08 12:59:04.000000 sextant-0.5.0/sextant/semver.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.181998 sextant-0.5.0/sextant.egg-info/
+-rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/PKG-INFO
+-rw-r--r--   0 joe       (1000) joe       (1000)     1979 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/SOURCES.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/dependency_links.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)       45 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/entry_points.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/not-zip-safe
+-rw-r--r--   0 joe       (1000) joe       (1000)       78 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/requires.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)       14 2023-08-08 13:03:22.000000 sextant-0.5.0/sextant.egg-info/top_level.txt
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/
+-rw-r--r--   0 joe       (1000) joe       (1000)       93 2022-10-17 06:53:02.000000 sextant-0.5.0/tests/__init__.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.181998 sextant-0.5.0/tests/fixtures/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/bar/
+-rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:39:51.000000 sextant-0.5.0/tests/fixtures/bar/beer_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:40:01.000000 sextant-0.5.0/tests/fixtures/bar/beer_2.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)      563 2022-10-12 05:38:33.000000 sextant-0.5.0/tests/fixtures/bar/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:15.000000 sextant-0.5.0/tests/fixtures/bar/stool_0.5.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:27.000000 sextant-0.5.0/tests/fixtures/bar/stool_0.5.1.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:38.000000 sextant-0.5.0/tests/fixtures/bar/stool_1.0.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/baz/
+-rw-r--r--   0 joe       (1000) joe       (1000)       20 2022-10-12 05:40:51.000000 sextant-0.5.0/tests/fixtures/baz/drunk-unicorn_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)      437 2022-10-17 14:10:38.000000 sextant-0.5.0/tests/fixtures/baz/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       23 2022-10-12 05:41:00.000000 sextant-0.5.0/tests/fixtures/baz/sitting-pangolin_1.0.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.181998 sextant-0.5.0/tests/fixtures/charts/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/charts/bad/
+-rw-r--r--   0 joe       (1000) joe       (1000)       59 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/bad/package.json
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/charts/bad/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/bad/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/charts/good/
+-rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-06-06 11:36:44.000000 sextant-0.5.0/tests/fixtures/charts/good/Chart.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       50 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/good/package.json
+-rw-r--r--   0 joe       (1000) joe       (1000)      395 2023-06-07 05:33:18.000000 sextant-0.5.0/tests/fixtures/charts/good/package.lock
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.185998 sextant-0.5.0/tests/fixtures/charts/good/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/good/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/charts/other/
+-rw-r--r--   0 joe       (1000) joe       (1000)       43 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/other/package.json
+-rw-r--r--   0 joe       (1000) joe       (1000)      248 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/other/package.lock
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/charts/other/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.5.0/tests/fixtures/charts/other/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/foo/
+-rw-r--r--   0 joe       (1000) joe       (1000)      418 2022-10-12 05:43:41.000000 sextant-0.5.0/tests/fixtures/foo/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       16 2022-10-12 05:41:58.000000 sextant-0.5.0/tests/fixtures/foo/pangolin_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       15 2022-10-12 05:41:43.000000 sextant-0.5.0/tests/fixtures/foo/unicorn_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       14 2022-10-12 05:41:53.000000 sextant-0.5.0/tests/fixtures/foo/unicorn_1.1.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/scaffold/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/scaffold/_skel/
+-rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/Chart.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       44 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/package.json
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.189998 sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)       20 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/configmap.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)      523 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)       18 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/service.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)       28 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/spurious.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)      151 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_skel/values.yaml
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-08-08 13:03:22.193998 sextant-0.5.0/tests/fixtures/scaffold/_wizard/
+-rw-r--r--   0 joe       (1000) joe       (1000)      427 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_wizard/ingress.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)      287 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_wizard/ingress_nginx.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)     1061 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/_wizard/scaffold.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       77 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/presets.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)      177 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/fixtures/scaffold/questions.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)     3269 2023-08-04 07:37:53.000000 sextant-0.5.0/tests/test_cli.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     1120 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/test_dependency.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     2167 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/test_module.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     3049 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/test_package.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     8969 2023-04-19 10:15:44.000000 sextant-0.5.0/tests/test_scaffold.py
+-rw-r--r--   0 joe       (1000) joe       (1000)      808 2023-08-04 07:12:31.000000 sextant-0.5.0/tox.ini
```

### Comparing `sextant-0.4.0/.gitlab-ci.yml` & `sextant-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/LICENSE` & `sextant-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/README.md` & `sextant-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/setup.py` & `sextant-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/sextant/cli.py` & `sextant-0.5.0/sextant/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,19 +137,35 @@
 
     def depends_on(self, query: str, strict_match: bool = True) -> bool:
         """Checks if the chart depends on a module, directly or indirectly."""
         if strict_match:
             return any(str(m) == query for m in self.package.get())
         return any(m.matches(query) for m in self.package.get())
 
-    def update_dependency(self, slug: str) -> bool:
+    def update_dependency(self, mod: module.Module) -> bool:
         """Update a dependency in package.json."""
+        slug = f"{mod.namespace}.{mod.name}:{mod.version.major}.{mod.version.minor}"
         # If the update needs to happen in package.json, or if
         # we have an implicit dependency on it, force a re-vendoring.
-        return self.package.update(slug) or self.depends_on(slug, strict_match=False)
+        # Case 1: we have the module declared explicitly in package.json;
+        # if the updated version is newer than the old one
+        if self.package.update(slug):
+            log.debug("Explicit dependency %s is newer than the one present in package.json", slug)
+            return True
+        # Case 2: we have the module imported as a dependency of another module.
+        for dep_module in self.package.get():
+            # Check that our update and the dependency are compatible.
+            # If not, we can't update
+            if not dep_module.matches(slug):
+                continue
+            # Now check that we are actually updating the module
+            if mod.is_newer(dep_module):
+                log.debug("Implicit dependency %s is newer than the current dependency %s", mod, dep_module)
+                return True
+        return False
 
     def bump_chart_version(self, specific_version="") -> Semver:
         """Bump the chart version after a vendor update."""
         with self.chart_yaml.open() as yaml:
             content = yaml.read()
         match = RE_VERSION.search(content)
         if not match:
@@ -235,15 +251,14 @@
         help="the directory where the chart's package.json file is located.",
     )
     return parser
 
 
 def main(args: Optional[List[str]] = None):
     """The main entrypoint."""
-
     if args is None:
         args = sys.argv[1:]
     params = argparser().parse_args(args)
     if params.debug:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO)
@@ -288,40 +303,44 @@
         for chart in results:
             print(chart)
 
 
 def run_update(params: argparse.Namespace, charts: ChartsCollection):
     """Perform the update action."""
     # First collect the modules to update
-    updated_modules: List[str] = []
+    updated_modules: List[module.Module] = []
     for mod in params.modules:
         try:
             namespace, module_name = mod.split(".", 1)
         except ValueError:
             log.error("Module names must be in the form 'namespace.module[:version]', got %s", mod)
             sys.exit(1)
         if ":" in module_name:
             module_name, version = module_name.split(":")
         else:
             version = None
         newest = charts.registry.get_newest(namespace=namespace, module=module_name, version=version)
         if newest is None:
             log.error("Could not find module '%s'", mod)
             sys.exit(1)
-        slug = f"{newest.namespace}.{newest.name}:{newest.version.major}.{newest.version.minor}"
-        log.debug("Selected %s", slug)
-        updated_modules.append(slug)
+        log.info("Charts will be updated to %s", newest)
+        updated_modules.append(newest)
 
     # Now update the dependencies in all charts.
     for chart in charts.charts():
+        log.info("Updating %s...", chart)
         to_vendor = False
-        for slug in updated_modules:
-            if chart.update_dependency(slug):
+        for mod in updated_modules:
+            log.debug("Checking updates to %s", mod)
+            if chart.update_dependency(mod):
                 to_vendor = True
         if to_vendor:
+            log.info("Re-vendoring dependencies after update")
             chart.vendor(True)
+        else:
+            log.info("No update needed for chart %s", chart)
 
 
 def run_update_version(params: argparse.Namespace, charts: ChartsCollection):
     """Bump chart version."""
     chart_path = pathlib.Path(params.chartdir)
     charts.chart(chart_path.name).bump_chart_version(params.version)
```

### Comparing `sextant-0.4.0/sextant/dependency.py` & `sextant-0.5.0/sextant/dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,30 +100,30 @@
             version = Semver(ver)
         except ValueError as exc:
             raise ValueError(f"Module {new_module} is badly formatted.") from exc
 
         # Cycle through the modules enumerated.
         for idx, mod in enumerate(self.modules):
             my_mod, my_ver = mod.split(":")
+
             if my_mod != name:
                 continue
-            if Semver(my_ver) > version:
+            current_version = Semver(my_ver)
+            if current_version >= version:
                 continue
             # We're here, we have to update modules.
             to_overwrite = idx
             break
 
         # If we're updating the package.json file, we want to also unlink the lockfile.
         if to_overwrite >= 0:
             self.modules[to_overwrite] = new_module
-            # TODO: move to use missing_ok=True when we drop python 3.7
-            if self.lockfile.exists():
-                self.lockfile.unlink()
+            self.lockfile.unlink(missing_ok=True)
             with self.path.open("w", encoding="utf-8") as fileh:
-                json.dump(self.modules, fileh, indent=4)
+                json.dump(sorted(self.modules), fileh, indent=4)
             log.debug("Updated modules: %s", self.modules)
             return True
         return False
 
     def _refresh(self):
         """Refresh the modules list"""
         self.modules = json.loads(self.path.read_bytes())
```

### Comparing `sextant-0.4.0/sextant/module.py` & `sextant-0.5.0/sextant/module.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/sextant/scaffold.py` & `sextant-0.5.0/sextant/scaffold.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/sextant/semver.py` & `sextant-0.5.0/sextant/semver.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,15 @@
                 return self.patch > other.patch
             return self.minor > other.minor
         return self.major > other.major
 
     def __lt__(self, other: "Semver") -> bool:
         return other.__gt__(self)
 
+    def __ge__(self, other: "Semver") -> bool:
+        return self.__gt__(other) or self.__eq__(other)
+
+    def __le__(self, other: "Semver") -> bool:
+        return self.__lt__(other) or self.__eq__(other)
+
     def __str__(self) -> str:
         return f"{self.major}.{self.minor}.{self.patch}"
```

### Comparing `sextant-0.4.0/sextant.egg-info/SOURCES.txt` & `sextant-0.5.0/sextant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/fixtures/bar/module.json` & `sextant-0.5.0/tests/fixtures/bar/module.json`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel` & `sextant-0.5.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/fixtures/scaffold/_wizard/scaffold.yaml` & `sextant-0.5.0/tests/fixtures/scaffold/_wizard/scaffold.yaml`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/test_cli.py` & `sextant-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/test_dependency.py` & `sextant-0.5.0/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/test_module.py` & `sextant-0.5.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/test_package.py` & `sextant-0.5.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tests/test_scaffold.py` & `sextant-0.5.0/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `sextant-0.4.0/tox.ini` & `sextant-0.5.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 2.5.0
-envlist = py{37,38,39,310,311}-{style,tests,lint}
+envlist = py{39,310,311}-{style,tests,lint}
 skip_missing_interpreters = True
 
 [testenv]
 usedevelop = True
 basepython =
     py39: python3.9
     py310: python3.10
```

