# Comparing `tmp/wonda-0.6.0a3.tar.gz` & `tmp/wonda-0.6.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonda-0.6.0a3.tar", max compression
+gzip compressed data, was "wonda-0.6.0a4.tar", max compression
```

## Comparing `wonda-0.6.0a3.tar` & `wonda-0.6.0a4.tar`

### file list

```diff
@@ -1,88 +1,87 @@
--rw-r--r--   0        0        0     1131 2023-01-08 13:20:34.909130 wonda-0.6.0a3/LICENSE
--rw-r--r--   0        0        0     2177 2023-08-01 13:12:06.355095 wonda-0.6.0a3/README.md
--rw-r--r--   0        0        0      542 2023-08-06 06:41:06.988417 wonda-0.6.0a3/pyproject.toml
--rw-r--r--   0        0        0      356 2023-08-01 13:12:06.359212 wonda-0.6.0a3/wonda/__init__.py
--rw-r--r--   0        0        0      220 2023-08-01 14:26:17.698469 wonda-0.6.0a3/wonda/api/__init__.py
--rw-r--r--   0        0        0     1957 2023-08-06 06:39:14.044449 wonda-0.6.0a3/wonda/api/abc.py
--rw-r--r--   0        0        0     1290 2023-08-06 06:39:14.061213 wonda-0.6.0a3/wonda/api/api.py
--rw-r--r--   0        0        0       68 2023-08-01 14:15:25.890716 wonda-0.6.0a3/wonda/api/response.py
--rw-r--r--   0        0        0       58 2023-07-09 17:08:19.452596 wonda-0.6.0a3/wonda/api/utils/__init__.py
--rw-r--r--   0        0        0      625 2023-08-06 06:29:08.810627 wonda-0.6.0a3/wonda/api/utils/file_util.py
--rw-r--r--   0        0        0     1076 2023-08-05 22:37:19.630447 wonda-0.6.0a3/wonda/api/utils/token_util.py
--rw-r--r--   0        0        0      249 2023-08-06 06:32:51.263484 wonda-0.6.0a3/wonda/api/validators/__init__.py
--rw-r--r--   0        0        0      650 2023-08-06 05:04:03.795643 wonda-0.6.0a3/wonda/api/validators/abc.py
--rw-r--r--   0        0        0      703 2023-08-06 06:38:39.934952 wonda-0.6.0a3/wonda/api/validators/request.py
--rw-r--r--   0        0        0      713 2023-08-02 09:55:43.097743 wonda-0.6.0a3/wonda/api/validators/response.py
--rw-r--r--   0        0        0      563 2023-08-06 06:24:50.579376 wonda-0.6.0a3/wonda/bot/__init__.py
--rw-r--r--   0        0        0      436 2023-08-06 06:27:50.780575 wonda-0.6.0a3/wonda/bot/abc.py
--rw-r--r--   0        0        0       68 2023-08-05 22:14:36.255732 wonda-0.6.0a3/wonda/bot/blueprint/__init__.py
--rw-r--r--   0        0        0      616 2023-08-06 06:19:47.368200 wonda-0.6.0a3/wonda/bot/blueprint/abc.py
--rw-r--r--   0        0        0      718 2023-08-05 23:41:38.529201 wonda-0.6.0a3/wonda/bot/blueprint/default.py
--rw-r--r--   0        0        0     2014 2023-08-06 06:28:26.794187 wonda-0.6.0a3/wonda/bot/bot.py
--rw-r--r--   0        0        0      212 2023-08-01 13:16:13.736421 wonda-0.6.0a3/wonda/bot/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-08-01 13:16:13.828532 wonda-0.6.0a3/wonda/bot/dispatch/dispatcher/__init__.py
--rw-r--r--   0        0        0      333 2023-08-03 10:01:04.474641 wonda-0.6.0a3/wonda/bot/dispatch/dispatcher/abc.py
--rw-r--r--   0        0        0     1158 2023-08-06 06:29:47.186172 wonda-0.6.0a3/wonda/bot/dispatch/dispatcher/default.py
--rw-r--r--   0        0        0       58 2023-08-01 13:12:06.387599 wonda-0.6.0a3/wonda/bot/dispatch/handler/__init__.py
--rw-r--r--   0        0        0      391 2023-08-01 13:12:06.387736 wonda-0.6.0a3/wonda/bot/dispatch/handler/abc.py
--rw-r--r--   0        0        0     1219 2023-08-05 22:38:35.651178 wonda-0.6.0a3/wonda/bot/dispatch/handler/func.py
--rw-r--r--   0        0        0       78 2023-08-01 13:12:06.362854 wonda-0.6.0a3/wonda/bot/dispatch/middlewares/__init__.py
--rw-r--r--   0        0        0      406 2023-08-01 13:12:06.388025 wonda-0.6.0a3/wonda/bot/dispatch/middlewares/abc.py
--rw-r--r--   0        0        0       62 2023-08-01 13:12:06.363015 wonda-0.6.0a3/wonda/bot/dispatch/router/__init__.py
--rw-r--r--   0        0        0      637 2023-08-01 14:10:44.271381 wonda-0.6.0a3/wonda/bot/dispatch/router/abc.py
--rw-r--r--   0        0        0     1072 2023-08-01 13:12:06.388166 wonda-0.6.0a3/wonda/bot/dispatch/router/default.py
--rw-r--r--   0        0        0      110 2023-08-01 13:12:06.363412 wonda-0.6.0a3/wonda/bot/dispatch/view/__init__.py
--rw-r--r--   0        0        0     3774 2023-08-06 06:20:40.808162 wonda-0.6.0a3/wonda/bot/dispatch/view/abc.py
--rw-r--r--   0        0        0     2103 2023-08-01 13:18:52.420643 wonda-0.6.0a3/wonda/bot/dispatch/view/impl.py
--rw-r--r--   0        0        0       62 2023-08-05 20:27:52.464488 wonda-0.6.0a3/wonda/bot/polling/__init__.py
--rw-r--r--   0        0        0      461 2023-08-06 05:59:11.740179 wonda-0.6.0a3/wonda/bot/polling/abc.py
--rw-r--r--   0        0        0     1516 2023-08-06 06:31:20.353867 wonda-0.6.0a3/wonda/bot/polling/default.py
--rw-r--r--   0        0        0      129 2023-08-01 13:12:06.364526 wonda-0.6.0a3/wonda/bot/rules/__init__.py
--rw-r--r--   0        0        0     1790 2023-08-06 06:17:13.112321 wonda-0.6.0a3/wonda/bot/rules/abc.py
--rw-r--r--   0        0        0     4437 2023-08-01 13:50:29.499615 wonda-0.6.0a3/wonda/bot/rules/base.py
--rw-r--r--   0        0        0     5535 2023-08-03 14:29:37.741552 wonda-0.6.0a3/wonda/bot/rules/message.py
--rw-r--r--   0        0        0      125 2023-08-01 13:12:06.365285 wonda-0.6.0a3/wonda/bot/states/__init__.py
--rw-r--r--   0        0        0       78 2023-08-01 13:12:06.365455 wonda-0.6.0a3/wonda/bot/states/dispenser/__init__.py
--rw-r--r--   0        0        0      822 2023-08-01 13:12:06.365624 wonda-0.6.0a3/wonda/bot/states/dispenser/abc.py
--rw-r--r--   0        0        0      832 2023-08-01 13:12:06.365811 wonda-0.6.0a3/wonda/bot/states/dispenser/default.py
--rw-r--r--   0        0        0      574 2023-08-01 13:12:06.365978 wonda-0.6.0a3/wonda/bot/states/types.py
--rw-r--r--   0        0        0      636 2023-08-01 13:12:06.366161 wonda-0.6.0a3/wonda/bot/updates/__init__.py
--rw-r--r--   0        0        0      269 2023-08-06 05:19:25.163176 wonda-0.6.0a3/wonda/bot/updates/base.py
--rw-r--r--   0        0        0     5287 2023-08-01 13:12:50.665638 wonda-0.6.0a3/wonda/bot/updates/types.py
--rw-r--r--   0        0        0        0 2022-12-09 12:31:48.203870 wonda-0.6.0a3/wonda/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:12:06.388351 wonda-0.6.0a3/wonda/contrib/middleware/__init__.py
--rw-r--r--   0        0        0        0 2022-12-09 12:31:48.204053 wonda-0.6.0a3/wonda/contrib/rules/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 19:17:57.296559 wonda-0.6.0a3/wonda/contrib/storage/__init__.py
--rw-r--r--   0        0        0     1475 2023-08-01 13:12:06.388804 wonda-0.6.0a3/wonda/contrib/storage/redis.py
--rw-r--r--   0        0        0      298 2023-08-01 13:12:06.366842 wonda-0.6.0a3/wonda/errors/__init__.py
--rw-r--r--   0        0        0      269 2023-08-01 13:12:06.367058 wonda-0.6.0a3/wonda/errors/base_exceptions.py
--rw-r--r--   0        0        0     1635 2023-08-01 14:03:19.646417 wonda-0.6.0a3/wonda/errors/code_exception.py
--rw-r--r--   0        0        0       73 2023-04-21 11:36:28.384533 wonda-0.6.0a3/wonda/errors/error_handler/__init__.py
--rw-r--r--   0        0        0      704 2023-08-01 13:12:06.367251 wonda-0.6.0a3/wonda/errors/error_handler/abc.py
--rw-r--r--   0        0        0     2031 2023-08-01 13:12:06.367470 wonda-0.6.0a3/wonda/errors/error_handler/error_handler.py
--rw-r--r--   0        0        0      533 2023-08-01 14:27:57.256711 wonda-0.6.0a3/wonda/modules.py
--rw-r--r--   0        0        0       76 2023-08-01 13:12:06.389026 wonda-0.6.0a3/wonda/net/__init__.py
--rw-r--r--   0        0        0      888 2023-08-06 06:35:28.380359 wonda-0.6.0a3/wonda/net/abc.py
--rw-r--r--   0        0        0     2234 2023-08-06 06:30:50.761253 wonda-0.6.0a3/wonda/net/default.py
--rw-r--r--   0        0        0      123 2023-08-01 13:12:06.368301 wonda-0.6.0a3/wonda/tools/__init__.py
--rw-r--r--   0        0        0      551 2023-08-01 13:12:06.368500 wonda-0.6.0a3/wonda/tools/delayed_task.py
--rw-r--r--   0        0        0      284 2023-08-01 13:12:06.368688 wonda-0.6.0a3/wonda/tools/keyboard/__init__.py
--rw-r--r--   0        0        0      730 2023-08-05 22:17:58.484731 wonda-0.6.0a3/wonda/tools/keyboard/abc.py
--rw-r--r--   0        0        0     2864 2023-08-05 19:39:08.370714 wonda-0.6.0a3/wonda/tools/keyboard/builder.py
--rw-r--r--   0        0        0     5281 2023-08-01 13:12:06.389685 wonda-0.6.0a3/wonda/tools/keyboard/elements.py
--rw-r--r--   0        0        0     2603 2023-08-01 14:08:40.080104 wonda-0.6.0a3/wonda/tools/loop_wrapper.py
--rw-r--r--   0        0        0      174 2023-08-01 13:12:06.369277 wonda-0.6.0a3/wonda/tools/storage/__init__.py
--rw-r--r--   0        0        0      648 2023-08-01 13:12:06.369452 wonda-0.6.0a3/wonda/tools/storage/abc.py
--rw-r--r--   0        0        0     1861 2023-08-01 13:12:06.369619 wonda-0.6.0a3/wonda/tools/storage/memory.py
--rw-r--r--   0        0        0      132 2023-08-01 13:12:06.369784 wonda-0.6.0a3/wonda/tools/storage/types.py
--rw-r--r--   0        0        0       73 2023-02-27 18:52:52.469528 wonda-0.6.0a3/wonda/tools/text/__init__.py
--rw-r--r--   0        0        0       29 2023-02-27 18:52:54.495531 wonda-0.6.0a3/wonda/tools/text/formatting/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-27 18:52:47.941301 wonda-0.6.0a3/wonda/tools/text/formatting/html.py
--rw-r--r--   0        0        0     2761 2023-02-27 18:52:50.221309 wonda-0.6.0a3/wonda/tools/text/formatting/markdown.py
--rw-r--r--   0        0        0       93 2022-12-09 12:31:48.210068 wonda-0.6.0a3/wonda/tools/text/parse_mode.py
--rw-r--r--   0        0        0       55 2023-02-01 05:24:13.893095 wonda-0.6.0a3/wonda/types/__init__.py
--rw-r--r--   0        0        0     4438 2023-08-01 13:13:03.042503 wonda-0.6.0a3/wonda/types/enums.py
--rw-r--r--   0        0        0      588 2023-08-05 19:34:57.249565 wonda-0.6.0a3/wonda/types/helper.py
--rw-r--r--   0        0        0    78297 2023-08-05 19:55:33.676987 wonda-0.6.0a3/wonda/types/methods.py
--rw-r--r--   0        0        0    59280 2023-08-05 19:56:33.820272 wonda-0.6.0a3/wonda/types/objects.py
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 wonda-0.6.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-01-08 13:20:34.909130 wonda-0.6.0a4/LICENSE
+-rw-r--r--   0        0        0     2177 2023-08-01 13:12:06.355095 wonda-0.6.0a4/README.md
+-rw-r--r--   0        0        0      542 2023-08-07 22:59:53.375979 wonda-0.6.0a4/pyproject.toml
+-rw-r--r--   0        0        0      356 2023-08-07 22:53:17.036909 wonda-0.6.0a4/wonda/__init__.py
+-rw-r--r--   0        0        0      220 2023-08-07 22:53:20.926073 wonda-0.6.0a4/wonda/api/__init__.py
+-rw-r--r--   0        0        0     1944 2023-08-07 22:52:35.133399 wonda-0.6.0a4/wonda/api/abc.py
+-rw-r--r--   0        0        0     1290 2023-08-06 06:39:14.061213 wonda-0.6.0a4/wonda/api/api.py
+-rw-r--r--   0        0        0       58 2023-08-07 22:54:02.808747 wonda-0.6.0a4/wonda/api/utils/__init__.py
+-rw-r--r--   0        0        0      625 2023-08-06 06:29:08.810627 wonda-0.6.0a4/wonda/api/utils/file_util.py
+-rw-r--r--   0        0        0     1076 2023-08-05 22:37:19.630447 wonda-0.6.0a4/wonda/api/utils/token_util.py
+-rw-r--r--   0        0        0      249 2023-08-06 06:32:51.263484 wonda-0.6.0a4/wonda/api/validators/__init__.py
+-rw-r--r--   0        0        0      650 2023-08-06 05:04:03.795643 wonda-0.6.0a4/wonda/api/validators/abc.py
+-rw-r--r--   0        0        0      703 2023-08-06 06:38:39.934952 wonda-0.6.0a4/wonda/api/validators/request.py
+-rw-r--r--   0        0        0      713 2023-08-02 09:55:43.097743 wonda-0.6.0a4/wonda/api/validators/response.py
+-rw-r--r--   0        0        0      563 2023-08-07 22:54:02.809255 wonda-0.6.0a4/wonda/bot/__init__.py
+-rw-r--r--   0        0        0      452 2023-08-07 23:01:47.391613 wonda-0.6.0a4/wonda/bot/abc.py
+-rw-r--r--   0        0        0       68 2023-08-07 22:54:02.809630 wonda-0.6.0a4/wonda/bot/blueprint/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-06 06:19:47.368200 wonda-0.6.0a4/wonda/bot/blueprint/abc.py
+-rw-r--r--   0        0        0      650 2023-08-07 23:03:48.458073 wonda-0.6.0a4/wonda/bot/blueprint/default.py
+-rw-r--r--   0        0        0     1973 2023-08-07 22:52:35.142314 wonda-0.6.0a4/wonda/bot/bot.py
+-rw-r--r--   0        0        0      212 2023-08-07 22:54:02.810185 wonda-0.6.0a4/wonda/bot/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-07 22:54:02.810372 wonda-0.6.0a4/wonda/bot/dispatch/dispatcher/__init__.py
+-rw-r--r--   0        0        0      333 2023-08-03 10:01:04.474641 wonda-0.6.0a4/wonda/bot/dispatch/dispatcher/abc.py
+-rw-r--r--   0        0        0     1469 2023-08-07 22:50:29.392367 wonda-0.6.0a4/wonda/bot/dispatch/dispatcher/default.py
+-rw-r--r--   0        0        0       58 2023-08-07 22:54:02.810561 wonda-0.6.0a4/wonda/bot/dispatch/handler/__init__.py
+-rw-r--r--   0        0        0      391 2023-08-01 13:12:06.387736 wonda-0.6.0a4/wonda/bot/dispatch/handler/abc.py
+-rw-r--r--   0        0        0     1153 2023-08-07 22:59:02.850597 wonda-0.6.0a4/wonda/bot/dispatch/handler/func.py
+-rw-r--r--   0        0        0       78 2023-08-01 13:12:06.362854 wonda-0.6.0a4/wonda/bot/dispatch/middlewares/__init__.py
+-rw-r--r--   0        0        0      406 2023-08-01 13:12:06.388025 wonda-0.6.0a4/wonda/bot/dispatch/middlewares/abc.py
+-rw-r--r--   0        0        0       62 2023-08-07 22:54:02.810890 wonda-0.6.0a4/wonda/bot/dispatch/router/__init__.py
+-rw-r--r--   0        0        0      619 2023-08-07 22:52:35.141941 wonda-0.6.0a4/wonda/bot/dispatch/router/abc.py
+-rw-r--r--   0        0        0     1067 2023-08-07 22:51:08.543444 wonda-0.6.0a4/wonda/bot/dispatch/router/default.py
+-rw-r--r--   0        0        0      110 2023-08-01 13:12:06.363412 wonda-0.6.0a4/wonda/bot/dispatch/view/__init__.py
+-rw-r--r--   0        0        0     3966 2023-08-07 22:43:37.767543 wonda-0.6.0a4/wonda/bot/dispatch/view/abc.py
+-rw-r--r--   0        0        0     2103 2023-08-01 13:18:52.420643 wonda-0.6.0a4/wonda/bot/dispatch/view/impl.py
+-rw-r--r--   0        0        0       62 2023-08-07 22:54:02.811413 wonda-0.6.0a4/wonda/bot/polling/__init__.py
+-rw-r--r--   0        0        0      448 2023-08-07 22:52:35.136133 wonda-0.6.0a4/wonda/bot/polling/abc.py
+-rw-r--r--   0        0        0     1516 2023-08-06 06:31:20.353867 wonda-0.6.0a4/wonda/bot/polling/default.py
+-rw-r--r--   0        0        0      129 2023-08-07 22:54:02.811671 wonda-0.6.0a4/wonda/bot/rules/__init__.py
+-rw-r--r--   0        0        0     1790 2023-08-06 06:17:13.112321 wonda-0.6.0a4/wonda/bot/rules/abc.py
+-rw-r--r--   0        0        0     4437 2023-08-01 13:50:29.499615 wonda-0.6.0a4/wonda/bot/rules/base.py
+-rw-r--r--   0        0        0     5535 2023-08-03 14:29:37.741552 wonda-0.6.0a4/wonda/bot/rules/message.py
+-rw-r--r--   0        0        0      125 2023-08-07 22:54:02.812102 wonda-0.6.0a4/wonda/bot/states/__init__.py
+-rw-r--r--   0        0        0       78 2023-08-07 22:54:02.812948 wonda-0.6.0a4/wonda/bot/states/dispenser/__init__.py
+-rw-r--r--   0        0        0      822 2023-08-01 13:12:06.365624 wonda-0.6.0a4/wonda/bot/states/dispenser/abc.py
+-rw-r--r--   0        0        0      832 2023-08-01 13:12:06.365811 wonda-0.6.0a4/wonda/bot/states/dispenser/default.py
+-rw-r--r--   0        0        0      574 2023-08-01 13:12:06.365978 wonda-0.6.0a4/wonda/bot/states/types.py
+-rw-r--r--   0        0        0      636 2023-08-01 13:12:06.366161 wonda-0.6.0a4/wonda/bot/updates/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-06 05:19:25.163176 wonda-0.6.0a4/wonda/bot/updates/base.py
+-rw-r--r--   0        0        0     5287 2023-08-01 13:12:50.665638 wonda-0.6.0a4/wonda/bot/updates/types.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.203870 wonda-0.6.0a4/wonda/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:12:06.388351 wonda-0.6.0a4/wonda/contrib/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.204053 wonda-0.6.0a4/wonda/contrib/rules/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:17:57.296559 wonda-0.6.0a4/wonda/contrib/storage/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-01 13:12:06.388804 wonda-0.6.0a4/wonda/contrib/storage/redis.py
+-rw-r--r--   0        0        0      298 2023-08-07 22:54:02.813297 wonda-0.6.0a4/wonda/errors/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-01 13:12:06.367058 wonda-0.6.0a4/wonda/errors/base_exceptions.py
+-rw-r--r--   0        0        0     1635 2023-08-01 14:03:19.646417 wonda-0.6.0a4/wonda/errors/code_exception.py
+-rw-r--r--   0        0        0       73 2023-08-07 22:54:02.813822 wonda-0.6.0a4/wonda/errors/error_handler/__init__.py
+-rw-r--r--   0        0        0      704 2023-08-01 13:12:06.367251 wonda-0.6.0a4/wonda/errors/error_handler/abc.py
+-rw-r--r--   0        0        0     2031 2023-08-01 13:12:06.367470 wonda-0.6.0a4/wonda/errors/error_handler/error_handler.py
+-rw-r--r--   0        0        0      533 2023-08-01 14:27:57.256711 wonda-0.6.0a4/wonda/modules.py
+-rw-r--r--   0        0        0       76 2023-08-07 22:54:02.814134 wonda-0.6.0a4/wonda/net/__init__.py
+-rw-r--r--   0        0        0      888 2023-08-06 06:35:28.380359 wonda-0.6.0a4/wonda/net/abc.py
+-rw-r--r--   0        0        0     2234 2023-08-06 06:30:50.761253 wonda-0.6.0a4/wonda/net/default.py
+-rw-r--r--   0        0        0      123 2023-08-07 22:54:02.814399 wonda-0.6.0a4/wonda/tools/__init__.py
+-rw-r--r--   0        0        0      551 2023-08-01 13:12:06.368500 wonda-0.6.0a4/wonda/tools/delayed_task.py
+-rw-r--r--   0        0        0      284 2023-08-07 22:54:02.814590 wonda-0.6.0a4/wonda/tools/keyboard/__init__.py
+-rw-r--r--   0        0        0      678 2023-08-07 22:52:35.120960 wonda-0.6.0a4/wonda/tools/keyboard/abc.py
+-rw-r--r--   0        0        0     2864 2023-08-05 19:39:08.370714 wonda-0.6.0a4/wonda/tools/keyboard/builder.py
+-rw-r--r--   0        0        0     5281 2023-08-01 13:12:06.389685 wonda-0.6.0a4/wonda/tools/keyboard/elements.py
+-rw-r--r--   0        0        0     2603 2023-08-01 14:08:40.080104 wonda-0.6.0a4/wonda/tools/loop_wrapper.py
+-rw-r--r--   0        0        0      174 2023-08-07 22:54:02.815029 wonda-0.6.0a4/wonda/tools/storage/__init__.py
+-rw-r--r--   0        0        0      648 2023-08-01 13:12:06.369452 wonda-0.6.0a4/wonda/tools/storage/abc.py
+-rw-r--r--   0        0        0     1861 2023-08-01 13:12:06.369619 wonda-0.6.0a4/wonda/tools/storage/memory.py
+-rw-r--r--   0        0        0      132 2023-08-01 13:12:06.369784 wonda-0.6.0a4/wonda/tools/storage/types.py
+-rw-r--r--   0        0        0       73 2023-08-07 22:54:02.815324 wonda-0.6.0a4/wonda/tools/text/__init__.py
+-rw-r--r--   0        0        0       29 2023-08-07 22:54:02.815699 wonda-0.6.0a4/wonda/tools/text/formatting/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-27 18:52:47.941301 wonda-0.6.0a4/wonda/tools/text/formatting/html.py
+-rw-r--r--   0        0        0     2761 2023-02-27 18:52:50.221309 wonda-0.6.0a4/wonda/tools/text/formatting/markdown.py
+-rw-r--r--   0        0        0       93 2022-12-09 12:31:48.210068 wonda-0.6.0a4/wonda/tools/text/parse_mode.py
+-rw-r--r--   0        0        0       55 2023-08-07 22:54:02.816023 wonda-0.6.0a4/wonda/types/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-01 13:13:03.042503 wonda-0.6.0a4/wonda/types/enums.py
+-rw-r--r--   0        0        0      588 2023-08-05 19:34:57.249565 wonda-0.6.0a4/wonda/types/helper.py
+-rw-r--r--   0        0        0    78297 2023-08-05 19:55:33.676987 wonda-0.6.0a4/wonda/types/methods.py
+-rw-r--r--   0        0        0    59226 2023-08-07 22:52:35.375335 wonda-0.6.0a4/wonda/types/objects.py
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 wonda-0.6.0a4/PKG-INFO
```

### Comparing `wonda-0.6.0a3/LICENSE` & `wonda-0.6.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/README.md` & `wonda-0.6.0a4/README.md`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/pyproject.toml` & `wonda-0.6.0a4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wonda"
-version = "0.6.0a3"
+version = "0.6.0a4"
 description = "Asynchronous feature-rich framework for building Telegram bots"
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/wondergram-org/wonda/"
 
 [tool.poetry.dependencies]
```

### Comparing `wonda-0.6.0a3/wonda/api/abc.py` & `wonda-0.6.0a4/wonda/api/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         return self.API_URL + f"file/bot{self.token}/"
 
     @abstractmethod
     async def request(self, method: str, params: dict = {}) -> bytes:
         """
         Opens a request session and makes a single API call
         """
-        pass
 
     async def request_many(
         self, requests: typing.Iterable[APIRequest]  # type: ignore
     ) -> typing.AsyncIterator[bytes | None]:
         """
         Makes multiple calls to the API opening session for each
         """
```

### Comparing `wonda-0.6.0a3/wonda/api/api.py` & `wonda-0.6.0a4/wonda/api/api.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/api/utils/file_util.py` & `wonda-0.6.0a4/wonda/api/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/api/utils/token_util.py` & `wonda-0.6.0a4/wonda/api/utils/token_util.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/api/validators/abc.py` & `wonda-0.6.0a4/wonda/api/validators/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/api/validators/request.py` & `wonda-0.6.0a4/wonda/api/validators/request.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/api/validators/response.py` & `wonda-0.6.0a4/wonda/api/validators/response.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/__init__.py` & `wonda-0.6.0a4/wonda/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/blueprint/abc.py` & `wonda-0.6.0a4/wonda/bot/blueprint/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/blueprint/default.py` & `wonda-0.6.0a4/wonda/bot/blueprint/default.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import TYPE_CHECKING, Any
+from typing import Any
 
 from wonda.bot.blueprint.abc import ABCBlueprint
-from wonda.bot.dispatch.dispatcher.abc import ABCDispatcher
-from wonda.bot.dispatch.dispatcher.default import DefaultDispatcher
+from wonda.bot.dispatch.dispatcher import ABCDispatcher, DefaultDispatcher
 
 
 class DefaultBlueprint(ABCBlueprint):
     def __init__(self, dispatcher: "ABCDispatcher | None" = None) -> None:
         self.dispatcher = dispatcher or DefaultDispatcher()
 
     def load_into(self, framework: Any) -> "DefaultBlueprint":
```

### Comparing `wonda-0.6.0a3/wonda/bot/bot.py` & `wonda-0.6.0a4/wonda/bot/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from asyncio import AbstractEventLoop, get_event_loop
 
-from wonda.api import ABCAPI, API, Token
+from wonda.api import API, Token
 from wonda.bot.abc import ABCFramework
 from wonda.bot.dispatch import (
     ABCDispatcher,
     ABCRouter,
     DefaultDispatcher,
     DefaultRouter,
 )
 from wonda.bot.polling import ABCPoller, DefaultPoller
 from wonda.bot.states import ABCStateDispenser, DefaultStateDispenser
 from wonda.errors import ABCErrorHandler, ErrorHandler
-from wonda.modules import logger
 from wonda.tools import LoopWrapper
 
 
 class Bot(ABCFramework):
     def __init__(
         self,
         token: Token | None = None,
```

### Comparing `wonda-0.6.0a3/wonda/bot/dispatch/dispatcher/default.py` & `wonda-0.6.0a4/wonda/bot/dispatch/dispatcher/default.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,12 +24,19 @@
         self.chosen_inline_result = ChosenInlineResultView()
         self.pre_checkout_query = PreCheckoutQueryView()
         self.shipping_query = ShippingQueryView()
         self.poll_answer = PollAnswerView()
         self.poll = PollView()
 
     def load(self, dispatcher: "ABCDispatcher") -> None:
-        raise NotImplemented("Not yet implemented")
+        for v in self.views():
+            view: "ABCView" = getattr(self, v, None)
+            assert view, f"View {v!r} is undefined"
 
+            external_view: "ABCView" = getattr(dispatcher, v, None)
+            assert (
+                external_view
+            ), f"External dispatcher should have {v!r} view available"
+            view.load(external_view)
 
     def views(self) -> dict[str, "ABCView"]:
         return {k: v for k, v in self.__dict__.items() if isinstance(v, ABCView)}
```

### Comparing `wonda-0.6.0a3/wonda/bot/dispatch/handler/func.py` & `wonda-0.6.0a4/wonda/bot/dispatch/handler/func.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,35 +11,33 @@
 
 class FuncHandler(ABCHandler):
     def __init__(
         self,
         func: Callable,
         rules: list[ABCRule],
         *,
-        dataclass: _ | None = None,
         blocking: bool = True,
     ):
         self.blocking = blocking
         self.rules = rules
         self.func = func
-        self.ctx = {}
 
     async def filter(self, update: "BaseUpdate", ctx: dict) -> bool:
         for rule in self.rules:
             result = await rule.check(update, ctx)
             if result is False or result is None:
                 return False
             elif result is True:
                 continue
-            ctx.update(result)
+            ctx |= result
         return True
 
     async def handle(self, update: "BaseUpdate", ctx: dict) -> _:
         sig = inspect.signature(self.func)
 
         args = [k for k in sig.parameters.keys()]
         accepts = {k: v for k, v in ctx.items() if k in args[1:]}
 
         return await self.func(update, **accepts)
 
     def __repr__(self):
-        return f"<FuncHandler {self.handler.__name__} blocking={self.blocking} rules={self.rules}>"
+        return f"<FuncHandler {self.func.__name__} blocking={self.blocking} rules={self.rules}>"
```

### Comparing `wonda-0.6.0a3/wonda/bot/dispatch/router/default.py` & `wonda-0.6.0a4/wonda/bot/dispatch/router/default.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wonda.api import ABCAPI, API
+from wonda.api import ABCAPI
 from wonda.bot.dispatch.router import ABCRouter
 from wonda.bot.dispatch.view.abc import ABCView
 from wonda.bot.states.dispenser.abc import ABCStateDispenser
 from wonda.errors.error_handler.abc import ABCErrorHandler
 from wonda.modules import logger
 from wonda.types.objects import Update
```

### Comparing `wonda-0.6.0a3/wonda/bot/dispatch/view/abc.py` & `wonda-0.6.0a4/wonda/bot/dispatch/view/abc.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,19 @@
         def decorator(func) -> None:
             self.register_handler(
                 FuncHandler(func, [*self.auto_rules, *rules], blocking=blocking)
             )
 
         return decorator
     
+    def load(self, view: "ABCView") -> None:
+        self.middlewares.extend(view.middlewares)
+        self.auto_rules.append(view.auto_rules)
+        self.handlers.extend(view.handlers)
+    
     def register_handler(self, handler: ABCHandler) -> None: 
         """
         Registers a handler.
         """
         if not isinstance(handler, ABCHandler):
             raise TypeError("Argument is not an instance of ABCHandler")
```

### Comparing `wonda-0.6.0a3/wonda/bot/dispatch/view/impl.py` & `wonda-0.6.0a4/wonda/bot/dispatch/view/impl.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/polling/default.py` & `wonda-0.6.0a4/wonda/bot/polling/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/rules/abc.py` & `wonda-0.6.0a4/wonda/bot/rules/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/rules/base.py` & `wonda-0.6.0a4/wonda/bot/rules/base.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/rules/message.py` & `wonda-0.6.0a4/wonda/bot/rules/message.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/states/dispenser/abc.py` & `wonda-0.6.0a4/wonda/bot/states/dispenser/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/states/dispenser/default.py` & `wonda-0.6.0a4/wonda/bot/states/dispenser/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/states/types.py` & `wonda-0.6.0a4/wonda/bot/states/types.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/updates/__init__.py` & `wonda-0.6.0a4/wonda/bot/updates/__init__.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/bot/updates/types.py` & `wonda-0.6.0a4/wonda/bot/updates/types.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/contrib/storage/redis.py` & `wonda-0.6.0a4/wonda/contrib/storage/redis.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/errors/code_exception.py` & `wonda-0.6.0a4/wonda/errors/code_exception.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/errors/error_handler/abc.py` & `wonda-0.6.0a4/wonda/errors/error_handler/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/errors/error_handler/error_handler.py` & `wonda-0.6.0a4/wonda/errors/error_handler/error_handler.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/modules.py` & `wonda-0.6.0a4/wonda/modules.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/net/abc.py` & `wonda-0.6.0a4/wonda/net/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/net/default.py` & `wonda-0.6.0a4/wonda/net/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/delayed_task.py` & `wonda-0.6.0a4/wonda/tools/delayed_task.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/keyboard/abc.py` & `wonda-0.6.0a4/wonda/tools/keyboard/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,31 +8,27 @@
     """
 
     @abstractmethod
     def add(self, button: "ABCButton") -> "ABCKeyboardBuilder":
         """
         Adds a button to the keyboard.
         """
-        pass
 
     @abstractmethod
     def row(self) -> "ABCKeyboardBuilder":
         """
         Adds a row to the keyboard. Panics if the last row was empty.
         """
-        pass
 
     @abstractmethod
     def build(self) -> Any:
         """
         Builds the keyboard.
         """
-        pass
 
 
 class ABCButton(ABC):
     @abstractmethod
     def dict(self) -> Any:
         """
         Returns the button data.
         """
-        pass
```

### Comparing `wonda-0.6.0a3/wonda/tools/keyboard/builder.py` & `wonda-0.6.0a4/wonda/tools/keyboard/builder.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/keyboard/elements.py` & `wonda-0.6.0a4/wonda/tools/keyboard/elements.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/loop_wrapper.py` & `wonda-0.6.0a4/wonda/tools/loop_wrapper.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/storage/abc.py` & `wonda-0.6.0a4/wonda/tools/storage/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/storage/memory.py` & `wonda-0.6.0a4/wonda/tools/storage/memory.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/text/formatting/html.py` & `wonda-0.6.0a4/wonda/tools/text/formatting/html.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/tools/text/formatting/markdown.py` & `wonda-0.6.0a4/wonda/tools/text/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/types/enums.py` & `wonda-0.6.0a4/wonda/types/enums.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/types/helper.py` & `wonda-0.6.0a4/wonda/types/helper.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/types/methods.py` & `wonda-0.6.0a4/wonda/types/methods.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a3/wonda/types/objects.py` & `wonda-0.6.0a4/wonda/types/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,14 @@
 
 class ForumTopicClosed(Model):
     """
     This object represents a service message about a forum topic closed in
     the chat. Currently holds no information.
     """
 
-    pass
 
 
 class ForumTopicEdited(Model):
     """
     This object represents a service message about an edited forum topic.
     """
 
@@ -447,33 +446,30 @@
 
 class ForumTopicReopened(Model):
     """
     This object represents a service message about a forum topic reopened
     in the chat. Currently holds no information.
     """
 
-    pass
 
 
 class GeneralForumTopicHidden(Model):
     """
     This object represents a service message about General forum topic
     hidden in the chat. Currently holds no information.
     """
 
-    pass
 
 
 class GeneralForumTopicUnhidden(Model):
     """
     This object represents a service message about General forum topic
     unhidden in the chat. Currently holds no information.
     """
 
-    pass
 
 
 class UserShared(Model):
     """
     This object contains information about the user whose identifier was
     shared with the bot using a KeyboardButtonRequestUser button.
     """
@@ -513,15 +509,14 @@
 
 class VideoChatStarted(Model):
     """
     This object represents a service message about a video chat started in
     the chat. Currently holds no information.
     """
 
-    pass
 
 
 class VideoChatEnded(Model):
     """
     This object represents a service message about a video chat ended in
     the chat.
     """
@@ -2066,15 +2061,14 @@
 
 class CallbackGame(Model):
     """
     A placeholder, currently holds no information. Use BotFather to set up
     your game.
     """
 
-    pass
 
 
 class GameHighScore(Model):
     """
     This object represents one row of the high scores table for a game.
     """
```

### Comparing `wonda-0.6.0a3/PKG-INFO` & `wonda-0.6.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wonda
-Version: 0.6.0a3
+Version: 0.6.0a4
 Summary: Asynchronous feature-rich framework for building Telegram bots
 Home-page: https://github.com/wondergram-org/wonda/
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

