# Comparing `tmp/gubchat-0.1.2.tar.gz` & `tmp/gubchat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gubchat-0.1.2.tar", last modified: Sun Aug  6 20:24:05 2023, max compression
+gzip compressed data, was "gubchat-0.1.3.tar", last modified: Tue Aug  8 19:37:39 2023, max compression
```

## Comparing `gubchat-0.1.2.tar` & `gubchat-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.247000 gubchat-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 20:23:56.000000 gubchat-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-06 20:24:05.247000 gubchat-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 20:23:56.000000 gubchat-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.243000 gubchat-0.1.2/gubchat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/gubchatapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/twitch_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/user_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.243000 gubchat-0.1.2/gubchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-06 20:23:56.000000 gubchat-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:24:05.247000 gubchat-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:39.051313 gubchat-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 19:37:30.000000 gubchat-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 19:37:39.051313 gubchat-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 19:37:30.000000 gubchat-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:39.051313 gubchat-0.1.3/gubchat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/gubchatapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/twitch_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-08 19:37:30.000000 gubchat-0.1.3/gubchat/user_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:39.051313 gubchat-0.1.3/gubchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 19:37:39.000000 gubchat-0.1.3/gubchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-08 19:37:30.000000 gubchat-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:37:39.051313 gubchat-0.1.3/setup.cfg
```

### Comparing `gubchat-0.1.2/LICENSE` & `gubchat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gubchat-0.1.2/PKG-INFO` & `gubchat-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gubchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gubchat is a twitch chat client built using Kivy
 Author-email: Douglas <hashy.software@gmail.com>
 Project-URL: Homepage, https://github.com/Hashy-Software/gubchat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gubchat-0.1.2/gubchat/gubchatapp.py` & `gubchat-0.1.3/gubchat/gubchatapp.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,29 +19,72 @@
 from kivymd.uix.button import MDFloatingActionButton
 from kivymd.uix.label import MDLabel
 from kivymd.uix.list import IconLeftWidget, OneLineAvatarIconListItem
 from kivymd.uix.navigationdrawer import MDNavigationDrawer, MDNavigationLayout
 from kivymd.uix.textfield import MDTextField
 from kivymd.uix.toolbar import MDTopAppBar
 
-from gubchat.twitch_websocket import TwitchWebsocket
+from gubchat.twitch_websocket import ParsedMessage, TwitchWebsocket
 from gubchat.user_auth import request_oauth_token
 
 Window.softinput_mode = "pan"
 
 
-_settings = {
+_configs = {
     "token": "",
     "user": "",
     "channel": "",
+    "color": "dd2020",
+    "user-id": "",
 }
 
+_APP_ID = "hvmj7blkwy2gw3xf820n47i85g4sub"
 _twitch_websocket = None
 
 
+async def update_configs_from_parsed_messages(messages: list[ParsedMessage]):
+    """
+    Get user-id and update user's chat color from GLOBALUSERSTATE and USERSTATE messages
+    """
+    try:
+        for message in messages:
+            if not message or not _configs["user"]:
+                continue
+
+            if not hasattr(message, "command"):
+                continue
+
+            if not hasattr(message, "tags"):
+                continue
+
+            if message.command is None or message.tags is None:
+                continue
+
+            command = message.command.get("command", "")
+            username = message.tags.get("display-name", "")
+
+            if not command or not username:
+                continue
+
+            if (
+                command in ("USERSTATE", "GLOBALUSERSTATE")
+                and username.lower() == _configs["user"].lower()
+            ):
+                logging.debug(f"Using data from userstate: {message}")
+                _configs["color"] = message.tags["color"]
+
+                if "user-id" in _configs:
+                    _configs["user-id"] = message.tags["user-id"]
+
+    except Exception as e:
+        logging.error(
+            f"Failed to get user chat color from parsed global state message: {e}"
+        )
+
+
 class ScrollableLabel(ScrollView):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.layout = GridLayout(cols=1, size_hint_y=None)
         self.add_widget(self.layout)
 
         self.chat_history = MDLabel(
@@ -116,29 +159,47 @@
 
     def focus_text_input(self, _):
         self.new_msg.focus = True
 
     def send_local_message(self, _):
         msg = self.new_msg.text
         self.new_msg.text = ""
-        username = "hash_table"
-        if msg:
-            Clock.schedule_once(
-                lambda _: asyncio.ensure_future(
-                    _twitch_websocket.send_message("hash_table", msg)
-                )
-            )
-            self.history.update_chat_history(
-                f"[color=dd2020]{username}[/color] [color=20dddd]:[/color] {msg}"
+
+        if not msg:
+            return
+
+        global _configs
+        Clock.schedule_once(
+            lambda _: asyncio.ensure_future(
+                _twitch_websocket.send_message(_configs["channel"], msg)
             )
+        )
+
+        self.history.update_chat_history(
+            f"[color={_configs['color']}]{_configs['user']}: [/color] {msg}"
+        ),
+
+    def incoming_message(self, parsed_message: ParsedMessage):
+        if parsed_message.command["command"] == "PRIVMSG":
+            try:
+                user = parsed_message.tags["display-name"]
+                color = parsed_message.tags["color"]
+                message = parsed_message.parameters
+            except KeyError as e:
+                logging.error(f"Failed to get parsed message data: {e}")
+                return
 
-    def incoming_message(self, username, message):
-        if message and username:
             self.history.update_chat_history(
-                f"[color=20dd20]{username}[/color] [color=20dddd]:[/color] {message}"
+                f"[color={color}]{user} :[/color] {message}"
+            )
+        else:
+            Clock.schedule_once(
+                lambda _: asyncio.ensure_future(
+                    update_configs_from_parsed_messages([parsed_message])
+                )
             )
 
     async def listen_for_messages(self):
         logging.debug("Listening for messages")
         while True:
             task = asyncio.create_task(
                 _twitch_websocket.listen_message(self.incoming_message)
@@ -185,42 +246,36 @@
         self.add_widget(MDLabel())
         self.add_widget(MDLabel())
         self.add_widget(self.float_layout)
 
     def connect_button(self, _):
         logging.debug("Clicked connect button")
 
-        global _settings
+        global _configs
 
-        _settings["user"] = self.user.text
-        _settings["channel"] = self.channel.text
+        _configs["user"] = self.user.text
+        _configs["channel"] = self.channel.text
 
         Clock.schedule_once(lambda _: asyncio.ensure_future(self.twitch_connect()))
 
     async def twitch_connect(self):
         global _twitch_websocket
-        global _settings
+        global _configs
 
-        await request_oauth_token(
-            "hvmj7blkwy2gw3xf820n47i85g4sub",  # twitch app_id
-            lambda token, s=_settings: _settings.__setitem__("token", token),
-        )
-
-        logging.debug("Waiting for token, channel and user")
-
-        while not all((_settings["token"], _settings["user"], _settings["channel"])):
-            await asyncio.sleep(0.2)
+        username, channel = _configs["user"], _configs["channel"]
 
-        logging.debug("Found token, channel and user. Connecting to twitch.")
-
-        token, user, channel = (_settings[key] for key in ("token", "user", "channel"))
+        _configs["token"] = await request_oauth_token(_APP_ID)
 
         _twitch_websocket = TwitchWebsocket()
         await _twitch_websocket.connect_websocket()
-        await _twitch_websocket.authenticate(token, user)
+        parsed_responses = await _twitch_websocket.authenticate(
+            _configs["token"], username
+        )
+        await update_configs_from_parsed_messages(parsed_responses)
+
         await _twitch_websocket.join_channel(channel)
 
         Clock.schedule_once(
             lambda _, chat_app=App.get_running_app(): chat_app.create_chat_page()
         )
```

### Comparing `gubchat-0.1.2/gubchat/main.py` & `gubchat-0.1.3/gubchat/main.py`

 * *Files identical despite different names*

### Comparing `gubchat-0.1.2/gubchat/user_auth.py` & `gubchat-0.1.3/gubchat/user_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 class _WebServerContextManager:
     def __init__(self) -> None:
         self._runner: web.AppRunner
 
     async def __aenter__(self):
         app = web.Application()
         app.add_routes(
-            [web.get("/", _home_callback), web.get("/auth", _browser_redirect_callback)]
+            [web.get("/", _home_callback),
+             web.get("/auth", _browser_redirect_callback)]
         )
         self._runner = web.AppRunner(app)
         await self._runner.setup()
         site = web.TCPSite(self._runner, "localhost", 17563)
         await site.start()
 
     async def __aexit__(self, exc_type, exc, tb):
@@ -72,31 +73,29 @@
     """
     Sends URL parameters passed by twitch as fragments(readable client-side only) to the auth route
     """
     with open("UserAuth.html", "r") as file:
         return web.Response(text=file.read(), content_type="text/html")
 
 
-async def request_oauth_token(
-    app_id: str, token_update_callback: Callable, existing_token: str = ""
-):
+async def request_oauth_token(app_id: str, existing_token: str = "") -> str:
     """
     Validate existing token or ask user to authenticate with twitch and provide a new one.
 
     Raises Exception if an issue occurs while getting the token
     """
     if await _is_valid_token(existing_token):
         logging.info("Provided token is valid, returning")
         return existing_token
 
     headers = {
         "client_id": app_id,
         "redirect_uri": "http://localhost:17563",
         "response_type": "token",
-        "scope": "chat:edit chat:read",
+        "scope": "chat:edit chat:read user:manage:chat_color",
         "state": _STATE,
     }
     url_formatted_headers = "&".join(
         f"{header}={value}" for header, value in headers.items()
     )
 
     # Open user's default web browser to request the OAuth token
@@ -109,8 +108,8 @@
         while not _token and not _error:
             await asyncio.sleep(1)
 
         if _error:
             raise Exception(_error)
 
         logging.info("Returning found token")
-        token_update_callback(_token)
+        return _token
```

### Comparing `gubchat-0.1.2/gubchat.egg-info/PKG-INFO` & `gubchat-0.1.3/gubchat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gubchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gubchat is a twitch chat client built using Kivy
 Author-email: Douglas <hashy.software@gmail.com>
 Project-URL: Homepage, https://github.com/Hashy-Software/gubchat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gubchat-0.1.2/pyproject.toml` & `gubchat-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "gubchat"
 description = "Gubchat is a twitch chat client built using Kivy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Douglas", email = "hashy.software@gmail.com" }
 ]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

