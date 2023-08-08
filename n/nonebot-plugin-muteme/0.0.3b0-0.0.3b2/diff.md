# Comparing `tmp/nonebot-plugin-muteme-0.0.3b0.tar.gz` & `tmp/nonebot-plugin-muteme-0.0.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-muteme-0.0.3b0.tar", last modified: Mon Aug  7 16:32:05 2023, max compression
+gzip compressed data, was "nonebot-plugin-muteme-0.0.3b2.tar", last modified: Tue Aug  8 03:50:12 2023, max compression
```

## Comparing `nonebot-plugin-muteme-0.0.3b0.tar` & `nonebot-plugin-muteme-0.0.3b2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:32:05.941664 nonebot-plugin-muteme-0.0.3b0/
--rw-r--r--   0 root         (0) root         (0)      292 2023-08-07 16:32:05.941664 nonebot-plugin-muteme-0.0.3b0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1911 2023-08-07 16:14:19.000000 nonebot-plugin-muteme-0.0.3b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:32:05.937664 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme/
--rw-r--r--   0 root         (0) root         (0)     1773 2023-08-07 16:30:34.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:32:05.937664 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      292 2023-08-07 16:32:05.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2023-08-07 16:32:05.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 16:32:05.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-08-07 16:32:05.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-07 16:32:05.000000 nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      930 2023-08-07 16:30:34.000000 nonebot-plugin-muteme-0.0.3b0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 16:32:05.941664 nonebot-plugin-muteme-0.0.3b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      390 2023-08-07 16:29:37.000000 nonebot-plugin-muteme-0.0.3b0/setup.py
+drwxrwxrwx   0 nightwind  (1000) nightwind  (1000)        0 2023-08-08 03:50:12.811143 nonebot-plugin-muteme-0.0.3b2/
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)    35149 2023-08-08 03:35:46.000000 nonebot-plugin-muteme-0.0.3b2/LICENSE
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)      332 2023-08-08 03:50:12.810963 nonebot-plugin-muteme-0.0.3b2/PKG-INFO
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)     1911 2023-08-08 03:35:46.000000 nonebot-plugin-muteme-0.0.3b2/README.md
+drwxrwxrwx   0 nightwind  (1000) nightwind  (1000)        0 2023-08-08 03:50:12.808837 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme/
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)     1773 2023-08-08 03:45:40.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme/__init__.py
+drwxrwxrwx   0 nightwind  (1000) nightwind  (1000)        0 2023-08-08 03:50:12.810555 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)      332 2023-08-08 03:50:12.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/PKG-INFO
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)      299 2023-08-08 03:50:12.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)        1 2023-08-08 03:50:12.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)       32 2023-08-08 03:50:12.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/requires.txt
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)       22 2023-08-08 03:50:12.000000 nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme.egg-info/top_level.txt
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)      928 2023-08-08 03:46:56.000000 nonebot-plugin-muteme-0.0.3b2/pyproject.toml
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)       38 2023-08-08 03:50:12.811207 nonebot-plugin-muteme-0.0.3b2/setup.cfg
+-rwxrwxrwx   0 nightwind  (1000) nightwind  (1000)      417 2023-08-08 03:49:43.000000 nonebot-plugin-muteme-0.0.3b2/setup.py
```

### Comparing `nonebot-plugin-muteme-0.0.3b0/README.md` & `nonebot-plugin-muteme-0.0.3b2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-muteme-0.0.3b0/nonebot_plugin_muteme/__init__.py` & `nonebot-plugin-muteme-0.0.3b2/nonebot_plugin_muteme/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 
 help_text = f"""
 muteme
 """.strip()
 
 __plugin_meta__ = PluginMetadata(
-    name = 'nonebot-plugin-muteme',
+    name = 'Muteme(我禁我自己)',
     description = '高仿@能干辉的muteme,我禁我自己',
     usage = help_text ,
     type="application",
     homepage="https://github.com/XTxiaoting14332/nonebot-plugin-muteme",
     extra={
         "unique_name": "muteme",
         "example": """muteme""",
         "author": "NightWind",
-        "version": "0.0.3-beta",
+        "version": "0.0.3-b2",
     },
 )
 
 muteme = on_regex('^muteme$')
 
 
 @muteme.handle()
```

### Comparing `nonebot-plugin-muteme-0.0.3b0/pyproject.toml` & `nonebot-plugin-muteme-0.0.3b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-muteme"
-version = "0.0.3-beta"
+version = "0.0.3-b2"
 description = "适用于nonebot2 v11的禁言自己插件 高仿 @能干辉 的muteme"
 authors = ["【夜风】NightWind <2125714976@qq.com>"]
 license = "GPL-3"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_muteme"}]
 homepage = "https://hub.xb6868.com/XTxiaoting14332/nonebot-plugin-muteme"
 repository = "https://hub.xb6868.com/XTxiaoting14332/nonebot-plugin-muteme"
```

