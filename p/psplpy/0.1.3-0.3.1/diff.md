# Comparing `tmp/psplpy-0.1.3.tar.gz` & `tmp/psplpy-0.3.1.tar.gz`

## Comparing `psplpy-0.1.3.tar` & `psplpy-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 psplpy-0.1.3/requirements.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/_test.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/autogui_util.py
--rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/data_access.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/file_util.py
--rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/image_util.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/interact_util.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/ocr_util.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/other_util.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/time_util.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/AdbWinApi.dll
--rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/AdbWinUsbApi.dll
--rw-r--r--   0        0        0  1073895 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/NOTICE.txt
--rwxr-xr-x   0        0        0  5938176 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/adb.exe
--rwxr-xr-x   0        0        0   241664 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/dmtracedump.exe
--rwxr-xr-x   0        0        0   430592 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/etc1tool.exe
--rwxr-xr-x   0        0        0  1830912 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/fastboot.exe
--rwxr-xr-x   0        0        0    44032 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/hprof-conv.exe
--rw-r--r--   0        0        0   231594 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/libwinpthread-1.dll
--rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/make_f2fs.exe
--rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/make_f2fs_casefold.exe
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/mke2fs.conf
--rwxr-xr-x   0        0        0   745472 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/mke2fs.exe
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/source.properties
--rwxr-xr-x   0        0        0  1330176 2020-02-02 00:00:00.000000 psplpy-0.1.3/psplpy/tools/platform-tools/sqlite3.exe
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 psplpy-0.1.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 psplpy-0.1.3/LICENSE
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 psplpy-0.1.3/README.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 psplpy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 psplpy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 psplpy-0.3.1/requirements.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/__init__.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/_test.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/auto_wechat.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/autogui_util.py
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/data_access.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/file_util.py
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/image_util.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/interact_util.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/ocr_util.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/other_util.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/time_it.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/time_util.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/data/time_it_template.txt
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/AdbWinApi.dll
+-rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/AdbWinUsbApi.dll
+-rw-r--r--   0        0        0  1073895 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/NOTICE.txt
+-rwxr-xr-x   0        0        0  5938176 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/adb.exe
+-rwxr-xr-x   0        0        0   241664 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/dmtracedump.exe
+-rwxr-xr-x   0        0        0   430592 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/etc1tool.exe
+-rwxr-xr-x   0        0        0  1830912 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/fastboot.exe
+-rwxr-xr-x   0        0        0    44032 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/hprof-conv.exe
+-rw-r--r--   0        0        0   231594 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/libwinpthread-1.dll
+-rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/make_f2fs.exe
+-rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/make_f2fs_casefold.exe
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/mke2fs.conf
+-rwxr-xr-x   0        0        0   745472 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/mke2fs.exe
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/source.properties
+-rwxr-xr-x   0        0        0  1330176 2020-02-02 00:00:00.000000 psplpy-0.3.1/psplpy/tools/platform-tools/sqlite3.exe
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 psplpy-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 psplpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 psplpy-0.3.1/README.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 psplpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 psplpy-0.3.1/PKG-INFO
```

### Comparing `psplpy-0.1.3/psplpy/autogui_util.py` & `psplpy-0.3.1/psplpy/autogui_util.py`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/data_access.py` & `psplpy-0.3.1/psplpy/data_access.py`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/image_util.py` & `psplpy-0.3.1/psplpy/image_util.py`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/interact_util.py` & `psplpy-0.3.1/psplpy/interact_util.py`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/ocr_util.py` & `psplpy-0.3.1/psplpy/ocr_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import re
 import time
 from typing import Tuple, List, Any
-
 import pyautogui
 from PIL import Image
 
 import file_util
 import image_util
 import other_util
 
@@ -23,14 +22,15 @@
 
     def __init__(self, detect_module: str = 'PaddleOCR', lang: str = 'chs', debug: bool = False,
                  debug_dir: str = os.path.join(file_util.get_this_dir_abspath(__file__), r'debug\ocr_pic'),
                  logger=other_util.default_logger(), log_path: str = None, use_gpu: bool = False):
         self.detect_module = detect_module.casefold()
         self.debug = debug
         self.debug_dir = debug_dir
+        file_util.create_dir(self.debug_dir)
         self.logger = logger
         if not log_path:
             self.log_path = os.path.join(self.debug_dir, 'pyocr.log')
         else:
             self.log_path = log_path
         if self.debug:
             t1 = time.monotonic()
@@ -137,7 +137,11 @@
         elif self.detect_module in ['paddleocr', 'easyocr']:
             raise ValueError(f'{self.detect_module} not support this function')
         else:
             raise ValueError(f'Module {self.detect_module} not exist')
         return result
 
 
+if __name__ == '__main__':
+    ocr = PyOcr(debug=True, use_gpu=True)
+    l = ocr.get_text_info_list()
+    print(l)
```

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/AdbWinApi.dll` & `psplpy-0.3.1/psplpy/tools/platform-tools/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/AdbWinUsbApi.dll` & `psplpy-0.3.1/psplpy/tools/platform-tools/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/NOTICE.txt` & `psplpy-0.3.1/psplpy/tools/platform-tools/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/adb.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/adb.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/dmtracedump.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/dmtracedump.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/etc1tool.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/etc1tool.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/fastboot.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/fastboot.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/hprof-conv.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/hprof-conv.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/libwinpthread-1.dll` & `psplpy-0.3.1/psplpy/tools/platform-tools/libwinpthread-1.dll`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/make_f2fs.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/make_f2fs.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/make_f2fs_casefold.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/make_f2fs_casefold.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/mke2fs.conf` & `psplpy-0.3.1/psplpy/tools/platform-tools/mke2fs.conf`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/mke2fs.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/mke2fs.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/psplpy/tools/platform-tools/sqlite3.exe` & `psplpy-0.3.1/psplpy/tools/platform-tools/sqlite3.exe`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/LICENSE` & `psplpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psplpy-0.1.3/pyproject.toml` & `psplpy-0.3.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "psplpy"
-version = "0.1.3"
+version = "0.3.1"
 authors = []
 description = "The Personal Study Purposes Library of PYthon."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ddddocr",
     "easyocr",
     "paddleocr",
+    "uiautomation",
     "numpy==1.24.4",
     "Pillow==9.5.0",
     "PyAutoGUI==0.9.54",
     "pynput==1.7.6",
 ]
```

### Comparing `psplpy-0.1.3/PKG-INFO` & `psplpy-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 0.1.3
+Version: 0.3.1
 Summary: The Personal Study Purposes Library of PYthon.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: ddddocr
 Requires-Dist: easyocr
 Requires-Dist: numpy==1.24.4
 Requires-Dist: paddleocr
 Requires-Dist: pillow==9.5.0
 Requires-Dist: pyautogui==0.9.54
 Requires-Dist: pynput==1.7.6
+Requires-Dist: uiautomation
 Description-Content-Type: text/markdown
 
 # PSPLPY
 
 The **P**ersonal **S**tudy **P**urposes **L**ibrary of **PY**thon.
 
 It's only a python library for personal study purposes.
```

