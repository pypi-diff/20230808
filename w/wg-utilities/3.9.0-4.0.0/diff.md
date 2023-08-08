# Comparing `tmp/wg_utilities-3.9.0.tar.gz` & `tmp/wg_utilities-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.9.0.tar", max compression
+gzip compressed data, was "wg_utilities-4.0.0.tar", max compression
```

## Comparing `wg_utilities-3.9.0.tar` & `wg_utilities-4.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1069 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/README.md
--rw-r--r--   0        0        0     4873 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      749 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4255 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    23785 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56658 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7580 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13262 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0     9984 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/json_api_client.py
--rw-r--r--   0        0        0    15946 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    18157 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    51568 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22442 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7006 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5786 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0      565 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0     1982 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/file_handler.py
--rw-r--r--   0        0        0     4486 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/list_handler.py
--rw-r--r--   0        0        0     1060 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/stream_handler.py
--rw-r--r--   0        0        0    11991 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/warehouse_handler.py
--rw-r--r--   0        0        0        0 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 wg_utilities-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-08 15:58:07.438941 wg_utilities-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-08-08 15:58:07.438941 wg_utilities-4.0.0/README.md
+-rw-r--r--   0        0        0     4840 2023-08-08 15:58:07.438941 wg_utilities-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      749 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4320 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0     9175 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    21048 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    54103 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7610 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13223 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    10028 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/json_api_client.py
+-rw-r--r--   0        0        0    16363 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    19032 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    48661 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22232 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1084 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7006 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     5997 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36158 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5786 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-08-08 15:58:07.526942 wg_utilities-4.0.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0      565 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0     1982 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/loggers/file_handler.py
+-rw-r--r--   0        0        0     4486 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/loggers/list_handler.py
+-rw-r--r--   0        0        0     1060 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/loggers/stream_handler.py
+-rw-r--r--   0        0        0    14201 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/loggers/warehouse_handler.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-08-08 15:58:07.530942 wg_utilities-4.0.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4023 1970-01-01 00:00:00.000000 wg_utilities-4.0.0/PKG-INFO
```

### Comparing `wg_utilities-3.9.0/LICENSE` & `wg_utilities-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/README.md` & `wg_utilities-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/pyproject.toml` & `wg_utilities-4.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.9.0"
+version = "4.0.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
@@ -14,32 +14,31 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 # Dependencies
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 async-upnp-client = { version = "*", optional = true }
 botocore = { version = "*", optional = true }
 flask = { version = ">=2.0.2", optional = true }
 "jetson.gpio" = { version = "*", platform = "linux", optional = true }
 lxml = { version = "==4.9.3", optional = true }
 pigpio = { version = "*", optional = true }
 pillow = { version = "*", optional = true }
 pyjwt = { version = ">=2.6,<2.9", optional = true }
 python-dotenv = { version = "*", optional = true }
 pytz = ">=2022.1"
 requests = { version = ">=2.26.0", optional = true }
 "rpi.gpio" = { version = "*", platform = "linux", optional = true }
 spidev = { version = "*", platform = "linux", optional = true }
-strenum = { version = "*", optional = true }
 tzlocal = { version = "*", optional = true }
 xmltodict = { version = "*", optional = true }
-pydantic = "<2.0.0"
+pydantic = "<3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pylint = "*"
 pre-commit = "*"
 mypy = "*"
@@ -65,26 +64,26 @@
 aioresponses = "*"
 pytest-cov = "*"
 pytest-randomly = "*"
 pytest-aws-config = "*"
 exceptiongroup = "*"
 tomli = "*"
 pytest-xdist = "*"
+pytest-asyncio = "^0.21.1"
 
 
 [tool.poetry.extras]
 clients = [
     "flask",
     "pyjwt",
     "requests",
     "pytz",
     "tzlocal",
     "pydantic",
     "python-dotenv",
-    "strenum",
 ]
 "devices.epd" = ["spidev", "rpi.gpio", "Pillow"]
 "devices.dht22" = ["pigpio"]
 "devices.yamaha_yas_209" = ["async-upnp-client", "pydantic", "xmltodict"]
 "exceptions" = ["python-dotenv", "requests"]
 "functions" = ["lxml"]
```

### Comparing `wg_utilities-3.9.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-4.0.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/__init__.py` & `wg_utilities-4.0.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/_google.py` & `wg_utilities-4.0.0/wg_utilities/clients/_google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Generic Google Client - having one client for all APIs is way too big."""
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from json import dumps
 from logging import DEBUG, getLogger
-from typing import TYPE_CHECKING, Any, Generic, Literal, TypeAlias, TypedDict, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, Literal, TypeAlias, TypeVar
 
 from requests import Response, get
+from typing_extensions import TypedDict
 
 from wg_utilities.clients.json_api_client import StrBytIntFlt
 from wg_utilities.clients.oauth_client import OAuthClient
 from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
@@ -80,15 +81,17 @@
         "pageSize": "50",
     }
 
     def get_items(
         self,
         url: str,
         *,
-        list_key: Literal["albums", "drives", "files", "items", "point"] = "items",
+        list_key: Literal[
+            "albums", "drives", "files", "items", "mediaItems", "point"
+        ] = "items",
         params: dict[
             StrBytIntFlt,
             StrBytIntFlt | Iterable[StrBytIntFlt] | None,
         ]
         | None = None,
         method_override: Callable[..., Response] | None = None,
     ) -> list[GetJsonResponseGoogleClient]:
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-4.0.0/wg_utilities/clients/_spotify_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 not sure if there's anything functional that is done with these types, but they
 are used for type hinting and to make the code more readable.
 """
 from __future__ import annotations
 
 from datetime import date
 from logging import DEBUG, getLogger
-from typing import Literal, TypeAlias, TypedDict, final
+from typing import Literal, TypeAlias, final
 
-from typing_extensions import NotRequired
+from typing_extensions import NotRequired, TypedDict
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 # <editor-fold desc="Simple/'Helper' Objects">
 
 
@@ -35,16 +35,15 @@
     """An object for the Spotify entity's image."""
 
     url: str
     height: int | None
     width: int | None
 
 
-# </editor-fold>
-# <editor-fold desc="Generic Objects">
+# Generic Objects
 
 
 class SpotifyBaseEntityJson(TypedDict):
     """The base JSON object for a Spotify entity."""
 
     external_urls: ExternalUrls
     href: str
@@ -54,24 +53,14 @@
 
 class SpotifyNamedEntityJson(SpotifyBaseEntityJson):
     """The base JSON object for a Spotify entity with a name."""
 
     name: str
 
 
-class SpotifyLocalEntityJson(TypedDict):
-    """The base JSON object for a local-only Spotify entity."""
-
-    external_urls: dict[None, None]
-    href: None
-    id: None
-    name: str
-    uri: None | str
-
-
 # </editor-fold>
 # <editor-fold desc="Album Objects">
 
 
 class AlbumSummaryJson(SpotifyNamedEntityJson, total=False):
     """Type info for Spotify albums in tracks.
 
@@ -95,26 +84,14 @@
     release_date: str | date
     release_date_precision: str
     total_tracks: int
     restrictions: NotRequired[dict[str, str]]
     type: Literal["album"]
 
 
-class AlbumLocalJson(SpotifyLocalEntityJson):
-    """Type info for a local-only Spotify album."""
-
-    album_type: None
-    artists: list[None]
-    available_markets: list[None]
-    images: list[None]
-    release_date: None
-    release_date_precision: None
-    type: Literal["album"]
-
-
 class AlbumFullJson(AlbumSummaryJson):
     """Response from `/albums/{id}`."""
 
     copyrights: list[dict[str, str]]
     external_ids: dict[str, str]
     genres: list[str]
     label: str
@@ -132,20 +109,14 @@
     See Also:
         ArtistFullJson
     """
 
     type: Literal["artist"]
 
 
-class ArtistLocalJson(SpotifyLocalEntityJson):
-    """Type info for a local-only Spotify artist."""
-
-    type: Literal["artist"]
-
-
 class ArtistFullJson(ArtistSummaryJson):
     """Response from `/artists/{id}`."""
 
     followers: Followers
     genres: list[str]
     images: list[Image]
     popularity: int
@@ -190,17 +161,17 @@
 
 
 class PlaylistFullJsonTracks(TypedDict):
     """Type info for the `tracks` field of `PlaylistFullJson`."""
 
     added_at: str
     added_by: UserSummaryJson
-    is_local: bool
+    is_local: Literal[False]
     primary_color: None  # Not implemented yet
-    track: TrackFullJson | TrackLocalJson
+    track: TrackFullJson
     video_thumbnail: NotRequired[_TrackVideoThumbnail]
 
 
 class PlaylistSummaryJson(_PlaylistBaseJson):
     """Type info for Spotify playlists in pages.
 
     See Also:
@@ -240,34 +211,14 @@
     """
 
     url: str | None
     height: NotRequired[int]
     width: NotRequired[int]
 
 
-class TrackLocalJson(SpotifyLocalEntityJson, total=False):
-    """Response from `/tracks/{id}`."""
-
-    album: AlbumLocalJson
-    artists: list[ArtistLocalJson]
-    available_markets: list[None]
-    disc_number: int
-    duration_ms: int
-    episode: NotRequired[bool]
-    explicit: bool
-    external_ids: dict[None, None]
-    is_local: Literal[True]
-    is_playable: NotRequired[bool]
-    linked_from: NotRequired[_LinkedFromInTrack]
-    popularity: int
-    preview_url: None
-    track_number: int
-    type: Literal["track"]
-
-
 class TrackFullJson(SpotifyNamedEntityJson, total=False):
     """Response from `/tracks/{id}`."""
 
     album: AlbumSummaryJson
     artists: list[ArtistSummaryJson]
     available_markets: list[str]
     disc_number: int
@@ -275,15 +226,15 @@
     episode: NotRequired[bool]
     explicit: bool
     external_ids: NotRequired[dict[str, str]]
     is_local: Literal[False]
     is_playable: NotRequired[bool]
     linked_from: NotRequired[_LinkedFromInTrack]
     popularity: int
-    preview_url: str
+    preview_url: str | None
     restrictions: NotRequired[
         dict[Literal["reason"], Literal["explicit", "market", "product"]]
     ]
     track: NotRequired[bool]
     track_number: int
     type: Literal["track"]
 
@@ -344,15 +295,15 @@
     """Typing info for paginated responses from Spotify."""
 
     devices: NotRequired[list[DeviceJson]]
     href: str
     limit: int
     next: str | None
     offset: int
-    previous: NotRequired[str]
+    previous: str | None
     total: int
 
 
 class PaginatedResponsePlaylistTracks(_PaginatedResponseBase):
     """Type info for the `tracks` field of `PlaylistFullJson`."""
 
     items: list[PlaylistFullJsonTracks]
@@ -448,11 +399,10 @@
 SpotifyEntityJson: TypeAlias = (
     AlbumSummaryJson
     | ArtistSummaryJson
     | ArtistFullJson
     | DeviceJson
     | PlaylistSummaryJson
     | TrackFullJson
-    | TrackLocalJson
     | UserSummaryJson
     | UserFullJson
 )
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-4.0.0/wg_utilities/clients/google_calendar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-# pylint: disable=too-few-public-methods
 """Custom client for interacting with Google's Calendar API."""
 from __future__ import annotations
 
-from collections.abc import Callable, Iterable, Mapping, Set
+from collections.abc import Iterable
 from datetime import date as date_
 from datetime import datetime as datetime_
 from datetime import timedelta, tzinfo
 from enum import Enum
-from typing import Any, Literal, TypeAlias, TypedDict, TypeVar
+from typing import Any, Literal, Self, TypeAlias
 
-from pydantic import Field, root_validator, validator
+from pydantic import Field, field_serializer, field_validator, model_validator
 from pytz import UTC, timezone
 from requests import delete
+from typing_extensions import NotRequired, TypedDict
 from tzlocal import get_localzone
 
 from wg_utilities.clients._google import GoogleClient
 from wg_utilities.clients.json_api_client import StrBytIntFlt
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    GenericModelWithConfig,
-)
+from wg_utilities.clients.oauth_client import BaseModelWithConfig
 
 
 class ResponseStatus(str, Enum):
     """Enumeration for event attendee response statuses."""
 
     ACCEPTED = "accepted"
     DECLINED = "declined"
@@ -36,20 +33,20 @@
     """Enumeration for event types."""
 
     DEFAULT = "default"
     FOCUS_TIME = "focusTime"
     OUT_OF_OFFICE = "outOfOffice"
 
 
-class _Attendee(BaseModelWithConfig):  # pylint: disable=too-few-public-methods
-    additionalGuests: int | None  # noqa: N815
-    comment: str | None
-    display_name: str | None = Field(alias="displayName", default=None)
+class _Attendee(BaseModelWithConfig):
+    additionalGuests: int | None = None  # noqa: N815
+    comment: str | None = None
+    display_name: str | None = Field(None, alias="displayName")
     email: str
-    id: str | None
+    id: str | None = None
     optional: bool = False
     organizer: bool = False
     resource: bool = False
     response_status: ResponseStatus = Field(
         alias="responseStatus", default=ResponseStatus.UNKNOWN
     )
     self: bool = False
@@ -85,28 +82,28 @@
     conferenceSolution: _ConferenceDataConferenceSolution
     conferenceId: str
     signature: str | None
     notes: str | None
     parameters: dict[str, object] | None
 
 
-class _Creator(BaseModelWithConfig):  # pylint: disable=too-few-public-methods
+class _Creator(BaseModelWithConfig):
     display_name: str | None = Field(alias="displayName", default=None)
     email: str
     self: bool = False
 
 
 class _StartEndDatetime(BaseModelWithConfig):
     """Model for `start` and `end` datetime objects."""
 
     datetime: datetime_ = Field(alias="dateTime")
     date: date_
     timezone: tzinfo = Field(alias="timeZone", default_factory=get_localzone)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def validate_datetime_or_date(  # pylint: disable=no-self-argument
         cls,  # noqa: N805
         values: dict[str, Any],
     ) -> dict[str, Any]:
         """Validate that either `datetime` or `date` is provided."""
 
         values["timeZone"] = (
@@ -129,14 +126,20 @@
             dttm = datetime_(dt.year, dt.month, dt.day, tzinfo=values["timeZone"])
 
         values["date"] = dt
         values["dateTime"] = dttm
 
         return values
 
+    @field_serializer("timezone", mode="plain", when_used="json", check_fields=True)
+    def serialize_timezone(self, tz: tzinfo) -> str:
+        """Serialize the timezone to a string."""
+
+        return tz.tzname(None) or ""
+
 
 class CalendarJson(TypedDict):
     """JSON representation of a Calendar."""
 
     description: str | None
     etag: str
     id: str
@@ -147,148 +150,43 @@
     timeZone: str
     conferenceProperties: dict[
         Literal["allowedConferenceSolutionTypes"],
         list[Literal["eventHangout", "eventNamedHangout", "hangoutsMeet"]],
     ]
 
 
-FJR = TypeVar("FJR", bound="GoogleCalendarEntity")
-
-
-class GoogleCalendarEntity(GenericModelWithConfig):
+class GoogleCalendarEntity(BaseModelWithConfig):
     """Base class for Google Calendar entities."""
 
-    description: str | None
+    description: str | None = None
     etag: str
     id: str
-    location: str | None
+    location: str | None = None
     summary: str
 
     google_client: GoogleCalendarClient = Field(exclude=True)
 
     @classmethod
     def from_json_response(
-        cls: type[FJR],
+        cls,
         value: GoogleCalendarEntityJson,
         google_client: GoogleCalendarClient,
         calendar: Calendar | None = None,
-        _waive_validation: bool = False,
-    ) -> FJR:
+    ) -> Self:
         """Create a Calendar/Event from a JSON response."""
 
         value_data: dict[str, Any] = {
             "google_client": google_client,
             **value,
         }
 
         if cls == Event:
             value_data["calendar"] = calendar
 
-        instance = cls.parse_obj(value_data)
-
-        if not _waive_validation:
-            instance._validate()  # pylint: disable=protected-access
-
-        return instance
-
-    def dict(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ) -> dict[str, Any]:
-        # pylint: disable=useless-parent-delegation
-        """Override the standard `BaseModel.dict` method.
-
-        Allows us to consistently return the dict with the same field names it came in
-        with, and exclude any null values that have been added when parsing.
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeldict
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-        """
-
-        return super().dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-        )
-
-    @staticmethod
-    def _json_encoder(o: Any) -> str:
-        """Custom-encode GoogleCalendarEntity JSON.
-
-        Args:
-            o (Any): object to encode
-
-        Returns:
-            str: encoded object
-        """
-
-        if isinstance(o, datetime_):
-            return o.isoformat()
-
-        if isinstance(o, tzinfo):
-            return o.tzname(None) or ""
-
-        return str(o)
-
-    def json(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: Callable[[Any], Any] | None = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
-        # pylint: disable=useless-parent-delegation
-        """Override the standard `BaseModel.json` method.
-
-        Allows us to consistently return the dict with the same field names it came in
-        with, and exclude any null values that have been added when parsing.
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeljson
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-            encoder: None -> self._json_encoder
-        """
-
-        return super().json(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-            encoder=encoder or self._json_encoder,
-            models_as_dict=models_as_dict,
-            **dumps_kwargs,
-        )
+        return cls.model_validate(value_data)
 
     def __eq__(self, other: Any) -> bool:
         """Compare two GoogleCalendarEntity objects by ID."""
         if not isinstance(other, type(self)):
             return NotImplemented
 
         return self.id == other.id
@@ -333,29 +231,36 @@
         Literal["notifications"],
         list[_Notification],
     ] = Field(
         alias="notificationSettings", default_factory=list  # type: ignore[assignment]
     )
     primary: bool = False
     selected: bool = False
-    summary_override: str | None = Field(alias="summaryOverride")
+    summary_override: str | None = Field(None, alias="summaryOverride")
     timezone: tzinfo = Field(alias="timeZone")
 
     # mypy can't get this type from the parent class for some reason...
     google_client: GoogleCalendarClient = Field(exclude=True)
 
-    @validator("timezone", pre=True)
+    @field_validator("timezone", mode="before")
     def validate_timezone(  # pylint: disable=no-self-argument
         cls, value: str  # noqa: N805
     ) -> tzinfo:
         """Convert the timezone string into a tzinfo object."""
         if isinstance(value, tzinfo):
             return value
+
         return timezone(value)
 
+    @field_serializer("timezone", mode="plain", when_used="json", check_fields=True)
+    def serialize_timezone(self, tz: tzinfo) -> str:
+        """Serialize the timezone to a string."""
+
+        return tz.tzname(None) or ""
+
     def get_event_by_id(self, event_id: str) -> Event:
         """Get an event by its ID.
 
         Args:
             event_id (str): ID of the event to get
 
         Returns:
@@ -433,15 +338,20 @@
         ]
 
     def __str__(self) -> str:
         """Return the calendar name."""
         return self.summary
 
 
-class EventJson(TypedDict):
+class _EventReminders(TypedDict):
+    useDefault: bool
+    overrides: NotRequired[list[_Reminder]]
+
+
+class EventJson(TypedDict, total=False):
     """JSON representation of an Event."""
 
     description: str | None
     etag: str
     id: str
     location: str | None
     summary: str | None
@@ -466,63 +376,65 @@
     kind: Literal["calendar#event"]
     locked: bool | None
     organizer: dict[str, bool | str]
     original_start_time: dict[str, str] | None
     privateCopy: bool | None
     recurrence: list[str] | None
     recurringEventId: str | None
-    reminders: dict[str, bool | dict[str, str | int]]
+    reminders: _EventReminders | None
     sequence: int
     source: dict[str, str] | None
     start: _StartEndDatetime
     status: Literal["cancelled", "confirmed", "tentative"] | None
     transparency: str | None
     updated: datetime_
     visibility: Literal["default", "public", "private", "confidential"] | None
 
 
 class Event(GoogleCalendarEntity):
     """Class for Google Calendar events."""
 
     summary: str = "(No Title)"
 
-    attachments: list[dict[str, str]] | None
+    attachments: list[dict[str, str]] | None = None
     attendees: list[_Attendee] = Field(default_factory=list)
-    attendees_omitted: bool | None = Field(alias="attendeesOmitted")
+    attendees_omitted: bool | None = Field(None, alias="attendeesOmitted")
     created: datetime_
-    color_id: str | None = Field(alias="colorId")
-    conference_data: _ConferenceData | None = Field(alias="conferenceData")
+    color_id: str | None = Field(None, alias="colorId")
+    conference_data: _ConferenceData | None = Field(None, alias="conferenceData")
     creator: _Creator
     end: _StartEndDatetime
-    end_time_unspecified: bool | None = Field(alias="endTimeUnspecified")
+    end_time_unspecified: bool | None = Field(None, alias="endTimeUnspecified")
     event_type: EventType = Field(alias="eventType")
     extended_properties: dict[str, dict[str, str]] | None = Field(
-        alias="extendedProperties"
+        None, alias="extendedProperties"
+    )
+    guests_can_invite_others: bool | None = Field(None, alias="guestsCanInviteOthers")
+    guests_can_modify: bool | None = Field(None, alias="guestsCanModify")
+    guests_can_see_other_guests: bool | None = Field(
+        None, alias="guestsCanSeeOtherGuests"
     )
-    guests_can_invite_others: bool | None = Field(alias="guestsCanInviteOthers")
-    guests_can_modify: bool | None = Field(alias="guestsCanModify")
-    guests_can_see_other_guests: bool | None = Field(alias="guestsCanSeeOtherGuests")
-    hangout_link: str | None = Field(alias="hangoutLink")
+    hangout_link: str | None = Field(None, alias="hangoutLink")
     html_link: str = Field(alias="htmlLink")
     ical_uid: str = Field(alias="iCalUID")
     kind: Literal["calendar#event"]
-    locked: bool | None
+    locked: bool | None = None
     organizer: dict[str, bool | str]
-    original_start_time: dict[str, str] | None = Field(alias="originalStartTime")
-    private_copy: bool | None = Field(alias="privateCopy")
-    recurrence: list[str] | None
-    recurring_event_id: str | None = Field(alias="recurringEventId")
-    reminders: dict[str, bool | dict[str, str | int]]
+    original_start_time: dict[str, str] | None = Field(None, alias="originalStartTime")
+    private_copy: bool | None = Field(None, alias="privateCopy")
+    recurrence: list[str] | None = None
+    recurring_event_id: str | None = Field(None, alias="recurringEventId")
+    reminders: _EventReminders | None = None
     sequence: int
-    source: dict[str, str] | None
+    source: dict[str, str] | None = None
     start: _StartEndDatetime
-    status: Literal["cancelled", "confirmed", "tentative"] | None
-    transparency: str | None  # != transparent
+    status: Literal["cancelled", "confirmed", "tentative"] | None = None
+    transparency: str | None = None  # != transparent
     updated: datetime_
-    visibility: Literal["default", "public", "private", "confidential"] | None
+    visibility: Literal["default", "public", "private", "confidential"] | None = None
 
     calendar: Calendar
 
     def delete(self) -> None:
         """Delete the event from the host calendar."""
         self.google_client.delete_event_by_id(event_id=self.id, calendar=self.calendar)
 
@@ -731,9 +643,9 @@
                 ),
                 google_client=self,
             )
 
         return self._primary_calendar
 
 
-Calendar.update_forward_refs()
-Event.update_forward_refs()
+Calendar.model_rebuild()
+Event.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/google_drive.py` & `wg_utilities-4.0.0/wg_utilities/clients/google_drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# pylint: disable=too-few-public-methods,too-many-lines,no-self-argument
+# pylint: disable=too-many-lines,no-self-argument
 """Custom client for interacting with Google's Drive API."""
 from __future__ import annotations
 
-from collections.abc import Callable, Mapping, Set
+from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from datetime import date, datetime
 from enum import Enum
 from pathlib import Path
 from re import sub
-from typing import Any, ClassVar, Literal, TypeVar
+from typing import Any, ClassVar, Literal, Self, TypeVar
 
-from pydantic import Field, validator
+from pydantic import Field, FieldValidationInfo, PrivateAttr, field_validator
 
 from wg_utilities.clients._google import GoogleClient
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    GenericModelWithConfig,
-)
+from wg_utilities.clients.json_api_client import StrBytIntFlt
+from wg_utilities.clients.oauth_client import BaseModelWithConfig
 from wg_utilities.functions.json import JSONObj
 
 
 class EntityKind(str, Enum):
     """Enum for the different kinds of entities that can be returned by the API."""
 
     COMMENT = "drive#comment"
@@ -49,41 +47,41 @@
 
 class _ImageMediaMetadata(BaseModelWithConfig):
     width: int
     height: int
     rotation: int | None
     location: dict[str, float] = {}
     time: str | None
-    camera_make: str | None = Field(alias="cameraMake")
-    camera_model: str | None = Field(alias="cameraModel")
-    exposure_time: float | None = Field(alias="exposureTime")
+    camera_make: str | None = Field(None, alias="cameraMake")
+    camera_model: str | None = Field(None, alias="cameraModel")
+    exposure_time: float | None = Field(None, alias="exposureTime")
     aperture: float | None
-    flash_used: bool | None = Field(alias="flashUsed")
-    focal_length: float | None = Field(alias="focalLength")
-    iso_speed: int | None = Field(alias="isoSpeed")
-    metering_mode: str | None = Field(alias="meteringMode")
+    flash_used: bool | None = Field(None, alias="flashUsed")
+    focal_length: float | None = Field(None, alias="focalLength")
+    iso_speed: int | None = Field(None, alias="isoSpeed")
+    metering_mode: str | None = Field(None, alias="meteringMode")
     sensor: str | None
-    exposure_mode: str | None = Field(alias="exposureMode")
-    color_space: str | None = Field(alias="colorSpace")
-    white_balance: str | None = Field(alias="whiteBalance")
-    exposure_bias: float | None = Field(alias="exposureBias")
-    max_aperture_value: float | None = Field(alias="maxApertureValue")
-    subject_distance: int | None = Field(alias="subjectDistance")
+    exposure_mode: str | None = Field(None, alias="exposureMode")
+    color_space: str | None = Field(None, alias="colorSpace")
+    white_balance: str | None = Field(None, alias="whiteBalance")
+    exposure_bias: float | None = Field(None, alias="exposureBias")
+    max_aperture_value: float | None = Field(None, alias="maxApertureValue")
+    subject_distance: int | None = Field(None, alias="subjectDistance")
     lens: str | None
 
 
 class _Label(BaseModelWithConfig):
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.LABEL)
+    kind: EntityKind = Field(alias="kind", default=EntityKind.LABEL)
     id: str
     revision_id: str = Field(alias="revisionId")
     fields: dict[str, _LabelField]
 
 
 class _LabelField(BaseModelWithConfig):
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.USER)
+    kind: EntityKind = Field(alias="kind", default=EntityKind.USER)
     id: str
     value_type: str = Field(alias="valueType")
     date_str: list[date] = Field(alias="datestr", default_factory=list)
     integer: list[float]
     selection: list[str]
     text: list[str]
     user: list[_User]
@@ -93,32 +91,34 @@
     permission_type: str = Field(alias="permissionType")
     role: str
     inherited_from: str = Field(alias="inheritedFrom")
     inherited: bool
 
 
 class _Permission(BaseModelWithConfig):
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.PERMISSION)
+    kind: EntityKind = Field(alias="kind", default=EntityKind.PERMISSION)
     id: str
     type: str
-    email_address: str | None = Field(alias="emailAddress")
-    domain: str | None
+    email_address: str | None = Field(None, alias="emailAddress")
+    domain: str | None = None
     role: str
-    view: str | None
-    allow_file_discovery: bool | None = Field(alias="allowFileDiscovery")
-    display_name: str | None = Field(alias="displayName")
-    photo_link: str | None = Field(alias="photoLink")
-    expiration_time: datetime | None = Field(alias="expirationTime")
-    permission_details: _PermissionDetails | None = Field(alias="permissionDetails")
-    deleted: bool | None
-    pending_owner: bool | None = Field(alias="pendingOwner")
+    view: str | None = None
+    allow_file_discovery: bool | None = Field(None, alias="allowFileDiscovery")
+    display_name: str | None = Field(None, alias="displayName")
+    photo_link: str | None = Field(None, alias="photoLink")
+    expiration_time: datetime | None = Field(None, alias="expirationTime")
+    permission_details: _PermissionDetails | None = Field(
+        None, alias="permissionDetails"
+    )
+    deleted: bool | None = None
+    pending_owner: bool | None = Field(None, alias="pendingOwner")
 
 
 class _User(BaseModelWithConfig):
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.USER)
+    kind: EntityKind = Field(alias="kind", default=EntityKind.USER)
     display_name: str = Field(alias="displayName")
     photo_link: str = Field(alias="photoLink")
     me: bool
     permission_id: str = Field(alias="permissionId")
     email_address: str = Field(alias="emailAddress")
 
 
@@ -137,33 +137,32 @@
     read_only: bool = Field(alias="readOnly")
     reason: str
     restricting_user: _User = Field(alias="restrictingUser")
     restriction_time: datetime = Field(alias="restrictionTime")
     type: str
 
 
-class _GoogleDriveEntity(GenericModelWithConfig):
+class _GoogleDriveEntity(BaseModelWithConfig):
     """Base class for Google Drive entities."""
 
     id: str
     name: str
     mime_type: str = Field(alias="mimeType")
 
     google_client: GoogleDriveClient = Field(exclude=True)
 
     @classmethod
     def from_json_response(
-        cls: type[FJR],
+        cls,
         value: Mapping[str, Any],
         google_client: GoogleDriveClient,
         host_drive: Drive | None = None,
         parent: _CanHaveChildren | Drive | Directory | None = None,
         _block_describe_call: bool = False,
-        _waive_validation: bool = False,
-    ) -> FJR:
+    ) -> Self:
         """Create a new instance from a JSON response.
 
         Args:
             value (dict): The JSON response.
             google_client (GoogleDriveClient): The Google Drive client.
             host_drive (Drive): The Drive that this entity belongs to.
             parent (Directory, optional): The parent directory.
@@ -175,18 +174,15 @@
         value_data: dict[str, Any] = {
             "google_client": google_client,
             "parent_": parent,
             "host_drive_": host_drive,
             **value,
         }
 
-        instance = cls.parse_obj(value_data)
-
-        if not _waive_validation:
-            instance._validate()  # pylint: disable=protected-access
+        instance = cls.model_validate(value_data)
 
         if isinstance(instance, File | Directory):
             if parent is not None:
                 parent.add_child(instance)
             elif host_drive is not None and host_drive.id == instance.parents[0]:
                 instance.parent_ = host_drive
                 host_drive.add_child(instance)
@@ -196,91 +192,14 @@
             and google_client.item_metadata_retrieval == IMR.ON_INIT
             and hasattr(instance, "describe")
         ):
             instance.describe()
 
         return instance
 
-    def dict(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ) -> dict[str, Any]:
-        # pylint: disable=useless-parent-delegation
-        """Override the standard `BaseModel.dict` method.
-
-        Allows us to consistently return the dict with the same field names it came in
-        with, and exclude any null values that have been added when parsing.
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeldict
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-        """
-
-        return super().dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-        )
-
-    def json(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: Callable[[Any], Any] | None = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
-        # pylint: disable=useless-parent-delegation
-        """Override the standard `BaseModel.json` method.
-
-        Allows us to consistently return the dict with the same field names it came in
-        with, and exclude any null values that have been added when parsing.
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeljson
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-            encoder: None -> self._json_encoder
-        """
-
-        return super().json(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-            encoder=encoder,
-            models_as_dict=models_as_dict,
-            **dumps_kwargs,
-        )
-
     @property
     def host_drive(self) -> Drive:
         """The drive that this directory is hosted on.
 
         Returns:
             Drive: the drive that this directory is hosted on
 
@@ -321,19 +240,19 @@
         """Return the file name."""
         return self.name
 
 
 class _CanHaveChildren(_GoogleDriveEntity):
     """Mixin for entities that can have children."""
 
-    _directories: list[Directory] = Field(exclude=True, default_factory=list)
-    _files: list[File] = Field(exclude=True, default_factory=list)
+    _directories: list[Directory] = PrivateAttr(default_factory=list)
+    _files: list[File] = PrivateAttr(default_factory=list)
 
-    _files_loaded: bool = Field(exclude=True, default=False)
-    _directories_loaded: bool = Field(exclude=True, default=False)
+    _files_loaded: bool = False
+    _directories_loaded: bool = False
 
     def _add_directory(self, directory: Directory) -> None:
         """Add a child directory to this directory's children record.
 
         Args:
             directory (Directory): the directory to add
 
@@ -343,21 +262,22 @@
         if not isinstance(directory, Directory):
             raise TypeError(
                 f"Cannot add `{directory.__class__.__name__}` instance to "
                 "`self.directories`."
             )
 
         if not isinstance(self._directories, list):
-            self._set_private_attr("_directories", [directory])
+            self._directories = [directory]
         elif directory not in self._directories:
             self._directories.append(directory)
 
-        if hasattr(self, "_all_directories"):
+        if isinstance(self, Drive):
+            # pylint: disable=access-member-before-definition,attribute-defined-outside-init
             if not isinstance(self._all_directories, list):
-                self._set_private_attr("_all_directories", [directory])
+                self._all_directories = [directory]
             elif directory not in self._all_directories:
                 self._all_directories.append(directory)
 
     def _add_file(self, file: File) -> None:
         """Add a file to this directory's files record.
 
         Args:
@@ -373,21 +293,22 @@
             # Liskov substitution principle, you should be able to process a Directory
             # as a File, but that would be illogical here.
             raise TypeError(
                 f"Cannot add `{file.__class__.__name__}` instance to `self.files`."
             )
 
         if not isinstance(self._files, list):
-            self._set_private_attr("_files", [file])
+            self._files = [file]
         elif file not in self._files:
             self._files.append(file)
 
-        if hasattr(self, "_all_files"):
+        if isinstance(self, Drive):
+            # pylint: disable=access-member-before-definition,attribute-defined-outside-init
             if not isinstance(self._all_files, list):
-                self._set_private_attr("_all_files", [file])
+                self._all_files = [file]
             elif file not in self._all_files:
                 self._all_files.append(file)
 
     def add_child(self, child: File | Directory) -> None:
         """Add a child to this directory's children record."""
 
         if isinstance(child, Directory):
@@ -495,18 +416,18 @@
                 return file
             case _:  # pragma: no cover
                 # I haven't found a way to trigger this but have kept it just in case
                 raise ValueError(f"Unprocessable path: {path!r}")
 
     def reset_known_children(self) -> None:
         """Reset the list of known children."""
-        self._set_private_attr("_directories", None)
-        self._set_private_attr("_directories_loaded", False)
-        self._set_private_attr("_files", None)
-        self._set_private_attr("_files_loaded", False)
+        self._directories = []
+        self._directories_loaded = False
+        self._files = []
+        self._files_loaded = False
 
     def tree(self, local_only: bool = False, include_files: bool = False) -> str:
         """Emulate the Linux `tree` command output.
 
         This builds a directory tree in text form for quick visualisation. Not really
         intended for use in production, but useful for debugging.
 
@@ -587,18 +508,18 @@
         No HTTP requests are made to get these children, so this may not be an
         exhaustive list.
 
         Returns:
             list[Directory | File]: The list of children.
         """
         if not isinstance(self._directories, list):
-            self._set_private_attr("_directories", [])
+            self._directories = []
 
         if not isinstance(self._files, list):
-            self._set_private_attr("_files", [])
+            self._files = []
 
         return self._files + self._directories  # type: ignore[operator]
 
     @property
     def children(self) -> list[Directory | File]:
         """Get all immediate children of this Drive/Directory.
 
@@ -624,40 +545,37 @@
                 if self.google_client.item_metadata_retrieval == IMR.ON_INIT
                 else "id, name, parents, mimeType, kind"
             )
 
             # TODO: this needs to be changed to only get *new* folders - currently this
             #   will overwrite any known children, including all metadata ad further
             #   descendents
-            self._set_private_attr(
-                "_directories",
-                sorted(
-                    [
-                        Directory.from_json_response(
-                            directory,
-                            google_client=self.google_client,
-                            parent=self,
-                            host_drive=self.host_drive,
-                            _block_describe_call=True,
-                        )
-                        for directory in self.google_client.get_items(
-                            "/files",
-                            list_key="files",
-                            params={
-                                "pageSize": 1000,
-                                "q": f"mimeType = '{Directory.MIME_TYPE}'"
-                                f" and '{self.id}' in parents",
-                                "fields": f"nextPageToken, files({file_fields})",
-                            },
-                        )
-                    ]
-                ),
+            self._directories = sorted(
+                [
+                    Directory.from_json_response(
+                        directory,
+                        google_client=self.google_client,
+                        parent=self,
+                        host_drive=self.host_drive,
+                        _block_describe_call=True,
+                    )
+                    for directory in self.google_client.get_items(
+                        "/files",
+                        list_key="files",
+                        params={
+                            "pageSize": 1000,
+                            "q": f"mimeType = '{Directory.MIME_TYPE}'"
+                            f" and '{self.id}' in parents",
+                            "fields": f"nextPageToken, files({file_fields})",
+                        },
+                    )
+                ]
             )
 
-            self._set_private_attr("_directories_loaded", True)
+            self._directories_loaded = True
 
         return self._directories
 
     @property
     def files(self) -> list[File]:
         """The files contained within this directory.
 
@@ -667,123 +585,125 @@
         if self._files_loaded is not True:
             file_fields = (
                 "*"
                 if self.google_client.item_metadata_retrieval == IMR.ON_INIT
                 else "id, name, parents, mimeType, kind"
             )
 
-            self._set_private_attr(
-                "_files",
-                [
-                    File.from_json_response(
-                        item,
-                        google_client=self.google_client,
-                        parent=self,
-                        host_drive=self.host_drive,
-                        _block_describe_call=True,
-                    )
-                    for item in self.google_client.get_items(
-                        "/files",
-                        list_key="files",
-                        params={
-                            "pageSize": 1000,
-                            "q": f"mimeType != '{Directory.MIME_TYPE}' and"
-                            f" '{self.id}' in parents",
-                            "fields": f"nextPageToken, files({file_fields})",
-                        },
-                    )
-                ],
-            )
-            self._set_private_attr("_files_loaded", True)
+            self._files = [
+                File.from_json_response(
+                    item,
+                    google_client=self.google_client,
+                    parent=self,
+                    host_drive=self.host_drive,
+                    _block_describe_call=True,
+                )
+                for item in self.google_client.get_items(
+                    "/files",
+                    list_key="files",
+                    params={
+                        "pageSize": 1000,
+                        "q": f"mimeType != '{Directory.MIME_TYPE}' and"
+                        f" '{self.id}' in parents",
+                        "fields": f"nextPageToken, files({file_fields})",
+                    },
+                )
+            ]
+
+            self._files_loaded = True
 
         return list(self._files)
 
 
 class File(_GoogleDriveEntity):
     """A file object within Google Drive."""
 
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.FILE)
+    kind: EntityKind = Field(alias="kind", default=EntityKind.FILE)
 
     # Optional, can be retrieved with the `describe` method or by getting the attribute
     app_properties: dict[str, str] = {}
-    capabilities: _DriveCapabilities | None
-    content_hints: _ContentHints | None = Field(alias="contentHints")
+    capabilities: _DriveCapabilities | None = None
+    content_hints: _ContentHints | None = Field(None, alias="contentHints")
     content_restrictions: list[_ContentRestriction] | None = Field(
-        alias="contentRestrictions"
+        None, alias="contentRestrictions"
     )
     copy_requires_writer_permission: bool | None = Field(
-        alias="copyRequiresWriterPermission"
+        None, alias="copyRequiresWriterPermission"
     )
-    created_time: datetime | None = Field(alias="createdTime")
-    description: str | None
-    drive_id: str | None = Field(alias="driveId")
-    explicitly_trashed: bool | None = Field(alias="explicitlyTrashed")
+    created_time: datetime | None = Field(None, alias="createdTime")
+    description: str | None = None
+    drive_id: str | None = Field(None, alias="driveId")
+    explicitly_trashed: bool | None = Field(None, alias="explicitlyTrashed")
     export_links: dict[str, str] = Field(alias="exportLinks", default_factory=dict)
-    folder_color_rgb: str | None = Field(alias="folderColorRgb")
-    file_extension: str | None = Field(alias="fileExtension")
-    full_file_extension: str | None = Field(alias="fullFileExtension")
-    has_augmented_permissions: bool | None = Field(alias="hasAugmentedPermissions")
-    has_thumbnail: bool | None = Field(alias="hasThumbnail")
-    head_revision_id: str | None = Field(alias="headRevisionId")
-    icon_link: str | None = Field(alias="iconLink")
-    image_media_metadata: _ImageMediaMetadata | None = Field(alias="imageMediaMetadata")
-    is_app_authorized: bool | None = Field(alias="isAppAuthorized")
+    folder_color_rgb: str | None = Field(None, alias="folderColorRgb")
+    file_extension: str | None = Field(None, alias="fileExtension")
+    full_file_extension: str | None = Field(None, alias="fullFileExtension")
+    has_augmented_permissions: bool | None = Field(
+        None, alias="hasAugmentedPermissions"
+    )
+    has_thumbnail: bool | None = Field(None, alias="hasThumbnail")
+    head_revision_id: str | None = Field(None, alias="headRevisionId")
+    icon_link: str | None = Field(None, alias="iconLink")
+    image_media_metadata: _ImageMediaMetadata | None = Field(
+        None, alias="imageMediaMetadata"
+    )
+    is_app_authorized: bool | None = Field(None, alias="isAppAuthorized")
     label_info: dict[Literal["labels"], list[_Label]] = Field(
         alias="labelInfo", default_factory=dict
     )
-    last_modifying_user: _User | None = Field(alias="lastModifyingUser")
+    last_modifying_user: _User | None = Field(None, alias="lastModifyingUser")
     link_share_metadata: dict[
         Literal["securityUpdateEligible", "securityUpdateEnabled"], bool
     ] = Field(alias="linkShareMetadata", default_factory=dict)
-    md5_checksum: str | None = Field(alias="md5Checksum")
-    modified_by_me: bool | None = Field(alias="modifiedByMe")
-    modified_by_me_time: datetime | None = Field(alias="modifiedByMeTime")
-    modified_time: datetime | None = Field(alias="modifiedTime")
-    original_filename: str | None = Field(alias="originalFilename")
-    owned_by_me: bool | None = Field(alias="ownedByMe")
+    md5_checksum: str | None = Field(None, alias="md5Checksum")
+    modified_by_me: bool | None = Field(None, alias="modifiedByMe")
+    modified_by_me_time: datetime | None = Field(None, alias="modifiedByMeTime")
+    modified_time: datetime | None = Field(None, alias="modifiedTime")
+    original_filename: str | None = Field(None, alias="originalFilename")
+    owned_by_me: bool | None = Field(None, alias="ownedByMe")
     owners: list[_User] = []
     parents: list[str]
     properties: dict[str, str] = {}
     permissions: list[_Permission] = []
     permission_ids: list[str] = Field(alias="permissionIds", default_factory=list)
-    quota_bytes_used: float | None = Field(alias="quotaBytesUsed")
-    resource_key: str | None = Field(alias="resourceKey")
-    shared: bool | None
-    sha1_checksum: str | None = Field(alias="sha1Checksum")
-    sha256_checksum: str | None = Field(alias="sha256Checksum")
-    shared_with_me_time: datetime | None = Field(alias="sharedWithMeTime")
-    sharing_user: _User | None = Field(alias="sharingUser")
+    quota_bytes_used: float | None = Field(None, alias="quotaBytesUsed")
+    resource_key: str | None = Field(None, alias="resourceKey")
+    shared: bool | None = None
+    sha1_checksum: str | None = Field(None, alias="sha1Checksum")
+    sha256_checksum: str | None = Field(None, alias="sha256Checksum")
+    shared_with_me_time: datetime | None = Field(None, alias="sharedWithMeTime")
+    sharing_user: _User | None = Field(None, alias="sharingUser")
     shortcut_details: dict[
         Literal[
             "targetId",
             "targetMimeType",
             "targetResourceKey",
         ],
         str,
     ] = Field(alias="shortcutDetails", default_factory=dict)
-    size: float | None
+    size: float | None = None
     spaces: list[str] = []
-    starred: bool | None
-    thumbnail_link: str | None = Field(alias="thumbnailLink")
-    thumbnail_version: int | None = Field(alias="thumbnailVersion")
-    trashed: bool | None
-    trashed_time: datetime | None = Field(alias="trashedTime")
-    trashing_user: _User | None = Field(alias="trashingUser")
-    version: int | None
-    video_media_metadata: _VideoMediaMetadata | None = Field(alias="videoMediaMetadata")
-    viewed_by_me: bool | None = Field(alias="viewedByMe")
-    viewed_by_me_time: datetime | None = Field(alias="viewedByMeTime")
-    viewers_can_copy_content: bool | None = Field(alias="viewersCanCopyContent")
-    web_content_link: str | None = Field(alias="webContentLink")
-    web_view_link: str | None = Field(alias="webViewLink")
-    writers_can_share: bool | None = Field(alias="writersCanShare")
-
-    _description: dict[str, str | bool | float | int] = Field(
-        exclude=True,
+    starred: bool | None = None
+    thumbnail_link: str | None = Field(None, alias="thumbnailLink")
+    thumbnail_version: int | None = Field(None, alias="thumbnailVersion")
+    trashed: bool | None = None
+    trashed_time: datetime | None = Field(None, alias="trashedTime")
+    trashing_user: _User | None = Field(None, alias="trashingUser")
+    version: int | None = None
+    video_media_metadata: _VideoMediaMetadata | None = Field(
+        None, alias="videoMediaMetadata"
     )
+    viewed_by_me: bool | None = Field(None, alias="viewedByMe")
+    viewed_by_me_time: datetime | None = Field(None, alias="viewedByMeTime")
+    viewers_can_copy_content: bool | None = Field(None, alias="viewersCanCopyContent")
+    web_content_link: str | None = Field(None, alias="webContentLink")
+    web_view_link: str | None = Field(None, alias="webViewLink")
+    writers_can_share: bool | None = Field(None, alias="writersCanShare")
+
+    _description: JSONObj = PrivateAttr(default_factory=dict)
     host_drive_: Drive = Field(exclude=True)
     parent_: Directory | Drive | None = Field(exclude=True)
 
     def __getattribute__(self, name: str) -> Any:
         """Override the default `__getattribute__` to allow for lazy metadata loading.
 
         Args:
@@ -791,85 +711,83 @@
 
         Returns:
             Any: The value of the attribute.
         """
 
         # If the attribute isn't a field, just return the value
         if (
-            (name.startswith("__") and name.endswith("__"))
-            or name not in self.__fields__
-            or self.__fields__[name].field_info.exclude is True
+            name in ("model_fields", "model_fields_set")
+            or name not in self.model_fields
+            or self.model_fields[name].exclude
         ):
             return super().__getattribute__(name)
 
-        if name not in self.__fields_set__ or not super().__getattribute__(name):
+        if name not in self.model_fields_set or not super().__getattribute__(name):
             # If IMR is enabled, load all metadata
             if self.google_client.item_metadata_retrieval == IMR.ON_FIRST_REQUEST:
                 self.describe()
                 return super().__getattribute__(name)
 
             # Otherwise just get the single field
-            google_key = self.__fields__[name].alias or name
+            google_key = self.model_fields[name].alias or name
 
             res = self.google_client.get_json_response(
                 f"/files/{self.id}",
                 params={"fields": google_key, "pageSize": None},
             )
             setattr(self, name, res.pop(google_key, None))
 
             # I can't just return the value of `res.pop(google_key, None)` here because
             # it needs to go through Pydantic's validators first
 
         return super().__getattribute__(name)
 
-    @validator("mime_type")
+    @field_validator("mime_type")
     def _validate_mime_type(cls, mime_type: str) -> str:  # noqa: N805
         if mime_type == Directory.MIME_TYPE:
             raise ValueError("Use `Directory` class to create a directory.")
 
         return mime_type
 
-    @validator("parents")
+    @field_validator("parents")
     def _validate_parents(cls, parents: list[str]) -> list[str]:  # noqa: N805
         if len(parents) != 1:
             raise ValueError(f"A {cls.__name__} must have exactly one parent.")
 
         return parents
 
-    @validator("parent_")
+    @field_validator("parent_")
     def _validate_parent_instance(
-        cls, value: Directory | Drive | None, values: dict[str, Any]  # noqa: N805
+        cls, value: Directory | Drive | None, info: FieldValidationInfo  # noqa: N805
     ) -> Directory | Drive | None:
         """Validate that the parent instance's ID matches the expected parent ID.
 
         Args:
             value (Directory, Drive): The parent instance.
-            values (dict): The values of the other fields
+            info (FieldValidationInfo): Object for extra validation information/data.
 
         Returns:
             Directory, Drive: The parent instance.
 
         Raises:
             ValueError: If the parent instance's ID doesn't match the expected parent
                 ID.
         """
 
         if value is None:
             return value
 
-        if value.id != values["parents"][0]:
+        if value.id != info.data["parents"][0]:
             raise ValueError(
-                f"Parent ID mismatch: {value.id} != {values['parents'][0]}"
+                f"Parent ID mismatch: {value.id} != {info.data['parents'][0]}"
             )
 
         return value
 
-    def describe(
-        self, force_update: bool = False
-    ) -> dict[str, str | bool | float | int]:
+    def describe(self, force_update: bool = False) -> JSONObj:
         """Describe the file by requesting all available fields from the Drive API.
 
         Args:
             force_update (bool): re-pull the description from Google Drive, even if we
              already have the description locally
 
         Returns:
@@ -879,21 +797,19 @@
             ValueError: if an unexpected field is returned from the Google Drive API.
         """
 
         if (
             force_update
             or not hasattr(self, "_description")
             or not isinstance(self._description, dict)
+            or not self._description
         ):
-            self._set_private_attr(
-                "_description",
-                self.google_client.get_json_response(
-                    f"/files/{self.id}",
-                    params={"fields": "*", "pageSize": None},
-                ),
+            self._description = self.google_client.get_json_response(
+                f"/files/{self.id}",
+                params={"fields": "*", "pageSize": None},
             )
 
             for key, value in self._description.items():
                 google_key = sub("([A-Z])", r"_\1", key).lower()
 
                 try:
                     setattr(self, google_key, value)
@@ -938,103 +854,113 @@
 class Directory(File, _CanHaveChildren):
     """A Google Drive directory - basically a File with extended functionality."""
 
     MIME_TYPE: ClassVar[
         Literal["application/vnd.google-apps.folder"]
     ] = "application/vnd.google-apps.folder"
 
-    kind: EntityKind = Field(default=EntityKind.DIRECTORY, const=True)
+    kind: Literal[EntityKind.DIRECTORY] = Field(default=EntityKind.DIRECTORY)
     mime_type: Literal["application/vnd.google-apps.folder"] = Field(
-        alias="mimeType", const=True, default=MIME_TYPE
+        alias="mimeType", default=MIME_TYPE
     )
 
     host_drive_: Drive = Field(exclude=True)
 
-    @validator("kind", always=True, pre=True)
+    @field_validator("kind", mode="before")
     def _validate_kind(cls, value: str | None) -> str:  # noqa: N805
         """Set the kind to "drive#folder"."""
 
         # Directories are just a subtype of files, so `"drive#file"` is okay too
         if value not in (EntityKind.DIRECTORY, EntityKind.FILE):
             raise ValueError(f"Invalid kind for Directory: {value}")
 
-        return "drive#folder"
+        return EntityKind.DIRECTORY
 
-    @validator("mime_type")
+    @field_validator("mime_type")
     def _validate_mime_type(cls, mime_type: str) -> str:  # noqa: N805
         """Just an override for the parent class's validator."""
 
         return mime_type
 
     def __repr__(self) -> str:
         """Return a string representation of the directory."""
         return f"Directory(id={self.id!r}, name={self.name!r})"
 
 
 class _DriveCapabilities(BaseModelWithConfig):
-    can_accept_ownership: bool | None = Field(alias="canAcceptOwnership")
-    can_add_children: bool | None = Field(alias="canAddChildren")
+    can_accept_ownership: bool | None = Field(None, alias="canAcceptOwnership")
+    can_add_children: bool | None = Field(None, alias="canAddChildren")
     can_add_folder_from_another_drive: bool | None = Field(
-        alias="canAddFolderFromAnotherDrive"
+        None, alias="canAddFolderFromAnotherDrive"
     )
-    can_add_my_drive_parent: bool | None = Field(alias="canAddMyDriveParent")
+    can_add_my_drive_parent: bool | None = Field(None, alias="canAddMyDriveParent")
     can_change_copy_requires_writer_permission: bool | None = Field(
-        alias="canChangeCopyRequiresWriterPermission"
+        None, alias="canChangeCopyRequiresWriterPermission"
     )
     can_change_copy_requires_writer_permission_restriction: bool | None = Field(
-        alias="canChangeCopyRequiresWriterPermissionRestriction"
+        None, alias="canChangeCopyRequiresWriterPermissionRestriction"
     )
     can_change_domain_users_only_restriction: bool | None = Field(
-        alias="canChangeDomainUsersOnlyRestriction"
+        None, alias="canChangeDomainUsersOnlyRestriction"
+    )
+    can_change_drive_background: bool | None = Field(
+        None, alias="canChangeDriveBackground"
     )
-    can_change_drive_background: bool | None = Field(alias="canChangeDriveBackground")
     can_change_drive_members_only_restriction: bool | None = Field(
-        alias="canChangeDriveMembersOnlyRestriction"
+        None, alias="canChangeDriveMembersOnlyRestriction"
     )
     can_change_security_update_enabled: bool | None = Field(
-        alias="canChangeSecurityUpdateEnabled"
+        None, alias="canChangeSecurityUpdateEnabled"
     )
     can_change_viewers_can_copy_content: bool | None = Field(
-        alias="canChangeViewersCanCopyContent"
+        None, alias="canChangeViewersCanCopyContent"
     )
-    can_comment: bool | None = Field(alias="canComment")
-    can_copy: bool | None = Field(alias="canCopy")
-    can_delete: bool | None = Field(alias="canDelete")
-    can_delete_children: bool | None = Field(alias="canDeleteChildren")
-    can_delete_drive: bool | None = Field(alias="canDeleteDrive")
-    can_download: bool | None = Field(alias="canDownload")
-    can_edit: bool | None = Field(alias="canEdit")
-    can_list_children: bool | None = Field(alias="canListChildren")
-    can_manage_members: bool | None = Field(alias="canManageMembers")
-    can_modify_content: bool | None = Field(alias="canModifyContent")
+    can_comment: bool | None = Field(None, alias="canComment")
+    can_copy: bool | None = Field(None, alias="canCopy")
+    can_delete: bool | None = Field(None, alias="canDelete")
+    can_delete_children: bool | None = Field(None, alias="canDeleteChildren")
+    can_delete_drive: bool | None = Field(None, alias="canDeleteDrive")
+    can_download: bool | None = Field(None, alias="canDownload")
+    can_edit: bool | None = Field(None, alias="canEdit")
+    can_list_children: bool | None = Field(None, alias="canListChildren")
+    can_manage_members: bool | None = Field(None, alias="canManageMembers")
+    can_modify_content: bool | None = Field(None, alias="canModifyContent")
     can_modify_content_restriction: bool | None = Field(
-        alias="canModifyContentRestriction"
+        None, alias="canModifyContentRestriction"
     )
-    can_modify_labels: bool | None = Field(alias="canModifyLabels")
+    can_modify_labels: bool | None = Field(None, alias="canModifyLabels")
     can_move_children_out_of_drive: bool | None = Field(
-        alias="canMoveChildrenOutOfDrive"
+        None, alias="canMoveChildrenOutOfDrive"
     )
     can_move_children_within_drive: bool | None = Field(
-        alias="canMoveChildrenWithinDrive"
+        None, alias="canMoveChildrenWithinDrive"
+    )
+    can_move_item_into_team_drive: bool | None = Field(
+        None, alias="canMoveItemIntoTeamDrive"
     )
-    can_move_item_into_team_drive: bool | None = Field(alias="canMoveItemIntoTeamDrive")
-    can_move_item_out_of_drive: bool | None = Field(alias="canMoveItemOutOfDrive")
-    can_move_item_within_drive: bool | None = Field(alias="canMoveItemWithinDrive")
-    can_read_labels: bool | None = Field(alias="canReadLabels")
-    can_read_revisions: bool = Field(alias="canReadRevisions")
-    can_read_drive: bool | None = Field(alias="canReadDrive")
-    can_remove_children: bool | None = Field(alias="canRemoveChildren")
-    can_remove_my_drive_parent: bool | None = Field(alias="canRemoveMyDriveParent")
-    can_rename: bool | None = Field(alias="canRename")
-    can_rename_drive: bool | None = Field(alias="canRenameDrive")
-    can_reset_drive_restrictions: bool | None = Field(alias="canResetDriveRestrictions")
-    can_share: bool | None = Field(alias="canShare")
-    can_trash: bool | None = Field(alias="canTrash")
-    can_trash_children: bool | None = Field(alias="canTrashChildren")
-    can_untrash: bool | None = Field(alias="canUntrash")
+    can_move_item_out_of_drive: bool | None = Field(None, alias="canMoveItemOutOfDrive")
+    can_move_item_within_drive: bool | None = Field(
+        None, alias="canMoveItemWithinDrive"
+    )
+    can_read_labels: bool | None = Field(None, alias="canReadLabels")
+    can_read_revisions: bool | None = Field(None, alias="canReadRevisions")
+    can_read_drive: bool | None = Field(None, alias="canReadDrive")
+    can_remove_children: bool | None = Field(None, alias="canRemoveChildren")
+    can_remove_my_drive_parent: bool | None = Field(
+        None, alias="canRemoveMyDriveParent"
+    )
+    can_rename: bool | None = Field(None, alias="canRename")
+    can_rename_drive: bool | None = Field(None, alias="canRenameDrive")
+    can_reset_drive_restrictions: bool | None = Field(
+        None, alias="canResetDriveRestrictions"
+    )
+    can_share: bool | None = Field(None, alias="canShare")
+    can_trash: bool | None = Field(None, alias="canTrash")
+    can_trash_children: bool | None = Field(None, alias="canTrashChildren")
+    can_untrash: bool | None = Field(None, alias="canUntrash")
 
 
 class _DriveRestrictions(BaseModelWithConfig):
     admin_managed_restrictions: bool = Field(alias="adminManagedRestrictions")
     copy_requires_writer_permission: bool = Field(alias="copyRequiresWriterPermission")
     domain_users_only: bool = Field(alias="domainUsersOnly")
     drive_members_only: bool = Field(alias="driveMembersOnly")
@@ -1049,79 +975,79 @@
 
 DriveSubEntity = TypeVar("DriveSubEntity", Directory, File)
 
 
 class Drive(_CanHaveChildren):
     """A Google Drive: Drive - basically a Directory with extended functionality."""
 
-    kind: EntityKind = Field(alias="kind", const=True, default=EntityKind.DRIVE)
+    kind: Literal[EntityKind.DRIVE] = Field(default=EntityKind.DRIVE)
     mime_type: Literal["application/vnd.google-apps.folder"] = Field(
-        alias="mimeType", const=True, default=Directory.MIME_TYPE
+        alias="mimeType", default=Directory.MIME_TYPE
     )
 
     # Optional, can be retrieved with the `describe` method or by getting the attribute
     background_image_file: _DriveBackgroundImageFile | None = Field(
-        alias="backgroundImageFile"
+        None, alias="backgroundImageFile"
     )
-    background_image_link: str | None = Field(alias="backgroundImageLink")
-    capabilities: _DriveCapabilities | None
-    color_rgb: str | None = Field(alias="colorRgb")
+    background_image_link: str | None = Field(None, alias="backgroundImageLink")
+    capabilities: _DriveCapabilities | None = None
+    color_rgb: str | None = Field(None, alias="colorRgb")
     copy_requires_writer_permission: bool | None = Field(
-        alias="copyRequiresWriterPermission"
+        None, alias="copyRequiresWriterPermission"
     )
-    created_time: datetime | None = Field(alias="createdTime")
-    explicitly_trashed: bool | None = Field(alias="explicitlyTrashed")
-    folder_color_rgb: str | None = Field(alias="folderColorRgb")
-    has_thumbnail: bool | None = Field(alias="hasThumbnail")
-    hidden: bool | None
-    icon_link: str | None = Field(alias="iconLink")
-    is_app_authorized: bool | None = Field(alias="isAppAuthorized")
-    last_modifying_user: _User | None = Field(alias="lastModifyingUser")
+    created_time: datetime | None = Field(None, alias="createdTime")
+    explicitly_trashed: bool | None = Field(None, alias="explicitlyTrashed")
+    folder_color_rgb: str | None = Field(None, alias="folderColorRgb")
+    has_thumbnail: bool | None = Field(None, alias="hasThumbnail")
+    hidden: bool | None = None
+    icon_link: str | None = Field(None, alias="iconLink")
+    is_app_authorized: bool | None = Field(None, alias="isAppAuthorized")
+    last_modifying_user: _User | None = Field(None, alias="lastModifyingUser")
     link_share_metadata: dict[
         Literal["securityUpdateEligible", "securityUpdateEnabled"], bool
     ] = Field(alias="linkShareMetadata", default_factory=dict)
-    modified_by_me: bool | None = Field(alias="modifiedByMe")
-    modified_by_me_time: datetime | None = Field(alias="modifiedByMeTime")
-    modified_time: datetime | None = Field(alias="modifiedTime")
-    org_unit_id: str | None = Field(alias="orgUnitId")
-    owned_by_me: bool | None = Field(alias="ownedByMe")
+    modified_by_me: bool | None = Field(None, alias="modifiedByMe")
+    modified_by_me_time: datetime | None = Field(None, alias="modifiedByMeTime")
+    modified_time: datetime | None = Field(None, alias="modifiedTime")
+    org_unit_id: str | None = Field(None, alias="orgUnitId")
+    owned_by_me: bool | None = Field(None, alias="ownedByMe")
     owners: list[_User] = []
     permissions: list[_Permission] = []
     permission_ids: list[str] = Field(alias="permissionIds", default_factory=list)
-    quota_bytes_used: float | None = Field(alias="quotaBytesUsed")
-    restrictions: _DriveRestrictions | None
-    shared: bool | None
+    quota_bytes_used: float | None = Field(None, alias="quotaBytesUsed")
+    restrictions: _DriveRestrictions | None = None
+    shared: bool | None = None
     spaces: list[str] = []
-    starred: bool | None
-    theme_id: str | None = Field(alias="themeId")
-    thumbnail_version: int | None = Field(alias="thumbnailVersion")
-    trashed: bool | None
-    version: int | None
-    viewed_by_me: bool | None = Field(alias="viewedByMe")
-    viewers_can_copy_content: bool | None = Field(alias="viewersCanCopyContent")
-    web_view_link: str | None = Field(alias="webViewLink")
-    writers_can_share: bool | None = Field(alias="writersCanShare")
-
-    parent_: None = Field(exclude=True, const=True, default=None)
-    host_drive_: None = Field(exclude=True, const=True, default=None)
-
-    _all_directories: list[Directory] = Field(exclude=True, default_factory=list)
-    _directories_mapped: bool = Field(exclude=True, default=False)
-    _all_files: list[File] = Field(exclude=True, default_factory=list)
-    _files_mapped: bool = Field(exclude=True, default=False)
+    starred: bool | None = None
+    theme_id: str | None = Field(None, alias="themeId")
+    thumbnail_version: int | None = Field(None, alias="thumbnailVersion")
+    trashed: bool | None = None
+    version: int | None = None
+    viewed_by_me: bool | None = Field(None, alias="viewedByMe")
+    viewers_can_copy_content: bool | None = Field(None, alias="viewersCanCopyContent")
+    web_view_link: str | None = Field(None, alias="webViewLink")
+    writers_can_share: bool | None = Field(None, alias="writersCanShare")
+
+    parent_: None = Field(exclude=True, frozen=True, default=None)
+    host_drive_: None = Field(exclude=True, frozen=True, default=None)
+
+    _all_directories: list[Directory] = PrivateAttr(default_factory=list)
+    _directories_mapped: bool = False
+    _all_files: list[File] = PrivateAttr(default_factory=list)
+    _files_mapped: bool = False
 
-    @validator("kind", always=True, pre=True)
+    @field_validator("kind", mode="before")
     def _validate_kind(cls, value: str | None) -> str:  # noqa: N805
         """Set the kind to "drive#drive"."""
 
         # Drives are just a subtype of files, so `"drive#file"` is okay too
         if value not in (EntityKind.DRIVE, EntityKind.FILE):
             raise ValueError(f"Invalid kind for Drive: {value}")
 
-        return "drive#drive"
+        return EntityKind.DRIVE
 
     def _get_entity_by_id(
         self, cls: type[DriveSubEntity], entity_id: str
     ) -> DriveSubEntity:
         """Get either a Directory or File by its ID.
 
         Args:
@@ -1202,15 +1128,18 @@
         # item anyway
         file_fields = (
             "*"
             if self.google_client.item_metadata_retrieval == IMR.ON_INIT
             else "id, name, parents, mimeType, kind"
         )
 
-        params = {
+        params: dict[
+            StrBytIntFlt,
+            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+        ] = {
             "pageSize": 1000,
             "fields": f"nextPageToken, files({file_fields})",
         }
 
         if map_type == EntityType.DIRECTORY:
             params["q"] = f"mimeType = '{Directory.MIME_TYPE}'"
 
@@ -1237,23 +1166,23 @@
             nonlocal all_items
 
             remaining_items = []
 
             to_be_mapped = []
             for item in all_items:
                 try:
-                    if parent_dir.id != item["parents"][0]:
+                    if parent_dir.id != item["parents"][0]:  # type: ignore[index]
                         remaining_items.append(item)
                         continue
                 except LookupError:  # pragma: no cover
                     continue
 
                 if item["id"] in known_descendent_ids:
                     if item["mimeType"] == Directory.MIME_TYPE:
-                        to_be_mapped.append(self.get_directory_by_id(item["id"]))
+                        to_be_mapped.append(self.get_directory_by_id(item["id"]))  # type: ignore[arg-type]
 
                 # Can't use `kind` here as it can be `drive#file` for directories
                 elif item["mimeType"] == Directory.MIME_TYPE:
                     directory = Directory.from_json_response(
                         item,
                         google_client=self.google_client,
                         parent=parent_dir,
@@ -1276,32 +1205,20 @@
 
             all_items = remaining_items
             for directory in to_be_mapped:
                 build_sub_structure(directory)
 
         build_sub_structure(self)
 
-        self._set_private_attr(
-            "_all_directories",
-            all_directories,
-        )
-        self._set_private_attr(
-            "_directories_mapped",
-            True,
-        )
+        self._all_directories = all_directories
+        self._directories_mapped = True
 
         if map_type != EntityType.DIRECTORY:
-            self._set_private_attr(
-                "_all_files",
-                all_files,
-            )
-            self._set_private_attr(
-                "_files_mapped",
-                True,
-            )
+            self._all_files = all_files
+            self._files_mapped = True
 
     def search(
         self,
         term: str,
         entity_type: EntityType | None = None,
         max_results: int = 50,
         exact_match: bool = False,
@@ -1330,15 +1247,18 @@
 
         file_fields = (
             "*"
             if self.google_client.item_metadata_retrieval == IMR.ON_INIT
             else "id, name, parents, mimeType, kind"
         )
 
-        params = {
+        params: dict[
+            StrBytIntFlt,
+            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+        ] = {
             "pageSize": 1 if exact_match else min(max_results, 1000),
             "fields": f"nextPageToken, files({file_fields})",
         }
 
         query_conditions = [
             f"name = '{term}'" if exact_match else f"name contains '{term}'",
         ]
@@ -1384,18 +1304,18 @@
         No HTTP requests are made to get these children, so this may not be an
         exhaustive list.
 
         Returns:
             list[Directory | File]: The list of children.
         """
         if not isinstance(self._all_directories, list):
-            self._set_private_attr("_all_directories", [])
+            self._all_directories = []
 
         if not isinstance(self._all_files, list):
-            self._set_private_attr("_all_files", [])
+            self._all_files = []
 
         return self._all_files + self._all_directories  # type: ignore[operator]
 
     @property
     def all_directories(self) -> list[Directory]:
         """Get all directories in the Drive."""
 
@@ -1522,13 +1442,11 @@
             )
             for drive in self.get_items(
                 "/drives", list_key="drives", params={"fields": "*"}
             )
         ]
 
 
-FJR = TypeVar("FJR", bound=_GoogleDriveEntity)
-
-_GoogleDriveEntity.update_forward_refs()
-File.update_forward_refs()
-Directory.update_forward_refs()
-Drive.update_forward_refs()
+_GoogleDriveEntity.model_rebuild()
+File.model_rebuild()
+Directory.model_rebuild()
+Drive.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/google_fit.py` & `wg_utilities-4.0.0/wg_utilities/clients/google_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Custom client for interacting with Google's Fit API."""
 from __future__ import annotations
 
 from collections.abc import Callable
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Literal, TypedDict
+from typing import Any, Literal
+
+from typing_extensions import TypedDict
 
 from wg_utilities.clients._google import GoogleClient
 from wg_utilities.functions.datetime_helpers import DatetimeFixedUnit as DFUnit
 from wg_utilities.functions.datetime_helpers import utcnow
 
 
 class _DataSourceDataTypeFieldInfo(TypedDict):
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/google_photos.py` & `wg_utilities-4.0.0/wg_utilities/clients/google_photos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# pylint: disable=too-few-public-methods,no-self-argument
+# pylint: disable=no-self-argument
 """Custom client for interacting with Google's Photos API."""
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from logging import DEBUG, getLogger
 from pathlib import Path
-from typing import Any, Literal, TypeAlias, TypedDict, TypeVar
+from typing import Any, Literal, Self, TypeAlias
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 from requests import post
+from typing_extensions import TypedDict
 
 from wg_utilities.clients._google import GoogleClient
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    GenericModelWithConfig,
-)
+from wg_utilities.clients.oauth_client import BaseModelWithConfig
 from wg_utilities.functions import force_mkdir
 from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 add_stream_handler(LOGGER)
 
@@ -35,106 +33,101 @@
     isOwned: bool
     shareableUrl: str
     sharedAlbumOptions: _SharedAlbumOptionsInfo
     shareToken: str
 
 
 class _MediaItemMetadataPhoto(BaseModelWithConfig):
-    camera_make: str | None = Field(alias="cameraMake")
-    camera_model: str | None = Field(alias="cameraModel")
-    focal_length: float | None = Field(alias="focalLength")
-    aperture_f_number: float | None = Field(alias="apertureFNumber")
-    iso_equivalent: int | None = Field(alias="isoEquivalent")
-    exposure_time: str | None = Field(alias="exposureTime")
+    camera_make: str | None = Field(None, alias="cameraMake")
+    camera_model: str | None = Field(None, alias="cameraModel")
+    focal_length: float | None = Field(None, alias="focalLength")
+    aperture_f_number: float | None = Field(None, alias="apertureFNumber")
+    iso_equivalent: int | None = Field(None, alias="isoEquivalent")
+    exposure_time: str | None = Field(None, alias="exposureTime")
 
 
 class _MediaItemMetadataVideo(BaseModelWithConfig):
-    camera_make: str | None = Field(alias="cameraMake")
-    camera_model: str | None = Field(alias="cameraModel")
-    status: Literal["READY"] | None
-    fps: float | None
+    camera_make: str | None = Field(None, alias="cameraMake")
+    camera_model: str | None = Field(None, alias="cameraModel")
+    status: Literal["READY"] | None = None
+    fps: float | None = None
 
 
 class _MediaItemMetadata(BaseModelWithConfig):
     creation_time: datetime = Field(alias="creationTime")
     height: int
     width: int
-    photo: _MediaItemMetadataPhoto | None
-    video: _MediaItemMetadataVideo | None
+    photo: _MediaItemMetadataPhoto | None = Field(default=None)
+    video: _MediaItemMetadataVideo | None = Field(default=None)
 
 
 class MediaType(Enum):
     """Enum for all potential media types."""
 
     IMAGE = "image"
     VIDEO = "video"
     UNKNOWN = "unknown"
 
 
-FJR = TypeVar("FJR", bound="GooglePhotosEntity")
+class _GooglePhotosEntityJson(TypedDict):
+    """JSON representation of a Google Photos entity."""
+
+    id: str
+    productUrl: str
 
 
-class GooglePhotosEntity(GenericModelWithConfig):
-    """Base class for Google Photos entities."""
+class GooglePhotosEntity(BaseModelWithConfig):
+    """Generic base class for Google Photos entities."""
 
     id: str
     product_url: str = Field(alias="productUrl")
 
     google_client: GooglePhotosClient = Field(exclude=True)
 
     @classmethod
     def from_json_response(
-        cls: type[FJR],
+        cls,
         value: GooglePhotosEntityJson,
         *,
         google_client: GooglePhotosClient,
-        _waive_validation: bool = False,
-    ) -> FJR:
+    ) -> Self:
         """Create an entity from a JSON response."""
 
         value_data: dict[str, Any] = {
             "google_client": google_client,
             **value,
         }
 
-        instance = cls.parse_obj(value_data)
-
-        if not _waive_validation:
-            instance._validate()  # pylint: disable=protected-access
-
-        return instance
+        return cls.model_validate(value_data)
 
 
-class AlbumJson(TypedDict):
+class AlbumJson(_GooglePhotosEntityJson):
     """JSON representation of an Album."""
 
-    id: str
-    productUrl: str
-
-    coverPhotoBaseUrl: str
-    coverPhotoMediaItemId: str
-    isWriteable: bool | None
-    mediaItemsCount: int
-    shareInfo: _ShareInfoInfo | None
+    coverPhotoBaseUrl: str  # noqa: N815
+    coverPhotoMediaItemId: str  # noqa: N815
+    isWriteable: bool | None  # noqa: N815
+    mediaItemsCount: int  # noqa: N815
+    shareInfo: _ShareInfoInfo | None  # noqa: N815
     title: str
 
 
 class Album(GooglePhotosEntity):
     """Class for Google Photos albums and their metadata/content."""
 
     cover_photo_base_url: str = Field(alias="coverPhotoBaseUrl")
     cover_photo_media_item_id: str = Field(alias="coverPhotoMediaItemId")
-    is_writeable: bool | None = Field(alias="isWriteable")
+    is_writeable: bool | None = Field(None, alias="isWriteable")
     media_items_count: int = Field(alias="mediaItemsCount")
-    share_info: _ShareInfoInfo | None = Field(alias="shareInfo")
+    share_info: _ShareInfoInfo | None = Field(None, alias="shareInfo")
     title: str
 
     _media_items: list[MediaItem]
 
-    @validator("title")
+    @field_validator("title")
     def _validate_title(cls, value: str) -> str:  # noqa: N805
         """Validate the title of the album."""
 
         if not value:
             raise ValueError("Album title cannot be empty.")
 
         return value.strip()
@@ -145,55 +138,51 @@
         """List all media items in the album.
 
         Returns:
             list: a list of MediaItem instances, representing the contents of the album
         """
 
         if not hasattr(self, "_media_items"):
-            self._set_private_attr(
-                "_media_items",
-                [
-                    MediaItem.from_json_response(item, google_client=self.google_client)
-                    for item in self.google_client.get_items(
-                        "/mediaItems:search",
-                        method_override=post,
-                        list_key="mediaItems",
-                        params={"albumId": self.id, "pageSize": 100},
-                    )
-                ],
-            )
+            self._media_items = [
+                MediaItem.from_json_response(item, google_client=self.google_client)
+                for item in self.google_client.get_items(
+                    "/mediaItems:search",
+                    method_override=post,
+                    list_key="mediaItems",
+                    params={"albumId": self.id, "pageSize": 100},
+                )
+            ]
 
         return self._media_items
 
     def __contains__(self, item: MediaItem) -> bool:
         """Check if the album contains the given media item."""
 
         return item.id in [media_item.id for media_item in self.media_items]
 
 
-class MediaItemJson(TypedDict):
+class MediaItemJson(_GooglePhotosEntityJson):
     """JSON representation of a Media Item (photo or video)."""
 
-    id: str
-    productUrl: str
-
-    baseUrl: str
-    contributorInfo: dict[str, str] | None
+    baseUrl: str  # noqa: N815
+    contributorInfo: dict[str, str] | None  # noqa: N815
     description: str | None
     filename: str
-    mediaMetadata: _MediaItemMetadata
-    mimeType: str
+    mediaMetadata: _MediaItemMetadata  # noqa: N815
+    mimeType: str  # noqa: N815
 
 
 class MediaItem(GooglePhotosEntity):
     """Class for representing a MediaItem and its metadata/content."""
 
     base_url: str = Field(alias="baseUrl")
-    contributor_info: dict[str, str] | None = Field(alias="contributorInfo")
-    description: str | None
+    contributor_info: dict[str, str] | None = Field(
+        alias="contributorInfo", default=None
+    )
+    description: str | None = Field(default=None)
     filename: str
     media_metadata: _MediaItemMetadata = Field(alias="mediaMetadata")
     mime_type: str = Field(alias="mimeType")
 
     _local_path: Path
 
     def download(
@@ -224,21 +213,18 @@
         """
 
         if isinstance(target_directory, str):
             target_directory = (
                 Path.cwd() if target_directory == "" else Path(target_directory)
             )
 
-        self._set_private_attr(
-            "_local_path",
-            (
-                target_directory
-                / self.creation_datetime.strftime("%Y/%m/%d")
-                / (file_name_override or self.filename)
-            ),
+        self._local_path = (
+            target_directory
+            / self.creation_datetime.strftime("%Y/%m/%d")
+            / (file_name_override or self.filename)
         )
 
         if self.local_path.is_file() and not force_download:
             LOGGER.warning(
                 "File already exists at `%s` and `force_download` is `False`;"
                 " skipping download.",
                 self.local_path,
@@ -434,9 +420,9 @@
             )
 
             self._album_count = len(self._albums)
 
         return self._albums
 
 
-Album.update_forward_refs()
-MediaItem.update_forward_refs()
+Album.model_rebuild()
+MediaItem.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/json_api_client.py` & `wg_utilities-4.0.0/wg_utilities/clients/json_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,16 @@
                 return {}  # type: ignore[return-value]
 
             raise ValueError(res.text) from exc
 
     def get_json_response(
         self,
         url: str,
+        /,
+        *,
         params: dict[
             StrBytIntFlt,
             StrBytIntFlt | Iterable[StrBytIntFlt] | None,
         ]
         | None = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
         timeout: float | None = None,
@@ -252,14 +254,16 @@
             json=json,
             data=data,
         )
 
     def post_json_response(
         self,
         url: str,
+        /,
+        *,
         params: dict[
             StrBytIntFlt,
             StrBytIntFlt | Iterable[StrBytIntFlt] | None,
         ]
         | None = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
         timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/monzo.py` & `wg_utilities-4.0.0/wg_utilities/clients/monzo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# pylint: disable=too-few-public-methods
 """Custom client for interacting with Monzo's API."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from logging import DEBUG, getLogger
-from typing import Any, Literal, TypedDict, final
+from typing import Any, Literal, final
 
-from pydantic import Field
+from pydantic import Field, field_validator
 from requests import put
+from typing_extensions import TypedDict
 
 from wg_utilities.clients.json_api_client import StrBytIntFlt
 from wg_utilities.clients.oauth_client import BaseModelWithConfig, OAuthClient
 from wg_utilities.functions import DTU, cleanse_string, utcnow
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
@@ -141,48 +141,48 @@
 
 class Transaction(BaseModelWithConfig):
     """Pydantic representation of a transaction."""
 
     account_id: str
     amount: int
     amount_is_pending: bool
-    atm_fees_detailed: dict[str, int | str | None] | None
-    attachments: None
+    atm_fees_detailed: dict[str, int | str | None] | None = None
+    attachments: None = None
     can_add_to_tab: bool
     can_be_excluded_from_breakdown: bool
     can_be_made_subscription: bool
     can_match_transactions_in_categorization: bool
     can_split_the_bill: bool
     categories: dict[
         TransactionCategory,
         int,
     ]
     category: TransactionCategory
     counterparty: dict[str, str]
     created: str
     currency: str
-    decline_reason: str | None
+    decline_reason: str | None = None
     dedupe_id: str
     description: str
-    fees: dict[str, Any] | None
+    fees: dict[str, Any] | None = None
     id: str
     include_in_spending: bool
-    international: bool | None
+    international: bool | None = None
     is_load: bool
-    labels: list[str] | None
+    labels: list[str] | None = None
     local_amount: int
     local_currency: str
     merchant: str | None
     metadata: dict[str, str]
     notes: str
     originator: bool
     parent_account_id: str
     scheme: str
     settled: str
-    tab: dict[str, object] | None
+    tab: dict[str, object] | None = None
     updated: str
     user_id: str
 
 
 class BalanceVariables(BaseModelWithConfig):
     """Variables for an account's balance summary."""
 
@@ -203,57 +203,69 @@
     preferred_name: str
     user_id: str
 
 
 class Account(BaseModelWithConfig):
     """Class for managing individual bank accounts."""
 
-    account_number: str | None
+    account_number: str
     closed: bool
     country_code: str
     created: datetime
     currency: Literal["GBP"]
     description: str
     id: str
-    initial_balance: int | None = Field(alias="balance")
+    initial_balance: int | None = Field(None, validation_alias="balance")
     initial_balance_including_flexible_savings: int | None = Field(
-        alias="balance_including_flexible_savings"
+        None, validation_alias="balance_including_flexible_savings"
     )
-    initial_spend_today: int | None = Field(alias="spend_today")
-    initial_total_balance: int | None = Field(alias="total_balance")
+    initial_spend_today: int | None = Field(None, validation_alias="spend_today")
+    initial_total_balance: int | None = Field(None, validation_alias="total_balance")
     owners: list[AccountOwner]
-    payment_details: dict[str, dict[str, str]] | None
-    sort_code: str | None
+    payment_details: dict[str, dict[str, str]] | None = None
+    sort_code: str = Field(min_length=6, max_length=6)
     type: Literal["uk_monzo_flex", "uk_retail", "uk_retail_joint"]
 
     monzo_client: MonzoClient = Field(exclude=True)
     balance_update_threshold: int = Field(15, exclude=True)
     last_balance_update: datetime = Field(datetime(1970, 1, 1), exclude=True)
     _balance_variables: BalanceVariables
 
+    @field_validator("sort_code", mode="before")
+    def validate_sort_code(cls, sort_code: str | int) -> str:  # noqa: N805
+        """Ensure that the sort code is a 6-digit integer.
+
+        Represented as a string so leading zeroes aren't lost.
+        """
+
+        if isinstance(sort_code, int):
+            sort_code = str(sort_code)
+
+        if len(sort_code) != 6:
+            sort_code.ljust(6, "0")
+
+        if not sort_code.isdigit():
+            raise ValueError("Sort code must be a 6-digit integer")
+
+        return sort_code
+
     @classmethod
     def from_json_response(
         cls,
         value: AccountJson,
         monzo_client: MonzoClient,
-        _waive_validation: bool = False,
     ) -> Account:
         """Create an account from a JSON response."""
 
         value_data: dict[str, Any] = {
             "monzo_client": monzo_client,
             **value,
         }
 
-        instance = cls.parse_obj(value_data)
-
-        if not _waive_validation:
-            instance._validate()  # pylint: disable=protected-access
-
-        return instance
+        return cls.model_validate(value_data)
 
     def list_transactions(
         self,
         from_datetime: datetime | None = None,
         to_datetime: datetime | None = None,
         limit: int = 100,
     ) -> list[Transaction]:
@@ -299,22 +311,16 @@
         if not hasattr(self, "_balance_variables") or self.last_balance_update <= (
             datetime.utcnow() - timedelta(minutes=self.balance_update_threshold)
         ):
             LOGGER.debug(
                 "Balance variable update threshold crossed, getting new values"
             )
 
-            object.__setattr__(
-                self,
-                "_balance_variables",
-                BalanceVariables.parse_obj(
-                    self.monzo_client.get_json_response(
-                        f"/balance?account_id={self.id}"
-                    )
-                ),
+            self._balance_variables = BalanceVariables.model_validate(
+                self.monzo_client.get_json_response(f"/balance?account_id={self.id}")
             )
 
             self.last_balance_update = datetime.utcnow()
 
     @property
     def balance(self) -> int | None:
         """Current balance of the account, in pence.
@@ -378,32 +384,32 @@
 
 
 class Pot(BaseModelWithConfig):
     """Read-only class for Monzo pots."""
 
     available_for_bills: bool
     balance: float
-    charity_id: str | None
+    charity_id: str | None = None
     cover_image_url: str
     created: datetime
     currency: str
     current_account_id: str
     deleted: bool
-    goal_amount: float | None
+    goal_amount: float | None = None
     has_virtual_cards: bool
     id: str
     is_tax_pot: bool
     isa_wrapper: str
-    lock_type: Literal["until_date"] | None
+    lock_type: Literal["until_date"] | None = None
     locked: bool
-    locked_until: datetime | None
+    locked_until: datetime | None = None
     name: str
     product_id: str
     round_up: bool
-    round_up_multiplier: float | None
+    round_up_multiplier: float | None = None
     style: str
     type: str
     updated: datetime
 
 
 class MonzoGJR(TypedDict):
     """The response type for `MonzoClient.get_json_response`."""
@@ -555,8 +561,8 @@
             dict: auth headers for HTTP requests
         """
         return {
             "Authorization": f"Bearer {self.access_token}",
         }
 
 
-Account.update_forward_refs()
+Account.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-4.0.0/wg_utilities/clients/oauth_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,127 +1,149 @@
-# pylint: disable=too-few-public-methods
 """Generic OAuth client to allow for reusable authentication flows/checks etc."""
 from __future__ import annotations
 
 from collections.abc import Callable
 from datetime import datetime
 from json import dumps
 from logging import DEBUG, getLogger
 from os import getenv
 from pathlib import Path
 from random import choice
 from string import ascii_letters
 from time import time
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, ClassVar, Literal
 from urllib.parse import urlencode
 from webbrowser import open as open_browser
 
 from jwt import DecodeError, decode
-from pydantic import BaseModel, Extra, validate_model
-from pydantic.generics import GenericModel
+from pydantic import BaseModel, ConfigDict
 
 from wg_utilities.api import TempAuthServer
 from wg_utilities.clients.json_api_client import GetJsonResponse, JsonApiClient
 from wg_utilities.functions import user_data_dir
 from wg_utilities.functions.file_management import force_mkdir
 
-LOGGER = getLogger(__name__)
-LOGGER.setLevel(DEBUG)
-
-
-class _ModelBase:
-    """Base class for `BaseModelWithConfig` and `GenericModelWithConfig`.
-
-    This is just to prevent duplicating the methods in both classes.
-    """
-
-    __fields__: dict[str, Any]
-
-    def _set_private_attr(self, attr_name: str, attr_value: Any) -> None:
-        """Set private attribute on the instance.
-
-        Args:
-            attr_name (str): the name of the attribute to set
-            attr_value (Any): the value to set the attribute to
-
-        Raises:
-            ValueError: if the attribute isn't private (i.e. the name doesn't start
-                with an underscore)
-        """
-        if not attr_name.startswith("_"):
-            raise ValueError("Only private attributes can be set via this method.")
-
-        object.__setattr__(self, attr_name, attr_value)
-
-    def _validate(self) -> None:
-        """Validate the model.
-
-        Any fields which have been renamed via `alias` will be renamed in the
-        validation dict before being passed to `validate_model`. Private attributes,
-        functions, and excluded fields are also ignored.
-
-        Raises:
-            ValidationError: if the model is invalid
-        """
+if TYPE_CHECKING:  # pragma: no cover
+    from pydantic.main import IncEx
 
-        model_dict = {
-            self.__fields__[k].alias if k in self.__fields__ else k: v
-            for k, v in self.__dict__.items()
-            if not k.startswith("_") and not callable(v)
-        }
+else:
+    IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
 
-        *_, validation_error = validate_model(
-            self.__class__, model_dict, self.__class__  # type: ignore[arg-type]
-        )
-
-        if validation_error:  # pragma: no cover
-            LOGGER.error(repr(validation_error))
-            raise validation_error
+LOGGER = getLogger(__name__)
+LOGGER.setLevel(DEBUG)
 
 
-class BaseModelWithConfig(_ModelBase, BaseModel):
+class BaseModelWithConfig(BaseModel):
     """Reusable `BaseModel` with Config to apply to all subclasses."""
 
-    class Config:
-        """Pydantic config."""
-
-        arbitrary_types_allowed = True
-        extra = Extra.forbid
-        validate_assignment = True
-
-
-class GenericModelWithConfig(_ModelBase, GenericModel):
-    """Reusable `GenericModel` with Config to apply to all subclasses."""
+    model_config: ClassVar[ConfigDict] = {
+        "arbitrary_types_allowed": True,
+        "extra": "forbid",
+        "validate_assignment": True,
+    }
 
-    class Config:
-        """Pydantic config."""
+    def model_dump(
+        self,
+        *,
+        mode: Literal["json", "python"] | str = "python",
+        include: IncEx = None,
+        exclude: IncEx = None,
+        by_alias: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        round_trip: bool = False,
+        warnings: bool = True,
+    ) -> dict[str, Any]:
+        # pylint: disable=useless-parent-delegation
+        """Create a dictionary representation of the model.
+
+        Overrides the standard `BaseModel.dict` method, so we can always return the
+        dict with the same field names it came in with, and exclude any null values
+        that have been added when parsing
+
+        Original documentation is here:
+          - https://docs.pydantic.dev/latest/usage/serialization/#modelmodel_dump
+
+        Overridden Parameters:
+            by_alias: False -> True
+            exclude_unset: False -> True
+        """
+
+        return super().model_dump(
+            mode=mode,
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            round_trip=round_trip,
+            warnings=warnings,
+        )
 
-        arbitrary_types_allowed = True
-        extra = Extra.forbid
-        validate_assignment = True
+    def model_dump_json(
+        self,
+        *,
+        indent: int | None = None,
+        include: IncEx = None,
+        exclude: IncEx = None,
+        by_alias: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        round_trip: bool = False,
+        warnings: bool = True,
+    ) -> str:
+        # pylint: disable=useless-parent-delegation
+        """Create a JSON string representation of the model.
+
+        Overrides the standard `BaseModel.json` method, so we can always return the
+        dict with the same field names it came in with, and exclude any null values
+        that have been added when parsing
+
+        Original documentation is here:
+          - https://docs.pydantic.dev/latest/usage/serialization/#modelmodel_dump_json
+
+        Overridden Parameters:
+            by_alias: False -> True
+            exclude_unset: False -> True
+        """
+
+        return super().model_dump_json(
+            indent=indent,
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            round_trip=round_trip,
+            warnings=warnings,
+        )
 
 
 class OAuthCredentials(BaseModelWithConfig):
     """Typing info for OAuth credentials."""
 
     access_token: str
     client_id: str
     expiry_epoch: float
     refresh_token: str
     scope: str
     token_type: Literal["Bearer"]
     client_secret: str
 
     # Monzo
-    user_id: str | None
+    user_id: str | None = None
 
     # Google
-    token: str | None
-    token_uri: str | None
-    scopes: list[str] | None
+    token: str | None = None
+    token_uri: str | None = None
+    scopes: list[str] | None = None
 
     @classmethod
     def parse_first_time_login(cls, value: dict[str, Any]) -> OAuthCredentials:
         """Parse the response from a first time login into a credentials object.
 
         The following fields are returned per API:
         +---------------+--------+-------+---------+-----------+
@@ -263,15 +285,17 @@
     def _load_local_credentials(self) -> bool:
         """Load credentials from the local cache.
 
         Returns:
             bool: True if the credentials were loaded successfully, False otherwise
         """
         try:
-            self._credentials = OAuthCredentials.parse_file(self.creds_cache_path)
+            self._credentials = OAuthCredentials.model_validate_json(
+                self.creds_cache_path.read_text()
+            )
         except FileNotFoundError:
             return False
 
         return True
 
     def delete_creds_file(self) -> None:
         """Delete the local creds file."""
@@ -304,15 +328,17 @@
         self.credentials.update_access_token(
             new_token=new_creds["access_token"],
             expires_in=new_creds["expires_in"],
             # Monzo
             refresh_token=new_creds.get("refresh_token"),
         )
 
-        self.creds_cache_path.write_text(self.credentials.json(exclude_none=True))
+        self.creds_cache_path.write_text(
+            self.credentials.model_dump_json(exclude_none=True)
+        )
 
     def run_first_time_login(self) -> None:
         """Run the first time login process.
 
         This is a blocking call which will not return until the user has
         authenticated with the OAuth provider.
 
@@ -477,15 +503,15 @@
     @credentials.setter
     def credentials(self, value: OAuthCredentials) -> None:
         """Set the client's credentials, and write to the local cache file."""
 
         self._credentials = value
 
         self.creds_cache_path.write_text(
-            dumps(self._credentials.dict(exclude_none=True))
+            dumps(self._credentials.model_dump(exclude_none=True))
         )
 
     @property
     def creds_cache_path(self) -> Path:
         """Path to the credentials cache file.
 
         Returns:
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/spotify.py` & `wg_utilities-4.0.0/wg_utilities/clients/spotify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# pylint: disable=too-many-lines,too-few-public-methods,no-self-argument
+# pylint: disable=too-many-lines,no-self-argument
 """Custom client for interacting with Spotify's Web API."""
 from __future__ import annotations
 
 from builtins import dict as dict_
 from builtins import type as type_
-from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence, Set
+from collections.abc import Callable, Iterable, Iterator, Sequence
 from datetime import date, datetime, timedelta
 from enum import Enum
 from http import HTTPStatus
 from json import dumps
 from logging import DEBUG, getLogger
 from re import sub
 from typing import (
     Any,
     ClassVar,
     Generic,
     Literal,
+    Self,
     TypeAlias,
-    TypedDict,
     TypeVar,
     cast,
     overload,
 )
 from urllib.parse import urlencode
 
-from pydantic import Field, root_validator, validator
+from pydantic import Field, FieldValidationInfo, field_validator, model_validator
 from requests import HTTPError, delete, put
-from typing_extensions import NotRequired
+from typing_extensions import NotRequired, TypedDict
 
 from wg_utilities.clients._spotify_types import (
-    AlbumFullJson,
     AlbumSummaryJson,
     AnyPaginatedResponse,
     ArtistSummaryJson,
     DeviceJson,
     Followers,
     Image,
     PaginatedResponseAlbums,
@@ -48,19 +47,15 @@
     SearchResponse,
     SpotifyBaseEntityJson,
     SpotifyEntityJson,
     TrackAudioFeaturesJson,
     TrackFullJson,
     UserSummaryJson,
 )
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    GenericModelWithConfig,
-    OAuthClient,
-)
+from wg_utilities.clients.oauth_client import BaseModelWithConfig, OAuthClient
 from wg_utilities.functions import chunk_list
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 
 class ParsedSearchResponse(TypedDict):
@@ -111,15 +106,14 @@
     time_signature: int
     track_href: str
     type: Literal["audio_features"]
     uri: str
     valence: float
 
 
-FJR = TypeVar("FJR", bound="SpotifyEntity[Any]")
 SJ = TypeVar("SJ", bound=SpotifyBaseEntityJson)
 
 
 class SpotifyClient(OAuthClient[SpotifyEntityJson]):
     """Custom client for interacting with Spotify's Web API.
 
     For authentication purposes either an already-instantiated OAuth manager or the
@@ -548,111 +542,33 @@
                 self.get_json_response("/me"),
                 spotify_client=self,
             )
 
         return self._current_user
 
 
-class SpotifyEntity(GenericModelWithConfig, Generic[SJ]):
+class SpotifyEntity(BaseModelWithConfig, Generic[SJ]):
     """Base model for Spotify entities."""
 
     description: str = ""
     external_urls: dict_[Literal["spotify"], str]
     href: str
     id: str
     name: str = ""
     uri: str
 
     metadata: dict_[str, Any] = Field(default_factory=dict)
     spotify_client: SpotifyClient = Field(exclude=True)
 
     summary_json: SJ = Field(
-        default_factory=dict, allow_mutation=False, exclude=True
+        default_factory=dict, frozen=True, exclude=True
     )  # type: ignore[assignment]
     sj_type: ClassVar[TypeAlias] = SpotifyBaseEntityJson
 
-    def dict(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ) -> dict[str, Any]:
-        # pylint: disable=useless-parent-delegation
-        """Create a dictionary representation of the model.
-
-        Overrides the standard `BaseModel.dict` method, so we can always return the
-        dict with the same field names it came in with, and exclude any null values
-        that have been added when parsing
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeldict
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-        """
-
-        return super().dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-        )
-
-    def json(
-        self,
-        *,
-        include: Set[int | str] | Mapping[int | str, Any] | None = None,
-        exclude: Set[int | str] | Mapping[int | str, Any] | None = None,
-        by_alias: bool = True,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = True,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: Callable[[Any], Any] | None = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
-        # pylint: disable=useless-parent-delegation
-        """Create a JSON string representation of the model.
-
-        Overrides the standard `BaseModel.json` method, so we can always return the
-        dict with the same field names it came in with, and exclude any null values
-        that have been added when parsing
-
-        Original documentation is here:
-          - https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeljson
-
-        Overridden Parameters:
-            by_alias: False -> True
-            exclude_unset: False -> True
-        """
-
-        return super().json(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-            encoder=encoder,
-            models_as_dict=models_as_dict,
-            **dumps_kwargs,
-        )
-
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def _set_summary_json(cls, values: dict_[str, Any]) -> Any:  # noqa: N805
         values["summary_json"] = {
             k: v for k, v in values.items() if k in cls.sj_type.__annotations__
         }
 
         # Playlists are a unique case, because the SummaryJson and the FullJson both
         # share the key "tracks", which means that if FullJson is passed into this,
@@ -666,21 +582,20 @@
                 "total": values["summary_json"]["tracks"]["total"],
             }
 
         return values
 
     @classmethod
     def from_json_response(
-        cls: type[FJR],
+        cls,
         value: SpotifyEntityJson,
         spotify_client: SpotifyClient,
         additional_fields: dict_[str, Any] | None = None,
         metadata: dict_[str, object] | None = None,
-        _waive_validation: bool = False,
-    ) -> FJR:
+    ) -> Self:
         """Parse a JSON response from the API into the given entity type model.
 
         Args:
             value (dict[str, object]): the JSON response from the API
             spotify_client (SpotifyClient): the client to use for future API calls
             additional_fields (dict[str, object] | None): additional fields to add to
                 the model
@@ -695,20 +610,15 @@
             **(additional_fields or {}),
             **value,
         }
 
         if metadata:
             value_data["metadata"] = metadata
 
-        instance = cls.parse_obj(value_data)
-
-        if not _waive_validation:
-            instance._validate()  # pylint: disable=protected-access
-
-        return instance
+        return cls.model_validate(value_data)
 
     @property
     def url(self) -> str:
         """URL of the entity.
 
         Returns:
             str: the URL of this entity
@@ -748,51 +658,51 @@
         """Get the string representation of this entity."""
         return self.name or f"{type(self).__name__} ({self.id})"
 
 
 class Album(SpotifyEntity[AlbumSummaryJson]):
     """An album on Spotify."""
 
-    album_group: Literal["album", "single", "compilation", "appears_on"] | None
+    album_group: Literal["album", "single", "compilation", "appears_on"] | None = None
     album_type_str: Literal["album", "single", "compilation"] = Field(
         alias="album_type"
     )
     artists_json: list[ArtistSummaryJson] = Field(alias="artists")
     available_markets: list[str]
-    copyrights: list[dict[str, str]] | None
-    external_ids: dict[str, str] | None
-    genres: list[str] | None
+    copyrights: list[dict[str, str]] | None = None
+    external_ids: dict[str, str] | None = None
+    genres: list[str] | None = None
     images: list[Image]
-    is_playable: bool | None
-    label: str | None
-    popularity: int | None
-    release_date_precision: Literal["year", "month", "day"] | None
+    is_playable: bool | None = None
+    label: str | None = None
+    popularity: int | None = None
+    release_date_precision: Literal["year", "month", "day"] | None = None
     release_date: date
-    restrictions: dict[str, str] | None
+    restrictions: dict[str, str] | None = None
     total_tracks: int
     tracks_json: PaginatedResponseTracks = Field(
         alias="tracks", default_factory=dict
     )  # type: ignore[assignment]
     type: Literal["album"]
 
     _artists: list[Artist]
     _tracks: list[Track]
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = AlbumSummaryJson
 
-    @validator("release_date", pre=True)
+    @field_validator("release_date", mode="before")
     def validate_release_date(
-        cls, value: str | date, values: AlbumFullJson  # noqa: N805
+        cls, value: str | date, info: FieldValidationInfo  # noqa: N805
     ) -> date:
         """Convert the release date string to a date object."""
 
         if isinstance(value, date):
             return value
 
-        rdp = (values.get("release_date_precision") or "day").lower()
+        rdp = (info.data.get("release_date_precision") or "day").lower()
 
         exception = ValueError(
             f"Incompatible release_date and release_date_precision values: {value!r}"
             f" and {rdp!r} respectively."
         )
 
         match value.split("-"):
@@ -830,15 +740,15 @@
                 Artist.from_json_response(
                     item,
                     spotify_client=self.spotify_client,
                 )
                 for item in self.artists_json
             ]
 
-            self._set_private_attr("_artists", artists)
+            self._artists = artists
 
         return self._artists
 
     @property
     def tracks(self) -> list[Track]:
         """List of tracks on the album.
 
@@ -878,26 +788,26 @@
                         additional_fields={"album": self.summary_json},
                     )
                     for item in self.spotify_client.get_items(
                         f"/albums/{self.id}/tracks"
                     )
                 ]
 
-            self._set_private_attr("_tracks", tracks)
+            self._tracks = tracks
 
         return self._tracks
 
 
 class Artist(SpotifyEntity[ArtistSummaryJson]):
     """An artist on Spotify."""
 
-    followers: Followers | None
-    genres: list[str] | None
-    images: list[Image] | None
-    popularity: int | None
+    followers: Followers | None = None
+    genres: list[str] | None = None
+    images: list[Image] | None = None
+    popularity: int | None = None
     type: Literal["artist"]
 
     _albums: list[Album]
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = ArtistSummaryJson
 
     @property
@@ -909,38 +819,40 @@
         """
         if not hasattr(self, "_albums"):
             albums = [
                 Album.from_json_response(item, spotify_client=self.spotify_client)
                 for item in self.spotify_client.get_items(f"/artists/{self.id}/albums")
             ]
 
-            self._set_private_attr("_albums", albums)
+            self._albums = albums
 
         return self._albums
 
 
 class Track(SpotifyEntity[TrackFullJson]):
     """A track on Spotify."""
 
     album_json: AlbumSummaryJson = Field(alias="album")
     artists_json: list[ArtistSummaryJson] = Field(alias="artists")
-    audio_features_json: TrackAudioFeaturesJson | None = Field(alias="audio_features")
+    audio_features_json: TrackAudioFeaturesJson | None = Field(
+        None, alias="audio_features"
+    )
     available_markets: list[str]
     disc_number: int
     duration_ms: int
-    episode: bool | None
+    episode: bool | None = None
     explicit: bool
-    external_ids: dict[str, str] | None
+    external_ids: dict[str, str] | None = None
     is_local: bool
-    is_playable: bool | None
-    linked_from: TrackFullJson | None
-    popularity: int | None
-    preview_url: str | None
-    restrictions: str | None
-    track: bool | None
+    is_playable: bool | None = None
+    linked_from: TrackFullJson | None = None
+    popularity: int | None = None
+    preview_url: str | None = None
+    restrictions: str | None = None
+    track: bool | None = None
     track_number: int
     type: Literal["track"]
 
     _artists: list[Artist]
     _album: Album
     _audio_features: TrackAudioFeatures | None
 
@@ -951,19 +863,16 @@
         """Track's parent album.
 
         Returns:
             Album: the album which this track is from
         """
 
         if not hasattr(self, "_album"):
-            self._set_private_attr(
-                "_album",
-                Album.from_json_response(
-                    self.album_json, spotify_client=self.spotify_client
-                ),
+            self._album = Album.from_json_response(
+                self.album_json, spotify_client=self.spotify_client
             )
 
         return self._album
 
     @property
     def artist(self) -> Artist:
         """Track's parent artist.
@@ -987,15 +896,15 @@
                 Artist.from_json_response(
                     item,
                     spotify_client=self.spotify_client,
                 )
                 for item in self.artists_json
             ]
 
-            self._set_private_attr("_artists", artists)
+            self._artists = artists
 
         return self._artists
 
     @property
     def audio_features(self) -> TrackAudioFeatures | None:
         """Audio features of the track.
 
@@ -1012,18 +921,15 @@
                     f"/audio-features/{self.id}"
                 )
             except HTTPError as exc:
                 if exc.response.status_code == HTTPStatus.NOT_FOUND:
                     return None
                 raise
 
-            self._set_private_attr(
-                "_audio_features",
-                TrackAudioFeatures(**audio_features),
-            )
+            self._audio_features = TrackAudioFeatures(**audio_features)
 
         return self._audio_features
 
     @property
     def release_date(self) -> date:
         """Album release date.
 
@@ -1045,76 +951,81 @@
             return None
 
 
 class Playlist(SpotifyEntity[PlaylistSummaryJson]):
     """A Spotify playlist."""
 
     collaborative: bool
-    followers: Followers | None
+    followers: Followers | None = None
     images: list[Image]
     owner_json: UserSummaryJson = Field(alias="owner")
-    primary_color: str | None
+    primary_color: str | None = None
     # TODO: the `None` cases here can be handled by defaulting `public` to
     #  `self.owner.id == <user ID>`
-    public: bool | None
+    public: bool | None = None
     snapshot_id: str
     tracks_json: PaginatedResponsePlaylistTracks | PlaylistSummaryJsonTracks = Field(
         alias="tracks"
     )
     type: Literal["playlist"]
 
     _tracks: list[Track]
     _owner: User
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = PlaylistSummaryJson
     _live_snapshot_id_timestamp: datetime
     _live_snapshot_id: str
 
+    @field_validator("tracks_json", mode="before")
+    def remove_local_tracks(
+        cls, tracks_json: PaginatedResponsePlaylistTracks  # noqa: N805
+    ) -> PaginatedResponsePlaylistTracks:
+        """Remove local tracks from the playlist's tracklist."""
+
+        if "items" in tracks_json:
+            tracks_json["items"] = [
+                item for item in tracks_json["items"] if not item["is_local"]
+            ]
+
+        return tracks_json
+
     @property
     def live_snapshot_id(self) -> str:
         """The live snapshot ID of the playlist.
 
         Returns:
             str: the live snapshot ID of the playlist
         """
         if (
             not hasattr(self, "_live_snapshot_id_timestamp")
             or not hasattr(self, "_live_snapshot_id")
             or datetime.utcnow() - self._live_snapshot_id_timestamp
             > timedelta(minutes=1)
         ):
-            self._set_private_attr(
-                "_live_snapshot_id",
-                self.spotify_client.get_json_response(
-                    f"/playlists/{self.id}", params={"fields": "snapshot_id"}
-                )[
-                    "snapshot_id"  # type: ignore[typeddict-item]
-                ],
-            )
-            self._set_private_attr(
-                "_live_snapshot_id_timestamp",
-                datetime.utcnow(),
-            )
+            self._live_snapshot_id = self.spotify_client.get_json_response(
+                f"/playlists/{self.id}", params={"fields": "snapshot_id"}
+            )[
+                "snapshot_id"  # type: ignore[typeddict-item]
+            ]
+
+            self._live_snapshot_id_timestamp = datetime.utcnow()
 
         return self._live_snapshot_id
 
     @property
     def owner(self) -> User:
         """Playlist owner.
 
         Returns:
             User: the Spotify user who owns this playlist
         """
 
         if not hasattr(self, "_owner"):
-            self._set_private_attr(
-                "_owner",
-                User.from_json_response(
-                    self.owner_json, spotify_client=self.spotify_client
-                ),
+            self._owner = User.from_json_response(
+                self.owner_json, spotify_client=self.spotify_client
             )
 
         return self._owner
 
     @property
     def tracks(self) -> list[Track]:
         """Return a list of tracks in the playlist.
@@ -1132,20 +1043,20 @@
                 for item in cast(
                     list[PlaylistFullJsonTracks],
                     self.spotify_client.get_items(f"/playlists/{self.id}/tracks"),
                 )
                 if "track" in item.keys() and item["is_local"] is False
             ]
 
-            self._set_private_attr("_tracks", tracks)
+            self._tracks = tracks
 
             if hasattr(self, "_live_snapshot_id"):
                 self.snapshot_id = self._live_snapshot_id
             else:
-                self._set_private_attr("_live_snapshot_id", self.snapshot_id)
+                self._live_snapshot_id = self.snapshot_id
 
         return self._tracks
 
     @property
     def updates_available(self) -> bool:
         """Check if the playlist has updates available.
 
@@ -1191,49 +1102,49 @@
 
 class User(SpotifyEntity[UserSummaryJson]):
     """A Spotify user, usually just the current user."""
 
     PLAYLIST_REFRESH_INTERVAL: ClassVar[timedelta] = timedelta(minutes=10)
 
     display_name: str
-    country: str | None
-    email: str | None
-    explicit_content: dict[str, bool] | None
-    followers: Followers | None
-    images: list[Image] | None
-    product: str | None
+    country: str | None = None
+    email: str | None = None
+    explicit_content: dict[str, bool] | None = None
+    followers: Followers | None = None
+    images: list[Image] | None = None
+    product: str | None = None
     type: Literal["user"]
 
     _albums: list[Album]
     _artists: list[Artist]
     _playlists: list[Playlist]
     _top_artists: tuple[Artist, ...]
     _top_tracks: tuple[Track, ...]
     _tracks: list[Track]
 
     _playlist_refresh_time: datetime
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = UserSummaryJson
 
-    @validator("display_name", pre=True)
+    @field_validator("display_name", mode="before")
     def set_user_name_value(
-        cls, value: str, values: dict[str, Any]  # noqa: N805
+        cls, value: str, info: FieldValidationInfo  # noqa: N805
     ) -> str:
         """Set the user's `name` field to the display name if it is not set.
 
         Args:
-            value: the display name
-            values: the values of the other fields
+            value (str): the display name
+            info (FieldValidationInfo): Object for extra validation information/data.
 
         Returns:
             str: the display name
         """
 
-        if not values["name"]:
-            values["name"] = value
+        if not info.data.get("name"):
+            info.data["name"] = value
 
         return value
 
     def get_playlists_by_name(
         self, name: str, return_all: bool = False
     ) -> list[Playlist] | Playlist | None:
         """Get Playlist instance(s) which have the given name.
@@ -1405,15 +1316,15 @@
                 )
                 for item in cast(
                     list[SavedItem],
                     self.spotify_client.get_items("/me/albums"),
                 )
             ]
 
-            self._set_private_attr("_albums", albums)
+            self._albums = albums
 
         return self._albums
 
     @property
     def artists(self) -> list[Artist]:
         """List of artists in the user's library.
 
@@ -1432,15 +1343,15 @@
                     params={
                         "type": "artist",
                     },
                     top_level_key="artists",
                 )
             ]
 
-            self._set_private_attr("_artists", artists)
+            self._artists = artists
 
         return self._artists
 
     @property
     def current_track(self) -> Track | None:
         """Get the currently playing track for the given user.
 
@@ -1481,15 +1392,15 @@
     def devices(self) -> list[Device]:
         """Return a list of devices that the user currently has access to.
 
         Returns:
             list[Device]: a list of devices available to the user
         """
         return [
-            Device.parse_obj(device_json)
+            Device.model_validate(device_json)
             for device_json in self.spotify_client.get_items(
                 "/me/player/devices", list_key="devices"
             )
         ]
 
     @property
     def playlists(self) -> list[Playlist]:
@@ -1502,28 +1413,28 @@
         if (
             hasattr(self, "_playlist_refresh_time")
             and (datetime.utcnow() - self._playlist_refresh_time)
             < self.PLAYLIST_REFRESH_INTERVAL
         ):
             return self._playlists
 
-        self._set_private_attr("_playlist_refresh_time", datetime.utcnow())
+        self._playlist_refresh_time = datetime.utcnow()
 
         all_playlist_json = cast(
             list[PlaylistSummaryJson], self.spotify_client.get_items("/me/playlists")
         )
 
         if not hasattr(self, "_playlists"):
             playlists = [
                 Playlist.from_json_response(item, spotify_client=self.spotify_client)
                 for item in all_playlist_json
                 if item["owner"]["id"] == self.id
             ]
 
-            self._set_private_attr("_playlists", playlists)
+            self._playlists = playlists
         else:
             existing_ids = (p.id for p in self._playlists)
             new_playlists = [
                 Playlist.from_json_response(item, spotify_client=self.spotify_client)
                 for item in all_playlist_json
                 if item["owner"]["id"] == self.id and item["id"] not in existing_ids
             ]
@@ -1546,15 +1457,15 @@
                     artist_json,
                     spotify_client=self.spotify_client,
                 )
                 for artist_json in self.spotify_client.get_items(
                     "/me/top/artists", params={"time_range": "short_term"}
                 )
             )
-            self._set_private_attr("_top_artists", top_artists)
+            self._top_artists = top_artists
 
         return self._top_artists
 
     @property
     def top_tracks(self) -> tuple[Track, ...]:
         """The top tracks for the user.
 
@@ -1568,15 +1479,15 @@
                     spotify_client=self.spotify_client,
                 )
                 for track_json in self.spotify_client.get_items(
                     "/me/top/tracks", params={"time_range": "short_term"}
                 )
             )
 
-            self._set_private_attr("_top_tracks", top_tracks)
+            self._top_tracks = top_tracks
 
         return self._top_tracks
 
     @property
     def tracks(self) -> list[Track]:
         """Liked Songs.
 
@@ -1592,15 +1503,15 @@
                 )
                 for item in cast(
                     list[SavedItem],
                     self.spotify_client.get_items("/me/tracks"),
                 )
             ]
 
-            self._set_private_attr("_tracks", tracks)
+            self._tracks = tracks
 
         return self._tracks
 
     def reset_properties(
         self,
         property_names: Iterable[
             Literal[
@@ -1629,11 +1540,11 @@
             if hasattr(self, attr_name := f"_{prop_name}"):
                 delattr(self, attr_name)
 
         if "playlists" in property_names:
             delattr(self, "_playlist_refresh_time")
 
 
-SpotifyEntity.update_forward_refs()
-Album.update_forward_refs()
-Artist.update_forward_refs()
-Track.update_forward_refs()
+SpotifyEntity.model_rebuild()
+Album.model_rebuild()
+Artist.model_rebuild()
+Track.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/clients/truelayer.py` & `wg_utilities-4.0.0/wg_utilities/clients/truelayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-# pylint: disable=too-few-public-methods
 """Custom client for interacting with TrueLayer's API."""
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from datetime import date, datetime, timedelta
-from enum import Enum, auto
+from enum import Enum, StrEnum, auto
 from logging import DEBUG, getLogger
 from os.path import sep
 from pathlib import Path
-from typing import Any, ClassVar, Literal, TypeAlias, TypedDict, TypeVar
+from typing import Any, ClassVar, Literal, Self, TypeAlias, TypeVar
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 from requests import HTTPError
-from strenum import StrEnum  # type: ignore[import]
+from typing_extensions import NotRequired, TypedDict
 
 from wg_utilities.clients.json_api_client import StrBytIntFlt
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    GenericModelWithConfig,
-    OAuthClient,
-)
+from wg_utilities.clients.oauth_client import BaseModelWithConfig, OAuthClient
 from wg_utilities.functions import user_data_dir
 from wg_utilities.functions.file_management import force_mkdir
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 
-class AccountType(StrEnum):  # type: ignore[misc]
+class AccountType(StrEnum):
     """Possible TrueLayer account types."""
 
     TRANSACTION = auto()
     SAVINGS = auto()
     BUSINESS_TRANSACTION = auto()
     BUSINESS_SAVINGS = auto()
 
@@ -127,17 +122,17 @@
 
     def __init__(self, value: tuple[str, str], description: tuple[str, str]):
         self._value_ = value
         self.description = description
 
 
 class _AccountNumber(BaseModelWithConfig):
-    iban: str | None
-    number: str | None
-    sort_code: str | None
+    iban: str | None = None
+    number: str | None = None
+    sort_code: str | None = None
     swift_bic: str
 
 
 class _TrueLayerBaseEntityJson(TypedDict):
     account_id: str
     currency: str
     display_name: str
@@ -155,16 +150,16 @@
 class CardJson(_TrueLayerBaseEntityJson):
     """JSON representation of a Card."""
 
     card_network: str
     card_type: str
     partial_card_number: str
     name_on_card: str
-    valid_from: date | None
-    valid_to: date | None
+    valid_from: NotRequired[date]
+    valid_to: NotRequired[date]
 
 
 class BalanceVariables(BaseModelWithConfig):
     """Variables for an account's balance summary."""
 
     available_balance: int
     current_balance: int
@@ -180,18 +175,16 @@
     display_name: str
     logo_uri: str
     id: str = Field(alias="provider_id")
 
 
 TrueLayerEntityJson: TypeAlias = AccountJson | CardJson
 
-FJR = TypeVar("FJR", bound="TrueLayerEntity")
 
-
-class TrueLayerEntity(GenericModelWithConfig):
+class TrueLayerEntity(BaseModelWithConfig):
     """Parent class for all TrueLayer entities (accounts, cards, etc.)."""
 
     BALANCE_FIELDS: ClassVar[Iterable[str]] = ()
 
     id: str = Field(alias="account_id")
     currency: str
     display_name: str
@@ -210,28 +203,24 @@
     truelayer_client: TrueLayerClient = Field(exclude=True)
     balance_update_threshold: timedelta = Field(timedelta(minutes=15), exclude=True)
     last_balance_update: datetime = Field(datetime(1970, 1, 1), exclude=True)
     _balance_variables: BalanceVariables
 
     @classmethod
     def from_json_response(
-        cls: type[FJR], value: TrueLayerEntityJson, *, truelayer_client: TrueLayerClient
-    ) -> FJR:
+        cls, value: TrueLayerEntityJson, *, truelayer_client: TrueLayerClient
+    ) -> Self:
         """Create an account from a JSON response."""
 
         value_data: dict[str, Any] = {
             "truelayer_client": truelayer_client,
             **value,
         }
 
-        instance = cls.parse_obj(value_data)
-
-        instance._validate()  # pylint: disable=protected-access
-
-        return instance
+        return cls.model_validate(value_data)
 
     def get_transactions(
         self,
         from_datetime: datetime | None = None,
         to_datetime: datetime | None = None,
     ) -> list[Transaction]:
         """Get transactions for this entity.
@@ -259,15 +248,15 @@
                 "from": from_datetime.isoformat(),
                 "to": to_datetime.isoformat(),
             }
         else:
             params = None
 
         return [
-            Transaction.parse_obj(result)
+            Transaction.model_validate(result)
             for result in self.truelayer_client.get_json_response(
                 f"/data/v1/{self.__class__.__name__.lower()}s/{self.id}/transactions",
                 params=params,
             ).get("results", [])
         ]
 
     def update_balance_values(self) -> None:
@@ -305,15 +294,16 @@
                 attr_name = f"_{k}"
 
             if attr_name.lstrip("_") not in self.BALANCE_FIELDS:
                 LOGGER.info("Skipping %s as it's not relevant for this entity type", k)
                 continue
 
             LOGGER.info("Updating %s with value %s", attr_name, v)
-            self._set_private_attr(attr_name, v)
+
+            setattr(self, attr_name, v)
 
         self.last_balance_update = datetime.utcnow()
 
     def _get_balance_property(
         self,
         prop_name: Literal[
             "available_balance",
@@ -433,25 +423,25 @@
 class Transaction(BaseModelWithConfig):
     """Class for individual transactions for data manipulation etc."""
 
     amount: float
     currency: str
     description: str
     id: str = Field(alias="transaction_id")
-    merchant_name: str | None
+    merchant_name: str | None = None
     meta: dict[str, str]
-    normalised_provider_transaction_id: str | None
+    normalised_provider_transaction_id: str | None = None
     provider_transaction_id: str | None
-    running_balance: dict[str, str | float] | None
+    running_balance: dict[str, str | float] | None = None
     timestamp: datetime
     transaction_category: TransactionCategory
     transaction_classification: list[str]
     transaction_type: str
 
-    @validator("transaction_category", pre=True)
+    @field_validator("transaction_category", mode="before")
     def validate_transaction_category(  # pylint: disable=no-self-argument
         cls, v: str  # noqa: N805
     ) -> TransactionCategory:
         """Validate the transaction category.
 
         The default Enum assignment doesn't work for some reason, so we have to do it
         here.
@@ -476,26 +466,26 @@
         "available_balance",
         "current_balance",
         "overdraft",
     )
     account_number: _AccountNumber
     account_type: AccountType
 
-    @validator("account_type", pre=True)
+    @field_validator("account_type", mode="before")
     def validate_account_type(  # pylint: disable=no-self-argument
         cls, value: str  # noqa: N805
     ) -> AccountType:
         """Validate `account_type` and parse it into an `AccountType` instance."""
         if isinstance(value, AccountType):
             return value
 
         if value not in AccountType.__members__:  # pragma: no cover
             raise ValueError(f"Invalid account type: `{value}`")
 
-        return AccountType[value.upper()]  # type: ignore[no-any-return,misc]
+        return AccountType[value.upper()]
 
 
 class Card(TrueLayerEntity):
     """Class for managing individual cards."""
 
     BALANCE_FIELDS: ClassVar[Iterable[str]] = (
         "available_balance",
@@ -507,16 +497,16 @@
         "payment_due_date",
     )
 
     card_network: str
     card_type: str
     partial_card_number: str
     name_on_card: str
-    valid_from: date | None
-    valid_to: date | None
+    valid_from: date | None = None
+    valid_to: date | None = None
 
 
 AccountOrCard = TypeVar("AccountOrCard", Account, Card)
 
 
 class TrueLayerClient(OAuthClient[dict[Literal["results"], list[TrueLayerEntityJson]]]):
     """Custom client for interacting with TrueLayer's APIs."""
@@ -695,10 +685,10 @@
 
         Returns:
             list[Account]: Account instances, containing all related info
         """
         return self._list_entities(Card)
 
 
-Account.update_forward_refs()
-Card.update_forward_refs()
-TrueLayerEntity.update_forward_refs()
+Account.model_rebuild()
+Card.model_rebuild()
+TrueLayerEntity.model_rebuild()
```

### Comparing `wg_utilities-3.9.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-4.0.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-4.0.0/wg_utilities/devices/epd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     FRAME_DELAY = 120
 else:
     from .epd7in5_v2 import EPD as EPD_ORIG
 
     _LOGGER.warning("Unable to import E-Paper Driver, running in test mode")
     FRAME_DELAY = 0
 
-    # pylint: disable=too-few-public-methods
     class EPD:  # type: ignore[no-redef]
         """Mirror the functionality of the EPD on devices which don't support it."""
 
     for method in dir(EPD_ORIG):
         if not method.startswith("_"):
             setattr(EPD, method, lambda *a, **k: None)
```

### Comparing `wg_utilities-3.9.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-4.0.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-4.0.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     for func in dir(implementation):
         if not func.startswith("_"):
             setattr(modules[__name__], func, getattr(implementation, func))
 
     TEST_MODE = False
 except (RuntimeError, ImportError):
-    # pylint: disable=too-few-public-methods
+
     class FakeImplementation:
         """Class to cover functionality of implementations on non-supporting devices."""
 
     for method in dir(RaspberryPi):
         if not method.startswith("_"):
             setattr(FakeImplementation, method, lambda *a, **k: None)
```

### Comparing `wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-4.0.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,137 +8,133 @@
 from enum import Enum
 from functools import wraps
 from logging import DEBUG, getLogger
 from re import compile as re_compile
 from textwrap import dedent
 from threading import Thread
 from time import sleep, strptime
-from typing import Any, Literal, TypedDict, TypeVar
+from typing import Any, Literal, TypeVar
 
 from async_upnp_client.aiohttp import AiohttpNotifyServer, AiohttpRequester
 from async_upnp_client.client import UpnpDevice, UpnpService, UpnpStateVariable
 from async_upnp_client.client_factory import UpnpFactory
 from async_upnp_client.exceptions import UpnpCommunicationError
 from async_upnp_client.utils import get_local_ip
-from pydantic import BaseModel, Extra, Field, ValidationError
-from pydantic.error_wrappers import ErrorWrapper
+from pydantic import BaseModel, Field
+from typing_extensions import TypedDict
 from xmltodict import parse as parse_xml
 
 from wg_utilities.functions import traverse_dict
 from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 add_stream_handler(LOGGER)
 
 
-# pylint: disable=too-few-public-methods
-class StateVariable(BaseModel, extra=Extra.allow):
+class StateVariable(BaseModel, extra="allow"):
     """BaseModel for state variables in DLNA payload."""
 
     channel: str
     val: str
 
 
-# pylint: disable=too-few-public-methods
-class CurrentTrackMetaDataItemRes(BaseModel, extra=Extra.allow):
+class CurrentTrackMetaDataItemRes(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     protocolInfo: str  # noqa: N815
     duration: str
-    text: str | None
+    text: str | None = None
 
 
-# pylint: disable=too-few-public-methods
-class TrackMetaDataItem(BaseModel, extra=Extra.allow):
+class TrackMetaDataItem(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     id: str
-    song_subid: str | None = Field("", alias="song:subid")
-    song_description: str | None = Field("", alias="song:description")
-    song_skiplimit: str = Field("", alias="song:skiplimit")
-    song_id: str | None = Field("", alias="song:id")
-    song_like: str = Field("", alias="song:like")
-    song_singerid: str = Field("", alias="song:singerid")
-    song_albumid: str = Field("", alias="song:albumid")
+    song_subid: str | None = Field(None, alias="song:subid")
+    song_description: str | None = Field(None, alias="song:description")
+    song_skiplimit: str | None = Field(None, alias="song:skiplimit")
+    song_id: str | None = Field(None, alias="song:id")
+    song_like: str | None = Field(None, alias="song:like")
+    song_singerid: str | None = Field(None, alias="song:singerid")
+    song_albumid: str | None = Field(None, alias="song:albumid")
     res: CurrentTrackMetaDataItemRes
-    dc_title: str | None = Field(..., alias="dc:title")
-    dc_creator: str | None = Field("", alias="dc:creator")
-    upnp_artist: str | None = Field(..., alias="upnp:artist")
-    upnp_album: str | None = Field(..., alias="upnp:album")
-    upnp_albumArtURI: str = Field(..., alias="upnp:albumArtURI")  # noqa: N815
+    dc_title: str | None = Field(None, alias="dc:title")
+    dc_creator: str | None = Field(None, alias="dc:creator")
+    upnp_artist: str | None = Field(None, alias="upnp:artist")
+    upnp_album: str | None = Field(None, alias="upnp:album")
+    upnp_albumArtURI: str | None = Field(None, alias="upnp:albumArtURI")  # noqa: N815
 
 
-# pylint: disable=too-few-public-methods
-class TrackMetaData(BaseModel, extra=Extra.allow):
+class TrackMetaData(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     item: TrackMetaDataItem
 
 
-class InstanceIDAVTransport(BaseModel, extra=Extra.allow):
+class InstanceIDAVTransport(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     val: str
     TransportState: str
-    TransportStatus: str | None
-    NumberOfTracks: str | None
-    CurrentTrack: str | None
-    CurrentTrackDuration: str | None
-    CurrentMediaDuration: str | None
-    CurrentTrackURI: str | None
-    AVTransportURI: str | None
-    TrackSource: str | None
-    CurrentTrackMetaData: TrackMetaData | None
-    AVTransportURIMetaData: TrackMetaData | None
-    PlaybackStorageMedium: str | None
-    PossiblePlaybackStorageMedia: str | None
-    PossibleRecordStorageMedia: str | None
-    RecordStorageMedium: str | None
-    CurrentPlayMode: str | None
-    TransportPlaySpeed: str | None
-    RecordMediumWriteStatus: str | None
-    CurrentRecordQualityMode: str | None
-    PossibleRecordQualityModes: str | None
-    RelativeTimePosition: str | None
-    AbsoluteTimePosition: str | None
-    RelativeCounterPosition: str | None
-    AbsoluteCounterPosition: str | None
-    CurrentTransportActions: str | None
+    TransportStatus: str | None = None
+    NumberOfTracks: str | None = None
+    CurrentTrack: str | None = None
+    CurrentTrackDuration: str | None = None
+    CurrentMediaDuration: str | None = None
+    CurrentTrackURI: str | None = None
+    AVTransportURI: str | None = None
+    TrackSource: str | None = None
+    CurrentTrackMetaData: TrackMetaData | None = None
+    AVTransportURIMetaData: TrackMetaData | None = None
+    PlaybackStorageMedium: str | None = None
+    PossiblePlaybackStorageMedia: str | None = None
+    PossibleRecordStorageMedia: str | None = None
+    RecordStorageMedium: str | None = None
+    CurrentPlayMode: str | None = None
+    TransportPlaySpeed: str | None = None
+    RecordMediumWriteStatus: str | None = None
+    CurrentRecordQualityMode: str | None = None
+    PossibleRecordQualityModes: str | None = None
+    RelativeTimePosition: str | None = None
+    AbsoluteTimePosition: str | None = None
+    RelativeCounterPosition: str | None = None
+    AbsoluteCounterPosition: str | None = None
+    CurrentTransportActions: str | None = None
 
 
-class InstanceIDRenderingControl(BaseModel, extra=Extra.allow):
+class InstanceIDRenderingControl(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     val: str
     Mute: StateVariable
-    Channel: StateVariable | None
-    Equalizer: StateVariable | None
+    Channel: StateVariable | None = None
+    Equalizer: StateVariable | None = None
     # There's a typo in the schema, this is correct for some payloads -.-
-    Equaluzer: StateVariable | None
+    Equaluzer: StateVariable | None = None
     Volume: StateVariable
-    PresetNameList: str | None
-    TimeStamp: str | None
+    PresetNameList: str | None = None
+    TimeStamp: str | None = None
 
 
-class EventAVTransport(BaseModel, extra=Extra.allow):
+class EventAVTransport(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     xmlns: Literal["urn:schemas-upnp-org:metadata-1-0/AVT/"]
     InstanceID: InstanceIDAVTransport
 
 
-class EventRenderingControl(BaseModel, extra=Extra.allow):
+class EventRenderingControl(BaseModel, extra="allow"):
     """BaseModel for part of the DLNA payload."""
 
     xmlns: Literal["urn:schemas-upnp-org:metadata-1-0/RCS/"]
     InstanceID: InstanceIDRenderingControl
 
 
-class LastChange(BaseModel, extra=Extra.allow):
+class LastChange(BaseModel, extra="allow"):
     """BaseModel for the DLNA payload."""
 
     Event: Any
 
     @classmethod
     def parse(cls, payload: dict[Literal["Event"], object]) -> LastChange:
         """Parse a `LastChange` model from the payload dictionary.
@@ -147,32 +143,26 @@
             payload (Dict[str, Any]): the DLNA DMR payload
 
         Returns:
             LastChange: The parsed `Case`.
 
         Raises:
             TypeError: if the payload isn't a dict
-            ValidationError: If any of the specified model fields are empty or of the
-             wrong type.
-            ValidationError: if more than just "Event" is in the payload
+            ValueError: if more than just "Event" is in the payload
         """
         if not isinstance(payload, dict):
             raise TypeError("Expected a dict")
 
         payload = payload.copy()
 
         event = payload.pop("Event")
 
         if payload:
-            raise ValidationError(
-                [
-                    ErrorWrapper(ValueError("extra fields not permitted"), loc=key)
-                    for key in payload.keys()
-                ],
-                model=cls,
+            raise ValueError(
+                f"Extra fields not permitted: {list(payload.keys())!r}",
             )
 
         return cls(Event=event)
 
 
 class LastChangeAVTransport(LastChange):
     """BaseModel for an AVTransport DLNA payload."""
@@ -1024,15 +1014,15 @@
 
         Returns:
             dict: the current track's info
         """
         if not hasattr(self, "_current_track"):
             media_info = self.get_media_info()
             self._current_track = CurrentTrack.from_get_media_info(
-                GetMediaInfoResponse.parse_obj(media_info)
+                GetMediaInfoResponse.model_validate(media_info)
             )
 
         return self._current_track
 
     @current_track.setter
     def current_track(self, value: CurrentTrack) -> None:
         """Set the current track.
```

### Comparing `wg_utilities-3.9.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-4.0.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/__init__.py` & `wg_utilities-4.0.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/_functions.py` & `wg_utilities-4.0.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-4.0.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/file_management.py` & `wg_utilities-4.0.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/json.py` & `wg_utilities-4.0.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/processes.py` & `wg_utilities-4.0.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-4.0.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/functions/xml.py` & `wg_utilities-4.0.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/loggers/__init__.py` & `wg_utilities-4.0.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/loggers/file_handler.py` & `wg_utilities-4.0.0/wg_utilities/loggers/file_handler.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/loggers/list_handler.py` & `wg_utilities-4.0.0/wg_utilities/loggers/list_handler.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/loggers/stream_handler.py` & `wg_utilities-4.0.0/wg_utilities/loggers/stream_handler.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/wg_utilities/loggers/warehouse_handler.py` & `wg_utilities-4.0.0/wg_utilities/loggers/warehouse_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 """Custom handler to allow logging directly into an Item Warehouse."""
 
 from __future__ import annotations
 
+from asyncio import get_running_loop, run
+from collections.abc import Callable, Iterable, Mapping
 from hashlib import md5
 from http import HTTPStatus
 from json import JSONDecodeError, dumps
-from logging import (
-    CRITICAL,
-    DEBUG,
-    ERROR,
-    INFO,
-    WARNING,
-    Formatter,
-    Handler,
-    Logger,
-    LogRecord,
-    getLogger,
-)
+from logging import DEBUG, WARNING, Formatter, Handler, Logger, LogRecord, getLogger
 from os import getenv
 from socket import gethostname
 from time import gmtime
 from traceback import format_exception
-from typing import Final, Literal, TypedDict, cast
+from types import TracebackType
+from typing import Any, Final, Literal, Protocol, TypeVar
 
 from requests import HTTPError
 from requests.exceptions import RequestException
+from typing_extensions import TypedDict
 
-from wg_utilities.clients.json_api_client import JsonApiClient
+from wg_utilities.clients.json_api_client import JsonApiClient, StrBytIntFlt
 from wg_utilities.loggers.stream_handler import add_stream_handler
 
 FORMATTER = Formatter(
     fmt="%(asctime)s\t%(name)s\t[%(levelname)s]\t%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S%z",
 )
 FORMATTER.converter = gmtime
 
 
 LOGGER = getLogger(__name__)
-LOGGER.setLevel(ERROR)
+LOGGER.setLevel(WARNING)
 add_stream_handler(LOGGER)
 
 
 class WarehouseLogPage(TypedDict):
     """Type for a page of log records."""
 
     count: int
@@ -62,14 +55,67 @@
     logger: str
     message: str
     module: str
     process: str
     thread: str
 
 
+T = TypeVar("T")
+
+
+class _PyscriptTaskExecutorProtocol(Protocol[T]):
+    async def __call__(self, func: Callable[..., T], *args: Any, **kwargs: Any) -> T:
+        ...  # pragma: no cover
+
+
+class HttpErrorHandler:
+    def __init__(self, allow_connection_errors: bool):
+        self._allow_connection_errors = allow_connection_errors
+
+    def __enter__(self) -> HttpErrorHandler:
+        return self
+
+    def __exit__(
+        self,
+        _: type[type] | None,
+        exc: Exception | None,
+        __: TracebackType | None,
+    ) -> bool:
+        if isinstance(exc, HTTPError):
+            error_detail = exc.response.text
+            try:
+                if (error_detail := exc.response.json()).get("detail", {}).get(
+                    "type"
+                ) == "ItemExistsError":
+                    return True
+            except (AttributeError, LookupError, JSONDecodeError):
+                pass
+
+            LOGGER.error(
+                "Error posting log to Warehouse: %i %s; %r",
+                exc.response.status_code,
+                exc.response.reason,
+                error_detail,
+            )
+        elif isinstance(
+            exc,
+            (ConnectionError | RequestException),
+        ):
+            LOGGER.error("Error posting log to Warehouse: %r", exc)
+
+            return self._allow_connection_errors
+        elif exc is not None:  # pragma: no cover
+            raise RuntimeError(f"Unhandled logging exception: {exc!r}") from exc
+
+        return True
+
+
+http_error_handler = HttpErrorHandler
+
+
 class WarehouseHandler(Handler, JsonApiClient[WarehouseLog | WarehouseLogPage]):
     """Custom handler to allow logging directly into an Item Warehouse.
 
     https://github.com/worgarside/addon-item-warehouse
 
     The primary key of the log warehouse is a combination of:
         - log_hash (message content)
@@ -158,91 +204,83 @@
     def __init__(
         self,
         *,
         level: int | Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO",
         warehouse_host: str | None = None,
         warehouse_port: int | None = None,
         allow_connection_errors: bool = False,
+        pyscript_task_executor: _PyscriptTaskExecutorProtocol[
+            WarehouseLog | WarehouseLogPage
+        ]
+        | None = None,
     ) -> None:
         """Initialize the handler and Log Warehouse."""
 
         Handler.__init__(self, level=level)
 
-        warehouse_host = warehouse_host or str(
-            getenv("ITEM_WAREHOUSE_HOST", "http://homeassistant.local")
+        JsonApiClient.__init__(
+            self, base_url=self.get_base_url(warehouse_host, warehouse_port)
         )
-        warehouse_port = warehouse_port or int(getenv("ITEM_WAREHOUSE_PORT", "0"))
-
-        base_url = warehouse_host
-        if warehouse_port:
-            base_url += f":{warehouse_port}"
-        base_url += "/v1"
-
-        JsonApiClient.__init__(self, base_url=base_url)
 
         self._allow_connection_errors = allow_connection_errors
+        self._pyscript_task_executor = pyscript_task_executor
 
-        self._initialize_warehouse()
+        if self._pyscript_task_executor is not None:
+            # Workaround for ensuring the warehouse is still created from Pyscript
+            self._post_json_response(
+                "/warehouses", json=self._WAREHOUSE_SCHEMA, timeout=5
+            )
+        else:
+            self._initialize_warehouse()
 
     def _initialize_warehouse(self) -> None:
         schema: WarehouseLog
         try:
             schema = self.get_json_response(  # type: ignore[assignment]
                 self.WAREHOUSE_ENDPOINT, timeout=5
             )
         except HTTPError as exc:
             if exc.response.status_code == HTTPStatus.NOT_FOUND:
-                schema = self.post_json_response(  # type: ignore[assignment]
+                schema = self._post_json_response(  # type: ignore[assignment]
                     "/warehouses", json=self._WAREHOUSE_SCHEMA, timeout=5
                 )
                 LOGGER.info("Created new Warehouse: %r", schema)
         except (
             ConnectionError,
             RequestException,
         ) as exc:
             LOGGER.exception("Error creating Warehouse: %r", exc)
 
             if not self._allow_connection_errors:
                 raise
         else:
             LOGGER.info(
-                "Warehouse already exists - created at %s",
+                "Warehouse %s already exists - created at %s",
+                schema.get("name", None),
                 schema.pop("created_at", None),  # type: ignore[misc]
             )
             if schema != self._WAREHOUSE_SCHEMA:  # type: ignore[comparison-overlap]
                 raise ValueError(
                     "Warehouse schema does not match expected schema: "
                     + dumps(schema, default=repr)
                 )
 
-    @staticmethod
-    def _get_log_hash(record: LogRecord) -> str:
-        """Get a hash of the log message.
-
-        Args:
-            record (LogRecord): the log record to hash
-
-        Returns:
-            str: the hexdigest of the hash
-        """
-        return md5(record.getMessage().encode()).hexdigest()
-
     def emit(self, record: LogRecord) -> None:
         """Add log record to the internal record store.
 
         Args:
             record (LogRecord): the new log record being "emitted"
         """
 
         log_payload = {
             "created_at": record.created,
             "file": record.pathname,
             "level": record.levelno,
             "line": record.lineno,
-            "log_hash": self._get_log_hash(record),
+            "log_hash": self.get_log_hash(record),
             "log_host": self.HOST_NAME,
             "logger": record.name,
             "message": record.getMessage(),
             "module": record.module,
             "process": record.processName,
             "thread": record.threadName,
         }
@@ -250,154 +288,161 @@
         if record.exc_info and record.exc_info[0]:
             log_payload["exception_message"] = str(record.exc_info[1])
             log_payload["exception_type"] = record.exc_info[0].__name__
             log_payload["exception_traceback"] = "".join(
                 format_exception(record.exc_info[1])
             )
 
-        try:
-            self.post_json_response(
-                f"{self.WAREHOUSE_ENDPOINT}/items",
-                json=log_payload,
-            )
-        except HTTPError as exc:
-            error_detail = exc.response.text
-            try:
-                if (error_detail := exc.response.json()).get("detail", {}).get(
-                    "type"
-                ) == "ItemExistsError":
-                    return
-            except (AttributeError, LookupError, JSONDecodeError):
-                pass
+        self._post_json_response(
+            f"{self.WAREHOUSE_ENDPOINT}/items", json=log_payload, timeout=5
+        )
 
-            LOGGER.error(
-                "Error posting log to Warehouse: %i %s; %r",
-                exc.response.status_code,
-                exc.response.reason,
-                error_detail,
-            )
-        except (
-            ConnectionError,
-            RequestException,
-        ) as exc:
-            LOGGER.error("Error posting log to Warehouse: %r", exc)
+    def _post_json_response(
+        self,
+        url: str,
+        /,
+        *,
+        params: dict[StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None]
+        | None = None,
+        header_overrides: Mapping[str, str | bytes] | None = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
+        json: Any | None = None,
+        data: Any | None = None,
+    ) -> WarehouseLog | WarehouseLogPage | None:
+        """Post a JSON response to the warehouse.
 
-            if not self._allow_connection_errors:
-                raise
-        except Exception as exc:  # pylint: disable=broad-except # pragma: no cover
-            LOGGER.error(repr(exc))
+        This is overridden to allow compatibility with Pyscript.
+        https://hacs-pyscript.readthedocs.io/en/latest/reference.html#task-executor
+        """
+        if self._pyscript_task_executor is not None:
+            self._run_pyscript_task_executor(
+                self.post_json_response,
+                url,
+                params=params,
+                header_overrides=header_overrides,
+                timeout=timeout,
+                json=json,
+                data=data,
+            )
+            return None
 
-    def _get_records(self, level: int | None = None) -> list[LogRecord]:
-        """Get log records from the warehouse.
+        with http_error_handler(self._allow_connection_errors):
+            return self.post_json_response(
+                url,
+                params=params,
+                header_overrides=header_overrides,
+                timeout=timeout,
+                json=json,
+                data=data,
+            )
 
-        Args:
-            level (int): the logging level to filter by
+        return None
 
-        Returns:
-            list: a list of log records
-        """
-        url = f"{self.WAREHOUSE_ENDPOINT}/items?log_host={self.HOST_NAME}"
+    async def _async_task_executor(
+        self, func: Callable[..., Any], *args: Any, **kwargs: Any
+    ) -> None:
+        if (
+            not hasattr(self, "_pyscript_task_executor")
+            or not self._pyscript_task_executor
+        ):
+            raise NotImplementedError("Pyscript task executor is not defined")
 
-        if level is not None:
-            url += f"&level={level}"
+        with http_error_handler(self._allow_connection_errors):
+            await self._pyscript_task_executor(func, *args, **kwargs)
 
-        return [
-            LogRecord(
-                name=record["logger"],
-                level=record["level"],
-                pathname=record["file"],
-                lineno=record["line"],
-                msg=record["message"],
-                args=(),
-                exc_info=None,  # TODO: add exception info
-            )
-            for record in cast(WarehouseLogPage, self.get_json_response(url))["items"]
-        ]
+    def _run_pyscript_task_executor(
+        self, func: Callable[..., Any], *args: Any, **kwargs: Any
+    ) -> None:
+        try:
+            loop = get_running_loop()
+        except RuntimeError:
+            loop = None
+
+        if loop and loop.is_running():
+            loop.create_task(self._async_task_executor(func, *args, **kwargs))
+            return
 
-    @property
-    def records(self) -> list[LogRecord]:
-        """All records.
+        run(self._async_task_executor(func, *args, **kwargs))
 
-        Returns:
-            list: a list of all log records
-        """
-        return self._get_records()
+    @staticmethod
+    def get_base_url(host: str | None, port: int | None) -> str:
+        """Get the base URL for the Item Warehouse.
 
-    @property
-    def debug_records(self) -> list[LogRecord]:
-        """Debug level records.
+        Args:
+            host (str): the hostname of the Item Warehouse
+            port (int): the port of the Item Warehouse
 
         Returns:
-            list: a list of log records with the level DEBUG
+            str: the base URL for the Item Warehouse
         """
-        return self._get_records(DEBUG)
 
-    @property
-    def info_records(self) -> list[LogRecord]:
-        """Info level records.
+        host = host or str(getenv("ITEM_WAREHOUSE_HOST", "http://homeassistant.local"))
+        port = port or int(getenv("ITEM_WAREHOUSE_PORT", "0"))
 
-        Returns:
-            list: a list of log records with the level INFO
-        """
-        return self._get_records(INFO)
+        if port:
+            host += f":{port}"
 
-    @property
-    def warning_records(self) -> list[LogRecord]:
-        """Warning level records.
+        host += "/v1"
 
-        Returns:
-            list: a list of log records with the level WARNING
-        """
-        return self._get_records(WARNING)
-
-    @property
-    def error_records(self) -> list[LogRecord]:
-        """Error level records.
+        return host
 
-        Returns:
-            list: a list of log records with the level ERROR
-        """
-        return self._get_records(ERROR)
+    @staticmethod
+    def get_log_hash(record: LogRecord) -> str:
+        """Get a hash of the log message.
 
-    @property
-    def critical_records(self) -> list[LogRecord]:
-        """Critical level records.
+        Args:
+            record (LogRecord): the log record to hash
 
         Returns:
-            list: a list of log records with the level CRITICAL
+            str: the hexdigest of the hash
         """
-        return self._get_records(CRITICAL)
+        return md5(record.getMessage().encode()).hexdigest()
 
 
 def add_warehouse_handler(
     logger: Logger,
     *,
     level: int = DEBUG,
     warehouse_host: str | None = None,
     warehouse_port: int | None = None,
     allow_connection_errors: bool = False,
+    pyscript_task_executor: _PyscriptTaskExecutorProtocol[
+        WarehouseLog | WarehouseLogPage
+    ]
+    | None = None,
 ) -> WarehouseHandler:
     """Add a ListHandler to an existing logger.
 
     Args:
         logger (Logger): the logger to add a file handler to
         level (int): the logging level to be used for the WarehouseHandler
         warehouse_host (str): the hostname of the Item Warehouse
         warehouse_port (int): the port of the Item Warehouse
         allow_connection_errors (bool): whether to allow connection errors
+        pyscript_task_executor (Callable): the Pyscript task executor (if applicable)
 
     Returns:
         WarehouseHandler: the WarehouseHandler that was added to the logger
     """
 
+    for handler in logger.handlers:
+        if isinstance(
+            handler, WarehouseHandler
+        ) and handler.base_url == WarehouseHandler.get_base_url(
+            warehouse_host, warehouse_port
+        ):
+            LOGGER.warning("WarehouseHandler already exists for %s", handler.base_url)
+            return handler
+
     wh_handler = WarehouseHandler(
         level=level,
         warehouse_host=warehouse_host,
         warehouse_port=warehouse_port,
         allow_connection_errors=allow_connection_errors,
+        pyscript_task_executor=pyscript_task_executor,
     )
 
     logger.addHandler(wh_handler)
 
     return wh_handler
```

### Comparing `wg_utilities-3.9.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-4.0.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.9.0/PKG-INFO` & `wg_utilities-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.9.0
+Version: 4.0.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: clients
 Provides-Extra: devices-dht22
 Provides-Extra: devices-epd
 Provides-Extra: devices-yamaha-yas-209
 Provides-Extra: exceptions
 Provides-Extra: functions
 Requires-Dist: async-upnp-client ; extra == "devices-yamaha-yas-209"
 Requires-Dist: botocore
 Requires-Dist: flask (>=2.0.2) ; extra == "clients"
 Requires-Dist: jetson.gpio ; sys_platform == "linux"
 Requires-Dist: lxml (==4.9.3) ; extra == "functions"
 Requires-Dist: pigpio ; extra == "devices-dht22"
 Requires-Dist: pillow ; extra == "devices-epd"
-Requires-Dist: pydantic (<2.0.0) ; extra == "clients" or extra == "devices-yamaha-yas-209"
+Requires-Dist: pydantic (<3.0.0) ; extra == "clients" or extra == "devices-yamaha-yas-209"
 Requires-Dist: pyjwt (>=2.6,<2.9) ; extra == "clients"
 Requires-Dist: python-dotenv ; extra == "clients" or extra == "exceptions"
 Requires-Dist: pytz (>=2022.1) ; extra == "clients"
 Requires-Dist: requests (>=2.26.0) ; extra == "clients" or extra == "exceptions"
 Requires-Dist: rpi.gpio ; (sys_platform == "linux") and (extra == "devices-epd")
 Requires-Dist: spidev ; (sys_platform == "linux") and (extra == "devices-epd")
-Requires-Dist: strenum ; extra == "clients"
 Requires-Dist: tzlocal ; extra == "clients"
 Requires-Dist: xmltodict ; extra == "devices-yamaha-yas-209"
 Project-URL: Repository, https://github.com/worgarside/wg-utilities
 Description-Content-Type: text/markdown
 
 # WG Utilities
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/worgarside/wg-utilities)
```

