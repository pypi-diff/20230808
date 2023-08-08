# Comparing `tmp/nonebot_plugin_chatrecorder-0.3.0.tar.gz` & `tmp/nonebot_plugin_chatrecorder-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatrecorder-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatrecorder-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_chatrecorder-0.3.0.tar` & `nonebot_plugin_chatrecorder-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4619 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/README.md
--rw-r--r--   0        0        0     1031 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/__init__.py
--rw-r--r--   0        0        0       75 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/__init__.py
--rw-r--r--   0        0        0     4528 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/console.py
--rw-r--r--   0        0        0     4908 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/kaiheila.py
--rw-r--r--   0        0        0     5209 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3675 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
--rw-r--r--   0        0        0     4150 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/qqguild.py
--rw-r--r--   0        0        0     5091 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/telegram.py
--rw-r--r--   0        0        0      317 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/config.py
--rw-r--r--   0        0        0      766 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/consts.py
--rw-r--r--   0        0        0      402 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/exception.py
--rw-r--r--   0        0        0     2389 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/message.py
--rw-r--r--   0        0        0     1703 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
--rw-r--r--   0        0        0     1917 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/44cce443d2c0_drop_column.py
--rw-r--r--   0        0        0     3732 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
--rw-r--r--   0        0        0     2992 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/902a51ac4032_add_session.py
--rw-r--r--   0        0        0     1517 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
--rw-r--r--   0        0        0     1165 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/de6827ead8fe_foreignkey.py
--rw-r--r--   0        0        0     1429 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/model.py
--rw-r--r--   0        0        0     9675 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.py
--rw-r--r--   0        0        0     4624 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.pyi
--rw-r--r--   0        0        0      273 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/utils.py
--rw-r--r--   0        0        0     1402 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4619 2023-08-08 11:21:06.957873 nonebot_plugin_chatrecorder-0.3.1/README.md
+-rw-r--r--   0        0        0     1031 2023-08-08 11:21:06.957873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/__init__.py
+-rw-r--r--   0        0        0       75 2023-08-08 11:21:06.957873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/__init__.py
+-rw-r--r--   0        0        0     4528 2023-08-08 11:21:06.957873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/console.py
+-rw-r--r--   0        0        0     4908 2023-08-08 11:21:06.957873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/kaiheila.py
+-rw-r--r--   0        0        0     5209 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3675 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     4150 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/qqguild.py
+-rw-r--r--   0        0        0     5091 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/telegram.py
+-rw-r--r--   0        0        0      317 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/config.py
+-rw-r--r--   0        0        0      766 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/consts.py
+-rw-r--r--   0        0        0      402 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/exception.py
+-rw-r--r--   0        0        0     2389 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/message.py
+-rw-r--r--   0        0        0     1703 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
+-rw-r--r--   0        0        0     1917 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/44cce443d2c0_drop_column.py
+-rw-r--r--   0        0        0     3732 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
+-rw-r--r--   0        0        0     4626 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/902a51ac4032_add_session.py
+-rw-r--r--   0        0        0     1517 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
+-rw-r--r--   0        0        0     1165 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/de6827ead8fe_foreignkey.py
+-rw-r--r--   0        0        0     1429 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/model.py
+-rw-r--r--   0        0        0     9675 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/record.py
+-rw-r--r--   0        0        0     4624 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/record.pyi
+-rw-r--r--   0        0        0      273 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/utils.py
+-rw-r--r--   0        0        0     1402 2023-08-08 11:21:06.961873 nonebot_plugin_chatrecorder-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_chatrecorder-0.3.0/README.md` & `nonebot_plugin_chatrecorder-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/__init__.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/console.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/kaiheila.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v11.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v12.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/qqguild.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/telegram.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/consts.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/consts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/message.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/44cce443d2c0_drop_column.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/44cce443d2c0_drop_column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/de6827ead8fe_foreignkey.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/migrations/de6827ead8fe_foreignkey.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/model.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.py` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.pyi` & `nonebot_plugin_chatrecorder-0.3.1/nonebot_plugin_chatrecorder/record.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.3.0/pyproject.toml` & `nonebot_plugin_chatrecorder-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_chatrecorder"
-version = "0.3.0"
+version = "0.3.1"
 description = "适用于 Nonebot2 的聊天记录插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
 repository = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
```

### Comparing `nonebot_plugin_chatrecorder-0.3.0/PKG-INFO` & `nonebot_plugin_chatrecorder-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatrecorder
-Version: 0.3.0
+Version: 0.3.1
 Summary: 适用于 Nonebot2 的聊天记录插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-chatrecorder
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

