# Comparing `tmp/tsutils-8.0.5.tar.gz` & `tmp/tsutils-8.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsutils-8.0.5.tar", last modified: Fri May  5 02:29:01 2023, max compression
+gzip compressed data, was "tsutils-8.0.6.tar", last modified: Tue Aug  8 11:07:42 2023, max compression
```

## Comparing `tsutils-8.0.5.tar` & `tsutils-8.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.700374 tsutils-8.0.5/
--rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.5/LICENSE
--rw-r--r--   0 chasehult   (501) staff       (20)      618 2023-05-05 02:29:01.700239 tsutils-8.0.5/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.5/README.md
--rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-05-05 02:29:01.700409 tsutils-8.0.5/setup.cfg
--rw-r--r--   0 chasehult   (501) staff       (20)      789 2023-05-05 02:15:55.000000 tsutils-8.0.5/setup.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.692471 tsutils-8.0.5/tsutils/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3940 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/cog_mixins.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/cog_settings.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.695055 tsutils-8.0.5/tsutils/cogs/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/cogs/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/cogs/donations.py
--rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/cogs/globaladmin.py
--rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/cogs/userpreferences.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.5/tsutils/emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.5/tsutils/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/errors.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.5/tsutils/formatting.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.5/tsutils/helper_classes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3289 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/helper_functions.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.5/tsutils/json_utils.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.695816 tsutils-8.0.5/tsutils/menu/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/menu/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.5/tsutils/menu/closable_embed_base.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.696517 tsutils-8.0.5/tsutils/menu/components/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.5/tsutils/menu/components/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.5/tsutils/menu/components/config.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1291 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/menu/components/footers.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.5/tsutils/menu/components/panes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3332 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/menu/pad_view.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.5/tsutils/menu/simple_text.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.697268 tsutils-8.0.5/tsutils/menu/view/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.5/tsutils/menu/view/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.5/tsutils/menu/view/closable_embed.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.5/tsutils/menu/view/simple_text.py
--rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.5/tsutils/menu/view/view_state_base.py
--rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.5/tsutils/old_menu.py
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.5/tsutils/pad.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.698271 tsutils-8.0.5/tsutils/query_settings/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.5/tsutils/query_settings/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.5/tsutils/query_settings/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.5/tsutils/query_settings/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.5/tsutils/query_settings/query_settings.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.5/tsutils/time.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.699952 tsutils-8.0.5/tsutils/tsubaki/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.5/tsutils/tsubaki/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     4708 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/tsubaki/custom_emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3620 2023-03-14 02:42:07.000000 tsutils-8.0.5/tsutils/tsubaki/links.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2736 2023-05-04 15:15:12.000000 tsutils-8.0.5/tsutils/tsubaki/monster_header.py
--rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.5/tsutils/user_interaction.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-05 02:29:01.694603 tsutils-8.0.5/tsutils.egg-info/
--rw-r--r--   0 chasehult   (501) staff       (20)      618 2023-05-05 02:29:01.000000 tsutils-8.0.5/tsutils.egg-info/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-05-05 02:29:01.000000 tsutils-8.0.5/tsutils.egg-info/SOURCES.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-05-05 02:29:01.000000 tsutils-8.0.5/tsutils.egg-info/dependency_links.txt
--rw-r--r--   0 chasehult   (501) staff       (20)       60 2023-05-05 02:29:01.000000 tsutils-8.0.5/tsutils.egg-info/requires.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-05-05 02:29:01.000000 tsutils-8.0.5/tsutils.egg-info/top_level.txt
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.129166 tsutils-8.0.6/
+-rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.6/LICENSE
+-rw-r--r--   0 chasehult   (501) staff       (20)      618 2023-08-08 11:07:42.129065 tsutils-8.0.6/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.6/README.md
+-rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-08-08 11:07:42.129198 tsutils-8.0.6/setup.cfg
+-rw-r--r--   0 chasehult   (501) staff       (20)      789 2023-08-08 10:58:12.000000 tsutils-8.0.6/setup.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.124401 tsutils-8.0.6/tsutils/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3940 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/cog_mixins.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/cog_settings.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.125392 tsutils-8.0.6/tsutils/cogs/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/cogs/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/cogs/donations.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/cogs/globaladmin.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/cogs/userpreferences.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.6/tsutils/emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.6/tsutils/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/errors.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.6/tsutils/formatting.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.6/tsutils/helper_classes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3289 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/helper_functions.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.6/tsutils/json_utils.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.125976 tsutils-8.0.6/tsutils/menu/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/menu/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.6/tsutils/menu/closable_embed_base.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.126697 tsutils-8.0.6/tsutils/menu/components/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.6/tsutils/menu/components/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.6/tsutils/menu/components/config.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1291 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/menu/components/footers.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.6/tsutils/menu/components/panes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3332 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/menu/pad_view.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.6/tsutils/menu/simple_text.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.127338 tsutils-8.0.6/tsutils/menu/view/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.6/tsutils/menu/view/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.6/tsutils/menu/view/closable_embed.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.6/tsutils/menu/view/simple_text.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.6/tsutils/menu/view/view_state_base.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.6/tsutils/old_menu.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.6/tsutils/pad.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.128063 tsutils-8.0.6/tsutils/query_settings/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.6/tsutils/query_settings/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.6/tsutils/query_settings/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.6/tsutils/query_settings/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.6/tsutils/query_settings/query_settings.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.6/tsutils/time.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.128811 tsutils-8.0.6/tsutils/tsubaki/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.6/tsutils/tsubaki/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     4708 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/tsubaki/custom_emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     4087 2023-08-08 11:00:05.000000 tsutils-8.0.6/tsutils/tsubaki/links.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2736 2023-05-04 15:15:12.000000 tsutils-8.0.6/tsutils/tsubaki/monster_header.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.6/tsutils/user_interaction.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-08-08 11:07:42.124986 tsutils-8.0.6/tsutils.egg-info/
+-rw-r--r--   0 chasehult   (501) staff       (20)      618 2023-08-08 11:07:42.000000 tsutils-8.0.6/tsutils.egg-info/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-08-08 11:07:42.000000 tsutils-8.0.6/tsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-08-08 11:07:42.000000 tsutils-8.0.6/tsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)       60 2023-08-08 11:07:42.000000 tsutils-8.0.6/tsutils.egg-info/requires.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-08-08 11:07:42.000000 tsutils-8.0.6/tsutils.egg-info/top_level.txt
```

### Comparing `tsutils-8.0.5/LICENSE` & `tsutils-8.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/PKG-INFO` & `tsutils-8.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.5
+Version: 8.0.6
 Summary: A collection of helper commands for Red-DiscordBot
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPAD@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsutils-8.0.5/setup.py` & `tsutils-8.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsutils",
-    version="8.0.5",
+    version="8.0.6",
     author="The Tsubotki Team",
     author_email="69992611+TsubakiBotPAD@users.noreply.github.com",
     license="MIT",
     description="A collection of helper commands for Red-DiscordBot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `tsutils-8.0.5/tsutils/cog_mixins.py` & `tsutils-8.0.6/tsutils/cog_mixins.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/cog_settings.py` & `tsutils-8.0.6/tsutils/cog_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/cogs/donations.py` & `tsutils-8.0.6/tsutils/cogs/donations.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/cogs/globaladmin.py` & `tsutils-8.0.6/tsutils/cogs/globaladmin.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/cogs/userpreferences.py` & `tsutils-8.0.6/tsutils/cogs/userpreferences.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/converters.py` & `tsutils-8.0.6/tsutils/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/emoji.py` & `tsutils-8.0.6/tsutils/emoji.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/enums.py` & `tsutils-8.0.6/tsutils/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/errors.py` & `tsutils-8.0.6/tsutils/errors.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/formatting.py` & `tsutils-8.0.6/tsutils/formatting.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/helper_classes.py` & `tsutils-8.0.6/tsutils/helper_classes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/helper_functions.py` & `tsutils-8.0.6/tsutils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/json_utils.py` & `tsutils-8.0.6/tsutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/closable_embed_base.py` & `tsutils-8.0.6/tsutils/menu/closable_embed_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/components/config.py` & `tsutils-8.0.6/tsutils/menu/components/config.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/components/footers.py` & `tsutils-8.0.6/tsutils/menu/components/footers.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/components/panes.py` & `tsutils-8.0.6/tsutils/menu/components/panes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/pad_view.py` & `tsutils-8.0.6/tsutils/menu/pad_view.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/simple_text.py` & `tsutils-8.0.6/tsutils/menu/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/view/simple_text.py` & `tsutils-8.0.6/tsutils/menu/view/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/menu/view/view_state_base.py` & `tsutils-8.0.6/tsutils/menu/view/view_state_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/old_menu.py` & `tsutils-8.0.6/tsutils/old_menu.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/pad.py` & `tsutils-8.0.6/tsutils/pad.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/query_settings/converters.py` & `tsutils-8.0.6/tsutils/query_settings/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/query_settings/enums.py` & `tsutils-8.0.6/tsutils/query_settings/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/query_settings/query_settings.py` & `tsutils-8.0.6/tsutils/query_settings/query_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/time.py` & `tsutils-8.0.6/tsutils/time.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/tsubaki/custom_emoji.py` & `tsutils-8.0.6/tsutils/tsubaki/custom_emoji.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/tsubaki/links.py` & `tsutils-8.0.6/tsutils/tsubaki/links.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
 INFO_PDX_TEMPLATE = 'http://www.puzzledragonx.com/en/monster.asp?n={}'
 YT_SEARCH_TEMPLATE = 'https://www.youtube.com/results?search_query={}'
 SKYOZORA_TEMPLATE = 'http://pad.skyozora.com/pets/{}'
 ILMINA_TEMPLATE = 'https://ilmina.com/#/CARD/{}'
 PADINDEX_TEMPLATE = 'https://pad.chesterip.cc/{}'
 
+ID_CONFIG_SHEET_TEMPLATE = 'https://docs.google.com/spreadsheets/d/1EoZJ3w5xsXZ67kmarLE4vfrZSIIIAfj04HXeZVST3eY' \
+                           '/pub?gid={}&single=true&output=csv'
+
 
 class MonsterImage:
     @staticmethod
     def icon(idx: int, cachebreak: Optional[Union[str, int]] = None):
         if cachebreak is None:
             return ICON_TEMPLATE.format(idx) + REGULAR_SUFFIX
         return ICON_TEMPLATE.format(idx) + CACHEBREAK_SUFFIX.format(cachebreak)
@@ -100,7 +103,18 @@
         elif not m.on_jp:
             return MonsterLink.ilmina(m)
 
         if qs is None or qs.linktarget == MonsterLinkTarget.padindex:
             return MonsterLink.padindex(m)
         else:
             return MonsterLink.ilmina(m)
+
+
+class ConfigTab:
+    CARDNAME_OVERRIDE = 0
+    TREENAME_OVERRIDES = 2070615818
+    CARD_MODIFIER_OVERRIDE = 2089525837
+    TREE_MODIFIER_OVERRIDE = 1372419168
+    CONTENT_TOKEN_ALIAS = 1229125459
+    SERIES_OVERRIDES = 959933643
+    AWOKEN_SKILL = 1063132392
+    DUNGEONS = 1224404198
```

### Comparing `tsutils-8.0.5/tsutils/tsubaki/monster_header.py` & `tsutils-8.0.6/tsutils/tsubaki/monster_header.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils/user_interaction.py` & `tsutils-8.0.6/tsutils/user_interaction.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.5/tsutils.egg-info/PKG-INFO` & `tsutils-8.0.6/tsutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.5
+Version: 8.0.6
 Summary: A collection of helper commands for Red-DiscordBot
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPAD@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsutils-8.0.5/tsutils.egg-info/SOURCES.txt` & `tsutils-8.0.6/tsutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

