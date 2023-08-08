# Comparing `tmp/pysk8-0.0.8-py3-none-any.whl.zip` & `tmp/pysk8-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23270 bytes, number of entries: 14
+Zip file size: 23266 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       87 b- defN 18-Mar-09 11:29 pysk8/__init__.py
--rw-rw-rw-  2.0 fat       63 b- defN 18-Apr-20 13:56 pysk8/__version__.py
+-rw-rw-rw-  2.0 fat       63 b- defN 18-Apr-20 16:06 pysk8/__version__.py
 -rw-rw-rw-  2.0 fat     2798 b- defN 18-Apr-20 13:21 pysk8/constants.py
--rw-rw-rw-  2.0 fat    64875 b- defN 18-Apr-20 13:41 pysk8/core.py
+-rw-rw-rw-  2.0 fat    64901 b- defN 18-Apr-20 16:05 pysk8/core.py
 -rw-rw-rw-  2.0 fat     2373 b- defN 18-Mar-08 16:34 pysk8/discovery.py
 -rw-rw-rw-  2.0 fat      865 b- defN 18-Apr-17 13:14 pysk8/extana.py
 -rw-rw-rw-  2.0 fat     3857 b- defN 18-Apr-20 09:06 pysk8/imu.py
 -rw-rw-rw-  2.0 fat     1297 b- defN 18-Mar-08 16:42 pysk8/util.py
--rw-rw-rw-  2.0 fat     1227 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      972 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        6 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2069 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1066 b- defN 18-Apr-20 13:56 pysk8-0.0.8.dist-info/RECORD
-14 files, 81652 bytes uncompressed, 21548 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat     1227 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      972 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        6 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2069 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1066 b- defN 18-Apr-20 16:07 pysk8-0.0.9.dist-info/RECORD
+14 files, 81678 bytes uncompressed, 21544 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: pysk8/imu.py
 Comment: 
 
 Filename: pysk8/util.py
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/DESCRIPTION.rst
+Filename: pysk8-0.0.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/metadata.json
+Filename: pysk8-0.0.9.dist-info/metadata.json
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/top_level.txt
+Filename: pysk8-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/WHEEL
+Filename: pysk8-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/METADATA
+Filename: pysk8-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pysk8-0.0.8.dist-info/RECORD
+Filename: pysk8-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pysk8/__version__.py

```diff
@@ -1,3 +1,3 @@
-VERSION = (0, 0, 8)
+VERSION = (0, 0, 9)
 
 __version__ = '.'.join(map(str, VERSION))
```

## pysk8/core.py

```diff
@@ -217,15 +217,15 @@
         self.streaming = False
         self.packets = 0
         self.services = {}
         self.imu_callback = None
         self.imu_callback_data = None
         self.extana_callback = None
         self.extana_callback_data = None
-        self.led_state = (0, 0, 0)
+        self.led_state = None
         self.hardware = None
         if calibration:
             logger.debug('Attempting to load calibration for addr={}'.format(self.addr))
             self.load_calibration()
 
     def __eq__(self, v):
         """Devices considered equal if address or name match"""
@@ -376,15 +376,15 @@
             cached (bool): if True, returns the locally cached state of the LED (based
                 on the last call to :meth:`set_extana_led`). Otherwise query the device
                 for the current state.
 
         Returns:
             a 3-tuple (r, g, b) (all unsigned integers) in the range 0-255, or `None` on error.
         """
-        if cached:
+        if cached and self.led_state is not None:
             return self.led_state
 
         rgb = self.dongle._read_attribute(self.conn_handle, HANDLE_EXTANA_LED, israw=True)
         if rgb is None:
             return rgb
 
         return list(map(lambda x: int(x * (LED_MAX / INT_LED_MAX)), struct.unpack('<HHH', rgb)))
```

## Comparing `pysk8-0.0.8.dist-info/DESCRIPTION.rst` & `pysk8-0.0.9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `pysk8-0.0.8.dist-info/metadata.json` & `pysk8-0.0.9.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -40,9 +40,9 @@
                 "bgapi",
                 "future",
                 "pyserial"
             ]
         }
     ],
     "summary": "Python driver for SK8 BLE sensor pack",
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

## Comparing `pysk8-0.0.8.dist-info/METADATA` & `pysk8-0.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: pysk8
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python driver for SK8 BLE sensor pack
 Home-page: https://github.com/andrewramsay/sk8-drivers/pysk8
 Author: Andrew Ramsay
 Author-email: andrew.ramsay@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

