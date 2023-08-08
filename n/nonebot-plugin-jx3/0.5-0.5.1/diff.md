# Comparing `tmp/nonebot_plugin_jx3-0.5.tar.gz` & `tmp/nonebot_plugin_jx3-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_jx3-0.5.tar", last modified: Tue Aug  8 18:00:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_jx3-0.5.1.tar", last modified: Tue Aug  8 18:39:38 2023, max compression
```

## Comparing `nonebot_plugin_jx3-0.5.tar` & `nonebot_plugin_jx3-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 18:00:13.966634 nonebot_plugin_jx3-0.5/
--rw-rw-rw-   0        0        0     1084 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/LICENSE
--rw-rw-rw-   0        0        0     2899 2023-08-08 18:00:13.966634 nonebot_plugin_jx3-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2591 2023-08-08 17:52:17.000000 nonebot_plugin_jx3-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 18:00:13.948515 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/
--rw-rw-rw-   0        0        0    13540 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/bind.py
--rw-rw-rw-   0        0        0      204 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/config.py
--rw-rw-rw-   0        0        0     3735 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/subscribe.py
--rw-rw-rw-   0        0        0     2900 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/userdefine.py
--rw-rw-rw-   0        0        0    11457 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/websocket_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-08 18:00:13.965626 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/
--rw-rw-rw-   0        0        0     2899 2023-08-08 18:00:13.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-08-08 18:00:13.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 18:00:13.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-08-08 18:00:13.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-08 18:00:13.000000 nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      446 2023-08-08 18:00:07.000000 nonebot_plugin_jx3-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 18:00:13.966634 nonebot_plugin_jx3-0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 18:39:38.972463 nonebot_plugin_jx3-0.5.1/
+-rw-rw-rw-   0        0        0     1084 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2901 2023-08-08 18:39:38.971461 nonebot_plugin_jx3-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2591 2023-08-08 17:52:17.000000 nonebot_plugin_jx3-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:39:38.955919 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/
+-rw-rw-rw-   0        0        0    13540 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/bind.py
+-rw-rw-rw-   0        0        0      204 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/config.py
+-rw-rw-rw-   0        0        0     3735 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/subscribe.py
+-rw-rw-rw-   0        0        0     2900 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/userdefine.py
+-rw-rw-rw-   0        0        0    11457 2023-08-08 17:41:12.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/websocket_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:39:38.970458 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/
+-rw-rw-rw-   0        0        0     2901 2023-08-08 18:39:38.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-08 18:39:38.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:39:38.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-08 18:39:38.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-08 18:39:38.000000 nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      617 2023-08-08 18:39:31.000000 nonebot_plugin_jx3-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 18:39:38.972463 nonebot_plugin_jx3-0.5.1/setup.cfg
```

### Comparing `nonebot_plugin_jx3-0.5/LICENSE` & `nonebot_plugin_jx3-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/PKG-INFO` & `nonebot_plugin_jx3-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_jx3
-Version: 0.5
+Version: 0.5.1
 Summary: 一个nonebot2的jx3插件
 Author-email: fuyang <415276785@qq.com>
 Project-URL: Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_jx3 Version: 0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_jx3 Version: 0.5.1 Summary:
 ä¸ä¸ªnonebot2çjx3æä»¶ Author-email: fuyang <415276785@qq.com> Project-URL:
 Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                # nonebot-plugin-jx3 _è¿æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼æä¾å¤ç§åè½å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ã_
```

### Comparing `nonebot_plugin_jx3-0.5/README.md` & `nonebot_plugin_jx3-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/__init__.py` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/bind.py` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/subscribe.py` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/userdefine.py` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/userdefine.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3/websocket_handler.py` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5/nonebot_plugin_jx3.egg-info/PKG-INFO` & `nonebot_plugin_jx3-0.5.1/nonebot_plugin_jx3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-jx3
-Version: 0.5
+Version: 0.5.1
 Summary: 一个nonebot2的jx3插件
 Author-email: fuyang <415276785@qq.com>
 Project-URL: Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.1 Summary:
 ä¸ä¸ªnonebot2çjx3æä»¶ Author-email: fuyang <415276785@qq.com> Project-URL:
 Homepage, https://github.com/fuyang0811/nonebot-plugin-jx3.git Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                # nonebot-plugin-jx3 _è¿æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼æä¾å¤ç§åè½å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ã_
```

