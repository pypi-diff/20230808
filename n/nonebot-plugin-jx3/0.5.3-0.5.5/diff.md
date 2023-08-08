# Comparing `tmp/nonebot_plugin_jx3-0.5.3.tar.gz` & `tmp/nonebot_plugin_jx3-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_jx3-0.5.3.tar", last modified: Tue Aug  8 18:57:41 2023, max compression
+gzip compressed data, was "nonebot_plugin_jx3-0.5.5.tar", max compression
```

## Comparing `nonebot_plugin_jx3-0.5.3.tar` & `nonebot_plugin_jx3-0.5.5.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 18:57:41.527110 nonebot_plugin_jx3-0.5.3/
--rw-rw-rw-   0        0        0     1084 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     2901 2023-08-08 18:57:41.527110 nonebot_plugin_jx3-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2591 2023-08-08 17:52:17.000000 nonebot_plugin_jx3-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 18:57:41.516081 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/
--rw-rw-rw-   0        0        0    13540 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/bind.py
--rw-rw-rw-   0        0        0      204 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/config.py
--rw-rw-rw-   0        0        0     3735 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/subscribe.py
--rw-rw-rw-   0        0        0     2900 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/userdefine.py
--rw-rw-rw-   0        0        0    11457 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/websocket_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-08 18:57:41.526109 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3.egg-info/
--rw-rw-rw-   0        0        0     2901 2023-08-08 18:57:41.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-08-08 18:57:41.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 18:57:41.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-08 18:57:41.000000 nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2023-08-08 18:57:35.000000 nonebot_plugin_jx3-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 18:57:41.527110 nonebot_plugin_jx3-0.5.3/setup.cfg
+-rw-r--r--   0        0        0     1084 2023-08-08 17:41:12.049341 nonebot_plugin_jx3-0.5.5/LICENSE
+-rw-r--r--   0        0        0    13540 2023-08-08 17:41:12.050342 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/__init__.py
+-rw-r--r--   0        0        0     1722 2023-08-08 17:41:12.050342 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/bind.py
+-rw-r--r--   0        0        0      204 2023-08-08 17:41:12.051462 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/config.py
+-rw-r--r--   0        0        0     3735 2023-08-08 17:41:12.718224 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/subscribe.py
+-rw-r--r--   0        0        0     2900 2023-08-08 17:41:12.718224 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/userdefine.py
+-rw-r--r--   0        0        0    11457 2023-08-08 17:41:12.718224 nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/websocket_handler.py
+-rw-r--r--   0        0        0      562 2023-08-08 19:42:37.563880 nonebot_plugin_jx3-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2591 2023-08-08 17:52:17.014942 nonebot_plugin_jx3-0.5.5/README.md
+-rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 nonebot_plugin_jx3-0.5.5/PKG-INFO
```

### Comparing `nonebot_plugin_jx3-0.5.3/LICENSE` & `nonebot_plugin_jx3-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.3/PKG-INFO` & `nonebot_plugin_jx3-0.5.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_jx3
-Version: 0.5.3
-Summary: 一个nonebot2的jx3插件
-Author-email: fuyang <415276785@qq.com>
-Project-URL: Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_jx3 Version: 0.5.3 Summary:
-ä¸ä¸ªnonebot2çjx3æä»¶ Author-email: fuyang <415276785@qq.com> Project-URL:
-Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                # nonebot-plugin-jx3 _è¿æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼æä¾å¤ç§åè½å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ã_
                            [license] [pypi] [python]
 ## ð ä»ç» nonebot-plugin-jx3 æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼å®æä¾äºå¤ç§åè½ï¼ä¾å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ï¼ä¾å¦"818",
```

### Comparing `nonebot_plugin_jx3-0.5.3/README.md` & `nonebot_plugin_jx3-0.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,89 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-jx3
-
-_这是一个使用 NoneBot 框架编写的插件，提供多种功能如日常查询，预测，金价查询，鲜花，公告，沙盘，jjc，黑市，骚话，奇遇，招募以及多种消息推送功能。_
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/water/nonebot-plugin-jx3.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-jx3">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-jx3.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-
-## 📖 介绍
-
-nonebot-plugin-jx3 是一个使用 NoneBot 框架编写的插件，它提供了多种功能，例如日常查询，预测，金价查询，鲜花，公告，沙盘，jjc，黑市，骚话，奇遇，招募以及多种消息推送功能，例如"818", "开服", "新闻", "抓马", "扶摇", "诛恶", "阵营活动提醒", "攻防实况", "玄晶","奇遇","绝世奇遇" 等。
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-jx3
-
-</details>
-
-<details>
-<summary>手动安装</summary>
-将插件文件夹复制到你的 NoneBot 项目的 plugins 目录下。
-
-在你的 NoneBot 配置文件中，添加插件的导入路径，例如：
-
-nonebot.load_plugins("plugins.nonebot_plugin_jx3")
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| jx3api_key | 否 | 无 | jx3.api.com购买的key |
-| jx3_tuilan_ticket | 否 | 无 | 推栏ticket |
-| jx3wss_token| 否 | 无 | jx3.api.com购买的wss |
-| jx3_command_header | 否 | 无 | 指令的前缀，防止和其他插件冲突 |
-| jx3_bot_name | 是 | 无 | api生成图片用的名字 |
-
-第一步使用插件是要绑定服务器。例如：-绑定 绝代天骄
-
-一旦服务器是绑定的，就可以使用各种查询功能。通过-订阅，你可以查询能够订阅的功能。
-
-开发者:water
-
-qq:415276785
+Metadata-Version: 2.1
+Name: nonebot-plugin-jx3
+Version: 0.5.5
+Summary: 一个nonebot2的jx3插件
+Home-page: https://github.com/fuyang0811/nonebot-plugin-jx3.git
+License: MIT
+Author: water
+Author-email: 415276785@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: httpx (>=0.19.0,<0.20.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: tinydb (>=4.5.1,<5.0.0)
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-jx3
+
+_这是一个使用 NoneBot 框架编写的插件，提供多种功能如日常查询，预测，金价查询，鲜花，公告，沙盘，jjc，黑市，骚话，奇遇，招募以及多种消息推送功能。_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/water/nonebot-plugin-jx3.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-jx3">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-jx3.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+
+## 📖 介绍
+
+nonebot-plugin-jx3 是一个使用 NoneBot 框架编写的插件，它提供了多种功能，例如日常查询，预测，金价查询，鲜花，公告，沙盘，jjc，黑市，骚话，奇遇，招募以及多种消息推送功能，例如"818", "开服", "新闻", "抓马", "扶摇", "诛恶", "阵营活动提醒", "攻防实况", "玄晶","奇遇","绝世奇遇" 等。
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-jx3
+
+</details>
+
+<details>
+<summary>手动安装</summary>
+将插件文件夹复制到你的 NoneBot 项目的 plugins 目录下。
+
+在你的 NoneBot 配置文件中，添加插件的导入路径，例如：
+
+nonebot.load_plugins("plugins.nonebot_plugin_jx3")
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| jx3api_key | 否 | 无 | jx3.api.com购买的key |
+| jx3_tuilan_ticket | 否 | 无 | 推栏ticket |
+| jx3wss_token| 否 | 无 | jx3.api.com购买的wss |
+| jx3_command_header | 否 | 无 | 指令的前缀，防止和其他插件冲突 |
+| jx3_bot_name | 是 | 无 | api生成图片用的名字 |
+
+第一步使用插件是要绑定服务器。例如：-绑定 绝代天骄
+
+一旦服务器是绑定的，就可以使用各种查询功能。通过-订阅，你可以查询能够订阅的功能。
+
+开发者:water
+
+qq:415276785
+
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.5 Summary:
+ä¸ä¸ªnonebot2çjx3æä»¶ Home-page: https://github.com/fuyang0811/nonebot-
+plugin-jx3.git License: MIT Author: water Author-email: 415276785@qq.com
+Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-
+Dist: httpx (>=0.19.0,<0.20.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.0.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Requires-Dist:
+tinydb (>=4.5.1,<5.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                # nonebot-plugin-jx3 _è¿æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼æä¾å¤ç§åè½å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ã_
                            [license] [pypi] [python]
 ## ð ä»ç» nonebot-plugin-jx3 æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼å®æä¾äºå¤ç§åè½ï¼ä¾å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ï¼ä¾å¦"818",
```

### Comparing `nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/__init__.py` & `nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/bind.py` & `nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/subscribe.py` & `nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/userdefine.py` & `nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/userdefine.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.3/nonebot_plugin_jx3/websocket_handler.py` & `nonebot_plugin_jx3-0.5.5/nonebot_plugin_jx3/websocket_handler.py`

 * *Files identical despite different names*

