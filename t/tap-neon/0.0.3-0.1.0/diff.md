# Comparing `tmp/tap_neon-0.0.3.tar.gz` & `tmp/tap_neon-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_neon-0.0.3.tar", max compression
+gzip compressed data, was "tap_neon-0.1.0.tar", max compression
```

## Comparing `tap_neon-0.0.3.tar` & `tap_neon-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2631 2023-07-12 23:27:58.701577 tap_neon-0.0.3/README.md
--rw-r--r--   0        0        0     1815 2023-07-12 23:28:15.361608 tap_neon-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       79 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/__init__.py
--rw-r--r--   0        0        0      107 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/__main__.py
--rw-r--r--   0        0        0     2593 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/client.py
--rw-r--r--   0        0        0     3543 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/streams.py
--rw-r--r--   0        0        0     2905 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/tap.py
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 tap_neon-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2631 2023-08-08 16:38:17.655396 tap_neon-0.1.0/README.md
+-rw-r--r--   0        0        0     1815 2023-08-08 16:38:38.824642 tap_neon-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-08-08 16:38:17.655396 tap_neon-0.1.0/tap_neon/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-08 16:38:17.655396 tap_neon-0.1.0/tap_neon/__main__.py
+-rw-r--r--   0        0        0     2593 2023-08-08 16:38:17.655396 tap_neon-0.1.0/tap_neon/client.py
+-rw-r--r--   0        0        0     3543 2023-08-08 16:38:17.655396 tap_neon-0.1.0/tap_neon/streams.py
+-rw-r--r--   0        0        0     2905 2023-08-08 16:38:17.655396 tap_neon-0.1.0/tap_neon/tap.py
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 tap_neon-0.1.0/PKG-INFO
```

### Comparing `tap_neon-0.0.3/README.md` & `tap_neon-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.3/pyproject.toml` & `tap_neon-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core<2,>=1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-neon"
-version = "0.0.3"
+version = "0.1.0"
 description = "`tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramirez <edgarrm358@gmail.com>"]
 keywords = ["ELT", "singer.io", "Neon Serverless Postgres"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-neon"
 repository = "https://github.com/edgarrmondragon/tap-neon"
```

### Comparing `tap_neon-0.0.3/tap_neon/client.py` & `tap_neon-0.1.0/tap_neon/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             "User-Agent": f"{self.tap_name}/{self._tap.plugin_version}",
             "Content-Type": "application/json",
         }
 
     def get_url_params(
         self,
         context: dict | None,  # noqa: ARG002
-        next_page_token: Any | None,
+        next_page_token: str | None,
     ) -> dict[str, Any]:
         """Get URL query parameters.
 
         Args:
             context: Stream sync context.
             next_page_token: Next offset.
```

### Comparing `tap_neon-0.0.3/tap_neon/streams.py` & `tap_neon-0.1.0/tap_neon/streams.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.3/tap_neon/tap.py` & `tap_neon-0.1.0/tap_neon/tap.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.3/PKG-INFO` & `tap_neon-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-neon
-Version: 0.0.3
+Version: 0.1.0
 Summary: `tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-neon
 License: Apache 2.0
 Keywords: ELT,singer.io,Neon Serverless Postgres
 Author: Edgar Ramirez
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
```

