# Comparing `tmp/lastfm-mpris2-scrobbler-0.3.0.tar.gz` & `tmp/lastfm-mpris2-scrobbler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastfm-mpris2-scrobbler-0.3.0.tar", last modified: Thu Aug  3 03:43:05 2023, max compression
+gzip compressed data, was "lastfm-mpris2-scrobbler-1.0.0.tar", last modified: Tue Aug  8 15:25:42 2023, max compression
```

## Comparing `lastfm-mpris2-scrobbler-0.3.0.tar` & `lastfm-mpris2-scrobbler-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.3.0/LICENSE
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2738 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2441 2023-08-03 03:25:48.000000 lastfm-mpris2-scrobbler-0.3.0/README.md
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1943 2023-08-03 03:32:51.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/PlayerState.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     4379 2023-08-03 03:40:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/Scrobbler.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/__init__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1449 2023-08-03 03:40:23.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/__main__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      249 2023-08-03 02:39:01.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/globals.py
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2738 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      539 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       82 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       45 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/requires.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       24 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/top_level.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/setup.cfg
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      912 2023-08-03 03:33:32.000000 lastfm-mpris2-scrobbler-0.3.0/setup.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-1.0.0/LICENSE
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3561 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3264 2023-08-08 15:20:01.000000 lastfm-mpris2-scrobbler-1.0.0/README.md
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2460 2023-08-08 14:56:15.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Cache.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2407 2023-08-08 14:44:07.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/PlayerState.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     5606 2023-08-08 14:57:19.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Scrobbler.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__init__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1449 2023-08-08 14:02:15.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__main__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      180 2023-08-08 14:05:27.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/globals.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3561 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      572 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       82 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       45 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/requires.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       24 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/top_level.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/setup.cfg
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      912 2023-08-08 15:24:00.000000 lastfm-mpris2-scrobbler-1.0.0/setup.py
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/LICENSE` & `lastfm-mpris2-scrobbler-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-0.3.0/PKG-INFO` & `lastfm-mpris2-scrobbler-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-Metadata-Version: 2.1
-Name: lastfm-mpris2-scrobbler
-Version: 0.3.0
-Summary: Last.fm scrobbler via MPRIS2 in Linux
-Home-page: https://github.com/Ladbaby/lastfm-scrobbler
-Author: Ladbaby
-Author-email: Ladbabyms@outlook.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Last.fm scrobbler
+﻿# 🎵 Last.fm scrobbler
 
 A Last.fm scrobbler via MPRIS2 in Linux, implemented via [pylast](https://github.com/pylast/pylast) and [mpris2](https://pythonhosted.org/mpris2/index.html)
 
 Modified based on [dbus-scrobbler](https://github.com/spezifisch/dbus-scrobbler)
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
 - [x] update now playing status
-- [ ] offline storage support
-
-## Alternatives
-
-If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
-
-Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+- [x] offline scrobble cache support
 
 ## What is MPRIS2?
 
 > MPRIS (Media Player Remote Interfacing Specification) is a standard D-Bus (Desktop Bus) interface that allows applications to communicate with and control media players running on a Linux desktop environment.
 
 Thus, this scrobbler is a general-purpose one under the Linux desktop environment, supporting scrobble music from media players without a built-in Last.fm scrobbling feature.
 
@@ -54,15 +37,17 @@
 
     ```bash
     pip install lastfm-mpris2-scrobbler
     ```
 
 ## Configurations
 
-The program expects a `config.yaml` file, example and detailed information can be found in `config.yaml.example`:
+The program expects a `config.yaml` file and can be placed wherever you like, for example `~/.config/lastfm-mpris2-scrobbler/`
+
+Example and detailed information can be found in `config.yaml.example`:
 
 ```yaml
 # username for that service
 user_name: foo
 
 # md5 hash of your password (obtained via `echo -n password | md5sum`)
 password_hash: abc123492abccf4f1997f7ccaabc123b
@@ -70,21 +55,59 @@
 # last.fm api, which can be created via https://www.last.fm/api/account/create
 api_key: 11111111111111111111111111111111
 api_secret: 11111111111111111111111111111111
 
 # the app's uri you want to scrobble
 # use `lastfm-mpris2-scrobbler --list-players` to check the uri name
 application_whitelist: [ "org.mpris.MediaPlayer2.harmonoid" ]
+
+# app's log level
+log_level: DEBUG
 ```
 
 ## Usage
 
 ```bash
 lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
 ```
 
 For more options, see:
 
 ```bash
 lastfm-mpris2-scrobbler --help
 ```
 
+---
+
+If you want to run it as a daemon service, here's a systemd service in user space for reference:
+
+```ini
+[Unit]
+Description=Last.fm scrobbler via MPRIS2
+Documentation=https://github.com/Ladbaby/lastfm-scrobbler
+
+[Service]
+ExecStart=PATH_TO_YOUR_BIN/lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
+
+[Install]
+WantedBy=default.target
+```
+
+You'll have to place the service file under `~/.config/systemd/user/` and name it like `scrobbler.service`
+
+To run the daemon:
+
+```shell
+systemctl --user start scrobbler.service
+```
+
+To run at user login:
+
+```shell
+systemctl --user enable scrobbler.service
+```
+
+## Alternatives
+
+If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
+
+Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/README.md` & `lastfm-mpris2-scrobbler-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-# Last.fm scrobbler
+Metadata-Version: 2.1
+Name: lastfm-mpris2-scrobbler
+Version: 1.0.0
+Summary: Last.fm scrobbler via MPRIS2 in Linux
+Home-page: https://github.com/Ladbaby/lastfm-scrobbler
+Author: Ladbaby
+Author-email: Ladbabyms@outlook.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿# 🎵 Last.fm scrobbler
 
 A Last.fm scrobbler via MPRIS2 in Linux, implemented via [pylast](https://github.com/pylast/pylast) and [mpris2](https://pythonhosted.org/mpris2/index.html)
 
 Modified based on [dbus-scrobbler](https://github.com/spezifisch/dbus-scrobbler)
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
 - [x] update now playing status
-- [ ] offline storage support
-
-## Alternatives
-
-If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
-
-Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+- [x] offline scrobble cache support
 
 ## What is MPRIS2?
 
 > MPRIS (Media Player Remote Interfacing Specification) is a standard D-Bus (Desktop Bus) interface that allows applications to communicate with and control media players running on a Linux desktop environment.
 
 Thus, this scrobbler is a general-purpose one under the Linux desktop environment, supporting scrobble music from media players without a built-in Last.fm scrobbling feature.
 
@@ -43,15 +48,17 @@
 
     ```bash
     pip install lastfm-mpris2-scrobbler
     ```
 
 ## Configurations
 
-The program expects a `config.yaml` file, example and detailed information can be found in `config.yaml.example`:
+The program expects a `config.yaml` file and can be placed wherever you like, for example `~/.config/lastfm-mpris2-scrobbler/`
+
+Example and detailed information can be found in `config.yaml.example`:
 
 ```yaml
 # username for that service
 user_name: foo
 
 # md5 hash of your password (obtained via `echo -n password | md5sum`)
 password_hash: abc123492abccf4f1997f7ccaabc123b
@@ -59,21 +66,59 @@
 # last.fm api, which can be created via https://www.last.fm/api/account/create
 api_key: 11111111111111111111111111111111
 api_secret: 11111111111111111111111111111111
 
 # the app's uri you want to scrobble
 # use `lastfm-mpris2-scrobbler --list-players` to check the uri name
 application_whitelist: [ "org.mpris.MediaPlayer2.harmonoid" ]
+
+# app's log level
+log_level: DEBUG
 ```
 
 ## Usage
 
 ```bash
 lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
 ```
 
 For more options, see:
 
 ```bash
 lastfm-mpris2-scrobbler --help
 ```
 
+---
+
+If you want to run it as a daemon service, here's a systemd service in user space for reference:
+
+```ini
+[Unit]
+Description=Last.fm scrobbler via MPRIS2
+Documentation=https://github.com/Ladbaby/lastfm-scrobbler
+
+[Service]
+ExecStart=PATH_TO_YOUR_BIN/lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
+
+[Install]
+WantedBy=default.target
+```
+
+You'll have to place the service file under `~/.config/systemd/user/` and name it like `scrobbler.service`
+
+To run the daemon:
+
+```shell
+systemctl --user start scrobbler.service
+```
+
+To run at user login:
+
+```shell
+systemctl --user enable scrobbler.service
+```
+
+## Alternatives
+
+If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
+
+Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/PlayerState.py` & `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/PlayerState.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 from lastfm_mpris2_scrobbler.globals import get_unix_timestamp
 
 class PlayerState:
-    def __init__(self, metadata_dict, playback_status) -> None:
+    def __init__(self, metadata_dict = None, playback_status = "Playing") -> None:
         self.total_played_time = 0
         self.last_observation_timestamp = get_unix_timestamp()
         self.trackid = ""
         self.if_scrobbled = False
-        self.update_status(metadata_dict, playback_status, self.last_observation_timestamp)
+        if metadata_dict is not None:
+            self.update_status(metadata_dict, playback_status, self.last_observation_timestamp)
+
+    def set_value(self, trackid, artist, title, timestamp, album, album_artist, track_number, duration):
+        self.trackid = trackid
+        self.artist = artist
+        self.title = title
+        self.last_observation_timestamp = timestamp
+        self.album = album
+        self.albumArtist = album_artist
+        self.trackNumber = track_number
+        self.length = duration
+        return self
 
     def handle_multiple_artists(self, artist_array):
         # convert artist array into a single string
         return ", ".join(artist_array)
     
     def update_status(self, metadata_dict, playback_status, timestamp):
         # time length of the current song in seconds
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/__main__.py` & `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__main__.py`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO` & `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 0.3.0
+Version: 1.0.0
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Last.fm scrobbler
+﻿# 🎵 Last.fm scrobbler
 
 A Last.fm scrobbler via MPRIS2 in Linux, implemented via [pylast](https://github.com/pylast/pylast) and [mpris2](https://pythonhosted.org/mpris2/index.html)
 
 Modified based on [dbus-scrobbler](https://github.com/spezifisch/dbus-scrobbler)
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
 - [x] update now playing status
-- [ ] offline storage support
-
-## Alternatives
-
-If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
-
-Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+- [x] offline scrobble cache support
 
 ## What is MPRIS2?
 
 > MPRIS (Media Player Remote Interfacing Specification) is a standard D-Bus (Desktop Bus) interface that allows applications to communicate with and control media players running on a Linux desktop environment.
 
 Thus, this scrobbler is a general-purpose one under the Linux desktop environment, supporting scrobble music from media players without a built-in Last.fm scrobbling feature.
 
@@ -54,15 +48,17 @@
 
     ```bash
     pip install lastfm-mpris2-scrobbler
     ```
 
 ## Configurations
 
-The program expects a `config.yaml` file, example and detailed information can be found in `config.yaml.example`:
+The program expects a `config.yaml` file and can be placed wherever you like, for example `~/.config/lastfm-mpris2-scrobbler/`
+
+Example and detailed information can be found in `config.yaml.example`:
 
 ```yaml
 # username for that service
 user_name: foo
 
 # md5 hash of your password (obtained via `echo -n password | md5sum`)
 password_hash: abc123492abccf4f1997f7ccaabc123b
@@ -70,21 +66,59 @@
 # last.fm api, which can be created via https://www.last.fm/api/account/create
 api_key: 11111111111111111111111111111111
 api_secret: 11111111111111111111111111111111
 
 # the app's uri you want to scrobble
 # use `lastfm-mpris2-scrobbler --list-players` to check the uri name
 application_whitelist: [ "org.mpris.MediaPlayer2.harmonoid" ]
+
+# app's log level
+log_level: DEBUG
 ```
 
 ## Usage
 
 ```bash
 lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
 ```
 
 For more options, see:
 
 ```bash
 lastfm-mpris2-scrobbler --help
 ```
 
+---
+
+If you want to run it as a daemon service, here's a systemd service in user space for reference:
+
+```ini
+[Unit]
+Description=Last.fm scrobbler via MPRIS2
+Documentation=https://github.com/Ladbaby/lastfm-scrobbler
+
+[Service]
+ExecStart=PATH_TO_YOUR_BIN/lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
+
+[Install]
+WantedBy=default.target
+```
+
+You'll have to place the service file under `~/.config/systemd/user/` and name it like `scrobbler.service`
+
+To run the daemon:
+
+```shell
+systemctl --user start scrobbler.service
+```
+
+To run at user login:
+
+```shell
+systemctl --user enable scrobbler.service
+```
+
+## Alternatives
+
+If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
+
+Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt` & `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+lastfm_mpris2_scrobbler/Cache.py
 lastfm_mpris2_scrobbler/PlayerState.py
 lastfm_mpris2_scrobbler/Scrobbler.py
 lastfm_mpris2_scrobbler/__init__.py
 lastfm_mpris2_scrobbler/__main__.py
 lastfm_mpris2_scrobbler/globals.py
 lastfm_mpris2_scrobbler.egg-info/PKG-INFO
 lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
```

### Comparing `lastfm-mpris2-scrobbler-0.3.0/setup.py` & `lastfm-mpris2-scrobbler-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = path.abspath(path.dirname(__file__))
 with open(path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='lastfm-mpris2-scrobbler',
-    version='0.3.0',
+    version='1.0.0',
     description="Last.fm scrobbler via MPRIS2 in Linux",
     url="https://github.com/Ladbaby/lastfm-scrobbler",
     author="Ladbaby",
     author_email="Ladbabyms@outlook.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

