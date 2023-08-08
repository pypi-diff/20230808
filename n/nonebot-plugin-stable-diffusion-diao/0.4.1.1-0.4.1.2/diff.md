# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.4.1.1.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.1.1.tar", last modified: Mon Aug  7 05:12:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.1.2.tar", last modified: Tue Aug  8 01:31:55 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1.tar` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.1.1/LICENSE
--rw-r--r--   0        0        0      703 2023-08-06 09:18:32.524827 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    28643 2023-08-05 16:15:52.274941 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6220 2023-08-07 03:34:07.767680 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    17343 2023-08-05 06:16:23.495307 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    21114 2023-08-07 03:37:09.688742 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    12018 2023-08-07 05:12:25.889959 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     8489 2023-08-07 05:12:23.157396 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/civitai.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2724 2023-08-05 06:16:27.628128 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    47944 2023-08-07 03:34:25.072810 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6378 2023-08-07 03:33:48.271023 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     5222 2023-08-07 03:27:37.914834 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2065 2023-08-05 16:30:13.201017 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0     1005 2023-08-05 16:23:26.586630 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      728 2023-08-07 05:12:39.598075 nonebot_plugin_stable_diffusion_diao-0.4.1.1/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.1.2/LICENSE
+-rw-r--r--   0        0        0      703 2023-08-06 09:18:32.524827 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    28643 2023-08-05 16:15:52.274941 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6220 2023-08-07 03:34:07.767680 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    17343 2023-08-05 06:16:23.495307 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    21114 2023-08-07 03:37:09.688742 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    12018 2023-08-07 05:12:25.889959 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     8579 2023-08-08 01:31:36.255262 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/civitai.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2724 2023-08-05 06:16:27.628128 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    47944 2023-08-07 03:34:25.072810 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6328 2023-08-07 11:46:56.200537 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     5222 2023-08-07 03:27:37.914834 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2065 2023-08-05 16:30:13.201017 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0     1005 2023-08-05 16:23:26.586630 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-08-08 01:31:55.961964 nonebot_plugin_stable_diffusion_diao-0.4.1.2/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/civitai.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/civitai.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,16 @@
                 text_msg += f"模型名称: {model['name']}\n模型id: {model['id']}\n模型类型: {model_type}\n是否为R18: {model['nsfw']}\n"
                 metrics_replace_list = ["评论总数", "喜欢次数", "下载次数", "评分", "评分总数", "加权评分"]
                 metrics_msg = ""
                 metrics_dict: dict = model['metrics']
                 for replace, value in zip(metrics_replace_list, list(metrics_dict.values())):
                     metrics_msg += f"{replace}: {value}\n"
                 hash_str = '\n'.join(model['hashes'])
-                text_msg += f"{metrics_msg}\n下载id: {download_id}\n作者: {model['user']['username']}, id: {model['user']['id']}\n哈希值: {hash_str}\n触发词: {model['triggerWords'][0]}\n以下是返图"
+                trigger_words = model['triggerWords'][0] if len(model['triggerWords']) != 0 else ""
+                text_msg += f"{metrics_msg}\n下载id: {download_id}\n作者: {model['user']['username']}, id: {model['user']['id']}\n哈希值: {hash_str}\n触发词: {trigger_words}\n以下是返图"
                 
                 images = model['images']
                 task_list = []
                 for image in images:
                     if len(task_list) > 1:
                         break
                     url = f"https://image.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/{image['url']}/{image['name']}"
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             async with session.post('https://api.cognitive.microsofttranslator.com/translate', json=body, params=params, headers=header) as resp:
                 if resp.status != 200:
                     logger.error(f"Bing翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
                 jsonresult = await resp.json()
                 result=jsonresult[0]["translations"][0]["text"]
                 logger.debug(f"Bing翻译启动，获取到{text},翻译后{result}")
                 return result
-    except Exception:
+    except:
         return None
 
 
 async def translate_deepl(text: str, to: str):
     """
     EN,JA,ZH
     """
@@ -72,15 +72,15 @@
             async with session.get('https://api-free.deepl.com/v2/translate', params=params) as resp:
                 if resp.status != 200:
                     logger.error(f"DeepL翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
                 jsonresult = await resp.json()
                 result=jsonresult["translations"][0]["text"]
                 logger.debug(f"DeepL翻译启动，获取到{text},翻译后{result}")
                 return result
-    except Exception:
+    except:
         return None
 
 
 async def translate_youdao(input: str, type: str):
     """
     默认auto
     ZH_CH2EN 中译英
@@ -100,15 +100,15 @@
             async with session.post("http://fanyi.youdao.com/translate", data=data) as resp:
                 if resp.status != 200:
                     logger.error(f"有道翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
                 result = await resp.json()
                 result=result["translateResult"][0][0]["tgt"]
                 logger.debug(f"有道翻译启动，获取到{input},翻译后{result}")
                 return result
-    except Exception:
+    except:
         return None
 
 
 async def translate_google_proxy(input: str, to: str):
     """
     en,jp,zh 需要来源语言
     """
@@ -122,15 +122,15 @@
             async with session.post("https://mikeee-gradio-gtr.hf.space/api/predict", json=data, proxy=config.proxy_site)as resp:
                 if resp.status != 200:
                     logger.error(f"谷歌代理翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
                 result = await resp.json()
                 result=result["data"][0]
                 logger.debug(f"谷歌代理翻译启动，获取到{input},翻译后{result}")
                 return result
-    except Exception:
+    except:
         return None
 
 
 async def get_access_token():
     """
     百度云access_token
     使用 AK，SK 生成鉴权签名（Access Token）
@@ -158,9 +158,9 @@
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.post(url=url, json=payload) as resp:
                 if resp.status != 200:
                     logger.error(f"百度翻译接口错误, 错误代码{resp.status},{await resp.text()}")
                 json_ = await resp.json()
                 result = json_["result"]["trans_result"][0]["dst"]
         return result
-    except Exception:
+    except:
         return None
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.1.1/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.4.1.1"
+version = "0.4.1.2"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

