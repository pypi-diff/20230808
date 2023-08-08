# Comparing `tmp/TikTokApi-5.2.2.tar.gz` & `tmp/TikTokApi-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TikTokApi-5.2.2.tar", last modified: Fri Jul 15 22:30:25 2022, max compression
+gzip compressed data, was "TikTokApi-6.0.0.tar", last modified: Tue Aug  8 06:51:53 2023, max compression
```

## Comparing `TikTokApi-5.2.2.tar` & `TikTokApi-6.0.0.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.111083 TikTokApi-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-07-15 22:30:25.111083 TikTokApi-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.107083 TikTokApi-5.2.2/TikTokApi/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.107083 TikTokApi-5.2.2/TikTokApi/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/comment.py
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/hashtag.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     5795 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/sound.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/trending.py
--rw-r--r--   0 runner    (1001) docker     (121)     9665 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.107083 TikTokApi-5.2.2/TikTokApi/browser_utilities/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/browser_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8444 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/browser_utilities/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/browser_utilities/browser_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    60334 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/browser_utilities/get_acrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    23818 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/tiktok.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/TikTokApi/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.107083 TikTokApi-5.2.2/TikTokApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-07-15 22:30:25.000000 TikTokApi-5.2.2/TikTokApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-07-15 22:30:25.000000 TikTokApi-5.2.2/TikTokApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 22:30:25.000000 TikTokApi-5.2.2/TikTokApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-15 22:30:25.000000 TikTokApi-5.2.2/TikTokApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-15 22:30:25.000000 TikTokApi-5.2.2/TikTokApi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.111083 TikTokApi-5.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/comment_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/hashtag_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/search_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/sound_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/trending_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/user_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/examples/video_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-15 22:30:25.111083 TikTokApi-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:25.111083 TikTokApi-5.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_hashtag.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_sound.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_trending.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-07-15 22:30:17.000000 TikTokApi-5.2.2/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.948604 TikTokApi-6.0.0/TikTokApi/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.952604 TikTokApi-6.0.0/TikTokApi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.952604 TikTokApi-6.0.0/TikTokApi/stealth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/stealth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/stealth/stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/tiktok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.948604 TikTokApi-6.0.0/TikTokApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_video.py
```

### Comparing `TikTokApi-5.2.2/LICENSE` & `TikTokApi-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokApi-5.2.2/LICENSE.txt` & `TikTokApi-6.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TikTokApi-5.2.2/PKG-INFO` & `TikTokApi-6.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,76 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 5.2.2
+Version: 6.0.0
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
+Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
-Download-URL: https://github.com/davidteather/TikTok-Api/tarball/master
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 
 # Unofficial TikTok API in Python
 
 This is an unofficial api wrapper for TikTok.com in python. With this api you are able to call most trending and fetch specific user information as well as much more.
 
- [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+ [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+
+This api is designed to **retrieve data** TikTok. It **can not be used post or upload** content to TikTok on the behalf of a user. It has **no support any user-authenticated routes**, if you can't access it while being logged out on their website you can't access it here.
 
 ## Sponsors
 These sponsors have paid to be placed here and beyond that I do not have any affiliation with them, the TikTokAPI package will always be free and open-source. If you wish to be a sponsor of this project check out my [GitHub sponsors page](https://github.com/sponsors/davidteather).
 
 <div align="center">
-    <p>
     <a href="https://tikapi.io/?ref=davidteather" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/tikapi.png" width="100" alt="TikApi">
-			</div>
-			<b></b>
-			<div>
-				<b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
-			</div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://trendpop.social/?ref=github-davidteather-tiktokapi" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/trendpop.png" width="100" alt="Trendpop">
-			</div>
-			<div>
-				Trendpop builds software to help creators and businesses go viral on social video platforms.
-			</div>
-            <div>
-                <sub>
-                    Excited about building in this space?
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi">
-                        <sub>We're hiring engineers across all roles</sub>
-                    </a>
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi" target="_blank">
-                    <sub>- shoot us a message at </sub>
-                    </a>
-                    <a href="mailto:founders@trendpop.social" target="_blank">
-                    <sub><code>founders@trendpop.social</code></sub>
-                    </a>
-                </sub>
-            </div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://influencerhunters.com/docs.html?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_t" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/andrearama/TikTok-Api/master/imgs/IH_LOGO.png" width="100" alt="IH_logo">
-			</div>
-			<b></b>
-			<div>
-				TikTok data through APIs, providing 10+ Million posts / day to the largest Marketing and Social listening platforms.
-			</div>
-		</a>
-    </p>
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/tikapi.png" width="100" alt="TikApi">
+        <div>
+            <b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
+        </div>
+    </a>
+    <br>
+    <a href="https://www.ensembledata.com/?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_thea_github" target="_blank">
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/EnsembleData.png" width="100" alt="Ensemble Data">
+        <b></b>
+        <div>
+            <b>Ensemble Data</b> is the leading API provider for scraping all the major Social Media. <br> We provide 100+ Million posts / day to the largest Marketing and Social listening platforms.
+        </div>
+	</a>
 </div>
 
 ## Table of Contents
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
     - [How to Support The Project](#how-to-support-the-project)
     - [Installing](#installing)
     - [Common Issues](#common-issues)
 - [Quick Start Guide](#quick-start-guide)
-    - [Examples](https://github.com/davidteather/TikTok-Api/tree/master/examples)
+    - [Examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
 
-[**Upgrading from V4 to V5**](#upgrading-from-v4-to-v5)
+[**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
 
 ## Documentation
 
-You can find the full documentation [here](https://davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class](https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where you'll probably spend most of your time.
+You can find the full documentation [here](https://davidteather.github.io/TikTok-Api)
 ## Getting Started
 
-To get started using this api follow the instructions below.
+To get started using this API follow the instructions below.
 
-**Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
+**Note:** If you want to learn how to web scrape websites check my [free and open-source course for learning everything web scraping](https://github.com/davidteather/everything-web-scraping)
 
 ### How to Support The Project
 * Star the repo 😎
 * Consider [sponsoring](https://github.com/sponsors/davidteather) me on GitHub
 * Send me an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what you're using the API for, I really like hearing what people are using it for.
 * Submit PRs for issues :)
 
@@ -120,15 +78,15 @@
 
 If you run into an issue please check the closed issues on the github, although feel free to re-open a new issue if you find an issue that's been closed for a few months. The codebase can and does run into similar issues as it has before, because TikTok changes things up.
 
 ```sh
 pip install TikTokApi
 python -m playwright install
 ```
-If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that.
+If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date, installation is the same though)
 
 If you want a quick video to listen for [TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
 
 #### Docker Installation
 
 Clone this repository onto a local machine (or just the Dockerfile since it installs TikTokApi from pip) then run the following commands.
 
@@ -144,92 +102,58 @@
 
 Please don't open an issue if you're experiencing one of these just comment if the provided solution do not work for you.
 
 * **Browser Has no Attribute** - make sure you ran `python3 -m playwright install`, if your error persists try the [playwright-python](https://github.com/microsoft/playwright-python) quickstart guide and diagnose issues from there.
 
 ## Quick Start Guide
 
-Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
+Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/main/examples) directory.
 
 **Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
 
 ```py
 from TikTokApi import TikTokApi
+import asyncio
+import os
 
-# Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api:
-    for trending_video in api.trending.videos(count=50):
-        # Prints the author's username of the trending video.
-        print(trending_video.author.username)
-```
+ms_token = os.environ.get("ms_token", None) # get your own ms_token from your cookies on tiktok.com
+
+async def trending_videos():
+    async with TikTokApi() as api:
+        await api.create_sessions(ms_tokens=[ms_token], num_sessions=1, sleep_after=3)
+        async for video in api.trending.videos(count=30):
+            print(video)
+            print(video.as_dict)
 
-**Note**: Jupyter (ipynb) only works on linux, see [microsoft/playwright-python #178](https://github.com/microsoft/playwright-python/issues/178)
+if __name__ == "__main__":
+    asyncio.run(trending_videos())
+```
 
-To run the example scripts from the repository root, make sure you use the `-m` option on python.
+To directly run the example scripts from the repository root, use the `-m` option on python.
 ```sh
 python -m examples.get_trending
 ```
 
-You can access the dictionary type of an object using `.as_dict`. On a video this may look like
-[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
-
-## Upgrading from V4 to V5
+You can access the full data dictionary the object was created from with `.as_dict`. On a video this may look like
+[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
 
-All changes will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if you want more information.
+## Upgrading from V5 to V6
 
-### Motivation
+All changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/releases/tag/V6.0.0) if you want more information.
 
-This package has been difficult to maintain due to it's structure, difficult to work with since the user of the package must write parsing methods to extract information from dictionaries, more memory intensive than it needs to be (although this can be further improved), and in general just difficult to work with for new users. 
-
-As a result, I've decided to at least attempt to remedy some of these issues, the biggest changes are that 
-1. The package has shifted to using classes for different TikTok objects resulting in an easier, higher-level programming experience.
-2. All methods that used to return a list of objects have been switched to using iterators, to hopefully decrease memory utilization for most users.
+### Changes & Motivations
 
+* Maintainability
+    * Was getting difficult to maintain with how TikTok was directly detecting HTTP requests.
+    * Switched to using a pool of **async** playwright pages to make it more difficult to detect, and hopefully easier to maintain in the future
+* Async
+    * It's been asked for a lot, and now fully async needed especially since the package is using a pool of playwright instances
+* User Flexibility
+    * Added a lot of function argument options that should be much more explicit than what was done previously.
+    * Hopefully if something is broken there's a workaround without having to modify the package itself (although if you do notice an issue please open an issue or submit a PR)
+* Documentation
+    * Goes with user flexibility a little bit but switched over to sphinx documentation for more explicit content
+    * If you run into an issue or are confused please open a github issue or submit a PR to fix documentation, it's always welcome! 🤠
 
 ### Upgrading Examples
 
-
-#### Accessing Dictionary on Objects (similar to V4)
-
-You'll probably need to use this beyond just for legacy support, since not all attributes are parsed out and attached
-to the different objects.
-
-You may want to use this as a workaround for legacy applications while you upgrade the rest of the app. I'd suggest that you do eventually upgrade to using the higher-level approach fully.
-```py
-user = api.user(username='therock')
-user.as_dict # -> dict of the user_object
-for video in user.videos():
-    video.as_dict # -> dict of TikTok's video object as found when requesting the videos endpoint
-```
-
-Here's a few more examples that help illustrate the differences in the flow of the usage of the package with V5.
-
-```py
-# V4
-api = TikTokApi.get_instance()
-trending_videos = api.by_trending()
-
-#V5.1
-with TikTokApi() as api: # .get_instance no longer exists
-    for trending_video in api.trending.videos():
-        # do something
-```
-
-Where in V4 you had to extract information yourself, the package now handles that for you. So it's much easier to do chained related function calls.
-```py
-# V4
-trending_videos = api.by_trending()
-for video in trending_videos:
-    # The dictionary responses are also different depending on what endpoint you got them from
-    # So, it's usually more painful than this to deal with
-    trending_user = api.get_user(id=video['author']['id'], secUid=video['author']['secUid'])
-
-
-# V5
-# This is more complicated than above, but it illustrates the simplified approach
-for trending_video in api.trending.videos():
-    user_stats = trending_video.author.info_full['stats']
-    if user_stats['followerCount'] >= 10000:
-        # maybe save the user in a database
-```
-
-
+The biggest change is that everything is now async. You can see above how you might want to call an async function in python as well as the examples directory for more examples.
```

#### html2text {}

```diff
@@ -1,135 +1,113 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 5.2.2 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.0 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
-tiktok-api Author: David Teather Author-email: contact.davidteather@gmail.com
-License: MIT Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
-master Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
-File: LICENSE License-File: LICENSE.txt # Unofficial TikTok API in Python This
-is an unofficial api wrapper for TikTok.com in python. With this api you are
-able to call most trending and fetch specific user information as well as much
-more. [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/
-badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-
-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)]
-(https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://
-img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://
-github.com/sponsors/davidteather) [![GitHub release (latest by date)](https://
+tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
+main Author: David Teather Author-email: contact.davidteather@gmail.com
+License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE License-File: LICENSE.txt # Unofficial TikTok API in
+Python This is an unofficial api wrapper for TikTok.com in python. With this
+api you are able to call most trending and fetch specific user information as
+well as much more. [![DOI](https://zenodo.org/badge/188710490.svg)](https://
+zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/
+badge/LinkedIn-0077B5?style=for-the-
+badge&logo=linkedin&logoColor=white&style=flat-square)](https://
+www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/
+static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/
+sponsors/davidteather) [![GitHub release (latest by date)](https://
 img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/
-davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/
-github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://
-github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [!
-[GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https:
-//github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https:/
-/pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://
-visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support
-Server](https://img.shields.io/discord/
+davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/
+license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/
+blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://
+pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/
+badge?page_id=davidteather.TikTok-Api) [![Support Server](https://
+img.shields.io/discord/
 783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://
-discord.gg/yyPhbfma6f) ## Sponsors These sponsors have paid to be placed here
-and beyond that I do not have any affiliation with them, the TikTokAPI package
-will always be free and open-source. If you wish to be a sponsor of this
-project check out my [GitHub sponsors page](https://github.com/sponsors/
-davidteather).
+discord.gg/yyPhbfma6f) This api is designed to **retrieve data** TikTok. It
+**can not be used post or upload** content to TikTok on the behalf of a user.
+It has **no support any user-authenticated routes**, if you can't access it
+while being logged out on their website you can't access it here. ## Sponsors
+These sponsors have paid to be placed here and beyond that I do not have any
+affiliation with them, the TikTokAPI package will always be free and open-
+source. If you wish to be a sponsor of this project check out my [GitHub
+sponsors page](https://github.com/sponsors/davidteather).
                                    [TikApi]
  TikAPI_is_a_paid_TikTok_API_service_providing_a_full_out-of-the-box_solution,
        making_life_easier_for_developers_â_trusted_by_500+_companies.
 
-                                  [Trendpop]
-  Trendpop_builds_software_to_help_creators_and_businesses_go_viral_on_social
-                               video_platforms.
-Excited_about_building_in_this_space?_We're_hiring_engineers_across_all_roles_-
-                shoot_us_a_message_at_founders@trendpop.social
-
-                                   [IH_logo]
-  TikTok_data_through_APIs,_providing_10+_Million_posts_/_day_to_the_largest
-                   Marketing_and_Social_listening_platforms.
+                               [Ensemble_Data]
+  Ensemble_Data_is_the_leading_API_provider_for_scraping_all_the_major_Social
+                                    Media.
+    We_provide_100+_Million_posts_/_day_to_the_largest_Marketing_and_Social
+                             listening_platforms.
 ## Table of Contents - [Documentation](#documentation) - [Getting Started]
 (#getting-started) - [How to Support The Project](#how-to-support-the-project)
 - [Installing](#installing) - [Common Issues](#common-issues) - [Quick Start
 Guide](#quick-start-guide) - [Examples](https://github.com/davidteather/TikTok-
-Api/tree/master/examples) [**Upgrading from V4 to V5**](#upgrading-from-v4-to-
-v5) ## Documentation You can find the full documentation [here](https://
-davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class]
-(https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where
-you'll probably spend most of your time. ## Getting Started To get started
-using this api follow the instructions below. **Note:** If you want to learn
-how to web scrape websites check my [free and open-source course for web
-scraping](https://github.com/davidteather/web-scraping-with-reverse-
-engineering) ### How to Support The Project * Star the repo ð * Consider
-[sponsoring](https://github.com/sponsors/davidteather) me on GitHub * Send me
-an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message
-telling me what you're using the API for, I really like hearing what people are
-using it for. * Submit PRs for issues :) ### Installing If you run into an
-issue please check the closed issues on the github, although feel free to re-
-open a new issue if you find an issue that's been closed for a few months. The
-codebase can and does run into similar issues as it has before, because TikTok
-changes things up. ```sh pip install TikTokApi python -m playwright install ```
-If you would prefer a video walk through of setting up this package [YouTube
-video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. If you want
-a quick video to listen for [TikTok Live](https://www.youtube.com/
-watch?v=307ijmA3_lc) events in python. #### Docker Installation Clone this
-repository onto a local machine (or just the Dockerfile since it installs
-TikTokApi from pip) then run the following commands. ```sh docker pull
-mcr.microsoft.com/playwright:focal docker build . -t tiktokapi:latest docker
-run -v TikTokApi --rm tiktokapi:latest python3 your_script.py ``` **Note** this
-assumes your script is named your_script.py and lives in the root of this
-directory. ### Common Issues Please don't open an issue if you're experiencing
-one of these just comment if the provided solution do not work for you. *
-**Browser Has no Attribute** - make sure you ran `python3 -m playwright
-install`, if your error persists try the [playwright-python](https://
-github.com/microsoft/playwright-python) quickstart guide and diagnose issues
-from there. ## Quick Start Guide Here's a quick bit of code to get the most
-recent trending videos on TikTok. There's more examples in the [examples]
-(https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
-**Note:** If you want to learn how to web scrape websites check my [free and
-open-source course for web scraping](https://github.com/davidteather/web-
-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi #
-Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api: for trending_video in api.trending.videos(count=50): #
-Prints the author's username of the trending video. print
-(trending_video.author.username) ``` **Note**: Jupyter (ipynb) only works on
-linux, see [microsoft/playwright-python #178](https://github.com/microsoft/
-playwright-python/issues/178) To run the example scripts from the repository
-root, make sure you use the `-m` option on python. ```sh python -
-m examples.get_trending ``` You can access the dictionary type of an object
-using `.as_dict`. On a video this may look like [this](https://gist.github.com/
-davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their
-structure from time to time so it's worth investigating the structure of the
-dictionary when you use this package. ## Upgrading from V4 to V5 All changes
-will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if
-you want more information. ### Motivation This package has been difficult to
-maintain due to it's structure, difficult to work with since the user of the
-package must write parsing methods to extract information from dictionaries,
-more memory intensive than it needs to be (although this can be further
-improved), and in general just difficult to work with for new users. As a
-result, I've decided to at least attempt to remedy some of these issues, the
-biggest changes are that 1. The package has shifted to using classes for
-different TikTok objects resulting in an easier, higher-level programming
-experience. 2. All methods that used to return a list of objects have been
-switched to using iterators, to hopefully decrease memory utilization for most
-users. ### Upgrading Examples #### Accessing Dictionary on Objects (similar to
-V4) You'll probably need to use this beyond just for legacy support, since not
-all attributes are parsed out and attached to the different objects. You may
-want to use this as a workaround for legacy applications while you upgrade the
-rest of the app. I'd suggest that you do eventually upgrade to using the
-higher-level approach fully. ```py user = api.user(username='therock')
-user.as_dict # -> dict of the user_object for video in user.videos():
-video.as_dict # -> dict of TikTok's video object as found when requesting the
-videos endpoint ``` Here's a few more examples that help illustrate the
-differences in the flow of the usage of the package with V5. ```py # V4 api =
-TikTokApi.get_instance() trending_videos = api.by_trending() #V5.1 with
-TikTokApi() as api: # .get_instance no longer exists for trending_video in
-api.trending.videos(): # do something ``` Where in V4 you had to extract
-information yourself, the package now handles that for you. So it's much easier
-to do chained related function calls. ```py # V4 trending_videos =
-api.by_trending() for video in trending_videos: # The dictionary responses are
-also different depending on what endpoint you got them from # So, it's usually
-more painful than this to deal with trending_user = api.get_user(id=video
-['author']['id'], secUid=video['author']['secUid']) # V5 # This is more
-complicated than above, but it illustrates the simplified approach for
-trending_video in api.trending.videos(): user_stats =
-trending_video.author.info_full['stats'] if user_stats['followerCount'] >=
-10000: # maybe save the user in a database ```
+Api/tree/main/examples) [**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
+## Documentation You can find the full documentation [here](https://
+davidteather.github.io/TikTok-Api) ## Getting Started To get started using this
+API follow the instructions below. **Note:** If you want to learn how to web
+scrape websites check my [free and open-source course for learning everything
+web scraping](https://github.com/davidteather/everything-web-scraping) ### How
+to Support The Project * Star the repo ð * Consider [sponsoring](https://
+github.com/sponsors/davidteather) me on GitHub * Send me an email or a
+[LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what
+you're using the API for, I really like hearing what people are using it for. *
+Submit PRs for issues :) ### Installing If you run into an issue please check
+the closed issues on the github, although feel free to re-open a new issue if
+you find an issue that's been closed for a few months. The codebase can and
+does run into similar issues as it has before, because TikTok changes things
+up. ```sh pip install TikTokApi python -m playwright install ``` If you would
+prefer a video walk through of setting up this package [YouTube video](https://
+www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date,
+installation is the same though) If you want a quick video to listen for
+[TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
+#### Docker Installation Clone this repository onto a local machine (or just
+the Dockerfile since it installs TikTokApi from pip) then run the following
+commands. ```sh docker pull mcr.microsoft.com/playwright:focal docker build . -
+t tiktokapi:latest docker run -v TikTokApi --rm tiktokapi:latest python3
+your_script.py ``` **Note** this assumes your script is named your_script.py
+and lives in the root of this directory. ### Common Issues Please don't open an
+issue if you're experiencing one of these just comment if the provided solution
+do not work for you. * **Browser Has no Attribute** - make sure you ran
+`python3 -m playwright install`, if your error persists try the [playwright-
+python](https://github.com/microsoft/playwright-python) quickstart guide and
+diagnose issues from there. ## Quick Start Guide Here's a quick bit of code to
+get the most recent trending videos on TikTok. There's more examples in the
+[examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
+directory. **Note:** If you want to learn how to web scrape websites check my
+[free and open-source course for web scraping](https://github.com/davidteather/
+web-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi
+import asyncio import os ms_token = os.environ.get("ms_token", None) # get your
+own ms_token from your cookies on tiktok.com async def trending_videos(): async
+with TikTokApi() as api: await api.create_sessions(ms_tokens=[ms_token],
+num_sessions=1, sleep_after=3) async for video in api.trending.videos
+(count=30): print(video) print(video.as_dict) if __name__ == "__main__":
+asyncio.run(trending_videos()) ``` To directly run the example scripts from the
+repository root, use the `-m` option on python. ```sh python -
+m examples.get_trending ``` You can access the full data dictionary the object
+was created from with `.as_dict`. On a video this may look like [this](https://
+gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes
+their structure from time to time so it's worth investigating the structure of
+the dictionary when you use this package. ## Upgrading from V5 to V6 All
+changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/
+releases/tag/V6.0.0) if you want more information. ### Changes & Motivations *
+Maintainability * Was getting difficult to maintain with how TikTok was
+directly detecting HTTP requests. * Switched to using a pool of **async**
+playwright pages to make it more difficult to detect, and hopefully easier to
+maintain in the future * Async * It's been asked for a lot, and now fully async
+needed especially since the package is using a pool of playwright instances *
+User Flexibility * Added a lot of function argument options that should be much
+more explicit than what was done previously. * Hopefully if something is broken
+there's a workaround without having to modify the package itself (although if
+you do notice an issue please open an issue or submit a PR) * Documentation *
+Goes with user flexibility a little bit but switched over to sphinx
+documentation for more explicit content * If you run into an issue or are
+confused please open a github issue or submit a PR to fix documentation, it's
+always welcome! ð¤  ### Upgrading Examples The biggest change is that
+everything is now async. You can see above how you might want to call an async
+function in python as well as the examples directory for more examples.
```

### Comparing `TikTokApi-5.2.2/README.md` & `TikTokApi-6.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,55 @@
 
 # Unofficial TikTok API in Python
 
 This is an unofficial api wrapper for TikTok.com in python. With this api you are able to call most trending and fetch specific user information as well as much more.
 
- [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+ [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+
+This api is designed to **retrieve data** TikTok. It **can not be used post or upload** content to TikTok on the behalf of a user. It has **no support any user-authenticated routes**, if you can't access it while being logged out on their website you can't access it here.
 
 ## Sponsors
 These sponsors have paid to be placed here and beyond that I do not have any affiliation with them, the TikTokAPI package will always be free and open-source. If you wish to be a sponsor of this project check out my [GitHub sponsors page](https://github.com/sponsors/davidteather).
 
 <div align="center">
-    <p>
     <a href="https://tikapi.io/?ref=davidteather" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/tikapi.png" width="100" alt="TikApi">
-			</div>
-			<b></b>
-			<div>
-				<b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
-			</div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://trendpop.social/?ref=github-davidteather-tiktokapi" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/trendpop.png" width="100" alt="Trendpop">
-			</div>
-			<div>
-				Trendpop builds software to help creators and businesses go viral on social video platforms.
-			</div>
-            <div>
-                <sub>
-                    Excited about building in this space?
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi">
-                        <sub>We're hiring engineers across all roles</sub>
-                    </a>
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi" target="_blank">
-                    <sub>- shoot us a message at </sub>
-                    </a>
-                    <a href="mailto:founders@trendpop.social" target="_blank">
-                    <sub><code>founders@trendpop.social</code></sub>
-                    </a>
-                </sub>
-            </div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://influencerhunters.com/docs.html?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_t" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/andrearama/TikTok-Api/master/imgs/IH_LOGO.png" width="100" alt="IH_logo">
-			</div>
-			<b></b>
-			<div>
-				TikTok data through APIs, providing 10+ Million posts / day to the largest Marketing and Social listening platforms.
-			</div>
-		</a>
-    </p>
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/tikapi.png" width="100" alt="TikApi">
+        <div>
+            <b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
+        </div>
+    </a>
+    <br>
+    <a href="https://www.ensembledata.com/?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_thea_github" target="_blank">
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/EnsembleData.png" width="100" alt="Ensemble Data">
+        <b></b>
+        <div>
+            <b>Ensemble Data</b> is the leading API provider for scraping all the major Social Media. <br> We provide 100+ Million posts / day to the largest Marketing and Social listening platforms.
+        </div>
+	</a>
 </div>
 
 ## Table of Contents
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
     - [How to Support The Project](#how-to-support-the-project)
     - [Installing](#installing)
     - [Common Issues](#common-issues)
 - [Quick Start Guide](#quick-start-guide)
-    - [Examples](https://github.com/davidteather/TikTok-Api/tree/master/examples)
+    - [Examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
 
-[**Upgrading from V4 to V5**](#upgrading-from-v4-to-v5)
+[**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
 
 ## Documentation
 
-You can find the full documentation [here](https://davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class](https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where you'll probably spend most of your time.
+You can find the full documentation [here](https://davidteather.github.io/TikTok-Api)
 ## Getting Started
 
-To get started using this api follow the instructions below.
+To get started using this API follow the instructions below.
 
-**Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
+**Note:** If you want to learn how to web scrape websites check my [free and open-source course for learning everything web scraping](https://github.com/davidteather/everything-web-scraping)
 
 ### How to Support The Project
 * Star the repo 😎
 * Consider [sponsoring](https://github.com/sponsors/davidteather) me on GitHub
 * Send me an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what you're using the API for, I really like hearing what people are using it for.
 * Submit PRs for issues :)
 
@@ -97,15 +57,15 @@
 
 If you run into an issue please check the closed issues on the github, although feel free to re-open a new issue if you find an issue that's been closed for a few months. The codebase can and does run into similar issues as it has before, because TikTok changes things up.
 
 ```sh
 pip install TikTokApi
 python -m playwright install
 ```
-If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that.
+If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date, installation is the same though)
 
 If you want a quick video to listen for [TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
 
 #### Docker Installation
 
 Clone this repository onto a local machine (or just the Dockerfile since it installs TikTokApi from pip) then run the following commands.
 
@@ -121,90 +81,58 @@
 
 Please don't open an issue if you're experiencing one of these just comment if the provided solution do not work for you.
 
 * **Browser Has no Attribute** - make sure you ran `python3 -m playwright install`, if your error persists try the [playwright-python](https://github.com/microsoft/playwright-python) quickstart guide and diagnose issues from there.
 
 ## Quick Start Guide
 
-Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
+Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/main/examples) directory.
 
 **Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
 
 ```py
 from TikTokApi import TikTokApi
+import asyncio
+import os
 
-# Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api:
-    for trending_video in api.trending.videos(count=50):
-        # Prints the author's username of the trending video.
-        print(trending_video.author.username)
-```
+ms_token = os.environ.get("ms_token", None) # get your own ms_token from your cookies on tiktok.com
 
-**Note**: Jupyter (ipynb) only works on linux, see [microsoft/playwright-python #178](https://github.com/microsoft/playwright-python/issues/178)
+async def trending_videos():
+    async with TikTokApi() as api:
+        await api.create_sessions(ms_tokens=[ms_token], num_sessions=1, sleep_after=3)
+        async for video in api.trending.videos(count=30):
+            print(video)
+            print(video.as_dict)
 
-To run the example scripts from the repository root, make sure you use the `-m` option on python.
+if __name__ == "__main__":
+    asyncio.run(trending_videos())
+```
+
+To directly run the example scripts from the repository root, use the `-m` option on python.
 ```sh
 python -m examples.get_trending
 ```
 
-You can access the dictionary type of an object using `.as_dict`. On a video this may look like
-[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
-
-## Upgrading from V4 to V5
-
-All changes will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if you want more information.
+You can access the full data dictionary the object was created from with `.as_dict`. On a video this may look like
+[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
 
-### Motivation
+## Upgrading from V5 to V6
 
-This package has been difficult to maintain due to it's structure, difficult to work with since the user of the package must write parsing methods to extract information from dictionaries, more memory intensive than it needs to be (although this can be further improved), and in general just difficult to work with for new users. 
+All changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/releases/tag/V6.0.0) if you want more information.
 
-As a result, I've decided to at least attempt to remedy some of these issues, the biggest changes are that 
-1. The package has shifted to using classes for different TikTok objects resulting in an easier, higher-level programming experience.
-2. All methods that used to return a list of objects have been switched to using iterators, to hopefully decrease memory utilization for most users.
+### Changes & Motivations
 
+* Maintainability
+    * Was getting difficult to maintain with how TikTok was directly detecting HTTP requests.
+    * Switched to using a pool of **async** playwright pages to make it more difficult to detect, and hopefully easier to maintain in the future
+* Async
+    * It's been asked for a lot, and now fully async needed especially since the package is using a pool of playwright instances
+* User Flexibility
+    * Added a lot of function argument options that should be much more explicit than what was done previously.
+    * Hopefully if something is broken there's a workaround without having to modify the package itself (although if you do notice an issue please open an issue or submit a PR)
+* Documentation
+    * Goes with user flexibility a little bit but switched over to sphinx documentation for more explicit content
+    * If you run into an issue or are confused please open a github issue or submit a PR to fix documentation, it's always welcome! 🤠
 
 ### Upgrading Examples
 
-
-#### Accessing Dictionary on Objects (similar to V4)
-
-You'll probably need to use this beyond just for legacy support, since not all attributes are parsed out and attached
-to the different objects.
-
-You may want to use this as a workaround for legacy applications while you upgrade the rest of the app. I'd suggest that you do eventually upgrade to using the higher-level approach fully.
-```py
-user = api.user(username='therock')
-user.as_dict # -> dict of the user_object
-for video in user.videos():
-    video.as_dict # -> dict of TikTok's video object as found when requesting the videos endpoint
-```
-
-Here's a few more examples that help illustrate the differences in the flow of the usage of the package with V5.
-
-```py
-# V4
-api = TikTokApi.get_instance()
-trending_videos = api.by_trending()
-
-#V5.1
-with TikTokApi() as api: # .get_instance no longer exists
-    for trending_video in api.trending.videos():
-        # do something
-```
-
-Where in V4 you had to extract information yourself, the package now handles that for you. So it's much easier to do chained related function calls.
-```py
-# V4
-trending_videos = api.by_trending()
-for video in trending_videos:
-    # The dictionary responses are also different depending on what endpoint you got them from
-    # So, it's usually more painful than this to deal with
-    trending_user = api.get_user(id=video['author']['id'], secUid=video['author']['secUid'])
-
-
-# V5
-# This is more complicated than above, but it illustrates the simplified approach
-for trending_video in api.trending.videos():
-    user_stats = trending_video.author.info_full['stats']
-    if user_stats['followerCount'] >= 10000:
-        # maybe save the user in a database
-```
+The biggest change is that everything is now async. You can see above how you might want to call an async function in python as well as the examples directory for more examples.
```

#### html2text {}

```diff
@@ -4,121 +4,99 @@
 zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
 badge&logo=linkedin&logoColor=white&style=flat-square)](https://
 www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/
 static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/
 sponsors/davidteather) [![GitHub release (latest by date)](https://
 img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/
-davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/
-github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://
-github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [!
-[GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https:
-//github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https:/
-/pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://
-visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support
-Server](https://img.shields.io/discord/
+davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/
+license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/
+blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://
+pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/
+badge?page_id=davidteather.TikTok-Api) [![Support Server](https://
+img.shields.io/discord/
 783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://
-discord.gg/yyPhbfma6f) ## Sponsors These sponsors have paid to be placed here
-and beyond that I do not have any affiliation with them, the TikTokAPI package
-will always be free and open-source. If you wish to be a sponsor of this
-project check out my [GitHub sponsors page](https://github.com/sponsors/
-davidteather).
+discord.gg/yyPhbfma6f) This api is designed to **retrieve data** TikTok. It
+**can not be used post or upload** content to TikTok on the behalf of a user.
+It has **no support any user-authenticated routes**, if you can't access it
+while being logged out on their website you can't access it here. ## Sponsors
+These sponsors have paid to be placed here and beyond that I do not have any
+affiliation with them, the TikTokAPI package will always be free and open-
+source. If you wish to be a sponsor of this project check out my [GitHub
+sponsors page](https://github.com/sponsors/davidteather).
                                    [TikApi]
  TikAPI_is_a_paid_TikTok_API_service_providing_a_full_out-of-the-box_solution,
        making_life_easier_for_developers_â_trusted_by_500+_companies.
 
-                                  [Trendpop]
-  Trendpop_builds_software_to_help_creators_and_businesses_go_viral_on_social
-                               video_platforms.
-Excited_about_building_in_this_space?_We're_hiring_engineers_across_all_roles_-
-                shoot_us_a_message_at_founders@trendpop.social
-
-                                   [IH_logo]
-  TikTok_data_through_APIs,_providing_10+_Million_posts_/_day_to_the_largest
-                   Marketing_and_Social_listening_platforms.
+                               [Ensemble_Data]
+  Ensemble_Data_is_the_leading_API_provider_for_scraping_all_the_major_Social
+                                    Media.
+    We_provide_100+_Million_posts_/_day_to_the_largest_Marketing_and_Social
+                             listening_platforms.
 ## Table of Contents - [Documentation](#documentation) - [Getting Started]
 (#getting-started) - [How to Support The Project](#how-to-support-the-project)
 - [Installing](#installing) - [Common Issues](#common-issues) - [Quick Start
 Guide](#quick-start-guide) - [Examples](https://github.com/davidteather/TikTok-
-Api/tree/master/examples) [**Upgrading from V4 to V5**](#upgrading-from-v4-to-
-v5) ## Documentation You can find the full documentation [here](https://
-davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class]
-(https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where
-you'll probably spend most of your time. ## Getting Started To get started
-using this api follow the instructions below. **Note:** If you want to learn
-how to web scrape websites check my [free and open-source course for web
-scraping](https://github.com/davidteather/web-scraping-with-reverse-
-engineering) ### How to Support The Project * Star the repo ð * Consider
-[sponsoring](https://github.com/sponsors/davidteather) me on GitHub * Send me
-an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message
-telling me what you're using the API for, I really like hearing what people are
-using it for. * Submit PRs for issues :) ### Installing If you run into an
-issue please check the closed issues on the github, although feel free to re-
-open a new issue if you find an issue that's been closed for a few months. The
-codebase can and does run into similar issues as it has before, because TikTok
-changes things up. ```sh pip install TikTokApi python -m playwright install ```
-If you would prefer a video walk through of setting up this package [YouTube
-video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. If you want
-a quick video to listen for [TikTok Live](https://www.youtube.com/
-watch?v=307ijmA3_lc) events in python. #### Docker Installation Clone this
-repository onto a local machine (or just the Dockerfile since it installs
-TikTokApi from pip) then run the following commands. ```sh docker pull
-mcr.microsoft.com/playwright:focal docker build . -t tiktokapi:latest docker
-run -v TikTokApi --rm tiktokapi:latest python3 your_script.py ``` **Note** this
-assumes your script is named your_script.py and lives in the root of this
-directory. ### Common Issues Please don't open an issue if you're experiencing
-one of these just comment if the provided solution do not work for you. *
-**Browser Has no Attribute** - make sure you ran `python3 -m playwright
-install`, if your error persists try the [playwright-python](https://
-github.com/microsoft/playwright-python) quickstart guide and diagnose issues
-from there. ## Quick Start Guide Here's a quick bit of code to get the most
-recent trending videos on TikTok. There's more examples in the [examples]
-(https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
-**Note:** If you want to learn how to web scrape websites check my [free and
-open-source course for web scraping](https://github.com/davidteather/web-
-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi #
-Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api: for trending_video in api.trending.videos(count=50): #
-Prints the author's username of the trending video. print
-(trending_video.author.username) ``` **Note**: Jupyter (ipynb) only works on
-linux, see [microsoft/playwright-python #178](https://github.com/microsoft/
-playwright-python/issues/178) To run the example scripts from the repository
-root, make sure you use the `-m` option on python. ```sh python -
-m examples.get_trending ``` You can access the dictionary type of an object
-using `.as_dict`. On a video this may look like [this](https://gist.github.com/
-davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their
-structure from time to time so it's worth investigating the structure of the
-dictionary when you use this package. ## Upgrading from V4 to V5 All changes
-will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if
-you want more information. ### Motivation This package has been difficult to
-maintain due to it's structure, difficult to work with since the user of the
-package must write parsing methods to extract information from dictionaries,
-more memory intensive than it needs to be (although this can be further
-improved), and in general just difficult to work with for new users. As a
-result, I've decided to at least attempt to remedy some of these issues, the
-biggest changes are that 1. The package has shifted to using classes for
-different TikTok objects resulting in an easier, higher-level programming
-experience. 2. All methods that used to return a list of objects have been
-switched to using iterators, to hopefully decrease memory utilization for most
-users. ### Upgrading Examples #### Accessing Dictionary on Objects (similar to
-V4) You'll probably need to use this beyond just for legacy support, since not
-all attributes are parsed out and attached to the different objects. You may
-want to use this as a workaround for legacy applications while you upgrade the
-rest of the app. I'd suggest that you do eventually upgrade to using the
-higher-level approach fully. ```py user = api.user(username='therock')
-user.as_dict # -> dict of the user_object for video in user.videos():
-video.as_dict # -> dict of TikTok's video object as found when requesting the
-videos endpoint ``` Here's a few more examples that help illustrate the
-differences in the flow of the usage of the package with V5. ```py # V4 api =
-TikTokApi.get_instance() trending_videos = api.by_trending() #V5.1 with
-TikTokApi() as api: # .get_instance no longer exists for trending_video in
-api.trending.videos(): # do something ``` Where in V4 you had to extract
-information yourself, the package now handles that for you. So it's much easier
-to do chained related function calls. ```py # V4 trending_videos =
-api.by_trending() for video in trending_videos: # The dictionary responses are
-also different depending on what endpoint you got them from # So, it's usually
-more painful than this to deal with trending_user = api.get_user(id=video
-['author']['id'], secUid=video['author']['secUid']) # V5 # This is more
-complicated than above, but it illustrates the simplified approach for
-trending_video in api.trending.videos(): user_stats =
-trending_video.author.info_full['stats'] if user_stats['followerCount'] >=
-10000: # maybe save the user in a database ```
+Api/tree/main/examples) [**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
+## Documentation You can find the full documentation [here](https://
+davidteather.github.io/TikTok-Api) ## Getting Started To get started using this
+API follow the instructions below. **Note:** If you want to learn how to web
+scrape websites check my [free and open-source course for learning everything
+web scraping](https://github.com/davidteather/everything-web-scraping) ### How
+to Support The Project * Star the repo ð * Consider [sponsoring](https://
+github.com/sponsors/davidteather) me on GitHub * Send me an email or a
+[LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what
+you're using the API for, I really like hearing what people are using it for. *
+Submit PRs for issues :) ### Installing If you run into an issue please check
+the closed issues on the github, although feel free to re-open a new issue if
+you find an issue that's been closed for a few months. The codebase can and
+does run into similar issues as it has before, because TikTok changes things
+up. ```sh pip install TikTokApi python -m playwright install ``` If you would
+prefer a video walk through of setting up this package [YouTube video](https://
+www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date,
+installation is the same though) If you want a quick video to listen for
+[TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
+#### Docker Installation Clone this repository onto a local machine (or just
+the Dockerfile since it installs TikTokApi from pip) then run the following
+commands. ```sh docker pull mcr.microsoft.com/playwright:focal docker build . -
+t tiktokapi:latest docker run -v TikTokApi --rm tiktokapi:latest python3
+your_script.py ``` **Note** this assumes your script is named your_script.py
+and lives in the root of this directory. ### Common Issues Please don't open an
+issue if you're experiencing one of these just comment if the provided solution
+do not work for you. * **Browser Has no Attribute** - make sure you ran
+`python3 -m playwright install`, if your error persists try the [playwright-
+python](https://github.com/microsoft/playwright-python) quickstart guide and
+diagnose issues from there. ## Quick Start Guide Here's a quick bit of code to
+get the most recent trending videos on TikTok. There's more examples in the
+[examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
+directory. **Note:** If you want to learn how to web scrape websites check my
+[free and open-source course for web scraping](https://github.com/davidteather/
+web-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi
+import asyncio import os ms_token = os.environ.get("ms_token", None) # get your
+own ms_token from your cookies on tiktok.com async def trending_videos(): async
+with TikTokApi() as api: await api.create_sessions(ms_tokens=[ms_token],
+num_sessions=1, sleep_after=3) async for video in api.trending.videos
+(count=30): print(video) print(video.as_dict) if __name__ == "__main__":
+asyncio.run(trending_videos()) ``` To directly run the example scripts from the
+repository root, use the `-m` option on python. ```sh python -
+m examples.get_trending ``` You can access the full data dictionary the object
+was created from with `.as_dict`. On a video this may look like [this](https://
+gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes
+their structure from time to time so it's worth investigating the structure of
+the dictionary when you use this package. ## Upgrading from V5 to V6 All
+changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/
+releases/tag/V6.0.0) if you want more information. ### Changes & Motivations *
+Maintainability * Was getting difficult to maintain with how TikTok was
+directly detecting HTTP requests. * Switched to using a pool of **async**
+playwright pages to make it more difficult to detect, and hopefully easier to
+maintain in the future * Async * It's been asked for a lot, and now fully async
+needed especially since the package is using a pool of playwright instances *
+User Flexibility * Added a lot of function argument options that should be much
+more explicit than what was done previously. * Hopefully if something is broken
+there's a workaround without having to modify the package itself (although if
+you do notice an issue please open an issue or submit a PR) * Documentation *
+Goes with user flexibility a little bit but switched over to sphinx
+documentation for more explicit content * If you run into an issue or are
+confused please open a github issue or submit a PR to fix documentation, it's
+always welcome! ð¤  ### Upgrading Examples The biggest change is that
+everything is now async. You can see above how you might want to call an async
+function in python as well as the examples directory for more examples.
```

### Comparing `TikTokApi-5.2.2/TikTokApi/api/comment.py` & `TikTokApi-6.0.0/TikTokApi/api/comment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from typing import ClassVar, Optional
-from typing import TYPE_CHECKING, ClassVar, Iterator, Optional
+from typing import TYPE_CHECKING, ClassVar, Optional
 
 if TYPE_CHECKING:
     from ..tiktok import TikTokApi
     from .user import User
 
 
 class Comment:
     """
     A TikTok Comment.
 
     Example Usage
-    ```py
-    for comment in video.comments:
-        print(comment.text)
-    ```
+        .. code-block:: python
+
+            for comment in video.comments:
+                print(comment.text)
+                print(comment.as_dict)
     """
 
     parent: ClassVar[TikTokApi]
 
     id: str
     """The id of the comment"""
     author: ClassVar[User]
@@ -34,29 +35,24 @@
 
     def __init__(self, data: Optional[dict] = None):
         if data is not None:
             self.as_dict = data
             self.__extract_from_data()
 
     def __extract_from_data(self):
+        data = self.as_dict
         self.id = self.as_dict["cid"]
         self.text = self.as_dict["text"]
 
         usr = self.as_dict["user"]
         self.author = self.parent.user(
             user_id=usr["uid"], username=usr["unique_id"], sec_uid=usr["sec_uid"]
         )
         self.likes_count = self.as_dict["digg_count"]
 
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
-        return f"TikTokApi.comment(comment_id='{self.id}', text='{self.text}')"
-
-    def __getattr__(self, name):
-        if name in ["as_dict"]:
-            self.as_dict = self.info()
-            self.__extract_from_data()
-            return self.__getattribute__(name)
-
-        raise AttributeError(f"{name} doesn't exist on TikTokApi.api.Comment")
+        id = getattr(self, "id", None)
+        text = getattr(self, "text", None)
+        return f"TikTokApi.comment(comment_id='{id}', text='{text}')"
```

### Comparing `TikTokApi-5.2.2/TikTokApi/api/hashtag.py` & `TikTokApi-6.0.0/TikTokApi/api/hashtag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
-import logging
-
-from urllib.parse import urlencode
 from ..exceptions import *
 
 from typing import TYPE_CHECKING, ClassVar, Iterator, Optional
 
 if TYPE_CHECKING:
     from ..tiktok import TikTokApi
     from .video import Video
 
 
 class Hashtag:
     """
     A TikTok Hashtag/Challenge.
 
     Example Usage
-    ```py
-    hashtag = api.hashtag(name='funny')
-    ```
+        .. code-block:: python
+
+            hashtag = api.hashtag(name='funny')
+            async for video in hashtag.videos():
+                print(video.id)
     """
 
     parent: ClassVar[TikTokApi]
 
     id: Optional[str]
     """The ID of the hashtag"""
     name: Optional[str]
@@ -45,104 +44,124 @@
         if id is not None:
             self.id = id
 
         if data is not None:
             self.as_dict = data
             self.__extract_from_data()
 
-    def info(self, **kwargs) -> dict:
-        """
-        Returns TikTok's dictionary representation of the hashtag object.
-        """
-        return self.info_full(**kwargs)["challengeInfo"]["challenge"]
-
-    def info_full(self, **kwargs) -> dict:
+    async def info(self, **kwargs) -> dict:
         """
         Returns all information sent by TikTok related to this hashtag.
 
         Example Usage
-        ```py
-        hashtag_data = api.hashtag(name='funny').info_full()
-        ```
-        """
-        processed = self.parent._process_kwargs(kwargs)
-        kwargs["custom_device_id"] = processed.device_id
-
-        if self.name is not None:
-            query = {"challengeName": self.name}
-        elif self.id is not None:
-            query = {"challengeId": self.id}
-        else:
-            self.parent.logger.warning("Malformed Hashtag Object")
-            return {}
+            .. code-block:: python
+
+                hashtag = api.hashtag(name='funny')
+                hashtag_data = await hashtag.info()
+        """
+        if not self.name:
+            raise TypeError(
+                "You must provide the name when creating this class to use this method."
+            )
 
-        path = "api/challenge/detail/?{}&{}".format(
-            self.parent._add_url_params(), urlencode(query)
+        url_params = {
+            "challengeName": self.name,
+            "msToken": kwargs.get("ms_token"),
+        }
+
+        resp = await self.parent.make_request(
+            url="https://www.tiktok.com/api/challenge/detail/",
+            params=url_params,
+            headers=kwargs.get("headers"),
+            session_index=kwargs.get("session_index"),
         )
 
-        data = self.parent.get_data(path, **kwargs)
+        if resp is None:
+            raise InvalidResponseException(resp, "TikTok returned an invalid response.")
+
+        self.as_dict = resp
+        self.__extract_from_data()
+        return resp
 
-        if data["challengeInfo"].get("challenge") is None:
-            raise NotFoundException("Challenge {} does not exist".format(self.name))
+    async def videos(self, count=30, cursor=0, **kwargs) -> Iterator[Video]:
+        """
+        Returns TikTok videos that have this hashtag in the caption.
 
-        return data
+        Args:
+            count (int): The amount of videos you want returned.
+            cursor (int): The the offset of videos from 0 you want to get.
 
-    def videos(self, count=30, offset=0, **kwargs) -> Iterator[Video]:
-        """Returns a dictionary listing TikToks with a specific hashtag.
+        Returns:
+            async iterator/generator: Yields TikTokApi.video objects.
 
-        - Parameters:
-            - count (int): The amount of videos you want returned.
-            - offset (int): The the offset of videos from 0 you want to get.
+        Raises:
+            InvalidResponseException: If TikTok returns an invalid response, or one we don't understand.
 
-        Example Usage
-        ```py
-        for video in api.hashtag(name='funny').videos():
-            # do something
-        ```
-        """
-        cursor = offset
-        page_size = 30
-        while cursor - offset < count:
-            query = {
-                "aid": 1988,
-                "count": page_size,
+        Example Usage:
+            .. code-block:: python
+
+                async for video in api.hashtag(name='funny').videos():
+                    # do something
+        """
+
+        id = getattr(self, "id", None)
+        if id is None:
+            await self.info(**kwargs)
+
+        found = 0
+        while found < count:
+            params = {
                 "challengeID": self.id,
+                "count": 30,
                 "cursor": cursor,
             }
-            path = "api/challenge/item_list/?{}".format(urlencode(query))
-            res = self.parent.get_data_no_sig(path, subdomain="us", **kwargs)
-            for result in res.get("itemList", []):
-                yield self.parent.video(data=result)
-            if not res.get("hasMore", False):
-                self.parent.logger.info(
-                    "TikTok isn't sending more TikToks beyond this point."
+
+            resp = await self.parent.make_request(
+                url="https://www.tiktok.com/api/challenge/item_list/",
+                params=params,
+                headers=kwargs.get("headers"),
+                session_index=kwargs.get("session_index"),
+            )
+
+            if resp is None:
+                raise InvalidResponseException(
+                    resp, "TikTok returned an invalid response."
                 )
+
+            for video in resp.get("itemList", []):
+                yield self.parent.video(data=video)
+                found += 1
+
+            if not resp.get("hasMore", False):
                 return
-            cursor = int(res["cursor"])
+
+            cursor = resp.get("cursor")
 
     def __extract_from_data(self):
         data = self.as_dict
         keys = data.keys()
 
         if "title" in keys:
             self.id = data["id"]
             self.name = data["title"]
 
-        if None in (self.name, self.id):
+        if "challengeInfo" in keys:
+            if "challenge" in data["challengeInfo"]:
+                self.id = data["challengeInfo"]["challenge"]["id"]
+                self.name = data["challengeInfo"]["challenge"]["title"]
+                self.split_name = data["challengeInfo"]["challenge"].get("splitTitle")
+
+            if "stats" in data["challengeInfo"]:
+                self.stats = data["challengeInfo"]["stats"]
+
+        id = getattr(self, "id", None)
+        name = getattr(self, "name", None)
+        if None in (id, name):
             Hashtag.parent.logger.error(
                 f"Failed to create Hashtag with data: {data}\nwhich has keys {data.keys()}"
             )
 
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
-        return f"TikTokApi.hashtag(id='{self.id}', name='{self.name}')"
-
-    def __getattr__(self, name):
-        # TODO: Maybe switch to using @property instead
-        if name in ["id", "name", "as_dict"]:
-            self.as_dict = self.info()
-            self.__extract_from_data()
-            return self.__getattribute__(name)
-
-        raise AttributeError(f"{name} doesn't exist on TikTokApi.api.Hashtag")
+        return f"TikTokApi.hashtag(id='{getattr(self, 'id', None)}', name='{getattr(self, 'name', None)}')"
```

### Comparing `TikTokApi-5.2.2/TikTokApi/api/search.py` & `TikTokApi-6.0.0/TikTokApi/api/search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,106 @@
 from __future__ import annotations
-
 from urllib.parse import urlencode
-
-from typing import TYPE_CHECKING, Iterator, Type
-
+from typing import TYPE_CHECKING, Iterator
 from .user import User
-from .sound import Sound
-from .hashtag import Hashtag
-from .video import Video
+from ..exceptions import InvalidResponseException
 
 if TYPE_CHECKING:
     from ..tiktok import TikTokApi
 
-import requests
-
 
 class Search:
-    """Contains static methods about searching."""
+    """Contains static methods about searching TikTok for a phrase."""
 
     parent: TikTokApi
 
     @staticmethod
-    def videos(search_term, count=28, offset=0, **kwargs) -> Iterator[Video]:
+    async def users(search_term, count=10, cursor=0, **kwargs) -> Iterator[User]:
         """
-        Searches for Videos
+        Searches for users.
 
-        - Parameters:
-            - search_term (str): The phrase you want to search for.
-            - count (int): The amount of videos you want returned.
-            - offset (int): The offset of videos from your data you want returned.
-
-        Example Usage
-        ```py
-        for video in api.search.videos('therock'):
-            # do something
-        ```
-        """
-        return Search.search_type(
-            search_term, "item", count=count, offset=offset, **kwargs
-        )
+        Note: Your ms_token needs to have done a search before for this to work.
 
-    @staticmethod
-    def users(search_term, count=28, offset=0, **kwargs) -> Iterator[User]:
-        """
-        Searches for users using an alternate endpoint than Search.users
+        Args:
+            search_term (str): The phrase you want to search for.
+            count (int): The amount of users you want returned.
+
+        Returns:
+            async iterator/generator: Yields TikTokApi.user objects.
+
+        Raises:
+            InvalidResponseException: If TikTok returns an invalid response, or one we don't understand.
+
+        Example Usage:
+            .. code-block:: python
 
-        - Parameters:
-            - search_term (str): The phrase you want to search for.
-            - count (int): The amount of videos you want returned.
-
-        Example Usage
-        ```py
-        for user in api.search.users_alternate('therock'):
-            # do something
-        ```
+                async for user in api.search.users('david teather'):
+                    # do something
         """
-        return Search.search_type(
-            search_term, "user", count=count, offset=offset, **kwargs
-        )
+        async for user in Search.search_type(
+            search_term, "user", count=count, cursor=cursor, **kwargs
+        ):
+            yield user
 
     @staticmethod
-    def search_type(search_term, obj_type, count=28, offset=0, **kwargs) -> Iterator:
+    async def search_type(
+        search_term, obj_type, count=10, cursor=0, **kwargs
+    ) -> Iterator:
         """
-        Searches for users using an alternate endpoint than Search.users
+        Searches for a specific type of object. But you shouldn't use this directly, use the other methods.
 
-        - Parameters:
-            - search_term (str): The phrase you want to search for.
-            - count (int): The amount of videos you want returned.
-            - obj_type (str): user | item
+        Note: Your ms_token needs to have done a search before for this to work.
+        Note: Currently only supports searching for users, other endpoints require auth.
 
-        Just use .video & .users
-        ```
-        """
-        processed = Search.parent._process_kwargs(kwargs)
-        kwargs["custom_device_id"] = processed.device_id
+        Args:
+            search_term (str): The phrase you want to search for.
+            obj_type (str): The type of object you want to search for (user)
+            count (int): The amount of users you want returned.
+            cursor (int): The the offset of users from 0 you want to get.
+
+        Returns:
+            async iterator/generator: Yields TikTokApi.video objects.
+
+        Raises:
+            InvalidResponseException: If TikTok returns an invalid response, or one we don't understand.
 
-        cursor = offset
+        Example Usage:
+            .. code-block:: python
 
-        spawn = requests.head(
-            "https://www.tiktok.com",
-            proxies=Search.parent._format_proxy(processed.proxy),
-            **Search.parent._requests_extra_kwargs
-        )
-        ttwid = spawn.cookies["ttwid"]
-
-        # For some reason when <= it can be off by one.
-        while cursor - offset <= count:
-            query = {
+                async for user in api.search.search_type('david teather', 'user'):
+                    # do something
+        """
+        found = 0
+        while found < count:
+            params = {
                 "keyword": search_term,
                 "cursor": cursor,
-                "app_language": Search.parent._language,
+                "from_page": "search",
+                "web_search_code": """{"tiktok":{"client_params_x":{"search_engine":{"ies_mt_user_live_video_card_use_libra":1,"mt_search_general_user_live_card":1}},"search_server":{}}}""",
             }
-            path = "api/search/{}/full/?{}&{}".format(
-                obj_type, Search.parent._add_url_params(), urlencode(query)
-            )
 
-            if obj_type == "user":
-                subdomain = "www"
-            elif obj_type == "item":
-                subdomain = "us"
-            else:
-                raise TypeError("invalid obj_type")
-
-            api_response = Search.parent.get_data(
-                path, subdomain=subdomain, ttwid=ttwid, **kwargs
+            resp = await Search.parent.make_request(
+                url=f"https://www.tiktok.com/api/search/{obj_type}/full/",
+                params=params,
+                headers=kwargs.get("headers"),
+                session_index=kwargs.get("session_index"),
             )
 
-            # When I move to 3.10+ support make this a match switch.
-            for result in api_response.get("user_list", []):
-                yield User(data=result)
-
-            for result in api_response.get("item_list", []):
-                yield Video(data=result)
-
-            if api_response.get("has_more", 0) == 0:
-                Search.parent.logger.info(
-                    "TikTok is not sending videos beyond this point."
+            if resp is None:
+                raise InvalidResponseException(
+                    resp, "TikTok returned an invalid response."
                 )
+
+            if obj_type == "user":
+                for user in resp.get("user_list", []):
+                    sec_uid = user.get("user_info").get("sec_uid")
+                    uid = user.get("user_info").get("user_id")
+                    username = user.get("user_info").get("unique_id")
+                    yield Search.parent.user(
+                        sec_uid=sec_uid, user_id=uid, username=username
+                    )
+                    found += 1
+
+            if not resp.get("has_more", False):
                 return
 
-            cursor = int(api_response.get("cursor", cursor))
+            cursor = resp.get("cursor")
```

### Comparing `TikTokApi-5.2.2/TikTokApi/api/video.py` & `TikTokApi-6.0.0/TikTokApi/api/user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,203 +1,185 @@
 from __future__ import annotations
-
-from urllib.parse import urlencode
-from ..helpers import extract_video_id_from_url
 from typing import TYPE_CHECKING, ClassVar, Iterator, Optional
-from datetime import datetime
-import requests
+from ..exceptions import InvalidResponseException
 
 if TYPE_CHECKING:
     from ..tiktok import TikTokApi
-    from .user import User
-    from .sound import Sound
-    from .hashtag import Hashtag
-    from .comment import Comment
+    from .video import Video
 
 
-class Video:
+class User:
     """
-    A TikTok Video class
+    A TikTok User.
+
+    Example Usage:
+        .. code-block:: python
 
-    Example Usage
-    ```py
-    video = api.video(id='7041997751718137094')
-    ```
+            user = api.user(username='therock')
     """
 
     parent: ClassVar[TikTokApi]
 
-    id: Optional[str]
-    """TikTok's ID of the Video"""
-    create_time: Optional[datetime]
-    """The creation time of the Video"""
-    stats: Optional[dict]
-    """TikTok's stats of the Video"""
-    author: Optional[User]
-    """The User who created the Video"""
-    sound: Optional[Sound]
-    """The Sound that is associated with the Video"""
-    hashtags: Optional[list[Hashtag]]
-    """A List of Hashtags on the Video"""
+    user_id: str
+    """The  ID of the user."""
+    sec_uid: str
+    """The sec UID of the user."""
+    username: str
+    """The username of the user."""
     as_dict: dict
-    """The raw data associated with this Video."""
+    """The raw data associated with this user."""
 
     def __init__(
         self,
-        id: Optional[str] = None,
-        url: Optional[str] = None,
+        username: Optional[str] = None,
+        user_id: Optional[str] = None,
+        sec_uid: Optional[str] = None,
         data: Optional[dict] = None,
     ):
         """
-        You must provide the id or a valid url, else this will fail.
+        You must provide the username or (user_id and sec_uid) otherwise this
+        will not function correctly.
         """
-        self.id = id
+        self.__update_id_sec_uid_username(user_id, sec_uid, username)
         if data is not None:
             self.as_dict = data
             self.__extract_from_data()
-        elif url is not None:
-            self.id = extract_video_id_from_url(
-                url, headers={"user-agent": self.parent._user_agent}
-            )
 
-        if self.id is None:
-            raise TypeError("You must provide id or url parameter.")
-
-    def info(self, **kwargs) -> dict:
+    async def info(self, **kwargs) -> dict:
         """
-        Returns a dictionary of TikTok's Video object.
+        Returns a dictionary of information associated with this User.
 
-        Example Usage
-        ```py
-        video_data = api.video(id='7041997751718137094').info()
-        ```
-        """
-        return self.info_full(**kwargs)["itemInfo"]["itemStruct"]
+        Returns:
+            dict: A dictionary of information associated with this User.
 
-    def info_full(self, **kwargs) -> dict:
-        """
-        Returns a dictionary of all data associated with a TikTok Video.
+        Raises:
+            InvalidResponseException: If TikTok returns an invalid response, or one we don't understand.
+
+        Example Usage:
+            .. code-block:: python
 
-        Example Usage
-        ```py
-        video_data = api.video(id='7041997751718137094').info_full()
-        ```
+                user_data = await api.user(username='therock').info()
         """
-        processed = self.parent._process_kwargs(kwargs)
-        kwargs["custom_device_id"] = processed.device_id
 
-        device_id = kwargs.get("custom_device_id", None)
-        query = {
-            "itemId": self.id,
+        username = getattr(self, "username", None)
+        if not username:
+            raise TypeError(
+                "You must provide the username when creating this class to use this method."
+            )
+
+        sec_uid = getattr(self, "sec_uid", None)
+        url_params = {
+            "secUid": sec_uid if sec_uid is not None else "",
+            "uniqueId": username,
+            "msToken": kwargs.get("ms_token"),
         }
-        path = "api/item/detail/?{}&{}".format(
-            self.parent._add_url_params(), urlencode(query)
+
+        resp = await self.parent.make_request(
+            url="https://www.tiktok.com/api/user/detail/",
+            params=url_params,
+            headers=kwargs.get("headers"),
+            session_index=kwargs.get("session_index"),
         )
-        return self.parent.get_data(path, **kwargs)
 
-    def bytes(self, **kwargs) -> bytes:
-        """
-        Returns the bytes of a TikTok Video.
+        if resp is None:
+            raise InvalidResponseException(resp, "TikTok returned an invalid response.")
 
-        Example Usage
-        ```py
-        video_bytes = api.video(id='7041997751718137094').bytes()
+        self.as_dict = resp
+        self.__extract_from_data()
+        return resp
 
-        # Saving The Video
-        with open('saved_video.mp4', 'wb') as output:
-            output.write(video_bytes)
-        ```
+    async def videos(self, count=30, cursor=0, **kwargs) -> Iterator[Video]:
         """
-        processed = self.parent._process_kwargs(kwargs)
-        kwargs["custom_device_id"] = processed.device_id
+        Returns a user's videos.
 
-        video_data = self.info(**kwargs)
-        download_url = video_data["video"]["playAddr"]
+        Args:
+            count (int): The amount of videos you want returned.
+            cursor (int): The the offset of videos from 0 you want to get.
 
-        return self.parent.get_bytes(url=download_url, **kwargs)
+        Returns:
+            async iterator/generator: Yields TikTokApi.video objects.
 
-    def __extract_from_data(self) -> None:
-        data = self.as_dict
-        keys = data.keys()
-
-        if "author" in keys:
-            self.id = data["id"]
-            self.create_time = datetime.fromtimestamp(data["createTime"])
-            self.stats = data["stats"]
-            self.author = self.parent.user(data=data["author"])
-            self.sound = self.parent.sound(data=data["music"])
-
-            self.hashtags = [
-                self.parent.hashtag(data=hashtag)
-                for hashtag in data.get("challenges", [])
-            ]
-
-        if self.id is None:
-            Video.parent.logger.error(
-                f"Failed to create Video with data: {data}\nwhich has keys {data.keys()}"
-            )
+        Raises:
+            InvalidResponseException: If TikTok returns an invalid response, or one we don't understand.
 
-    def comments(self, count=20, offset=0, **kwargs) -> Iterator[Comment]:
-        """
-        Returns Comments from the video
+        Example Usage:
+            .. code-block:: python
 
-        - Parameters:
-            - count (int): The amount of videos you want returned.
-            - offset (int): The offset you want to check comments of
+                async for video in api.user(username="davidteathercodes").videos():
+                    # do something
         """
+        sec_uid = getattr(self, "sec_uid", None)
+        if sec_uid is None or sec_uid == "":
+            await self.info(**kwargs)
 
-        processed = Video.parent._process_kwargs(kwargs)
-        kwargs["custom_device_id"] = processed.device_id
-        cursor = offset
-
-        spawn = requests.head(
-            "https://www.tiktok.com",
-            proxies=Video.parent._format_proxy(processed.proxy),
-            **Video.parent._requests_extra_kwargs,
-        )
-        ttwid = spawn.cookies["ttwid"]
-
-        while cursor - offset <= count:
-            query = {
-                "aweme_id": self.id,
+        found = 0
+        while found < count:
+            params = {
+                "secUid": self.sec_uid,
+                "count": 35,
                 "cursor": cursor,
-                "app_language": Video.parent._language,
-                "count": 30,
             }
-            path = "api/comment/list/?{}&{}".format(
-                Video.parent._add_url_params(), urlencode(query)
-            )
 
-            api_response = Video.parent.get_data(
-                path, subdomain="www", ttwid=ttwid, **kwargs
+            resp = await self.parent.make_request(
+                url="https://www.tiktok.com/api/post/item_list/",
+                params=params,
+                headers=kwargs.get("headers"),
+                session_index=kwargs.get("session_index"),
             )
 
-            for comment_data in api_response.get("comments", []):
-                yield self.parent.comment(data=comment_data)
-
-            if api_response.get("has_more", 0) == 0:
-                Video.parent.logger.info(
-                    "TikTok is not sending comments beyond this point."
+            if resp is None:
+                raise InvalidResponseException(
+                    resp, "TikTok returned an invalid response."
                 )
+
+            for video in resp.get("itemList", []):
+                yield self.parent.video(data=video)
+                found += 1
+
+            if not resp.get("hasMore", False):
                 return
 
-            cursor = int(api_response.get("cursor", cursor))
+            cursor = resp.get("cursor")
 
-    def __repr__(self):
-        return self.__str__()
+    def liked(self, count: int = 30, cursor: int = 0, **kwargs) -> Iterator[Video]:
+        """
+        Returns a dictionary listing TikToks that a given a user has liked.
 
-    def __str__(self):
-        return f"TikTokApi.video(id='{self.id}')"
+        TODO: Not currently implemented
+        """
+        raise NotImplementedError
 
-    def __getattr__(self, name):
-        # Handle author, sound, hashtags, as_dict
-        if name in ["author", "sound", "hashtags", "stats", "create_time", "as_dict"]:
-            self.as_dict = self.info()
-            self.__extract_from_data()
-            return self.__getattribute__(name)
+    def __extract_from_data(self):
+        data = self.as_dict
+        keys = data.keys()
+
+        if "userInfo" in keys:
+            self.__update_id_sec_uid_username(
+                data["userInfo"]["user"]["id"],
+                data["userInfo"]["user"]["secUid"],
+                data["userInfo"]["user"]["uniqueId"],
+            )
+        else:
+            self.__update_id_sec_uid_username(
+                data["id"],
+                data["secUid"],
+                data["uniqueId"],
+            )
+
+        if None in (self.username, self.user_id, self.sec_uid):
+            User.parent.logger.error(
+                f"Failed to create User with data: {data}\nwhich has keys {data.keys()}"
+            )
 
-        if name in ["comments"]:
-            # Requires a different request to produce the comments
-            self.__extract_comments()
-            return self.__getattribute__(name)
+    def __update_id_sec_uid_username(self, id, sec_uid, username):
+        self.user_id = id
+        self.sec_uid = sec_uid
+        self.username = username
 
-        raise AttributeError(f"{name} doesn't exist on TikTokApi.api.Video")
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        username = getattr(self, "username", None)
+        user_id = getattr(self, "user_id", None)
+        sec_uid = getattr(self, "sec_uid", None)
+        return f"TikTokApi.user(username='{username}', user_id='{user_id}', sec_uid='{sec_uid}')"
```

### Comparing `TikTokApi-5.2.2/TikTokApi/exceptions.py` & `TikTokApi-6.0.0/TikTokApi/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 class TikTokException(Exception):
     """Generic exception that all other TikTok errors are children of."""
 
-    def __init__(self, error_code, raw_response, message):
+    def __init__(self, raw_response, message, error_code=None):
         self.error_code = error_code
         self.raw_response = raw_response
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
-        return f'{self.error_code} -> {self.message}'
+        return f"{self.error_code} -> {self.message}"
 
 
 class CaptchaException(TikTokException):
     """TikTok is showing captcha"""
 
 
 class NotFoundException(TikTokException):
@@ -24,12 +24,12 @@
 
 
 class SoundRemovedException(TikTokException):
     """This TikTok sound has no id from being removed by TikTok."""
 
 
 class InvalidJSONException(TikTokException):
-    """TikTok returned invalid JSON."""
+    """TikTok returned invalid JSON.""" 
 
 
-class NotAvailableException(TikTokException):
-    """The requested object is not available in this region."""
+class InvalidResponseException(TikTokException):
+    """The response from TikTok was invalid."""
```

### Comparing `TikTokApi-5.2.2/TikTokApi.egg-info/PKG-INFO` & `TikTokApi-6.0.0/TikTokApi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,76 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 5.2.2
+Version: 6.0.0
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
+Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
-Download-URL: https://github.com/davidteather/TikTok-Api/tarball/master
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 
 # Unofficial TikTok API in Python
 
 This is an unofficial api wrapper for TikTok.com in python. With this api you are able to call most trending and fetch specific user information as well as much more.
 
- [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+ [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/davidteather)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support Server](https://img.shields.io/discord/783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://discord.gg/yyPhbfma6f)
+
+This api is designed to **retrieve data** TikTok. It **can not be used post or upload** content to TikTok on the behalf of a user. It has **no support any user-authenticated routes**, if you can't access it while being logged out on their website you can't access it here.
 
 ## Sponsors
 These sponsors have paid to be placed here and beyond that I do not have any affiliation with them, the TikTokAPI package will always be free and open-source. If you wish to be a sponsor of this project check out my [GitHub sponsors page](https://github.com/sponsors/davidteather).
 
 <div align="center">
-    <p>
     <a href="https://tikapi.io/?ref=davidteather" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/tikapi.png" width="100" alt="TikApi">
-			</div>
-			<b></b>
-			<div>
-				<b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
-			</div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://trendpop.social/?ref=github-davidteather-tiktokapi" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/master/imgs/trendpop.png" width="100" alt="Trendpop">
-			</div>
-			<div>
-				Trendpop builds software to help creators and businesses go viral on social video platforms.
-			</div>
-            <div>
-                <sub>
-                    Excited about building in this space?
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi">
-                        <sub>We're hiring engineers across all roles</sub>
-                    </a>
-                    <a href="https://trendpop.social/careers?ref=github-davidteather-tiktokapi" target="_blank">
-                    <sub>- shoot us a message at </sub>
-                    </a>
-                    <a href="mailto:founders@trendpop.social" target="_blank">
-                    <sub><code>founders@trendpop.social</code></sub>
-                    </a>
-                </sub>
-            </div>
-		</a>
-    </p>
-</div>
-
-<br>
-
-<div align="center">
-    <p>
-    <a href="https://influencerhunters.com/docs.html?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_t" target="_blank">
-			<div>
-				<img src="https://raw.githubusercontent.com/andrearama/TikTok-Api/master/imgs/IH_LOGO.png" width="100" alt="IH_logo">
-			</div>
-			<b></b>
-			<div>
-				TikTok data through APIs, providing 10+ Million posts / day to the largest Marketing and Social listening platforms.
-			</div>
-		</a>
-    </p>
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/tikapi.png" width="100" alt="TikApi">
+        <div>
+            <b>TikAPI</b> is a paid TikTok API service providing a full out-of-the-box solution, making life easier for developers — trusted by 500+ companies.
+        </div>
+    </a>
+    <br>
+    <a href="https://www.ensembledata.com/?utm_source=github&utm_medium=githubpage&utm_campaign=david_thea_github&utm_id=david_thea_github" target="_blank">
+        <img src="https://raw.githubusercontent.com/davidteather/TikTok-Api/main/imgs/EnsembleData.png" width="100" alt="Ensemble Data">
+        <b></b>
+        <div>
+            <b>Ensemble Data</b> is the leading API provider for scraping all the major Social Media. <br> We provide 100+ Million posts / day to the largest Marketing and Social listening platforms.
+        </div>
+	</a>
 </div>
 
 ## Table of Contents
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
     - [How to Support The Project](#how-to-support-the-project)
     - [Installing](#installing)
     - [Common Issues](#common-issues)
 - [Quick Start Guide](#quick-start-guide)
-    - [Examples](https://github.com/davidteather/TikTok-Api/tree/master/examples)
+    - [Examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
 
-[**Upgrading from V4 to V5**](#upgrading-from-v4-to-v5)
+[**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
 
 ## Documentation
 
-You can find the full documentation [here](https://davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class](https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where you'll probably spend most of your time.
+You can find the full documentation [here](https://davidteather.github.io/TikTok-Api)
 ## Getting Started
 
-To get started using this api follow the instructions below.
+To get started using this API follow the instructions below.
 
-**Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
+**Note:** If you want to learn how to web scrape websites check my [free and open-source course for learning everything web scraping](https://github.com/davidteather/everything-web-scraping)
 
 ### How to Support The Project
 * Star the repo 😎
 * Consider [sponsoring](https://github.com/sponsors/davidteather) me on GitHub
 * Send me an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what you're using the API for, I really like hearing what people are using it for.
 * Submit PRs for issues :)
 
@@ -120,15 +78,15 @@
 
 If you run into an issue please check the closed issues on the github, although feel free to re-open a new issue if you find an issue that's been closed for a few months. The codebase can and does run into similar issues as it has before, because TikTok changes things up.
 
 ```sh
 pip install TikTokApi
 python -m playwright install
 ```
-If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that.
+If you would prefer a video walk through of setting up this package [YouTube video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date, installation is the same though)
 
 If you want a quick video to listen for [TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
 
 #### Docker Installation
 
 Clone this repository onto a local machine (or just the Dockerfile since it installs TikTokApi from pip) then run the following commands.
 
@@ -144,92 +102,58 @@
 
 Please don't open an issue if you're experiencing one of these just comment if the provided solution do not work for you.
 
 * **Browser Has no Attribute** - make sure you ran `python3 -m playwright install`, if your error persists try the [playwright-python](https://github.com/microsoft/playwright-python) quickstart guide and diagnose issues from there.
 
 ## Quick Start Guide
 
-Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
+Here's a quick bit of code to get the most recent trending videos on TikTok. There's more examples in the [examples](https://github.com/davidteather/TikTok-Api/tree/main/examples) directory.
 
 **Note:** If you want to learn how to web scrape websites check my [free and open-source course for web scraping](https://github.com/davidteather/web-scraping-with-reverse-engineering)
 
 ```py
 from TikTokApi import TikTokApi
+import asyncio
+import os
 
-# Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api:
-    for trending_video in api.trending.videos(count=50):
-        # Prints the author's username of the trending video.
-        print(trending_video.author.username)
-```
+ms_token = os.environ.get("ms_token", None) # get your own ms_token from your cookies on tiktok.com
+
+async def trending_videos():
+    async with TikTokApi() as api:
+        await api.create_sessions(ms_tokens=[ms_token], num_sessions=1, sleep_after=3)
+        async for video in api.trending.videos(count=30):
+            print(video)
+            print(video.as_dict)
 
-**Note**: Jupyter (ipynb) only works on linux, see [microsoft/playwright-python #178](https://github.com/microsoft/playwright-python/issues/178)
+if __name__ == "__main__":
+    asyncio.run(trending_videos())
+```
 
-To run the example scripts from the repository root, make sure you use the `-m` option on python.
+To directly run the example scripts from the repository root, use the `-m` option on python.
 ```sh
 python -m examples.get_trending
 ```
 
-You can access the dictionary type of an object using `.as_dict`. On a video this may look like
-[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
-
-## Upgrading from V4 to V5
+You can access the full data dictionary the object was created from with `.as_dict`. On a video this may look like
+[this](https://gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes their structure from time to time so it's worth investigating the structure of the dictionary when you use this package.
 
-All changes will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if you want more information.
+## Upgrading from V5 to V6
 
-### Motivation
+All changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/releases/tag/V6.0.0) if you want more information.
 
-This package has been difficult to maintain due to it's structure, difficult to work with since the user of the package must write parsing methods to extract information from dictionaries, more memory intensive than it needs to be (although this can be further improved), and in general just difficult to work with for new users. 
-
-As a result, I've decided to at least attempt to remedy some of these issues, the biggest changes are that 
-1. The package has shifted to using classes for different TikTok objects resulting in an easier, higher-level programming experience.
-2. All methods that used to return a list of objects have been switched to using iterators, to hopefully decrease memory utilization for most users.
+### Changes & Motivations
 
+* Maintainability
+    * Was getting difficult to maintain with how TikTok was directly detecting HTTP requests.
+    * Switched to using a pool of **async** playwright pages to make it more difficult to detect, and hopefully easier to maintain in the future
+* Async
+    * It's been asked for a lot, and now fully async needed especially since the package is using a pool of playwright instances
+* User Flexibility
+    * Added a lot of function argument options that should be much more explicit than what was done previously.
+    * Hopefully if something is broken there's a workaround without having to modify the package itself (although if you do notice an issue please open an issue or submit a PR)
+* Documentation
+    * Goes with user flexibility a little bit but switched over to sphinx documentation for more explicit content
+    * If you run into an issue or are confused please open a github issue or submit a PR to fix documentation, it's always welcome! 🤠
 
 ### Upgrading Examples
 
-
-#### Accessing Dictionary on Objects (similar to V4)
-
-You'll probably need to use this beyond just for legacy support, since not all attributes are parsed out and attached
-to the different objects.
-
-You may want to use this as a workaround for legacy applications while you upgrade the rest of the app. I'd suggest that you do eventually upgrade to using the higher-level approach fully.
-```py
-user = api.user(username='therock')
-user.as_dict # -> dict of the user_object
-for video in user.videos():
-    video.as_dict # -> dict of TikTok's video object as found when requesting the videos endpoint
-```
-
-Here's a few more examples that help illustrate the differences in the flow of the usage of the package with V5.
-
-```py
-# V4
-api = TikTokApi.get_instance()
-trending_videos = api.by_trending()
-
-#V5.1
-with TikTokApi() as api: # .get_instance no longer exists
-    for trending_video in api.trending.videos():
-        # do something
-```
-
-Where in V4 you had to extract information yourself, the package now handles that for you. So it's much easier to do chained related function calls.
-```py
-# V4
-trending_videos = api.by_trending()
-for video in trending_videos:
-    # The dictionary responses are also different depending on what endpoint you got them from
-    # So, it's usually more painful than this to deal with
-    trending_user = api.get_user(id=video['author']['id'], secUid=video['author']['secUid'])
-
-
-# V5
-# This is more complicated than above, but it illustrates the simplified approach
-for trending_video in api.trending.videos():
-    user_stats = trending_video.author.info_full['stats']
-    if user_stats['followerCount'] >= 10000:
-        # maybe save the user in a database
-```
-
-
+The biggest change is that everything is now async. You can see above how you might want to call an async function in python as well as the examples directory for more examples.
```

#### html2text {}

```diff
@@ -1,135 +1,113 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 5.2.2 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.0 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
-tiktok-api Author: David Teather Author-email: contact.davidteather@gmail.com
-License: MIT Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
-master Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
-File: LICENSE License-File: LICENSE.txt # Unofficial TikTok API in Python This
-is an unofficial api wrapper for TikTok.com in python. With this api you are
-able to call most trending and fetch specific user information as well as much
-more. [![DOI](https://zenodo.org/badge/188710490.svg)](https://zenodo.org/
-badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/badge/LinkedIn-
-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)]
-(https://www.linkedin.com/in/davidteather/) [![Sponsor Me](https://
-img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://
-github.com/sponsors/davidteather) [![GitHub release (latest by date)](https://
+tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
+main Author: David Teather Author-email: contact.davidteather@gmail.com
+License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE License-File: LICENSE.txt # Unofficial TikTok API in
+Python This is an unofficial api wrapper for TikTok.com in python. With this
+api you are able to call most trending and fetch specific user information as
+well as much more. [![DOI](https://zenodo.org/badge/188710490.svg)](https://
+zenodo.org/badge/latestdoi/188710490) [![LinkedIn](https://img.shields.io/
+badge/LinkedIn-0077B5?style=for-the-
+badge&logo=linkedin&logoColor=white&style=flat-square)](https://
+www.linkedin.com/in/davidteather/) [![Sponsor Me](https://img.shields.io/
+static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/
+sponsors/davidteather) [![GitHub release (latest by date)](https://
 img.shields.io/github/v/release/davidteather/TikTok-Api)](https://github.com/
-davidteather/TikTok-Api/releases) [![Build Status](https://img.shields.io/
-github/workflow/status/davidteather/tiktok-api/TikTokApi%20CI/master)](https://
-github.com/davidteather/TikTok-Api/actions/workflows/package-test.yml) [!
-[GitHub](https://img.shields.io/github/license/davidteather/TikTok-Api)](https:
-//github.com/davidteather/TikTok-Api/blob/master/LICENSE) [![Downloads](https:/
-/pepy.tech/badge/tiktokapi)](https://pypi.org/project/TikTokApi/) ![](https://
-visitor-badge.laobi.icu/badge?page_id=davidteather.TikTok-Api) [![Support
-Server](https://img.shields.io/discord/
+davidteather/TikTok-Api/releases) [![GitHub](https://img.shields.io/github/
+license/davidteather/TikTok-Api)](https://github.com/davidteather/TikTok-Api/
+blob/main/LICENSE) [![Downloads](https://pepy.tech/badge/tiktokapi)](https://
+pypi.org/project/TikTokApi/) ![](https://visitor-badge.laobi.icu/
+badge?page_id=davidteather.TikTok-Api) [![Support Server](https://
+img.shields.io/discord/
 783108952111579166.svg?color=7289da&logo=discord&style=flat-square)](https://
-discord.gg/yyPhbfma6f) ## Sponsors These sponsors have paid to be placed here
-and beyond that I do not have any affiliation with them, the TikTokAPI package
-will always be free and open-source. If you wish to be a sponsor of this
-project check out my [GitHub sponsors page](https://github.com/sponsors/
-davidteather).
+discord.gg/yyPhbfma6f) This api is designed to **retrieve data** TikTok. It
+**can not be used post or upload** content to TikTok on the behalf of a user.
+It has **no support any user-authenticated routes**, if you can't access it
+while being logged out on their website you can't access it here. ## Sponsors
+These sponsors have paid to be placed here and beyond that I do not have any
+affiliation with them, the TikTokAPI package will always be free and open-
+source. If you wish to be a sponsor of this project check out my [GitHub
+sponsors page](https://github.com/sponsors/davidteather).
                                    [TikApi]
  TikAPI_is_a_paid_TikTok_API_service_providing_a_full_out-of-the-box_solution,
        making_life_easier_for_developers_â_trusted_by_500+_companies.
 
-                                  [Trendpop]
-  Trendpop_builds_software_to_help_creators_and_businesses_go_viral_on_social
-                               video_platforms.
-Excited_about_building_in_this_space?_We're_hiring_engineers_across_all_roles_-
-                shoot_us_a_message_at_founders@trendpop.social
-
-                                   [IH_logo]
-  TikTok_data_through_APIs,_providing_10+_Million_posts_/_day_to_the_largest
-                   Marketing_and_Social_listening_platforms.
+                               [Ensemble_Data]
+  Ensemble_Data_is_the_leading_API_provider_for_scraping_all_the_major_Social
+                                    Media.
+    We_provide_100+_Million_posts_/_day_to_the_largest_Marketing_and_Social
+                             listening_platforms.
 ## Table of Contents - [Documentation](#documentation) - [Getting Started]
 (#getting-started) - [How to Support The Project](#how-to-support-the-project)
 - [Installing](#installing) - [Common Issues](#common-issues) - [Quick Start
 Guide](#quick-start-guide) - [Examples](https://github.com/davidteather/TikTok-
-Api/tree/master/examples) [**Upgrading from V4 to V5**](#upgrading-from-v4-to-
-v5) ## Documentation You can find the full documentation [here](https://
-davidteather.github.io/TikTok-Api/docs/TikTokApi.html), the [TikTokApi Class]
-(https://davidteather.github.io/TikTok-Api/docs/TikTokApi/tiktok.html) is where
-you'll probably spend most of your time. ## Getting Started To get started
-using this api follow the instructions below. **Note:** If you want to learn
-how to web scrape websites check my [free and open-source course for web
-scraping](https://github.com/davidteather/web-scraping-with-reverse-
-engineering) ### How to Support The Project * Star the repo ð * Consider
-[sponsoring](https://github.com/sponsors/davidteather) me on GitHub * Send me
-an email or a [LinkedIn](https://www.linkedin.com/in/davidteather/) message
-telling me what you're using the API for, I really like hearing what people are
-using it for. * Submit PRs for issues :) ### Installing If you run into an
-issue please check the closed issues on the github, although feel free to re-
-open a new issue if you find an issue that's been closed for a few months. The
-codebase can and does run into similar issues as it has before, because TikTok
-changes things up. ```sh pip install TikTokApi python -m playwright install ```
-If you would prefer a video walk through of setting up this package [YouTube
-video](https://www.youtube.com/watch?v=-uCt1x8kINQ) just for that. If you want
-a quick video to listen for [TikTok Live](https://www.youtube.com/
-watch?v=307ijmA3_lc) events in python. #### Docker Installation Clone this
-repository onto a local machine (or just the Dockerfile since it installs
-TikTokApi from pip) then run the following commands. ```sh docker pull
-mcr.microsoft.com/playwright:focal docker build . -t tiktokapi:latest docker
-run -v TikTokApi --rm tiktokapi:latest python3 your_script.py ``` **Note** this
-assumes your script is named your_script.py and lives in the root of this
-directory. ### Common Issues Please don't open an issue if you're experiencing
-one of these just comment if the provided solution do not work for you. *
-**Browser Has no Attribute** - make sure you ran `python3 -m playwright
-install`, if your error persists try the [playwright-python](https://
-github.com/microsoft/playwright-python) quickstart guide and diagnose issues
-from there. ## Quick Start Guide Here's a quick bit of code to get the most
-recent trending videos on TikTok. There's more examples in the [examples]
-(https://github.com/davidteather/TikTok-Api/tree/master/examples) directory.
-**Note:** If you want to learn how to web scrape websites check my [free and
-open-source course for web scraping](https://github.com/davidteather/web-
-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi #
-Watch https://www.youtube.com/watch?v=-uCt1x8kINQ for a brief setup tutorial
-with TikTokApi() as api: for trending_video in api.trending.videos(count=50): #
-Prints the author's username of the trending video. print
-(trending_video.author.username) ``` **Note**: Jupyter (ipynb) only works on
-linux, see [microsoft/playwright-python #178](https://github.com/microsoft/
-playwright-python/issues/178) To run the example scripts from the repository
-root, make sure you use the `-m` option on python. ```sh python -
-m examples.get_trending ``` You can access the dictionary type of an object
-using `.as_dict`. On a video this may look like [this](https://gist.github.com/
-davidteather/7c30780bbc30772ba11ec9e0b909e99d), although TikTok changes their
-structure from time to time so it's worth investigating the structure of the
-dictionary when you use this package. ## Upgrading from V4 to V5 All changes
-will be noted on [#803](https://github.com/davidteather/TikTok-Api/pull/803) if
-you want more information. ### Motivation This package has been difficult to
-maintain due to it's structure, difficult to work with since the user of the
-package must write parsing methods to extract information from dictionaries,
-more memory intensive than it needs to be (although this can be further
-improved), and in general just difficult to work with for new users. As a
-result, I've decided to at least attempt to remedy some of these issues, the
-biggest changes are that 1. The package has shifted to using classes for
-different TikTok objects resulting in an easier, higher-level programming
-experience. 2. All methods that used to return a list of objects have been
-switched to using iterators, to hopefully decrease memory utilization for most
-users. ### Upgrading Examples #### Accessing Dictionary on Objects (similar to
-V4) You'll probably need to use this beyond just for legacy support, since not
-all attributes are parsed out and attached to the different objects. You may
-want to use this as a workaround for legacy applications while you upgrade the
-rest of the app. I'd suggest that you do eventually upgrade to using the
-higher-level approach fully. ```py user = api.user(username='therock')
-user.as_dict # -> dict of the user_object for video in user.videos():
-video.as_dict # -> dict of TikTok's video object as found when requesting the
-videos endpoint ``` Here's a few more examples that help illustrate the
-differences in the flow of the usage of the package with V5. ```py # V4 api =
-TikTokApi.get_instance() trending_videos = api.by_trending() #V5.1 with
-TikTokApi() as api: # .get_instance no longer exists for trending_video in
-api.trending.videos(): # do something ``` Where in V4 you had to extract
-information yourself, the package now handles that for you. So it's much easier
-to do chained related function calls. ```py # V4 trending_videos =
-api.by_trending() for video in trending_videos: # The dictionary responses are
-also different depending on what endpoint you got them from # So, it's usually
-more painful than this to deal with trending_user = api.get_user(id=video
-['author']['id'], secUid=video['author']['secUid']) # V5 # This is more
-complicated than above, but it illustrates the simplified approach for
-trending_video in api.trending.videos(): user_stats =
-trending_video.author.info_full['stats'] if user_stats['followerCount'] >=
-10000: # maybe save the user in a database ```
+Api/tree/main/examples) [**Upgrading from V5 to V6**](#upgrading-from-v5-to-v6)
+## Documentation You can find the full documentation [here](https://
+davidteather.github.io/TikTok-Api) ## Getting Started To get started using this
+API follow the instructions below. **Note:** If you want to learn how to web
+scrape websites check my [free and open-source course for learning everything
+web scraping](https://github.com/davidteather/everything-web-scraping) ### How
+to Support The Project * Star the repo ð * Consider [sponsoring](https://
+github.com/sponsors/davidteather) me on GitHub * Send me an email or a
+[LinkedIn](https://www.linkedin.com/in/davidteather/) message telling me what
+you're using the API for, I really like hearing what people are using it for. *
+Submit PRs for issues :) ### Installing If you run into an issue please check
+the closed issues on the github, although feel free to re-open a new issue if
+you find an issue that's been closed for a few months. The codebase can and
+does run into similar issues as it has before, because TikTok changes things
+up. ```sh pip install TikTokApi python -m playwright install ``` If you would
+prefer a video walk through of setting up this package [YouTube video](https://
+www.youtube.com/watch?v=-uCt1x8kINQ) just for that. (is a version out of date,
+installation is the same though) If you want a quick video to listen for
+[TikTok Live](https://www.youtube.com/watch?v=307ijmA3_lc) events in python.
+#### Docker Installation Clone this repository onto a local machine (or just
+the Dockerfile since it installs TikTokApi from pip) then run the following
+commands. ```sh docker pull mcr.microsoft.com/playwright:focal docker build . -
+t tiktokapi:latest docker run -v TikTokApi --rm tiktokapi:latest python3
+your_script.py ``` **Note** this assumes your script is named your_script.py
+and lives in the root of this directory. ### Common Issues Please don't open an
+issue if you're experiencing one of these just comment if the provided solution
+do not work for you. * **Browser Has no Attribute** - make sure you ran
+`python3 -m playwright install`, if your error persists try the [playwright-
+python](https://github.com/microsoft/playwright-python) quickstart guide and
+diagnose issues from there. ## Quick Start Guide Here's a quick bit of code to
+get the most recent trending videos on TikTok. There's more examples in the
+[examples](https://github.com/davidteather/TikTok-Api/tree/main/examples)
+directory. **Note:** If you want to learn how to web scrape websites check my
+[free and open-source course for web scraping](https://github.com/davidteather/
+web-scraping-with-reverse-engineering) ```py from TikTokApi import TikTokApi
+import asyncio import os ms_token = os.environ.get("ms_token", None) # get your
+own ms_token from your cookies on tiktok.com async def trending_videos(): async
+with TikTokApi() as api: await api.create_sessions(ms_tokens=[ms_token],
+num_sessions=1, sleep_after=3) async for video in api.trending.videos
+(count=30): print(video) print(video.as_dict) if __name__ == "__main__":
+asyncio.run(trending_videos()) ``` To directly run the example scripts from the
+repository root, use the `-m` option on python. ```sh python -
+m examples.get_trending ``` You can access the full data dictionary the object
+was created from with `.as_dict`. On a video this may look like [this](https://
+gist.github.com/davidteather/7c30780bbc30772ba11ec9e0b909e99d). TikTok changes
+their structure from time to time so it's worth investigating the structure of
+the dictionary when you use this package. ## Upgrading from V5 to V6 All
+changes will be noted on [V6.0.0](https://github.com/davidteather/TikTok-Api/
+releases/tag/V6.0.0) if you want more information. ### Changes & Motivations *
+Maintainability * Was getting difficult to maintain with how TikTok was
+directly detecting HTTP requests. * Switched to using a pool of **async**
+playwright pages to make it more difficult to detect, and hopefully easier to
+maintain in the future * Async * It's been asked for a lot, and now fully async
+needed especially since the package is using a pool of playwright instances *
+User Flexibility * Added a lot of function argument options that should be much
+more explicit than what was done previously. * Hopefully if something is broken
+there's a workaround without having to modify the package itself (although if
+you do notice an issue please open an issue or submit a PR) * Documentation *
+Goes with user flexibility a little bit but switched over to sphinx
+documentation for more explicit content * If you run into an issue or are
+confused please open a github issue or submit a PR to fix documentation, it's
+always welcome! ð¤  ### Upgrading Examples The biggest change is that
+everything is now async. You can see above how you might want to call an async
+function in python as well as the examples directory for more examples.
```

### Comparing `TikTokApi-5.2.2/setup.py` & `TikTokApi-6.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TikTokApi",
     packages=setuptools.find_packages(),
-    version="5.2.2",
+    version="6.0.0",
     license="MIT",
     description="The Unofficial TikTok API Wrapper in Python 3.",
     author="David Teather",
     author_email="contact.davidteather@gmail.com",
     url="https://github.com/davidteather/tiktok-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    download_url="https://github.com/davidteather/TikTok-Api/tarball/master",
+    download_url="https://github.com/davidteather/TikTok-Api/tarball/main",
     keywords=["tiktok", "python3", "api", "unofficial", "tiktok-api", "tiktok api"],
     install_requires=["requests", "playwright"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `TikTokApi-5.2.2/tests/test_integration.py` & `TikTokApi-6.0.0/tests/test_integration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from TikTokApi import TikTokApi
 import os
+import pytest
 
+ms_token = os.environ.get("ms_token", None)
 
-def test_video_attributes():
-    with TikTokApi(custom_verify_fp=os.environ.get("verifyFp", None)) as api:
+
+@pytest.mark.asyncio
+async def test_hashtag_videos():
+    async with TikTokApi() as api:
+        await api.create_sessions(ms_tokens=[ms_token], num_sessions=1, sleep_after=3)
         tag_name = "funny"
-        for video in api.hashtag(name=tag_name).videos():
-            # Test hashtags on video.
+        count = 0
+        async for video in api.hashtag(name=tag_name).videos(count=1):
+            count += 1
             tag_included = False
             for tag in video.hashtags:
                 if tag.name == tag_name:
                     tag_included = True
 
             assert tag_included
 
@@ -18,7 +24,9 @@
             assert video.sound is not None
             assert video.sound.id is not None
 
             # Test author.
             assert video.author is not None
             assert video.author.user_id is not None
             assert video.author.sec_uid is not None
+
+        assert count > 0
```

