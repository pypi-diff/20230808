# Comparing `tmp/django-alert-winglet-0.1.6.tar.gz` & `tmp/django-alert-winglet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-alert-winglet-0.1.6.tar", last modified: Mon Aug  7 19:39:22 2023, max compression
+gzip compressed data, was "django-alert-winglet-0.1.7.tar", last modified: Tue Aug  8 16:25:27 2023, max compression
```

## Comparing `django-alert-winglet-0.1.6.tar` & `django-alert-winglet-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.879943 django-alert-winglet-0.1.6/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.879943 django-alert-winglet-0.1.6/apps/alert_winglet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.917791 django-alert-winglet-0.1.7/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.917791 django-alert-winglet-0.1.7/apps/alert_winglet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.917791 django-alert-winglet-0.1.7/apps/alert_winglet/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/base/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/apps/alert_winglet/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/discord/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/discord/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/apps/alert_winglet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/apps/alert_winglet/tests/test_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-08 16:25:27.000000 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-08 16:25:27.000000 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:25:27.000000 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 16:25:27.000000 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 16:25:27.000000 django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-08 16:25:27.921791 django-alert-winglet-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-08 16:25:16.000000 django-alert-winglet-0.1.7/setup.py
```

### Comparing `django-alert-winglet-0.1.6/LICENSE` & `django-alert-winglet-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/PKG-INFO` & `django-alert-winglet-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.6
-Summary: A Django app to send any exception to discord channel.
+Version: 0.1.7
+Summary: Seamlessly Send Django or Python Exceptions to Discord Channels!
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
 Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 alert-winglet
 =============
 
 A Django app to send any exception to a Discord channel.
@@ -49,39 +49,44 @@
     ]
 
 Discord
 -------
 
 1. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-2. Use the `DiscordEmbedManager` class to create a Discord Embed object.::
+2. Use the `DiscordEmbedManager` class to create a Discord Embed object. ::
+
+    from alert_winglet.discord.manager import DiscordEmbedManager
 
     # If the request is not provided, the `extra_detail` variable will be None
     discord_manager = DiscordEmbedManager(
           exc,
       )
     formatted_exc, extra_detail = discord_manager.format_exception()
     data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
 
 3. Then use the `DiscordDelivery` class to send the exception to your Discord channel using the webhook.
-This class can be used for other purposes as well, like sending messages or files... ::
+This class can be used for other purposes as well, like sending messages or files... . ::
+
+    from alert_winglet.discord.sender import DiscordDelivery
 
     delivery = DiscordDelivery(
         embeds=[
             data,
         ]
     )
     delivery.send()
 
+
 Requirements
 ------------
 
 - django >= 3.0
-- discord.py ~=2.2.3
-- requests ~=2.28.2
+- discord.py >=2.2.3
+- requests >=2.28.2
 
 License
 -------
 
 This project is licensed under the MIT License.
 
 Bug Reports and Feature Requests
```

### Comparing `django-alert-winglet-0.1.6/README.rst` & `django-alert-winglet-0.1.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -20,39 +20,44 @@
     ]
 
 Discord
 -------
 
 1. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-2. Use the `DiscordEmbedManager` class to create a Discord Embed object.::
+2. Use the `DiscordEmbedManager` class to create a Discord Embed object. ::
+
+    from alert_winglet.discord.manager import DiscordEmbedManager
 
     # If the request is not provided, the `extra_detail` variable will be None
     discord_manager = DiscordEmbedManager(
           exc,
       )
     formatted_exc, extra_detail = discord_manager.format_exception()
     data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
 
 3. Then use the `DiscordDelivery` class to send the exception to your Discord channel using the webhook.
-This class can be used for other purposes as well, like sending messages or files... ::
+This class can be used for other purposes as well, like sending messages or files... . ::
+
+    from alert_winglet.discord.sender import DiscordDelivery
 
     delivery = DiscordDelivery(
         embeds=[
             data,
         ]
     )
     delivery.send()
 
+
 Requirements
 ------------
 
 - django >= 3.0
-- discord.py ~=2.2.3
-- requests ~=2.28.2
+- discord.py >=2.2.3
+- requests >=2.28.2
 
 License
 -------
 
 This project is licensed under the MIT License.
 
 Bug Reports and Feature Requests
```

### Comparing `django-alert-winglet-0.1.6/apps/alert_winglet/discord/manager.py` & `django-alert-winglet-0.1.7/apps/alert_winglet/discord/manager.py`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/apps/alert_winglet/discord/sender.py` & `django-alert-winglet-0.1.7/apps/alert_winglet/discord/sender.py`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_manager.py` & `django-alert-winglet-0.1.7/apps/alert_winglet/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_sender.py` & `django-alert-winglet-0.1.7/apps/alert_winglet/tests/test_sender.py`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/PKG-INFO` & `django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.6
-Summary: A Django app to send any exception to discord channel.
+Version: 0.1.7
+Summary: Seamlessly Send Django or Python Exceptions to Discord Channels!
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
 Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 alert-winglet
 =============
 
 A Django app to send any exception to a Discord channel.
@@ -49,39 +49,44 @@
     ]
 
 Discord
 -------
 
 1. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-2. Use the `DiscordEmbedManager` class to create a Discord Embed object.::
+2. Use the `DiscordEmbedManager` class to create a Discord Embed object. ::
+
+    from alert_winglet.discord.manager import DiscordEmbedManager
 
     # If the request is not provided, the `extra_detail` variable will be None
     discord_manager = DiscordEmbedManager(
           exc,
       )
     formatted_exc, extra_detail = discord_manager.format_exception()
     data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
 
 3. Then use the `DiscordDelivery` class to send the exception to your Discord channel using the webhook.
-This class can be used for other purposes as well, like sending messages or files... ::
+This class can be used for other purposes as well, like sending messages or files... . ::
+
+    from alert_winglet.discord.sender import DiscordDelivery
 
     delivery = DiscordDelivery(
         embeds=[
             data,
         ]
     )
     delivery.send()
 
+
 Requirements
 ------------
 
 - django >= 3.0
-- discord.py ~=2.2.3
-- requests ~=2.28.2
+- discord.py >=2.2.3
+- requests >=2.28.2
 
 License
 -------
 
 This project is licensed under the MIT License.
 
 Bug Reports and Feature Requests
```

### Comparing `django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/SOURCES.txt` & `django-alert-winglet-0.1.7/apps/django_alert_winglet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.6/setup.cfg` & `django-alert-winglet-0.1.7/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-alert-winglet
-version = 0.1.6
-description = A Django app to send any exception to discord channel.
+version = 0.1.7
+description = Seamlessly Send Django or Python Exceptions to Discord Channels!
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 author = Mojtaba
 author_email = Mojtabadavi14@gmail.com
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
@@ -23,15 +23,15 @@
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
-python_requires = ~=3.10
+python_requires = >=3.10
 install_requires = 
 	django >= 3.0
 	discord.py ~=2.2.3
 	requests ~=2.28.2
 
 [egg_info]
 tag_build =
```

