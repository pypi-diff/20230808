# Comparing `tmp/HyIo-0.2.2.tar.gz` & `tmp/HyIo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyIo-0.2.2.tar", last modified: Tue Aug  1 18:26:01 2023, max compression
+gzip compressed data, was "HyIo-0.2.3.tar", last modified: Tue Aug  8 12:04:37 2023, max compression
```

## Comparing `HyIo-0.2.2.tar` & `HyIo-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-01 18:26:01.142907 HyIo-0.2.2/
-drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-01 18:26:01.142907 HyIo-0.2.2/HyIo/
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      226 2023-08-01 18:21:11.000000 HyIo-0.2.2/HyIo/__main__.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1280 2023-08-01 17:14:27.000000 HyIo-0.2.2/HyIo/debounce.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      456 2023-07-27 12:51:06.000000 HyIo-0.2.2/HyIo/device.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      517 2023-08-01 18:11:13.000000 HyIo-0.2.2/HyIo/gpioDevice.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      562 2023-08-01 18:11:22.000000 HyIo-0.2.2/HyIo/i2cDevice.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)     2170 2023-08-01 18:09:50.000000 HyIo-0.2.2/HyIo/ioManager.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)        0 2023-07-24 05:55:55.000000 HyIo-0.2.2/HyIo/main.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      662 2023-07-27 20:15:37.000000 HyIo-0.2.2/HyIo/parser.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1858 2023-08-01 18:11:31.000000 HyIo-0.2.2/HyIo/pin.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1020 2023-08-01 18:10:07.000000 HyIo-0.2.2/HyIo/test_debounce.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      415 2023-07-27 12:56:45.000000 HyIo-0.2.2/HyIo/test_device.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      779 2023-08-01 18:10:11.000000 HyIo-0.2.2/HyIo/test_ioManager.py
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      456 2023-08-01 18:09:58.000000 HyIo-0.2.2/HyIo/test_pin.py
-drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-01 18:26:01.142907 HyIo-0.2.2/HyIo.egg-info/
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      759 2023-08-01 18:26:01.000000 HyIo-0.2.2/HyIo.egg-info/PKG-INFO
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      401 2023-08-01 18:26:01.000000 HyIo-0.2.2/HyIo.egg-info/SOURCES.txt
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)        1 2023-08-01 18:26:01.000000 HyIo-0.2.2/HyIo.egg-info/dependency_links.txt
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)       16 2023-08-01 18:26:01.000000 HyIo-0.2.2/HyIo.egg-info/requires.txt
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)        5 2023-08-01 18:26:01.000000 HyIo-0.2.2/HyIo.egg-info/top_level.txt
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1069 2023-07-12 23:16:08.000000 HyIo-0.2.2/LICENSE
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      759 2023-08-01 18:26:01.142907 HyIo-0.2.2/PKG-INFO
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)       77 2023-08-01 18:20:48.000000 HyIo-0.2.2/README.md
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)       79 2023-08-01 18:26:01.146240 HyIo-0.2.2/setup.cfg
--rw-r--r--   0 erikcm    (1000) erikcm    (1000)      891 2023-08-01 18:24:29.000000 HyIo-0.2.2/setup.py
+drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-08 12:04:37.499979 HyIo-0.2.3/
+drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-08 12:04:37.496645 HyIo-0.2.3/HyIo/
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      226 2023-08-01 18:21:11.000000 HyIo-0.2.3/HyIo/__main__.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1511 2023-08-08 11:59:48.000000 HyIo-0.2.3/HyIo/debounce.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      456 2023-07-27 12:51:06.000000 HyIo-0.2.3/HyIo/device.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      517 2023-08-01 18:11:13.000000 HyIo-0.2.3/HyIo/gpioDevice.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      555 2023-08-03 20:09:35.000000 HyIo-0.2.3/HyIo/i2cDevice.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     2170 2023-08-01 18:09:50.000000 HyIo-0.2.3/HyIo/ioManager.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)        0 2023-07-24 05:55:55.000000 HyIo-0.2.3/HyIo/main.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     2385 2023-08-08 11:53:48.000000 HyIo-0.2.3/HyIo/parser.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1858 2023-08-01 18:11:31.000000 HyIo-0.2.3/HyIo/pin.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1020 2023-08-01 18:10:07.000000 HyIo-0.2.3/HyIo/test_debounce.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      415 2023-07-27 12:56:45.000000 HyIo-0.2.3/HyIo/test_device.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      779 2023-08-01 18:10:11.000000 HyIo-0.2.3/HyIo/test_ioManager.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      872 2023-08-08 11:57:40.000000 HyIo-0.2.3/HyIo/test_parser.py
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      456 2023-08-01 18:09:58.000000 HyIo-0.2.3/HyIo/test_pin.py
+drwxr-xr-x   0 erikcm    (1000) erikcm    (1000)        0 2023-08-08 12:04:37.496645 HyIo-0.2.3/HyIo.egg-info/
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      759 2023-08-08 12:04:37.000000 HyIo-0.2.3/HyIo.egg-info/PKG-INFO
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      421 2023-08-08 12:04:37.000000 HyIo-0.2.3/HyIo.egg-info/SOURCES.txt
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)        1 2023-08-08 12:04:37.000000 HyIo-0.2.3/HyIo.egg-info/dependency_links.txt
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)       16 2023-08-08 12:04:37.000000 HyIo-0.2.3/HyIo.egg-info/requires.txt
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)        5 2023-08-08 12:04:37.000000 HyIo-0.2.3/HyIo.egg-info/top_level.txt
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)     1069 2023-07-12 23:16:08.000000 HyIo-0.2.3/LICENSE
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      759 2023-08-08 12:04:37.499979 HyIo-0.2.3/PKG-INFO
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      156 2023-08-01 18:29:38.000000 HyIo-0.2.3/README.md
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)       79 2023-08-08 12:04:37.499979 HyIo-0.2.3/setup.cfg
+-rw-r--r--   0 erikcm    (1000) erikcm    (1000)      891 2023-08-08 11:55:20.000000 HyIo-0.2.3/setup.py
```

### Comparing `HyIo-0.2.2/HyIo/debounce.py` & `HyIo-0.2.3/HyIo/debounce.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,21 @@
         self.lastUpdateTime = 0
 
         self.addPeriod = addPeriod
         self.lastAddTime = 0
 
         self.block = Block(blockSize)
 
+    def __eq__(self, deb):
+        if self.updatePeriod != deb.updatePeriod:
+            return False
+        if self.addPeriod != deb.addPeriod:
+            return False
+        return self.block.blockSize == deb.block.blockSize
+
     def get(self):
         return self.block.get()
 
     def updateValueIfNeed(self, currentTime, func):
         if currentTime - self.lastUpdateTime < self.updatePeriod:
             return False
         func()
```

### Comparing `HyIo-0.2.2/HyIo/gpioDevice.py` & `HyIo-0.2.3/HyIo/gpioDevice.py`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/HyIo/i2cDevice.py` & `HyIo-0.2.3/HyIo/i2cDevice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import smbus2
 import device
 
 class I2CDevice(device.Device):
     def __init__(self, address) -> None:
         super().__init__()
-        self.bus = smbus2.SMBusWrapper(1)
+        self.bus = smbus2.SMBus(1)
         self.address = address
 
     def _read_pin(self, id):
         return self.bus.read_byte_data(self.address, id)
 
     def _write_pin(self, id, value):
         self.bus.write_byte_data(self.address, id, value)
```

### Comparing `HyIo-0.2.2/HyIo/ioManager.py` & `HyIo-0.2.3/HyIo/ioManager.py`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/HyIo/pin.py` & `HyIo-0.2.3/HyIo/pin.py`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/HyIo/test_debounce.py` & `HyIo-0.2.3/HyIo/test_debounce.py`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/HyIo/test_ioManager.py` & `HyIo-0.2.3/HyIo/test_ioManager.py`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/HyIo.egg-info/PKG-INFO` & `HyIo-0.2.3/HyIo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HyIo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Abstraction to Io device on raspberry pi
 Home-page: https://github.com/Erik-Morbach/HyIo
-Download-URL: https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.2.tar.gz
+Download-URL: https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.3.tar.gz
 Author: Erik Cruz Morbach
 Author-email: morbacherik@gmail.com
 License: MIT
 Keywords: io,raspberry,abstraction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HyIo-0.2.2/LICENSE` & `HyIo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HyIo-0.2.2/PKG-INFO` & `HyIo-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HyIo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Abstraction to Io device on raspberry pi
 Home-page: https://github.com/Erik-Morbach/HyIo
-Download-URL: https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.2.tar.gz
+Download-URL: https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.3.tar.gz
 Author: Erik Cruz Morbach
 Author-email: morbacherik@gmail.com
 License: MIT
 Keywords: io,raspberry,abstraction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HyIo-0.2.2/setup.py` & `HyIo-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'HyIo',
   packages = ['HyIo'],
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Abstraction to Io device on raspberry pi',
   author = 'Erik Cruz Morbach',
   author_email = 'morbacherik@gmail.com',
   url = 'https://github.com/Erik-Morbach/HyIo',
-  download_url = 'https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.2.tar.gz',
+  download_url = 'https://github.com/Erik-Morbach/HyIo/archive/refs/tags/V0.2.3.tar.gz',
   keywords = ['io', 'raspberry', 'abstraction'],
   install_requires=[
           'wiringpi',
           'smbus2',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

