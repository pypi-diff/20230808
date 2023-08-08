# Comparing `tmp/github_poster-2.5.1.tar.gz` & `tmp/github_poster-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_poster-2.5.1.tar", last modified: Wed Apr 19 01:23:59 2023, max compression
+gzip compressed data, was "github_poster-2.6.0.tar", last modified: Tue Aug  8 10:42:50 2023, max compression
```

## Comparing `github_poster-2.5.1.tar` & `github_poster-2.6.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.668129 github_poster-2.5.1/
--rw-r--r--   0 hyi        (502) staff       (20)     1063 2022-03-17 02:50:19.000000 github_poster-2.5.1/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-19 01:23:59.667199 github_poster-2.5.1/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)    24221 2023-04-18 14:37:48.000000 github_poster-2.5.1/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.609786 github_poster-2.5.1/github_poster/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     6361 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/circluar_drawer.py
--rw-r--r--   0 hyi        (502) staff       (20)     6547 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     1134 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     9710 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/drawer.py
--rw-r--r--   0 hyi        (502) staff       (20)      261 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/err.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.623035 github_poster-2.5.1/github_poster/html_parser/
--rw-r--r--   0 hyi        (502) staff       (20)      206 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     1143 2023-01-09 06:11:32.000000 github_poster-2.5.1/github_poster/html_parser/github_parser.py
--rw-r--r--   0 hyi        (502) staff       (20)      256 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/gitlab_parser.py
--rw-r--r--   0 hyi        (502) staff       (20)     2005 2022-07-12 13:26:45.000000 github_poster-2.5.1/github_poster/html_parser/jike_parse.py
--rw-r--r--   0 hyi        (502) staff       (20)      257 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/kindle_parser.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.662958 github_poster-2.5.1/github_poster/loader/
--rw-r--r--   0 hyi        (502) staff       (20)     3482 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/loader/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     5187 2023-03-31 14:51:05.000000 github_poster-2.5.1/github_poster/loader/apple_health_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     7132 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/base_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     4148 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/bbdc_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3296 2022-10-08 00:21:43.000000 github_poster-2.5.1/github_poster/loader/bilibili_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2196 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/loader/chatgpt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3287 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/cichang_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     6322 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/loader/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     1960 2022-07-12 13:26:45.000000 github_poster-2.5.1/github_poster/loader/covid_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1559 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/dota2_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2470 2023-04-19 01:23:31.000000 github_poster-2.5.1/github_poster/loader/duolingo_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2494 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/forest_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2826 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/from_github_issue_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2795 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/garmin_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1547 2022-11-24 14:02:11.000000 github_poster-2.5.1/github_poster/loader/github_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3407 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/gitlab_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3166 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/gpx_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     7133 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/jike_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1095 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/json_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1678 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/kindle_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2595 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/leetcode_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1393 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/multiple_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3095 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/notion_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3763 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/nrc_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3321 2022-04-13 04:14:41.000000 github_poster-2.5.1/github_poster/loader/ns_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3437 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/loader/openlanguage_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1637 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/shanbay_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3141 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/strava_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)      965 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/summary_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     5285 2023-03-31 14:51:00.000000 github_poster-2.5.1/github_poster/loader/todoist_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1828 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/twitter_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1807 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/wakatime_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2134 2022-11-24 13:15:31.000000 github_poster-2.5.1/github_poster/loader/weread_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1640 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/youtube_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3849 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/poster.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.664339 github_poster-2.5.1/github_poster/skyline/
--rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      185 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/config.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.665020 github_poster-2.5.1/github_poster/skyline/font/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/font/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     4008 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/skyline.py
--rw-r--r--   0 hyi        (502) staff       (20)     1674 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/structures.py
--rw-r--r--   0 hyi        (502) staff       (20)     2211 2023-01-09 14:20:16.000000 github_poster-2.5.1/github_poster/utils.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.615141 github_poster-2.5.1/github_poster.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     2205 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       57 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      243 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       20 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       31 2022-03-17 02:50:20.000000 github_poster-2.5.1/pyproject.toml
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-04-19 01:23:59.668202 github_poster-2.5.1/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1028 2023-04-19 01:23:46.000000 github_poster-2.5.1/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.666681 github_poster-2.5.1/tests/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/tests/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      732 2022-03-17 02:50:20.000000 github_poster-2.5.1/tests/test_poster_utils.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.072093 github_poster-2.6.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1063 2023-04-20 03:20:34.000000 github_poster-2.6.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      439 2023-08-08 10:42:50.071906 github_poster-2.6.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)    24923 2023-08-08 08:08:48.000000 github_poster-2.6.0/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.056459 github_poster-2.6.0/github_poster/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       74 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6361 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/circluar_drawer.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6547 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1156 2023-08-08 08:08:48.000000 github_poster-2.6.0/github_poster/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     9710 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/drawer.py
+-rw-r--r--   0 hyi        (502) staff       (20)      261 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/err.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.060146 github_poster-2.6.0/github_poster/html_parser/
+-rw-r--r--   0 hyi        (502) staff       (20)      206 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/html_parser/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1178 2023-08-08 10:35:52.000000 github_poster-2.6.0/github_poster/html_parser/github_parser.py
+-rw-r--r--   0 hyi        (502) staff       (20)      256 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/html_parser/gitlab_parser.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2005 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/html_parser/jike_parse.py
+-rw-r--r--   0 hyi        (502) staff       (20)      257 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/html_parser/kindle_parser.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.070106 github_poster-2.6.0/github_poster/loader/
+-rw-r--r--   0 hyi        (502) staff       (20)     3585 2023-08-08 08:08:48.000000 github_poster-2.6.0/github_poster/loader/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5187 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/apple_health_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7132 2023-07-11 08:21:20.000000 github_poster-2.6.0/github_poster/loader/base_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4148 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/bbdc_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3296 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/bilibili_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2196 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/chatgpt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3287 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/cichang_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6356 2023-08-08 08:08:48.000000 github_poster-2.6.0/github_poster/loader/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1960 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/covid_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1559 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/dota2_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2594 2023-04-20 04:14:57.000000 github_poster-2.6.0/github_poster/loader/duolingo_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2494 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/forest_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2826 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/from_github_issue_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2795 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/garmin_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1547 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/github_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3407 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/gitlab_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3166 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/gpx_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7133 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/jike_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1095 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/json_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1678 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/kindle_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2595 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/leetcode_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1393 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/multiple_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2713 2023-08-08 08:08:48.000000 github_poster-2.6.0/github_poster/loader/neodb_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3095 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/notion_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3763 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/nrc_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3321 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/ns_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3437 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/openlanguage_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2363 2023-06-19 02:36:08.000000 github_poster-2.6.0/github_poster/loader/shanbay_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3141 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/strava_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)      965 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/summary_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5285 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/todoist_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1828 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/twitter_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1807 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/wakatime_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2134 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/weread_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1640 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/loader/youtube_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3849 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/poster.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.070924 github_poster-2.6.0/github_poster/skyline/
+-rw-r--r--   0 hyi        (502) staff       (20)       74 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/skyline/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      185 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/skyline/config.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.071191 github_poster-2.6.0/github_poster/skyline/font/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/skyline/font/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4008 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/skyline/skyline.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1674 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/structures.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2211 2023-04-20 03:20:34.000000 github_poster-2.6.0/github_poster/utils.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.058188 github_poster-2.6.0/github_poster.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      439 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     2242 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       57 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      243 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       20 2023-08-08 10:42:49.000000 github_poster-2.6.0/github_poster.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       31 2023-04-20 03:20:34.000000 github_poster-2.6.0/pyproject.toml
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-08-08 10:42:50.072137 github_poster-2.6.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1028 2023-08-08 10:42:38.000000 github_poster-2.6.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-08-08 10:42:50.071639 github_poster-2.6.0/tests/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-04-20 03:20:34.000000 github_poster-2.6.0/tests/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      732 2023-04-20 03:20:34.000000 github_poster-2.6.0/tests/test_poster_utils.py
```

### Comparing `github_poster-2.5.1/LICENSE` & `github_poster-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/README.md` & `github_poster-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -194,39 +194,37 @@
 
 <details>
 <summary>Make your <code>多邻国（duolingo）</code> GitHub poster</summary>
 <br>
 
 1. login duolingo in broswer
 2. console `document.cookie.match(new RegExp('(^| )jwt_token=([^;]+)'))[0].slice(11)` get duolingo_jwt
-3. 点击 profile call 接口拿到你的 duolingo_id
 
 
 ```
-python3 -m github_poster duolingo --duolingo_id ${user_id} --duolingo_jwt ${duolingo_jwt} --year 2015-2021
+python3 -m github_poster duolingo --duolingo_user_name ${duolingo_user_name} --duolingo_jwt ${duolingo_jwt} --year 2015-2021
 or
-github_poster duolingo --duolingo_id ${user_id} --duolingo_duolingo_jwtpassword ${duolingo_jwt} --year 2015-2021
+github_poster duolingo --duolingo_user_name ${duolingo_user_name} --duolingo_duolingo_jwt ${duolingo_jwt} --year 2015-2021
 ```
 </details>
 
 ### 扇贝
 
 <details>
 <summary>Make your <code>扇贝（shanbay）</code> GitHub poster</summary>
 <br>
-
 需要找到你的扇贝 user_id, 从网页抓 xhr 就可以获得如下图
 ![image](https://user-images.githubusercontent.com/15976103/116340351-a02ac500-a811-11eb-938f-72ff141e4942.png)
 
-
 ```
-python3 -m github_poster shanbay --shanbay_user_name ${user_name} --year 2012-2021 --special-color1 '#33C6A4' --special-color2 '#33C6A4'
+python3 -m github_poster shanbay --shanbay_user_name ${user_name} --year 2012-2021 --special-color1 '#009688' --special-color2 '#007BFF' --track-color '#ADD8E6'
 or
-github_poster shanbay --shanbay_user_name ${user_name} --year 2012-2021 --special-color1 '#33C6A4' --special-color2 '#33C6A4'
+github_poster shanbay --shanbay_user_name ${user_name} --year 2012-2021 --special-color1 '#009688' --special-color2 '#007BFF' --track-color '#ADD8E6'
 ```
+
 </details>
 
 ### 不背单词
 
 <details>
 <summary>Make your <code>不背单词（bbdc）</code> GitHub poster</summary>
 <br>
@@ -679,14 +677,34 @@
 ```
 python3 -m github_poster chatgpt 
 or
 github_poster chatgpt --me yihong0618
 ```
 </details>
 
+### NeoDB
+
+<details>
+<summary>Make your <code>NeoDB</code> GitHub poster</summary>
+<br>
+
+利用 NeoDB 提供的 API，可以方便地制作以标注作为数据的 GitHub Poster。
+
+需要在 [NeoDB 的开发者页面](https://neodb.social/developer)获取访问用户信息的 token。
+
+neodb 模块需要两个参数，`neodb_token` 为获取到的 token，`mark_type` 对应 NeoDB 上标注的三种分类：`complete`, `wishlist`, `progress`.
+
+```
+python3 -m github_poster neodb --neodb_token <token> --mark_type <complete, wishlist, progress, all> --me "your name"
+```
+
+特别地，`mark_type` 也可以选择 `all`, 此时会将三种分类的标注都导入。
+
+</details>
+
 # 参与项目
 
 - 任何 Issues PR 均欢迎。
 - 可以提交新的 loader
 - 如何编写新的loader by `ruter` [如何为 GithubPoster 添加 loader](https://umm.js.org/p/c88bf4c7/)
 
 提交PR前:
```

### Comparing `github_poster-2.5.1/github_poster/circluar_drawer.py` & `github_poster-2.6.0/github_poster/circluar_drawer.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/cli.py` & `github_poster-2.6.0/github_poster/cli.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/config.py` & `github_poster-2.6.0/github_poster/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,8 +45,9 @@
     "jike": "Jike",
     "bbdc": "BBDC",
     "weread": "WeRead",
     "covid": "COVID-19",
     "todoist": "Todoist",
     "apple": "AppleHealth",
     "chatgpt": "ChatGPT",
+    "neodb": "NeoDB",
 }
```

### Comparing `github_poster-2.5.1/github_poster/drawer.py` & `github_poster-2.6.0/github_poster/drawer.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/html_parser/github_parser.py` & `github_poster-2.6.0/github_poster/html_parser/github_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 class GitHubParser(html.parser.HTMLParser):
     def __init__(self):
         html.parser.HTMLParser.__init__(self)
         self.recording = False
         self.rects = []
 
     def handle_starttag(self, tag, attrs):
-        if tag == "rect":
+        if tag == "td":
             self.rects.append(dict(attrs))
             self.recording = True
 
     def handle_data(self, data):
         if self.recording:
             contributions_texts = data.split("contribution")
+            print(contributions_texts)
             if contributions_texts:
                 self.rects[-1]["data-count"] = contributions_texts[0].rstrip()
 
     def handle_endtag(self, tag):
-        if tag == "rect":
+        if tag == "td":
             self.recording = False
 
     def make_contribution_dict(self, text):
         self.feed(text)
         number_by_date_dict = {}
         for r in self.rects:
             if r.get("data-count"):
```

### Comparing `github_poster-2.5.1/github_poster/html_parser/jike_parse.py` & `github_poster-2.6.0/github_poster/html_parser/jike_parse.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/__init__.py` & `github_poster-2.6.0/github_poster/loader/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from github_poster.loader.gitlab_loader import GitLabLoader
 from github_poster.loader.gpx_loader import GPXLoader
 from github_poster.loader.jike_loader import JikeLoader
 from github_poster.loader.json_loader import JsonLoader
 from github_poster.loader.kindle_loader import KindleLoader
 from github_poster.loader.leetcode_loader import LeetcodeLoader
 from github_poster.loader.multiple_loader import MultipleLoader
+from github_poster.loader.neodb_loader import NeoDBLoader
 from github_poster.loader.notion_loader import NotionLoader
 from github_poster.loader.nrc_loader import NRCLoader
 from github_poster.loader.ns_loader import NSLoader
 from github_poster.loader.openlanguage_loader import OpenLanguageLoader
 from github_poster.loader.shanbay_loader import ShanBayLoader
 from github_poster.loader.strava_loader import StravaLoader
 from github_poster.loader.summary_loader import SummaryLoader
@@ -58,14 +59,15 @@
     "jike": JikeLoader,
     "summary": SummaryLoader,
     "weread": WereadLoader,
     "covid": CovidLoader,
     "todoist": TodoistLoader,
     "openlanguage": OpenLanguageLoader,
     "chatgpt": ChatGPTLoader,
+    "neodb": NeoDBLoader,
 }
 
 __all__ = (
     "AppleHealthLoader",
     "BilibiliLoader",
     "CiChangLoader",
     "Dota2Loader",
@@ -93,8 +95,9 @@
     "SummaryLoader",
     "BBDCLoader",
     "WereadLoader",
     "CovidLoader",
     "TodoistLoader",
     "OpenLanguageLoader",
     "ChatGPTLoader",
+    "NeoDBLoader",
 )
```

### Comparing `github_poster-2.5.1/github_poster/loader/apple_health_loader.py` & `github_poster-2.6.0/github_poster/loader/apple_health_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/base_loader.py` & `github_poster-2.6.0/github_poster/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/bbdc_loader.py` & `github_poster-2.6.0/github_poster/loader/bbdc_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/bilibili_loader.py` & `github_poster-2.6.0/github_poster/loader/bilibili_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/chatgpt_loader.py` & `github_poster-2.6.0/github_poster/loader/chatgpt_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/cichang_loader.py` & `github_poster-2.6.0/github_poster/loader/cichang_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/config.py` & `github_poster-2.6.0/github_poster/loader/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from collections import namedtuple
 
 # China timezone if you are from others please change this
 TIME_ZONE = "Asia/Shanghai"
 
+# neodb -- need to get token from https://neodb.social/developer/
+NEODB_API = "https://neodb.social/api/me/shelf/{type}?page={page}"
+
 # shanbay -- no need to login
-SHANBAY_CALENDAR_API = (
-    "https://apiv3.shanbay.com/uc/checkin/calendar/dates"
-    "?user_id={user_name}&start_date={start_date}&end_date={end_date}"
+SHANBAY_WORD_API = (
+    "https://apiv3.shanbay.com/uc/checkin/logs?user_id={user_name}&ipp=20&page={page}"
 )
 
 # duolingo -- no need to login
 DUOLINGO_CALENDAR_API = (
     "https://ios-api-2.duolingo.com/2017-06-30/users/{user_id}/xp_summaries"
     "?endDate={end_date}&startDate={start_date}&timezone=Asia/Shanghai"
 )
-DUOLINGO_LOGIN_URL = "https://www.duolingo.com/login"
 
 # cichang -- need to login
 HJ_APPKEY = "45fd17e02003d89bee7f046bb494de13"
 CICHANG_LOGIN_URL = (
     "https://pass.hujiang.com/Handler/UCenter.json?action=Login&isapp=true"
     "&language=zh_CN&password={password}&timezone=8&user_domain=hj&username={user_name}"
 )
```

### Comparing `github_poster-2.5.1/github_poster/loader/covid_loader.py` & `github_poster-2.6.0/github_poster/loader/covid_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/dota2_loader.py` & `github_poster-2.6.0/github_poster/loader/dota2_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/duolingo_loader.py` & `github_poster-2.6.0/github_poster/loader/duolingo_loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import pendulum
 import requests
 
 from github_poster.loader.base_loader import BaseLoader
-from github_poster.loader.config import DUOLINGO_CALENDAR_API, DUOLINGO_LOGIN_URL
+from github_poster.loader.config import DUOLINGO_CALENDAR_API
 
 
 class DuolingoLoader(BaseLoader):
     unit = "XP"
     track_color = "#78C800"
 
     def __init__(self, from_year, to_year, _type, **kwargs):
         super().__init__(from_year, to_year, _type)
-        self.duolingo_id = kwargs.get("duolingo_user_id", "")
+        self.duolingo_user_name = kwargs.get("duolingo_user_name", "")
         self.duolingo_jwt = kwargs.get("duolingo_jwt", "")
         self.session = requests.Session()
         self.headers = {
             "Accept": "*/*",
             "User-Agent": "request",
         }
 
     @classmethod
     def add_loader_arguments(cls, parser, optional):
         parser.add_argument(
-            "--duolingo_user_id",
-            dest="duolingo_user_id",
+            "--duolingo_user_name",
+            dest="duolingo_user_name",
             type=str,
             help="",
             required=optional,
         )
         parser.add_argument(
             "--duolingo_jwt",
             dest="duolingo_jwt",
             type=str,
             help="use `document.cookie.match(new RegExp('(^| )jwt_token=([^;]+)'))[0].slice(11)` in console",
             required=optional,
         )
 
     def login(self):
         self.headers["Authorization"] = "Bearer " + self.duolingo_jwt
-        self.duolingo_id = self.duolingo_id
+        self.duolingo_id = self.session.get(
+            f"https://www.duolingo.com/users/{self.duolingo_user_name}",
+            headers=self.headers,
+        ).json()["id"]
 
     def get_api_data(self):
         month_list = self.make_month_list()
         for m in month_list:
             r = self.session.get(
                 DUOLINGO_CALENDAR_API.format(
                     user_id=self.duolingo_id,
```

### Comparing `github_poster-2.5.1/github_poster/loader/forest_loader.py` & `github_poster-2.6.0/github_poster/loader/forest_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/from_github_issue_loader.py` & `github_poster-2.6.0/github_poster/loader/from_github_issue_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/garmin_loader.py` & `github_poster-2.6.0/github_poster/loader/garmin_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/github_loader.py` & `github_poster-2.6.0/github_poster/loader/github_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/gitlab_loader.py` & `github_poster-2.6.0/github_poster/loader/gitlab_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/gpx_loader.py` & `github_poster-2.6.0/github_poster/loader/gpx_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/jike_loader.py` & `github_poster-2.6.0/github_poster/loader/jike_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/json_loader.py` & `github_poster-2.6.0/github_poster/loader/json_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/kindle_loader.py` & `github_poster-2.6.0/github_poster/loader/kindle_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/leetcode_loader.py` & `github_poster-2.6.0/github_poster/loader/leetcode_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/multiple_loader.py` & `github_poster-2.6.0/github_poster/loader/multiple_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/notion_loader.py` & `github_poster-2.6.0/github_poster/loader/notion_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/nrc_loader.py` & `github_poster-2.6.0/github_poster/loader/nrc_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/ns_loader.py` & `github_poster-2.6.0/github_poster/loader/ns_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/openlanguage_loader.py` & `github_poster-2.6.0/github_poster/loader/openlanguage_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/shanbay_loader.py` & `github_poster-2.6.0/github_poster/loader/weread_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,60 @@
+import pendulum
 import requests
 
 from github_poster.loader.base_loader import BaseLoader
-from github_poster.loader.config import SHANBAY_CALENDAR_API
+from github_poster.loader.config import WEREAD_BASE_URL, WEREAD_HISTORY_URL
 
 
-class ShanBayLoader(BaseLoader):
-    track_color = "#33C6A4"
-    unit = "days"
+class WereadLoader(BaseLoader):
+    track_color = "#2EA8F7"
+    unit = "mins"
 
     def __init__(self, from_year, to_year, _type, **kwargs):
         super().__init__(from_year, to_year, _type)
-        self.user_name = kwargs.get("shanbay_user_name", "")
+        self.weread_cookie = kwargs.get("weread_cookie", "")
+        self.session = requests.Session()
+        self._make_years_list()
 
     @classmethod
     def add_loader_arguments(cls, parser, optional):
         parser.add_argument(
-            "--shanbay_user_name",
-            dest="shanbay_user_name",
+            "--weread_cookie",
+            dest="weread_cookie",
             type=str,
             required=optional,
             help="",
         )
 
     def get_api_data(self):
-        month_list = self.make_month_list()
-        for m in month_list:
-            r = requests.get(
-                SHANBAY_CALENDAR_API.format(
-                    user_name=self.user_name,
-                    start_date=m.to_date_string(),
-                    end_date=m.end_of("month").to_date_string(),
-                )
-            )
-            if not r.ok:
-                print(f"get shanbay calendar api failed {str(r.text)}")
-            try:
-                yield from r.json()["logs"]
-            except Exception:
-                # just pass for now
-                pass
+        r = self.session.get(WEREAD_HISTORY_URL)
+        if not r.ok:
+            # need to refresh cookie WTF the design!!
+            if r.json()["errcode"] == -2012:
+                self.session.get(WEREAD_BASE_URL)
+                r = self.session.get(WEREAD_HISTORY_URL)
+            else:
+                raise Exception("Can not get weread history data")
+        return r.json()
 
     def make_track_dict(self):
-        data_list = self.get_api_data()
-        for d in data_list:
-            if d:
-                self.number_by_date_dict[d["date"]] = 1
-                self.number_list.append(1)
+        api_data = self.get_api_data()
+        month_data = api_data["datas"]
+        for m in month_data:
+            m_start_date = pendulum.from_timestamp(
+                m["baseTimestamp"], tz=self.time_zone
+            )
+            read_time_list = m["timeMeta"]["readTimeList"]
+            if not sum(read_time_list):
+                continue
+            m_end_date = m_start_date.end_of("month")
+            m_date_list = list(pendulum.period(m_start_date, m_end_date))
+            for k, v in zip(m_date_list, read_time_list):
+                self.number_by_date_dict[k.to_date_string()] = round(v / 60.0, 2)
+        for _, v in self.number_by_date_dict.items():
+            self.number_list.append(v)
 
     def get_all_track_data(self):
+        self.session.cookies = self.parse_cookie_string(self.weread_cookie)
         self.make_track_dict()
         self.make_special_number()
         return self.number_by_date_dict, self.year_list
```

### Comparing `github_poster-2.5.1/github_poster/loader/strava_loader.py` & `github_poster-2.6.0/github_poster/loader/strava_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/summary_loader.py` & `github_poster-2.6.0/github_poster/loader/summary_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/todoist_loader.py` & `github_poster-2.6.0/github_poster/loader/todoist_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/twitter_loader.py` & `github_poster-2.6.0/github_poster/loader/twitter_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/wakatime_loader.py` & `github_poster-2.6.0/github_poster/loader/wakatime_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/loader/youtube_loader.py` & `github_poster-2.6.0/github_poster/loader/youtube_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/poster.py` & `github_poster-2.6.0/github_poster/poster.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/skyline/skyline.py` & `github_poster-2.6.0/github_poster/skyline/skyline.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/structures.py` & `github_poster-2.6.0/github_poster/structures.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster/utils.py` & `github_poster-2.6.0/github_poster/utils.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.1/github_poster.egg-info/SOURCES.txt` & `github_poster-2.6.0/github_poster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 github_poster/loader/gitlab_loader.py
 github_poster/loader/gpx_loader.py
 github_poster/loader/jike_loader.py
 github_poster/loader/json_loader.py
 github_poster/loader/kindle_loader.py
 github_poster/loader/leetcode_loader.py
 github_poster/loader/multiple_loader.py
+github_poster/loader/neodb_loader.py
 github_poster/loader/notion_loader.py
 github_poster/loader/nrc_loader.py
 github_poster/loader/ns_loader.py
 github_poster/loader/openlanguage_loader.py
 github_poster/loader/shanbay_loader.py
 github_poster/loader/strava_loader.py
 github_poster/loader/summary_loader.py
```

### Comparing `github_poster-2.5.1/setup.py` & `github_poster-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name="github_poster",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     url="https://github.com/yihong0618/GitHubPoster",
     license="MIT",
-    version="2.5.1",
+    version="2.6.0",
     description="Make everything a GitHub svg poster and Skyline!",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "requests",
         "svgwrite",
         "pendulum",
```

### Comparing `github_poster-2.5.1/tests/test_poster_utils.py` & `github_poster-2.6.0/tests/test_poster_utils.py`

 * *Files identical despite different names*

