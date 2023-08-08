# Comparing `tmp/Chill-Streams-0.4.0.tar.gz` & `tmp/Chill-Streams-0.4.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chill-Streams-0.4.0.tar", last modified: Fri May 19 17:00:30 2023, max compression
+gzip compressed data, was "Chill-Streams-0.4.0.post0.tar", last modified: Tue Aug  8 19:50:19 2023, max compression
```

## Comparing `Chill-Streams-0.4.0.tar` & `Chill-Streams-0.4.0.post0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.405335 Chill-Streams-0.4.0/
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.402804 Chill-Streams-0.4.0/Chill_Streams.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     4892 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      839 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)       88 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/entry_points.txt
--rw-r--r--   0 zach       (502) staff       (20)      111 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       14 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)     1065 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     4892 2023-05-19 17:00:30.405382 Chill-Streams-0.4.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     4563 2022-12-03 03:18:33.000000 Chill-Streams-0.4.0/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.404706 Chill-Streams-0.4.0/chill_streams/
--rw-r--r--   0 zach       (502) staff       (20)      407 2023-05-19 16:58:06.000000 Chill-Streams-0.4.0/chill_streams/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)       75 2021-07-16 14:56:57.000000 Chill-Streams-0.4.0/chill_streams/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4902 2023-05-19 16:24:59.000000 Chill-Streams-0.4.0/chill_streams/app.py
--rw-r--r--   0 zach       (502) staff       (20)      728 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/ascii_art.py
--rw-r--r--   0 zach       (502) staff       (20)      365 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/cli.py
--rw-r--r--   0 zach       (502) staff       (20)     1105 2022-05-03 18:34:50.000000 Chill-Streams-0.4.0/chill_streams/cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     1331 2022-01-04 21:20:39.000000 Chill-Streams-0.4.0/chill_streams/config.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.405233 Chill-Streams-0.4.0/chill_streams/data/
--rw-r--r--   0 zach       (502) staff       (20)        0 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0/chill_streams/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)       59 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/data/https.txt
--rw-r--r--   0 zach       (502) staff       (20)     8270 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/chill_streams/data/stations.csv
--rw-r--r--   0 zach       (502) staff       (20)        0 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/chill_streams/data/videostreams.csv
--rwxr-xr-x   0 zach       (502) staff       (20)     2064 2023-01-06 17:08:51.000000 Chill-Streams-0.4.0/chill_streams/data/vlc-radio-template.sh
--rw-r--r--   0 zach       (502) staff       (20)      839 2022-05-03 18:26:46.000000 Chill-Streams-0.4.0/chill_streams/logging.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2023-01-06 17:08:27.000000 Chill-Streams-0.4.0/chill_streams/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)      912 2021-07-12 23:44:06.000000 Chill-Streams-0.4.0/chill_streams/script_path.py
--rw-r--r--   0 zach       (502) staff       (20)     2545 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/shell_script.py
--rw-r--r--   0 zach       (502) staff       (20)     5896 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/station_list.py
--rw-r--r--   0 zach       (502) staff       (20)     1893 2023-05-19 16:03:26.000000 Chill-Streams-0.4.0/chill_streams/url.py
--rw-r--r--   0 zach       (502) staff       (20)      288 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/version.py
--rw-r--r--   0 zach       (502) staff       (20)     1487 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/video_streams.py
--rw-r--r--   0 zach       (502) staff       (20)     3283 2022-05-03 18:35:20.000000 Chill-Streams-0.4.0/chill_streams/vlc.py
--rw-r--r--   0 zach       (502) staff       (20)      154 2023-05-19 17:00:30.405550 Chill-Streams-0.4.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     1126 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-08-08 19:50:19.655084 Chill-Streams-0.4.0.post0/
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-08-08 19:50:19.652303 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     4504 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      839 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)       88 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (502) staff       (20)      111 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       14 2023-08-08 19:50:19.000000 Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)     1065 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0.post0/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     4504 2023-08-08 19:50:19.655136 Chill-Streams-0.4.0.post0/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     4169 2023-08-08 19:36:58.000000 Chill-Streams-0.4.0.post0/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-08-08 19:50:19.654333 Chill-Streams-0.4.0.post0/chill_streams/
+-rw-r--r--   0 zach       (502) staff       (20)      413 2023-08-08 19:46:47.000000 Chill-Streams-0.4.0.post0/chill_streams/__about__.py
+-rw-r--r--   0 zach       (502) staff       (20)       75 2021-07-16 14:56:57.000000 Chill-Streams-0.4.0.post0/chill_streams/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4902 2023-05-19 16:24:59.000000 Chill-Streams-0.4.0.post0/chill_streams/app.py
+-rw-r--r--   0 zach       (502) staff       (20)      728 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/ascii_art.py
+-rw-r--r--   0 zach       (502) staff       (20)      365 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/cli.py
+-rw-r--r--   0 zach       (502) staff       (20)     1105 2022-05-03 18:34:50.000000 Chill-Streams-0.4.0.post0/chill_streams/cmd.py
+-rw-r--r--   0 zach       (502) staff       (20)     1331 2022-01-04 21:20:39.000000 Chill-Streams-0.4.0.post0/chill_streams/config.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-08-08 19:50:19.654966 Chill-Streams-0.4.0.post0/chill_streams/data/
+-rw-r--r--   0 zach       (502) staff       (20)        0 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0.post0/chill_streams/data/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)       59 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/data/https.txt
+-rw-r--r--   0 zach       (502) staff       (20)     8270 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0.post0/chill_streams/data/stations.csv
+-rw-r--r--   0 zach       (502) staff       (20)        0 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0.post0/chill_streams/data/videostreams.csv
+-rwxr-xr-x   0 zach       (502) staff       (20)     2064 2023-01-06 17:08:51.000000 Chill-Streams-0.4.0.post0/chill_streams/data/vlc-radio-template.sh
+-rw-r--r--   0 zach       (502) staff       (20)      839 2022-05-03 18:26:46.000000 Chill-Streams-0.4.0.post0/chill_streams/logging.py
+-rw-r--r--   0 zach       (502) staff       (20)      161 2023-01-06 17:08:27.000000 Chill-Streams-0.4.0.post0/chill_streams/pkg_resources.py
+-rw-r--r--   0 zach       (502) staff       (20)      912 2021-07-12 23:44:06.000000 Chill-Streams-0.4.0.post0/chill_streams/script_path.py
+-rw-r--r--   0 zach       (502) staff       (20)     2545 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/shell_script.py
+-rw-r--r--   0 zach       (502) staff       (20)     5896 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/station_list.py
+-rw-r--r--   0 zach       (502) staff       (20)     1893 2023-05-19 16:03:26.000000 Chill-Streams-0.4.0.post0/chill_streams/url.py
+-rw-r--r--   0 zach       (502) staff       (20)      288 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/version.py
+-rw-r--r--   0 zach       (502) staff       (20)     1487 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0.post0/chill_streams/video_streams.py
+-rw-r--r--   0 zach       (502) staff       (20)     3283 2022-05-03 18:35:20.000000 Chill-Streams-0.4.0.post0/chill_streams/vlc.py
+-rw-r--r--   0 zach       (502) staff       (20)      154 2023-08-08 19:50:19.655312 Chill-Streams-0.4.0.post0/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     1126 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0.post0/setup.py
```

### Comparing `Chill-Streams-0.4.0/Chill_Streams.egg-info/PKG-INFO` & `Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chill-Streams
-Version: 0.4.0
+Version: 0.4.0.post0
 Summary: Chill electronica streaming
 Home-page: https://github.com/zcutlip/chill_streams
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -33,28 +33,23 @@
   - Probably most modern (reasonable) Linux distros, but late Ubuntu releases are known to work
   - Late macOS versions (tested on macOS 11.4 with up-to-date homebrew installed)
   - Windows probably won't work (but might be easily made to, let me know)
 - Python >= 3.8 (3.9 preferred)
 - VLC, with the `vlc` command line utility on your `$PATH` (the homebrew VLC cask on macOS sets this up for you)
   - Alternatively you may set `VLC_PATH` to point to a `vlc` executable:
   - e.g. `export VLC_PATH=~/Applications/VLC.app/Contents/MacOS/VLC`
-- In order to stream Twitch video channels, the `streamlink` package is required (see installation below)
 
 > Note: VLC on Apple Silicon macOS doesn't support ncurses mode for some reason. I'm pretty sure it's a bug, but I haven't filed one yet. Run with `--gui`, or install the x86 version
 
-> Note: Twitch streams from DEF CON music are possible if `streamlink` is installed, but this is not a hard requirement. If it is not installed video channels will not be presented in the menu or available for playback.
-
 ### Installation, but for real this time
 
 You can install directly from PyPI:
 
 ```bash
-pip install --user Chill-Streams
-# Optional support for Twitch streams
-pip install --user streamlink
+pip3 install --user Chill-Streams
 ```
 
 ## CLI utility: `vlc-radio`
 
 The `vlc-radio` utility starts up VLC Media Player playing one of the stations in the directory.
 
 It has a few modes of operation:
```

### Comparing `Chill-Streams-0.4.0/Chill_Streams.egg-info/SOURCES.txt` & `Chill-Streams-0.4.0.post0/Chill_Streams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/LICENSE` & `Chill-Streams-0.4.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/PKG-INFO` & `Chill-Streams-0.4.0.post0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chill-Streams
-Version: 0.4.0
+Version: 0.4.0.post0
 Summary: Chill electronica streaming
 Home-page: https://github.com/zcutlip/chill_streams
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -33,28 +33,23 @@
   - Probably most modern (reasonable) Linux distros, but late Ubuntu releases are known to work
   - Late macOS versions (tested on macOS 11.4 with up-to-date homebrew installed)
   - Windows probably won't work (but might be easily made to, let me know)
 - Python >= 3.8 (3.9 preferred)
 - VLC, with the `vlc` command line utility on your `$PATH` (the homebrew VLC cask on macOS sets this up for you)
   - Alternatively you may set `VLC_PATH` to point to a `vlc` executable:
   - e.g. `export VLC_PATH=~/Applications/VLC.app/Contents/MacOS/VLC`
-- In order to stream Twitch video channels, the `streamlink` package is required (see installation below)
 
 > Note: VLC on Apple Silicon macOS doesn't support ncurses mode for some reason. I'm pretty sure it's a bug, but I haven't filed one yet. Run with `--gui`, or install the x86 version
 
-> Note: Twitch streams from DEF CON music are possible if `streamlink` is installed, but this is not a hard requirement. If it is not installed video channels will not be presented in the menu or available for playback.
-
 ### Installation, but for real this time
 
 You can install directly from PyPI:
 
 ```bash
-pip install --user Chill-Streams
-# Optional support for Twitch streams
-pip install --user streamlink
+pip3 install --user Chill-Streams
 ```
 
 ## CLI utility: `vlc-radio`
 
 The `vlc-radio` utility starts up VLC Media Player playing one of the stations in the directory.
 
 It has a few modes of operation:
```

### Comparing `Chill-Streams-0.4.0/README.md` & `Chill-Streams-0.4.0.post0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,23 @@
   - Probably most modern (reasonable) Linux distros, but late Ubuntu releases are known to work
   - Late macOS versions (tested on macOS 11.4 with up-to-date homebrew installed)
   - Windows probably won't work (but might be easily made to, let me know)
 - Python >= 3.8 (3.9 preferred)
 - VLC, with the `vlc` command line utility on your `$PATH` (the homebrew VLC cask on macOS sets this up for you)
   - Alternatively you may set `VLC_PATH` to point to a `vlc` executable:
   - e.g. `export VLC_PATH=~/Applications/VLC.app/Contents/MacOS/VLC`
-- In order to stream Twitch video channels, the `streamlink` package is required (see installation below)
 
 > Note: VLC on Apple Silicon macOS doesn't support ncurses mode for some reason. I'm pretty sure it's a bug, but I haven't filed one yet. Run with `--gui`, or install the x86 version
 
-> Note: Twitch streams from DEF CON music are possible if `streamlink` is installed, but this is not a hard requirement. If it is not installed video channels will not be presented in the menu or available for playback.
-
 ### Installation, but for real this time
 
 You can install directly from PyPI:
 
 ```bash
-pip install --user Chill-Streams
-# Optional support for Twitch streams
-pip install --user streamlink
+pip3 install --user Chill-Streams
 ```
 
 ## CLI utility: `vlc-radio`
 
 The `vlc-radio` utility starts up VLC Media Player playing one of the stations in the directory.
 
 It has a few modes of operation:
```

### Comparing `Chill-Streams-0.4.0/chill_streams/app.py` & `Chill-Streams-0.4.0.post0/chill_streams/app.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/ascii_art.py` & `Chill-Streams-0.4.0.post0/chill_streams/ascii_art.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/cmd.py` & `Chill-Streams-0.4.0.post0/chill_streams/cmd.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/config.py` & `Chill-Streams-0.4.0.post0/chill_streams/config.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/data/stations.csv` & `Chill-Streams-0.4.0.post0/chill_streams/data/stations.csv`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/data/vlc-radio-template.sh` & `Chill-Streams-0.4.0.post0/chill_streams/data/vlc-radio-template.sh`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/logging.py` & `Chill-Streams-0.4.0.post0/chill_streams/logging.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/script_path.py` & `Chill-Streams-0.4.0.post0/chill_streams/script_path.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/shell_script.py` & `Chill-Streams-0.4.0.post0/chill_streams/shell_script.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/station_list.py` & `Chill-Streams-0.4.0.post0/chill_streams/station_list.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/url.py` & `Chill-Streams-0.4.0.post0/chill_streams/url.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/video_streams.py` & `Chill-Streams-0.4.0.post0/chill_streams/video_streams.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/chill_streams/vlc.py` & `Chill-Streams-0.4.0.post0/chill_streams/vlc.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.4.0/setup.py` & `Chill-Streams-0.4.0.post0/setup.py`

 * *Files identical despite different names*

