# Comparing `tmp/feagi_agent_freenove-0.0.8.tar.gz` & `tmp/feagi_agent_freenove-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_freenove-0.0.8.tar", last modified: Thu Jul 13 15:50:48 2023, max compression
+gzip compressed data, was "feagi_agent_freenove-0.0.9.tar", last modified: Mon Aug  7 23:44:46 2023, max compression
```

## Comparing `feagi_agent_freenove-0.0.8.tar` & `feagi_agent_freenove-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/LICENSE
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4824 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/README.md
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.180426 feagi_agent_freenove-0.0.8/feagi_agent_freenove/
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/ADC.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6227 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/Led.py
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/PCA9685.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/__init__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2112 2023-07-13 15:26:51.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/__main__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2432 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/configuration.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    26436 2023-07-13 15:42:18.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/controller.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/requirements.txt
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/setup.sh
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/verify.sh
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/SOURCES.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/dependency_links.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/requires.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/top_level.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/pyproject.toml
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-08-07 23:44:46.346655 feagi_agent_freenove-0.0.9/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-08-07 23:44:46.346655 feagi_agent_freenove-0.0.9/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4824 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-08-07 23:44:46.346655 feagi_agent_freenove-0.0.9/feagi_agent_freenove/
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/ADC.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6123 2023-08-07 15:21:03.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/Led.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/PCA9685.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2112 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2498 2023-08-07 23:40:26.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/configuration.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    29239 2023-08-07 19:20:40.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/controller.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/requirements.txt
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/setup.sh
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove/verify.sh
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-08-07 23:44:46.346655 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-08-07 23:44:46.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-08-07 23:44:46.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-08-07 23:44:46.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-08-07 23:44:46.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-08-07 23:44:46.000000 feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-08-02 20:22:38.000000 feagi_agent_freenove-0.0.9/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-08-07 23:44:46.350655 feagi_agent_freenove-0.0.9/setup.cfg
```

### Comparing `feagi_agent_freenove-0.0.8/LICENSE` & `feagi_agent_freenove-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/PKG-INFO` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feagi_agent_freenove
-Version: 0.0.8
+Name: feagi-agent-freenove
+Version: 0.0.9
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_freenove-0.0.8/README.md` & `feagi_agent_freenove-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/ADC.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/ADC.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/Led.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/Led.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,19 +101,16 @@
                 self.strip.show()
                 time.sleep(wait_ms / 1000.0)
                 for i in range(0, strip.numPixels(), 3):
                     strip.setPixelColor(i + q, 0)
 
     def ledIndex(self, index, R, G, B):
         color = self.LED_TYPR(self.ORDER, Color(R, G, B))
-        for i in range(8):
-            if index & 0x01 == 1:
-                self.strip.setPixelColor(i, color)
-                self.strip.show()
-            index = index >> 1
+        self.strip.setPixelColor(index, color)
+        self.strip.show()
 
     def ledMode(self, n):
         self.mode = n
         while True:
             if self.mode == '1':
                 self.colorWipe(self.strip, Color(255, 0, 0))  # Red wipe
                 self.colorWipe(self.strip, Color(0, 255, 0))  # Green wipe
```

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/PCA9685.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/PCA9685.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/__main__.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/__main__.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/configuration.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         "disabled": False,
         "count": 4,
         'topic_identifier': '/M',
         "refresh_rate": 1,
         "cortical_mapping": "o__mot",
         "rolling_window_len": 5,
         "diameter_of_wheel": 0.065,
-        "power_amount": 650
+        "power_amount": 65
     },
     "infrared": {
         "type": "ipu",
         "disabled": False,
         "count": 3,
         "refresh_rate": 1,
         "cortical_mapping": "i__inf",
@@ -74,17 +74,19 @@
     },
     "camera": {
         "type": "ipu",
         "disabled": False,
         "count": 1,
         "width": 8,
         "height": 8,
-        "deviation_threshold": 0.7,
+        "deviation_threshold": 0.9,
         "retina_width_percent": 90,
         "retina_height_percent": 80,
         "central_vision_compression": [64, 64],
         "peripheral_vision_compression": [8, 8],
-        "previous_data": {}
+        "previous_data": {},
+        "aperture_range": [0.2, 2],
+        "aperture_default": 2
     },
 }
 
 message_to_feagi = {"data": {}}
```

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/controller.py` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from feagi_agent import feagi_interface as FEAGI
 import RPi.GPIO as GPIO
 from feagi_agent import retina as retina
 import requests
 import sys
+import os
 from feagi_agent_freenove.Led import *
 from feagi_agent_freenove.PCA9685 import PCA9685
 from picamera import PiCamera
 from datetime import datetime
 from collections import deque
 from picamera.array import PiRGBArray
 from time import sleep
+import time
+import cv2
+import traceback
 
 runtime_data = {
     "current_burst_id": 0,
     "feagi_state": None,
     "cortical_list": (),
     "battery_charge_level": 1,
     "host_network": {},
     'motor_status': {},
     'servo_status': {}
 }
 
 previous_data_frame = dict()
 
 
+def check_aptr(size):
+    try:
+        raw_aptr = requests.get(size).json()
+        return raw_aptr['cortical_dimensions'][2]
+    except Exception as error:
+        print("error: ", error)
+        return 10
+
+
 def window_average(sequence):
     return sum(sequence) // len(sequence)
 
 
 class LED:
     def __init__(self):
         self.led = Led()
@@ -386,45 +399,64 @@
             pulse_len = finish - start
             distance_cm[i] = pulse_len / 0.000058
         distance_cm = sorted(distance_cm)
         distance_meter = (distance_cm[1] * 0.01) * 2
         return distance_meter
 
 
+def process_retina_data(image, capabilities):
+    retina_data = retina.frame_split(image,
+                                     capabilities['camera']['retina_width_percent'],
+                                     capabilities['camera']['retina_height_percent'])
+
+    for key, data in retina_data.items():
+        compression = capabilities['camera']["central_vision_compression"] if 'C' in key else \
+            capabilities['camera']['peripheral_vision_compression']
+        retina_data[key] = retina.center_data_compression(data, compression)
+    return retina_data
+
+
+def get_rgb_for_key(key, data, capabilities, previous_data_frame):
+    compression = capabilities['camera']['central_vision_compression'] if 'C' in key else \
+        capabilities['camera']['peripheral_vision_compression']
+    previous_name = str(key) + "_prev"
+    return retina.get_rgb(data, compression, previous_data_frame[previous_name], key,
+                          capabilities['camera']['deviation_threshold'],
+                          capabilities['camera']["aperture_default"])
+
+
 # class Battery:
 #     def battery_total(self):
 #         adc = Adc()
 #         Power = adc.recvADC(2) * 3
 #         # print(Power)
 #         return Power
 
 def main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi, args):
     GPIO.cleanup()
     # # FEAGI REACHABLE CHECKER # #
     feagi_flag = False
     print("retrying...")
     print("Waiting on FEAGI...")
     while not feagi_flag:
-        feagi_flag = FEAGI.is_FEAGI_reachable(feagi_settings["feagi_host"], 3000)
+        feagi_flag = FEAGI.is_FEAGI_reachable(
+            os.environ.get('FEAGI_HOST_INTERNAL', feagi_settings["feagi_host"]),
+            int(os.environ.get('FEAGI_OPU_PORT', "3000")))
         sleep(2)
 
     # # FEAGI REACHABLE CHECKER COMPLETED # #
 
     # # # FEAGI registration # # # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # - - - - - - - - - - - - - - - - - - #
     print("Connecting to FEAGI resources...")
     runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_auth_url=feagi_auth_url,
                                                            feagi_settings=feagi_settings,
                                                            agent_settings=agent_settings,
                                                            capabilities=capabilities)
     api_address = runtime_data['feagi_state']["feagi_url"]
-
-    stimulation_period_endpoint = FEAGI.feagi_api_burst_engine()
-    burst_counter_endpoint = FEAGI.feagi_api_burst_counter()
-
     # agent_data_port = agent_settings["agent_data_port"]
     agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
 
     # todo: to obtain this info directly from FEAGI as part of registration
     # ipu_channel_address = FEAGI.feagi_inbound(agent_settings["agent_data_port"])
@@ -441,175 +473,212 @@
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # - - - # Initializer section
     motor = Motor()
     servo = Servo()
     ir = IR()
     ultrasonic = Ultrasonic()
-    # battery = Battery() - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+    led = LED()
+    # battery = Battery()
+    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # - - - - - - - - - - - - - #
-
     flag = False
     keyboard_flag = True
     rolling_window_len = capabilities['motor']['rolling_window_len']
     motor_count = capabilities['motor']['count']
     msg_counter = 0
+    led_flag = False
     # rpm = (50 * 60) / 2 DC motor has 2 poles, 50 is the freq and it's constant (why??) and 60
     # is the seconds of a minute w = (rpm / 60) * (2 * math.pi)  # 60 is second/minute velocity =
     # w * (configuration.capabilities['motor']['diameter_of_wheel'] / 2) ^ diameter is from
     # config and it just needs radius so I turned the diameter into a radius by divide it with 2
-
     motor_data = dict()
+    data_point_status = {}
     rolling_window = {}
     for motor_id in range(motor_count):
         rolling_window[motor_id] = deque([0] * rolling_window_len)
-    camera = PiCamera()
-    camera.resolution = (640, 480)
-    camera.framerate = 32
-    rawCapture = PiRGBArray(camera, size=(640, 480))
+    cam = cv2.VideoCapture(0)  # you need to do sudo rpi-update to be able to use this
     motor.stop()
     servo.set_default_position()
+    genome_tracker = 0
+    get_size_for_aptr_cortical = api_address + '/v1/feagi/genome/cortical_area?cortical_area=o_aptr'
+    raw_aptr = requests.get(get_size_for_aptr_cortical).json()
+    try:
+        aptr_cortical_size = raw_aptr['cortical_dimensions'][2]
+    except Exception as error:
+        aptr_cortical_size = None
+        print("aptr fetch error at: ", error)
     while True:
         try:
-            for frame in camera.capture_continuous(rawCapture, format="bgr", use_video_port=True):
-                if keyboard_flag:
-                    image = frame.array
-                    rawCapture.truncate(0)
-                    if capabilities['camera']['disabled'] is not True:
-                        retina_data = retina.frame_split(image,
-                                                         capabilities['camera'][
-                                                             'retina_width_percent'],
-                                                         capabilities['camera'][
-                                                             'retina_height_percent'])
-                        for i in retina_data:
-                            if 'C' in i:
-                                retina_data[i] = retina.center_data_compression(
-                                    retina_data[i],
-                                    capabilities['camera']["central_vision_compression"]
-                                )
-                            else:
-                                retina_data[i] = retina. \
-                                    center_data_compression(retina_data[i],
-                                                            capabilities['camera']
-                                                            ['peripheral_vision_compression'])
-                        rgb = dict()
-                        rgb['camera'] = dict()
-                        if previous_data_frame == {}:
-                            for i in retina_data:
-                                previous_name = str(i) + "_prev"
-                                previous_data_frame[previous_name] = {}
-                        for i in retina_data:
-                            name = i
-                            if 'prev' not in i:
-                                data = retina.ndarray_to_list(retina_data[i])
-                                if 'C' in i:
-                                    previous_name = str(i) + "_prev"
-                                    rgb_data, previous_data_frame[previous_name] = \
-                                        retina.get_rgb(data,
-                                                       capabilities[
-                                                           'camera'][
-                                                           'central_vision_compression'],
-                                                       previous_data_frame[
-                                                           previous_name],
-                                                       name,
-                                                       capabilities['camera'][
-                                                           'deviation_threshold'])
-                                else:
-                                    previous_name = str(i) + "_prev"
-                                    rgb_data, previous_data_frame[previous_name] = \
-                                        retina.get_rgb(data, capabilities['camera'][
-                                            'peripheral_vision_compression'],
-                                                       previous_data_frame[previous_name], name,
-                                                       capabilities['camera'][
-                                                           'deviation_threshold'])
-                                for a in rgb_data['camera']:
-                                    rgb['camera'][a] = rgb_data['camera'][a]
+            start = time.time()
+            ret, image = cam.read()
+            if capabilities['camera']['disabled'] is not True:
+                retina_data = retina.frame_split(image,
+                                                 capabilities['camera'][
+                                                     'retina_width_percent'],
+                                                 capabilities['camera'][
+                                                     'retina_height_percent'])
+                for i in retina_data:
+                    if 'C' in i:
+                        retina_data[i] = retina.center_data_compression(
+                            retina_data[i],
+                            capabilities['camera']["central_vision_compression"]
+                        )
                     else:
-                        rgb = {}
-                ir_data = ir.read()
-                if ir_data:
-                    formatted_ir_data = {'ir': {sensor: True for sensor in ir_data}}
-                else:
-                    formatted_ir_data = {}
-
-                if ir_data:
-                    for ir_sensor in range(int(capabilities['infrared']['count'])):
-                        if ir_sensor not in formatted_ir_data['ir']:
-                            formatted_ir_data['ir'][ir_sensor] = False
-                else:
-                    formatted_ir_data['ir'] = {}
-                    for ir_sensor in range(int(capabilities['infrared']['count'])):
-                        formatted_ir_data['ir'][ir_sensor] = False
+                        retina_data[i] = retina. \
+                            center_data_compression(retina_data[i],
+                                                    capabilities['camera']
+                                                    ['peripheral_vision_compression'])
+                rgb = dict()
+                rgb['camera'] = dict()
+                if previous_data_frame == {}:
+                    for i in retina_data:
+                        previous_name = str(i) + "_prev"
+                        previous_data_frame[previous_name] = {}
+                for i in retina_data:
+                    name = i
+                    if 'prev' not in i:
+                        data = retina.ndarray_to_list(retina_data[i])
+                        if 'C' in i:
+                            previous_name = str(i) + "_prev"
+                            rgb_data, previous_data_frame[previous_name] = \
+                                retina.get_rgb(data,
+                                               capabilities[
+                                                   'camera'][
+                                                   'central_vision_compression'],
+                                               previous_data_frame[
+                                                   previous_name],
+                                               name,
+                                               capabilities['camera'][
+                                                   'deviation_threshold'],
+                                               capabilities[
+                                                   'camera'][
+                                                   "aperture_default"]
+                                               )
+                        else:
+                            previous_name = str(i) + "_prev"
+                            rgb_data, previous_data_frame[previous_name] = \
+                                retina.get_rgb(data, capabilities['camera'][
+                                    'peripheral_vision_compression'],
+                                               previous_data_frame[previous_name], name,
+                                               capabilities['camera'][
+                                                   'deviation_threshold'],
+                                               capabilities[
+                                                   'camera'][
+                                                   "aperture_default"]
+                                               )
+                        for a in rgb_data['camera']:
+                            rgb['camera'][a] = rgb_data['camera'][a]
+            else:
+                rgb = {}
+            # print(time.time() - start)
+            ir_data = ir.read()
+            if ir_data:
+                formatted_ir_data = {'ir': {sensor: True for sensor in ir_data}}
+            else:
+                formatted_ir_data = {}
 
+            if ir_data:
                 for ir_sensor in range(int(capabilities['infrared']['count'])):
                     if ir_sensor not in formatted_ir_data['ir']:
                         formatted_ir_data['ir'][ir_sensor] = False
-                ultrasonic_data = ultrasonic.get_distance()
-                if ultrasonic_data:
-                    formatted_ultrasonic_data = {
-                        'ultrasonic': {
-                            sensor: data for sensor, data in enumerate([ultrasonic_data])
-                        }
+            else:
+                formatted_ir_data['ir'] = {}
+                for ir_sensor in range(int(capabilities['infrared']['count'])):
+                    formatted_ir_data['ir'][ir_sensor] = False
+
+            for ir_sensor in range(int(capabilities['infrared']['count'])):
+                if ir_sensor not in formatted_ir_data['ir']:
+                    formatted_ir_data['ir'][ir_sensor] = False
+            ultrasonic_data = ultrasonic.get_distance()
+            if ultrasonic_data:
+                formatted_ultrasonic_data = {
+                    'ultrasonic': {
+                        sensor: data for sensor, data in enumerate([ultrasonic_data])
                     }
-                else:
-                    formatted_ultrasonic_data = {}
-                message_to_feagi, battery = FEAGI.compose_message_to_feagi(
-                    original_message={**formatted_ir_data, **formatted_ultrasonic_data,
-                                      **rgb})  # Removed battery due to error
-                # Process OPU data received from FEAGI and pass it along
-                message_from_feagi = feagi_opu_channel.receive()
-                if message_from_feagi is not None:
-                    opu_data = FEAGI.opu_processor(message_from_feagi)
-                    if capabilities['motor']['disabled'] is not True:
-                        if 'motor' in opu_data:
-                            if opu_data['motor'] is not {}:
-                                for data_point in opu_data['motor']:
-                                    device_power = opu_data['motor'][data_point]
-                                    device_power = motor.power_convert(data_point, device_power)
-                                    device_id = motor.motor_converter(data_point)
-                                    if device_id not in motor_data:
-                                        motor_data[device_id] = dict()
-                                    rolling_window[device_id].append(device_power)
-                                    rolling_window[device_id].popleft()
-                                else:
-                                    # print("zero time")
-                                    for _ in range(motor_count):
-                                        rolling_window[_].append(0)
-                                        rolling_window[_].popleft()
-                    if capabilities['servo']['disabled'] is not True:
-                        if 'servo' in opu_data:
-                            for data_point in opu_data['servo']:
-                                device_id = data_point
-                                device_power = opu_data['servo'][data_point]
-                                servo.move(feagi_device_id=device_id, power=device_power)
-                message_to_feagi['timestamp'] = datetime.now()
-                message_to_feagi['counter'] = msg_counter
-                feagi_ipu_channel.send(message_to_feagi)
-                message_to_feagi.clear()
-                msg_counter += 1
-                flag += 1
-                if flag == 10:
-                    feagi_burst_speed = requests.get(
-                        api_address + stimulation_period_endpoint).json()
-                    feagi_burst_counter = requests.get(api_address + burst_counter_endpoint).json()
-                    flag = 0
-                    if msg_counter < feagi_burst_counter:
-                        feagi_opu_channel = FEAGI.sub_initializer(opu_address=opu_channel_address)
-                        if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
-                            feagi_settings['feagi_burst_speed'] = feagi_burst_speed
-                for id in range(motor_count):
-                    motor_power = window_average(rolling_window[id])
-                    motor_power = motor_power * capabilities["motor"]["power_amount"]
-                    motor.move(id, motor_power)
+                }
+            else:
+                formatted_ultrasonic_data = {}
+            message_to_feagi, battery = FEAGI.compose_message_to_feagi(
+                original_message={**formatted_ir_data, **formatted_ultrasonic_data,
+                                  **rgb})  # Removed battery due to error
+            # Removed battery due to error
+            # Process OPU data received from FEAGI and pass it along
+            message_from_feagi = feagi_opu_channel.receive()
+            if message_from_feagi is not None:
+                if "o_aptr" in message_from_feagi["opu_data"]:
+                    if message_from_feagi["opu_data"]["o_aptr"]:
+                        for i in message_from_feagi["opu_data"]["o_aptr"]:
+                            feagi_aptr = (int(i.split('-')[-1]))
+                            if aptr_cortical_size is None:
+                                aptr_cortical_size = check_aptr(aptr_cortical_size)
+                            elif aptr_cortical_size <= feagi_aptr:
+                                aptr_cortical_size = check_aptr(aptr_cortical_size)
+                            max_range = capabilities['camera']['aperture_range'][1]
+                            min_range = capabilities['camera']['aperture_range'][0]
+                            capabilities['camera']["aperture_default"] = \
+                                ((feagi_aptr / aptr_cortical_size) *
+                                 (max_range - min_range)) + min_range
+                opu_data = FEAGI.opu_processor(message_from_feagi)
+                if capabilities['motor']['disabled'] is not True:
+                    if 'misc' in opu_data:
+                        if opu_data['misc'] != {}:
+                            for data_point in opu_data['misc']:
+                                led_flag = True
+                                if data_point not in data_point_status:
+                                    data_point_status[data_point] = True
+                                if data_point_status[data_point]:
+                                    led.LED_on(
+                                        data_point,
+                                        int((opu_data['misc'][data_point]/100)*255),
+                                        0, 0)
+                                data_point_status[data_point] = not data_point_status[data_point]
+                        else:
+                            if led_flag:
+                                for i in range(8):
+                                    led.LED_on(i, 0, 0, 0)
+                                led_flag = False
+
+                    if 'motor' in opu_data:
+                        if opu_data['motor'] is not {}:
+                            for data_point in opu_data['motor']:
+                                device_power = opu_data['motor'][data_point]
+                                device_power = motor.power_convert(data_point, device_power)
+                                device_id = motor.motor_converter(data_point)
+                                if device_id not in motor_data:
+                                    motor_data[device_id] = dict()
+                                rolling_window[device_id].append(device_power)
+                                rolling_window[device_id].popleft()
+                            else:
+                                for _ in range(motor_count):
+                                    rolling_window[_].append(0)
+                                    rolling_window[_].popleft()
+                if capabilities['servo']['disabled'] is not True:
+                    if 'servo' in opu_data:
+                        for data_point in opu_data['servo']:
+                            device_id = data_point
+                            device_power = opu_data['servo'][data_point]
+                            servo.move(feagi_device_id=device_id, power=device_power)
+            message_to_feagi['timestamp'] = datetime.now()
+            message_to_feagi['counter'] = msg_counter
+            feagi_ipu_channel.send(message_to_feagi)
+            message_to_feagi.clear()
+            # if message_from_feagi is not None:
+            #     feagi_settings['feagi_burst_speed'] = message_from_feagi['burst_frequency']
+            # sleep(1 / 40)
+            for id in range(motor_count):
+                motor_power = window_average(rolling_window[id])
+                motor_power = motor_power * capabilities["motor"]["power_amount"]
+                motor.move(id, motor_power)
         except KeyboardInterrupt as ke:  # Keyboard error
             motor.stop()
-            camera.stop_preview()
-            camera.close()
-            keyboard_flag = False
+            cam.release()
             print("ke: ", ke)
+            led.leds_off()
             break
         except Exception as e:
             print("ERROR: ", e)
+            traceback.print_exc()
             motor.stop()
-            camera.stop_preview()
-            camera.close()
+            cam.release()
+            led.leds_off()
             break
```

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/setup.sh` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/setup.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove/verify.sh` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove/verify.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/PKG-INFO` & `feagi_agent_freenove-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feagi-agent-freenove
-Version: 0.0.8
+Name: feagi_agent_freenove
+Version: 0.0.9
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/SOURCES.txt` & `feagi_agent_freenove-0.0.9/feagi_agent_freenove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.8/setup.cfg` & `feagi_agent_freenove-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_freenove
-version = 0.0.8
+version = 0.0.9
 author = Neuraville LLC
 author_email = info@feagi.org
 description = Feagi agent freenove to connect feagi with your freenove_smartcar.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```

