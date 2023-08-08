# Comparing `tmp/pypdl-1.0.4.tar.gz` & `tmp/pypdl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdl-1.0.4.tar", last modified: Sat Jul  8 08:23:13 2023, max compression
+gzip compressed data, was "pypdl-1.0.5.tar", last modified: Tue Aug  8 16:08:21 2023, max compression
```

## Comparing `pypdl-1.0.4.tar` & `pypdl-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:23:13.261654 pypdl-1.0.4/
--rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     9378 2023-07-08 08:23:13.260660 pypdl-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8789 2023-07-08 08:22:59.000000 pypdl-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 08:23:13.243043 pypdl-1.0.4/pypdl/
--rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-1.0.4/pypdl/__init__.py
--rw-rw-rw-   0        0        0    14287 2023-07-08 08:14:48.000000 pypdl-1.0.4/pypdl/main.py
--rw-rw-rw-   0        0        0     1228 2023-07-08 08:11:19.000000 pypdl-1.0.4/pypdl/test.py
--rw-rw-rw-   0        0        0     6412 2023-07-08 08:14:46.000000 pypdl-1.0.4/pypdl/utls.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:23:13.259655 pypdl-1.0.4/pypdl.egg-info/
--rw-rw-rw-   0        0        0     9378 2023-07-08 08:23:13.000000 pypdl-1.0.4/pypdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-08 08:23:13.000000 pypdl-1.0.4/pypdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:23:13.000000 pypdl-1.0.4/pypdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 08:23:13.000000 pypdl-1.0.4/pypdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 08:23:13.000000 pypdl-1.0.4/pypdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 08:23:13.261654 pypdl-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-07-08 08:23:09.000000 pypdl-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 16:08:21.258651 pypdl-1.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     9378 2023-08-08 16:08:21.258651 pypdl-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8789 2023-07-08 08:22:59.000000 pypdl-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 16:08:21.238354 pypdl-1.0.5/pypdl/
+-rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-1.0.5/pypdl/__init__.py
+-rw-rw-rw-   0        0        0    14309 2023-08-08 16:03:12.000000 pypdl-1.0.5/pypdl/main.py
+-rw-rw-rw-   0        0        0     1226 2023-07-08 08:27:36.000000 pypdl-1.0.5/pypdl/test.py
+-rw-rw-rw-   0        0        0     6436 2023-08-08 15:59:37.000000 pypdl-1.0.5/pypdl/utls.py
+drwxrwxrwx   0        0        0        0 2023-08-08 16:08:21.256135 pypdl-1.0.5/pypdl.egg-info/
+-rw-rw-rw-   0        0        0     9378 2023-08-08 16:08:21.000000 pypdl-1.0.5/pypdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-08 16:08:21.000000 pypdl-1.0.5/pypdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 16:08:21.000000 pypdl-1.0.5/pypdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 16:08:21.000000 pypdl-1.0.5/pypdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 16:08:21.000000 pypdl-1.0.5/pypdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 16:08:21.259652 pypdl-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-08-08 16:04:52.000000 pypdl-1.0.5/setup.py
```

### Comparing `pypdl-1.0.4/LICENSE` & `pypdl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdl-1.0.4/PKG-INFO` & `pypdl-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 1.0.4
+Version: 1.0.5
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-1.0.4/README.md` & `pypdl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pypdl-1.0.4/pypdl/main.py` & `pypdl-1.0.5/pypdl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             multithread (bool): Whether to use multi-threaded download.
         """
         # progress file to keep track of download progress
         json_file = Path(filepath + ".progress.json")
         threads = []
         f_path = str(filepath)
         # get the header information for the file
-        head = requests.head(url, timeout=20)
+        head = requests.head(url, timeout=20, allow_redirects=True)
         # get the total size of the file from the header
         total = int(head.headers.get("content-length"))
         self.totalMB = total / 1048576  # 1MB = 1048576 bytes (size in MB)
         started = datetime.now()
         singlethread = False
 
         # adjust the number of connections for small files
```

### Comparing `pypdl-1.0.4/pypdl/test.py` & `pypdl-1.0.5/pypdl/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from main import Downloader
 import time
 
 if __name__ == "__main__":
     d = Downloader()
-    url = "https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe"
-    # url = r"https://upcdn.io/kW15bUL/raw/y2mate.com%20-%20How%20to%20make%20dlls%20for%20m%20centers%20Minecraft%20bedrock_1080p.mp4"
-    # d.headers = {"Authorization": "Bearer public_kW15bUL8oWrFf4ZvEEcU5cGfpMp3"}
+    # url = "https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe"
+    url = r"https://upcdn.io/kW15bUL/raw/y2mate.com%20-%20How%20to%20make%20dlls%20for%20m%20centers%20Minecraft%20bedrock_1080p.mp4"
+    d.headers = {"Authorization": "Bearer public_kW15bUL8oWrFf4ZvEEcU5cGfpMp3"}
     d.start(
         url,
-        "r.exe",
+        "r.mp4",
         2,
         retries=2,
         display=True,
         multithread=True,
         block=False
     )
```

### Comparing `pypdl-1.0.4/pypdl/utls.py` & `pypdl-1.0.5/pypdl/utls.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             # corruption check to make sure parts are not corrupted
             if start > end:
                 os.remove(path)
                 self.error.set()
                 print("corrupted file!")
 
         url = self.getval("url")
-        # not updating self.header because some wierd bug that cause the file to be unopenable
+        # not updating self.header because it will reference the orginal headers dict and adding to it will cause bugs
         headers = {"range": f"bytes={start}-{end}"}
         headers.update(self.headers)
 
         if self.curr != self.getval("size"):
             try:
                 # download part
                 with requests.session() as s, open(path, "ab+") as f:
```

### Comparing `pypdl-1.0.4/pypdl.egg-info/PKG-INFO` & `pypdl-1.0.5/pypdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 1.0.4
+Version: 1.0.5
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-1.0.4/setup.py` & `pypdl-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'A concurrent python download manager'
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="pypdl",
     version=VERSION,
```

