# Comparing `tmp/pymycobot-3.1.6b3.tar.gz` & `tmp/pymycobot-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.6b3.tar", last modified: Mon Jul 17 11:35:58 2023, max compression
+gzip compressed data, was "pymycobot-3.1.7.tar", last modified: Tue Aug  8 11:14:37 2023, max compression
```

## Comparing `pymycobot-3.1.6b3.tar` & `pymycobot-3.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.273342 pymycobot-3.1.6b3/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/MANIFEST.in
--rw-rw-rw-   0        0        0    59801 2023-07-17 11:35:58.272321 pymycobot-3.1.6b3/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.6b3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.240063 pymycobot-3.1.6b3/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.6b3/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1681 2023-07-17 11:32:05.000000 pymycobot-3.1.6b3/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.6b3/pymycobot/bluet.py
--rw-rw-rw-   0        0        0      201 2023-07-12 07:37:01.000000 pymycobot-3.1.6b3/pymycobot/cobotx.py
--rw-rw-rw-   0        0        0    12394 2023-07-13 12:24:05.000000 pymycobot-3.1.6b3/pymycobot/common.py
--rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.6b3/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/error.py
--rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.6b3/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.6b3/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9329 2023-07-17 11:31:19.000000 pymycobot-3.1.6b3/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.6b3/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.6b3/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.6b3/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.6b3/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7735 2023-07-17 11:32:34.000000 pymycobot-3.1.6b3/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.6b3/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.6b3/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.6b3/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.6b3/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.269822 pymycobot-3.1.6b3/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    59801 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 11:35:58.273342 pymycobot-3.1.6b3/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.6b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:14:37.436257 pymycobot-3.1.7/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.7/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    59799 2023-08-08 11:14:37.435257 pymycobot-3.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 11:14:37.399066 pymycobot-3.1.7/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.7/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1679 2023-08-08 11:11:27.000000 pymycobot-3.1.7/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.7/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0      754 2023-08-03 07:56:18.000000 pymycobot-3.1.7/pymycobot/cobotx.py
+-rw-rw-rw-   0        0        0    12605 2023-08-03 07:54:37.000000 pymycobot-3.1.7/pymycobot/common.py
+-rw-rw-rw-   0        0        0     9322 2023-07-28 08:31:11.000000 pymycobot-3.1.7/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.7/pymycobot/error.py
+-rw-rw-rw-   0        0        0    34669 2023-08-08 07:33:15.000000 pymycobot-3.1.7/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.7/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.7/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.7/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0    10703 2023-08-08 11:11:16.000000 pymycobot-3.1.7/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13314 2023-07-24 03:21:06.000000 pymycobot-3.1.7/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.7/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.7/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2023-07-26 07:59:20.000000 pymycobot-3.1.7/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     8216 2023-08-08 09:10:14.000000 pymycobot-3.1.7/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7386 2023-07-26 07:57:08.000000 pymycobot-3.1.7/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9151 2023-08-07 10:08:05.000000 pymycobot-3.1.7/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.7/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.7/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.7/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:14:37.433020 pymycobot-3.1.7/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59799 2023-08-08 11:14:37.000000 pymycobot-3.1.7/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-08-08 11:14:37.000000 pymycobot-3.1.7/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 11:14:37.000000 pymycobot-3.1.7/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 11:14:37.000000 pymycobot-3.1.7/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 11:14:37.000000 pymycobot-3.1.7/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 11:14:37.437265 pymycobot-3.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.7/setup.py
```

### Comparing `pymycobot-3.1.6b3/LICENSE` & `pymycobot-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/PKG-INFO` & `pymycobot-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.6b3
+Version: 3.1.7
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
@@ -192,16 +192,16 @@
     - [set\_eletric\_gripper](#set_eletric_gripper)
     - [set\_gripper\_mode](#set_gripper_mode)
     - [get\_gripper\_mode](#get_gripper_mode)
     - [set\_encoders\_drag](#set_encoders_drag)
     - [get\_solution\_angles](#get_solution_angles)
     - [set\_solution\_angles](#set_solution_angles)
     - [joint\_brake](#joint_brake)
-    - [get\_transpoendr\_mode](#get_transpoendr_mode)
-    - [set\_transpoendr\_mode](#set_transpoendr_mode)
+    - [get\_transponder\_mode](#get_transponder_mode)
+    - [set\_transponder\_mode](#set_transponder_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -1334,28 +1334,28 @@
 
 - **Description**: Make it stop when the joint is in motion, and the buffer distance is positively related to the existing speed
 
 - **Parameters**
 
   - `joint_id`: 1 - 7.
 
-### get_transpoendr_mode
+### get_transponder_mode
 
-- **Prototype**: `get_transpoendr_mode()`
+- **Prototype**: `get_transponder_mode()`
 
 - **Description**: Obtain the configuration information of serial transmission mode.(`This interface is only applicable to MyArm`)
 
 - **Return**
   - `0`: Turn off transparent transmission
   - `1`: Turn on transparent transmission, verify all data
   - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information (default is 0)
 
-### set_transpoendr_mode
+### set_transponder_mode
 
-- **Prototype**: `set_transpoendr_mode(mode)`
+- **Prototype**: `set_transponder_mode(mode)`
 
 - **Description**: Set serial port transmission mode.(`This interface is only applicable to MyArm`)
 
 - **Parameters**
   - `mode`:
     - `0`: Turn off transparent transmission
     - `1`: Turn on transparent transmission, verify all data
```

### Comparing `pymycobot-3.1.6b3/README.md` & `pymycobot-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/Interface.py` & `pymycobot-3.1.7/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/__init__.py` & `pymycobot-3.1.7/pymycobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.6b3"
+__version__ = "3.1.7"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.6b3/pymycobot/bluet.py` & `pymycobot-3.1.7/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/common.py` & `pymycobot-3.1.7/pymycobot/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 
     # JOG MODE AND OPERATION
     JOG_ANGLE = 0x30
     JOG_ABSOLUTE = 0x31
     JOG_COORD = 0x32
     JOG_INCREMENT = 0x33
     JOG_STOP = 0x34
+    
+    COBOTX_GET_SOLUTION_ANGLES = 0x35
+    COBOTX_SET_SOLUTION_ANGLES = 0x36
+    
     SET_ENCODER = 0x3A
     GET_ENCODER = 0x3B
     SET_ENCODERS = 0x3C
     GET_ENCODERS = 0x3D
     SET_ENCODERS_DRAG = 0x3E
 
     # RUNNING STATUS AND SETTINGS
@@ -144,14 +148,15 @@
 
     # planning speed
     GET_PLAN_SPEED = 0xD0
     GET_PLAN_ACCELERATION = 0xD1
     SET_PLAN_SPEED = 0xD2
     SET_PLAN_ACCELERATION = 0xD3
     SET_GSERVO_ROUND = 0xD4
+    GET_ANGLES_COORDS = 0xD5
 
     # Motor status read
     GET_SERVO_SPEED = 0xE1
     GET_SERVO_CURRENTS = 0xE2
     GET_SERVO_VOLTAGES = 0xE3
     GET_SERVO_STATUS = 0xE4
     GET_SERVO_TEMPS = 0xE5
@@ -280,15 +285,18 @@
         if arm == 6:
             data_len = data[header_i + 2] - 2
         elif arm == 12:
             data_len = data[header_i + 3] - 2
         unique_data = [ProtocolCode.GET_BASIC_INPUT, ProtocolCode.GET_DIGITAL_INPUT]
 
         if cmd_id in unique_data:
-            data_pos = header_i + 5
+            if arm == 12:
+                data_pos = header_i + 6
+            else:
+                data_pos = header_i + 5
             data_len -= 1
         else:
             if arm == 6:
                 data_pos = header_i + 4
             elif arm == 12:
                 data_pos = header_i + 5
```

### Comparing `pymycobot-3.1.6b3/pymycobot/elephantrobot.py` & `pymycobot-3.1.7/pymycobot/elephantrobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,18 @@
     def assign_variable(self, var_name, var_value):
         command = 'assign_variable("' + str(var_name) + '",' + str(var_value) + ")\n"
         self.send_command(command)
 
     def get_variable(self, var_name):
         command = 'get_variable("' + str(var_name) + '")\n'
         return self.send_command(command)
+    
+    def jog_relative(self, joint_id, angle, speed):
+        command = 'SendJogIncrement("' + str(var_name) + '")\n'
+        return self.send_command(command)
 
 
 if __name__ == "__main__":
     ep = ElephantRobot("192.168.124.28", 5001)
     res = ep.start_client()
     if res != "":
         print(res)
```

### Comparing `pymycobot-3.1.6b3/pymycobot/error.py` & `pymycobot-3.1.7/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/generate.py` & `pymycobot-3.1.7/pymycobot/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,26 +474,27 @@
         """
         return self._mesg(ProtocolCode.GET_SPEED, has_reply=True)
 
     def set_speed(self, speed):
         """Set speed value
 
         Args:
-            speed (int) - 0 ~ 100
+            speed (int): 0 ~ 100
         """
         # self.calibration_parameters(speed=speed)
         return self._mesg(ProtocolCode.SET_SPEED, speed)
 
     """
     def get_feed_override(self):
         return self._process_single(
             self._mesg(Command.GET_FEED_OVERRIDE, has_reply=True)
         )
     """
     def get_acceleration(self):
+        """get acceleration"""
         return self._process_single(
             self._mesg(ProtocolCode.GET_ACCELERATION, has_reply=True)
         )
 
     def set_acceleration(self, acc):
         """Set speed for all moves
         
@@ -1049,8 +1050,11 @@
     
     def set_communicate_mode(self, mode):
         """Set basic communication mode
         
         Args:
             mode: 0 - Turn off transparent transmission，1 - Open transparent transmission
         """
-        return self._mesg(ProtocolCode.SET_COMMUNICATE_MODE, mode)
+        return self._mesg(ProtocolCode.SET_COMMUNICATE_MODE, mode)
+    
+    def get_angles_coords(self):
+        return self._mesg(ProtocolCode.GET_ANGLES_COORDS, has_reply = True)
```

### Comparing `pymycobot-3.1.6b3/pymycobot/log.py` & `pymycobot-3.1.7/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/myarm.py` & `pymycobot-3.1.7/pymycobot/myarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,24 @@
                     return r
                 else:
                     return res
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
                 return [self._int2coord(angle) for angle in res]
             elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
                 return self._int2coord(res[0])
+            elif genre == ProtocolCode.GET_ANGLES_COORDS:
+                r = []
+                for index in range(len(res)):
+                    if index < 7:
+                        r.append(self._int2angle(res[index]))
+                    elif index < 10:
+                        r.append(self._int2coord(res[index]))
+                    else:
+                        r.append(self._int2angle(res[index]))
+                return r
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get the radians of all joints
 
@@ -142,15 +152,15 @@
         angles = self._mesg(ProtocolCode.GET_ANGLES, has_reply=True)
         return [round(angle * (math.pi / 180), 3) for angle in angles]
 
     def send_radians(self, radians, speed):
         """Send the radians of all joints to robot arm
 
         Args:
-            radians: a list of radian values( List[float]), length 6
+            radians: a list of radian values( List[float]), length 7
             speed: (int )0 ~ 100
         """
         degrees = [self._angle2int(radian * (180 / math.pi))
                    for radian in radians]
         return self._mesg(ProtocolCode.SEND_ANGLES, degrees, speed)
 
     def sync_send_angles(self, degrees, speed, timeout=7):
@@ -166,15 +176,15 @@
         while time.time() - t < timeout:
             f = self.is_in_position(degrees, 0)
             if f == 1:
                 break
             time.sleep(0.1)
         return self
 
-    def sync_send_coords(self, coords, speed, mode, timeout=7):
+    def sync_send_coords(self, coords, speed, mode=0, timeout=7):
         """Send the coord in synchronous state and return when the target point is reached
             
         Args:
             coords: a list of coord values(List[float])
             speed: (int) 0 ~ 100
             mode: (int): 0 - angular, 1 - linear
             timeout: default 7s.
@@ -230,23 +240,23 @@
             data: 1 - Undamping (The default is damping)
         """
         if data is None:
             return super().release_all_servos()
         else:
             return self._mesg(ProtocolCode.RELEASE_ALL_SERVOS, data)
             
-    def get_transpoendr_mode(self):
+    def get_transponder_mode(self):
         """Obtain the configuration information of serial transmission mode
         
         Return:
             mode: 0 - 1 - 2
         """
         return self._mesg(ProtocolCode.SET_SSID_PWD, has_reply=True)
     
-    def set_transpoendr_mode(self, mode):
+    def set_transponder_mode(self, mode):
         """Set serial port transmission mode
         
         Args:
             mode: 
                 0 - Turn off transparent transmission.\n
                 1 - Turn on transparent transmission. verify all data.\n
                 2 - Turn on transparent transmission, only verify the configuration information of communication forwarding mode (default is 0)
@@ -263,8 +273,36 @@
         """Set the color of the LED
         
         Args:
             r: Red
             g: Green
             b: Blue
         """
-        return self._mesg(ProtocolCode.SET_COLOR_MYARM, r, g, b)
+        return self._mesg(ProtocolCode.SET_COLOR_MYARM, r, g, b)
+    
+    def is_in_position(self, data, id=0):
+        """Judge whether in the position.
+
+        Args:
+            data: A data list, angles or coords.
+            id: 1 - coords, 0 - angles
+
+        Return:
+            1 - True\n
+            0 - False\n
+            -1 - Error
+        """
+        if id == 1:
+            # self.calibration_parameters(coords=data)
+            data_list = []
+            for idx in range(3):
+                data_list.append(self._coord2int(data[idx]))
+            for idx in range(3, 6):
+                data_list.append(self._angle2int(data[idx]))
+        elif id == 0:
+            # self.calibration_parameters(degrees=data)
+            data_list = [self._angle2int(i) for i in data]
+        else:
+            raise Exception("id is not right, please input 0 or 1")
+        return self._mesg(ProtocolCode.IS_IN_POSITION, id, data_list, has_reply=True)
+    
+
```

### Comparing `pymycobot-3.1.6b3/pymycobot/mybuddy.py` & `pymycobot-3.1.7/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.7/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.7/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/mybuddysocket.py` & `pymycobot-3.1.7/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/mycobot.py` & `pymycobot-3.1.7/pymycobot/mycobot.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,24 @@
                     return res
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
                 return [self._int2coord(angle) for angle in res]
             elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
                 return self._int2coord(res[0])
             elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION]:
                 return self._int2coord(self._process_single(res))
+            elif genre == ProtocolCode.GET_ANGLES_COORDS:
+                r = []
+                for index in range(len(res)):
+                    if index < 6:
+                        r.append(self._int2angle(res[index]))
+                    elif index < 9:
+                        r.append(self._int2coord(res[index]))
+                    else:
+                        r.append(self._int2angle(res[index]))
+                return r
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get the radians of all joints
 
@@ -164,26 +174,27 @@
             speed: (int) 0 ~ 100
             timeout: default 7s.
         """
         t = time.time()
         self.send_angles(degrees, speed)
         while time.time() - t < timeout:
             f = self.is_in_position(degrees, 0)
+            print(f)
             if f == 1:
                 break
             time.sleep(0.1)
         return self
 
-    def sync_send_coords(self, coords, speed, mode, timeout=7):
+    def sync_send_coords(self, coords, speed, mode=0, timeout=7):
         """Send the coord in synchronous state and return when the target point is reached
             
         Args:
             coords: a list of coord values(List[float])
             speed: (int) 0 ~ 100
-            mode: (int): 0 - angular, 1 - linear
+            mode: (int): 0 - angular（default）, 1 - linear
             timeout: default 7s.
         """
         t = time.time()
         self.send_coords(coords, speed, mode)
         while time.time() - t < timeout:
             if self.is_in_position(coords, 1) == 1:
                 break
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymycobot-3.1.6b3/pymycobot/mycobotsocket.py` & `pymycobot-3.1.7/pymycobot/mycobotsocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             ip: Server ip
             netport: Server port
         """
         super(MyCobotSocket, self).__init__()
         self.calibration_parameters = calibration_parameters
         self.SERVER_IP = ip
         self.SERVER_PORT = netport
-        self.rasp = True
+        self.rasp = False
         self.sock = self.connect_socket()
 
     def connect_socket(self):
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.connect((self.SERVER_IP, self.SERVER_PORT))
         return sock
```

### Comparing `pymycobot-3.1.6b3/pymycobot/mypalletizer.py` & `pymycobot-3.1.7/pymycobot/mypalletizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,24 @@
             elif genre in [
                 ProtocolCode.GET_JOINT_MIN_ANGLE,
                 ProtocolCode.GET_JOINT_MAX_ANGLE,
             ]:
                 return self._int2angle(res[0]) if res else 0
             elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION]:
                 return self._int2coord(self._process_single(res))
+            elif genre == ProtocolCode.GET_ANGLES_COORDS:
+                r = []
+                for index in range(len(res)):
+                    if index < 4:
+                        r.append(self._int2angle(res[index]))
+                    elif index < 7:
+                        r.append(self._int2coord(res[index]))
+                    else:
+                        r.append(self._int2angle(res[index]))
+                return r
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get all angle return a list
```

### Comparing `pymycobot-3.1.6b3/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.7/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/ultraArm.py` & `pymycobot-3.1.7/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot/utils.py` & `pymycobot-3.1.7/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.7/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.6b3
+Version: 3.1.7
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
@@ -192,16 +192,16 @@
     - [set\_eletric\_gripper](#set_eletric_gripper)
     - [set\_gripper\_mode](#set_gripper_mode)
     - [get\_gripper\_mode](#get_gripper_mode)
     - [set\_encoders\_drag](#set_encoders_drag)
     - [get\_solution\_angles](#get_solution_angles)
     - [set\_solution\_angles](#set_solution_angles)
     - [joint\_brake](#joint_brake)
-    - [get\_transpoendr\_mode](#get_transpoendr_mode)
-    - [set\_transpoendr\_mode](#set_transpoendr_mode)
+    - [get\_transponder\_mode](#get_transponder_mode)
+    - [set\_transponder\_mode](#set_transponder_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -1334,28 +1334,28 @@
 
 - **Description**: Make it stop when the joint is in motion, and the buffer distance is positively related to the existing speed
 
 - **Parameters**
 
   - `joint_id`: 1 - 7.
 
-### get_transpoendr_mode
+### get_transponder_mode
 
-- **Prototype**: `get_transpoendr_mode()`
+- **Prototype**: `get_transponder_mode()`
 
 - **Description**: Obtain the configuration information of serial transmission mode.(`This interface is only applicable to MyArm`)
 
 - **Return**
   - `0`: Turn off transparent transmission
   - `1`: Turn on transparent transmission, verify all data
   - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information (default is 0)
 
-### set_transpoendr_mode
+### set_transponder_mode
 
-- **Prototype**: `set_transpoendr_mode(mode)`
+- **Prototype**: `set_transponder_mode(mode)`
 
 - **Description**: Set serial port transmission mode.(`This interface is only applicable to MyArm`)
 
 - **Parameters**
   - `mode`:
     - `0`: Turn off transparent transmission
     - `1`: Turn on transparent transmission, verify all data
```

### Comparing `pymycobot-3.1.6b3/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.7/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b3/setup.py` & `pymycobot-3.1.7/setup.py`

 * *Files identical despite different names*

