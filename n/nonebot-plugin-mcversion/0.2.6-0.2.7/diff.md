# Comparing `tmp/nonebot-plugin-mcversion-0.2.6.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.2.6.tar", last modified: Mon Aug  7 07:32:07 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.7.tar", last modified: Mon Aug  7 08:33:55 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.2.6.tar` & `nonebot-plugin-mcversion-0.2.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/LICENSE
--rw-r--r--   0        0        0     1931 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/README.md
--rw-r--r--   0        0        0     2831 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      642 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 08:33:42.037154 nonebot-plugin-mcversion-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1931 2023-08-07 08:33:42.037154 nonebot-plugin-mcversion-0.2.7/README.md
+-rw-r--r--   0        0        0     2812 2023-08-07 08:33:42.037154 nonebot-plugin-mcversion-0.2.7/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-07 08:33:42.037154 nonebot-plugin-mcversion-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.7/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.2.6/LICENSE` & `nonebot-plugin-mcversion-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.6/README.md` & `nonebot-plugin-mcversion-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.6/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.2.7/nonebot_plugin_mcversion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="MC版本更新检测",
     description="一个用于检测MC最新版本的插件",
     usage="使用mcver以获取最新版本号",
-    config=Config,
     type="application",
     homepage="https://github.com/CN171-1/nonebot_plugin_mcversion",
 )
 
 # 导入必要的库
 import os
 import httpx
```

### Comparing `nonebot-plugin-mcversion-0.2.6/pyproject.toml` & `nonebot-plugin-mcversion-0.2.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.2.6"
+version = "0.2.7"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
@@ -14,15 +14,15 @@
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-Homepage = "https://github.com/CN171-1/nonebot-plugin-mcversion"
-Repository = "https://github.com/CN171-1/nonebot-plugin-mcversion"
+Homepage = "https://github.com/CN171-1/nonebot_plugin_mcversion"
+Repository = "https://github.com/CN171-1/nonebot_plugin_mcversion"
 
 [build-system]
 requires = [
     "pdm-pep517>=0.12.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `nonebot-plugin-mcversion-0.2.6/PKG-INFO` & `nonebot-plugin-mcversion-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.2.6
+Version: 0.2.7
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
-Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
-Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
+Project-URL: Homepage, https://github.com/CN171-1/nonebot_plugin_mcversion
+Project-URL: Repository, https://github.com/CN171-1/nonebot_plugin_mcversion
 Description-Content-Type: text/markdown
 
 # README
 <!--
 <div align="center">
   <img src="your_project_logo.png" alt="Logo" width="200">
 </div>
```

