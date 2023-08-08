# Comparing `tmp/paaster-1.1.0.tar.gz` & `tmp/paaster-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paaster-1.1.0.tar", max compression
+gzip compressed data, was "paaster-1.1.1.tar", max compression
```

## Comparing `paaster-1.1.0.tar` & `paaster-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-08-06 13:35:01.955941 paaster-1.1.0/LICENSE
--rw-r--r--   0        0        0     1044 2023-08-06 13:35:01.955941 paaster-1.1.0/README.md
--rw-r--r--   0        0        0     4176 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/__init__.py
--rw-r--r--   0        0        0      332 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/misc.py
--rw-r--r--   0        0        0     1445 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/storage.py
--rw-r--r--   0        0        0      522 2023-08-06 13:35:01.955941 paaster-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 paaster-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 00:21:19.412409 paaster-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1060 2023-08-08 00:21:19.412409 paaster-1.1.1/README.md
+-rw-r--r--   0        0        0     4176 2023-08-08 00:21:19.412409 paaster-1.1.1/paaster_cli/__init__.py
+-rw-r--r--   0        0        0      332 2023-08-08 00:21:19.412409 paaster-1.1.1/paaster_cli/misc.py
+-rw-r--r--   0        0        0     1445 2023-08-08 00:21:19.412409 paaster-1.1.1/paaster_cli/storage.py
+-rw-r--r--   0        0        0      522 2023-08-08 00:21:19.412409 paaster-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 paaster-1.1.1/PKG-INFO
```

### Comparing `paaster-1.1.0/LICENSE` & `paaster-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paaster-1.1.0/README.md` & `paaster-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 ## Commands
 - `paaster --help`: Shows available commands.
 - `paaster upload`: Upload locally encrypted clipboard to the API.
 
     Options:
     - `-m, --mode TEXT`: Specify the mode for the paste, choose from "clipboard", "file", or "inline". (default: clipboard)
-    - `-ctc, --copy_to_clipboard BOOLEAN`: Overwrite COPY_URL_TO_CLIPBOARD setting. (default: True)
-    - `-ob, --open_browser BOOLEAN`: Overwrite OPEN_URL_IN_BROWSER setting. (default: True)
-    - `-eu, --echo_url BOOLEAN`: Overwrite ECHO_URL setting. (default: False)
+    - `-ctc, --copy_to_clipboard BOOLEAN`: Overwrite COPY_URL_TO_CLIPBOARD setting.
+    - `-ob, --open_browser BOOLEAN`: Overwrite OPEN_URL_IN_BROWSER setting.
+    - `-eu, --echo_url BOOLEAN`: Overwrite ECHO_URL setting.
 
 - `paaster set --name "" --value ""`: Set config parameters.
 
 ## Parameters
 - `API_URL`: Backend URL, type: string.
 - `FRONTEND_URL`: Frontend URL, type: string.
 - `COPY_URL_TO_CLIPBOARD`: Copy URL to clipboard, type: "true/false".
 - `OPEN_URL_IN_BROWSER`: Open paste in the browser, type: "true/false".
+- `ECHO_URL`: Echo the paste URL in terminal, type: "true/false"
```

### Comparing `paaster-1.1.0/paaster_cli/__init__.py` & `paaster-1.1.1/paaster_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paaster-1.1.0/paaster_cli/storage.py` & `paaster-1.1.1/paaster_cli/storage.py`

 * *Files identical despite different names*

### Comparing `paaster-1.1.0/pyproject.toml` & `paaster-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paaster"
-version = "1.1.0"
+version = "1.1.1"
 description = "Upload locally encrypted pastes from your terminal to Paaster"
 authors = ["WardPearce <wardpearce@protonmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "paaster_cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `paaster-1.1.0/PKG-INFO` & `paaster-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paaster
-Version: 1.1.0
+Version: 1.1.1
 Summary: Upload locally encrypted pastes from your terminal to Paaster
 License: GPL-3.0
 Author: WardPearce
 Author-email: wardpearce@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -28,19 +28,20 @@
 
 ## Commands
 - `paaster --help`: Shows available commands.
 - `paaster upload`: Upload locally encrypted clipboard to the API.
 
     Options:
     - `-m, --mode TEXT`: Specify the mode for the paste, choose from "clipboard", "file", or "inline". (default: clipboard)
-    - `-ctc, --copy_to_clipboard BOOLEAN`: Overwrite COPY_URL_TO_CLIPBOARD setting. (default: True)
-    - `-ob, --open_browser BOOLEAN`: Overwrite OPEN_URL_IN_BROWSER setting. (default: True)
-    - `-eu, --echo_url BOOLEAN`: Overwrite ECHO_URL setting. (default: False)
+    - `-ctc, --copy_to_clipboard BOOLEAN`: Overwrite COPY_URL_TO_CLIPBOARD setting.
+    - `-ob, --open_browser BOOLEAN`: Overwrite OPEN_URL_IN_BROWSER setting.
+    - `-eu, --echo_url BOOLEAN`: Overwrite ECHO_URL setting.
 
 - `paaster set --name "" --value ""`: Set config parameters.
 
 ## Parameters
 - `API_URL`: Backend URL, type: string.
 - `FRONTEND_URL`: Frontend URL, type: string.
 - `COPY_URL_TO_CLIPBOARD`: Copy URL to clipboard, type: "true/false".
 - `OPEN_URL_IN_BROWSER`: Open paste in the browser, type: "true/false".
+- `ECHO_URL`: Echo the paste URL in terminal, type: "true/false"
```

