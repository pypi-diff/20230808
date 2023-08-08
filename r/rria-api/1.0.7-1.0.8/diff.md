# Comparing `tmp/rria_api-1.0.7.tar.gz` & `tmp/rria_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rria_api-1.0.7.tar", max compression
+gzip compressed data, was "rria_api-1.0.8.tar", max compression
```

## Comparing `rria_api-1.0.7.tar` & `rria_api-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      687 2023-08-03 15:15:54.258825 rria_api-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1509 2023-08-02 13:38:32.621902 rria_api-1.0.7/README.md
--rw-r--r--   0        0        0       29 2023-08-02 13:30:21.915376 rria_api-1.0.7/rria_api/__init__.py
--rw-r--r--   0        0        0     1411 2023-08-03 15:15:54.271270 rria_api-1.0.7/rria_api/gen3/action_gen3.py
--rw-r--r--   0        0        0     1559 2023-03-24 11:48:25.778442 rria_api-1.0.7/rria_api/gen3/api_gen3/device_connection.py
--rw-r--r--   0        0        0     8047 2023-08-03 15:16:50.209852 rria_api-1.0.7/rria_api/gen3/api_gen3/gen3_api.py
--rw-r--r--   0        0        0      637 2023-03-24 11:48:25.778442 rria_api-1.0.7/rria_api/gen3/connect_gen3.py
--rw-r--r--   0        0        0     1394 2023-08-03 15:19:41.328813 rria_api-1.0.7/rria_api/ned/action_ned.py
--rw-r--r--   0        0        0      360 2023-03-24 11:48:25.779454 rria_api-1.0.7/rria_api/ned/connect_ned.py
--rw-r--r--   0        0        0    22047 2023-04-10 17:18:59.258978 rria_api-1.0.7/rria_api/poetry.lock
--rw-r--r--   0        0        0    11308 2023-08-03 15:15:54.265254 rria_api-1.0.7/rria_api/robot_object.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 rria_api-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      687 2023-08-08 18:53:16.273643 rria_api-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1598 2023-08-08 18:52:28.019446 rria_api-1.0.8/README.md
+-rw-r--r--   0        0        0       74 2023-08-08 18:46:59.723365 rria_api-1.0.8/rria_api/__init__.py
+-rw-r--r--   0        0        0     1411 2023-08-03 15:15:54.271270 rria_api-1.0.8/rria_api/gen3/action_gen3.py
+-rw-r--r--   0        0        0     1559 2023-03-24 11:48:25.778442 rria_api-1.0.8/rria_api/gen3/api_gen3/device_connection.py
+-rw-r--r--   0        0        0     8047 2023-08-03 15:16:50.209852 rria_api-1.0.8/rria_api/gen3/api_gen3/gen3_api.py
+-rw-r--r--   0        0        0      637 2023-03-24 11:48:25.778442 rria_api-1.0.8/rria_api/gen3/connect_gen3.py
+-rw-r--r--   0        0        0     1394 2023-08-03 15:19:41.328813 rria_api-1.0.8/rria_api/ned/action_ned.py
+-rw-r--r--   0        0        0      360 2023-03-24 11:48:25.779454 rria_api-1.0.8/rria_api/ned/connect_ned.py
+-rw-r--r--   0        0        0    22047 2023-04-10 17:18:59.258978 rria_api-1.0.8/rria_api/poetry.lock
+-rw-r--r--   0        0        0      222 2023-08-08 18:29:31.398703 rria_api-1.0.8/rria_api/robot_enum.py
+-rw-r--r--   0        0        0    11514 2023-08-08 18:41:22.696370 rria_api-1.0.8/rria_api/robot_object.py
+-rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 rria_api-1.0.8/PKG-INFO
```

### Comparing `rria_api-1.0.7/pyproject.toml` & `rria_api-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rria-api"
-version = "1.0.7"
+version = "1.0.8"
 description = ""
 authors = ["felipeadsm <97059009+felipeadsm@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "rria_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rria_api-1.0.7/README.md` & `rria_api-1.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,41 +5,42 @@
 plans to support a Denso robot.
 
 ### **Requirements**
 
 - Python 3.9+
 - Kortex API .whl package
 
-### **Instalation**
+### **Installation**
 1. Download the v2.3.0 Kortex API .whl package (required for controlling the Kinova Gen3 and Gen3 lite):
 
-- [kortex_api-2.3.0.post34-py3-none-any.whl](https://artifactory.kinovaapps.com/ui/native/generic-public/kortex/API/2.3.0/kortex_api-2.3.0.post34-py3-none-any.whl).
+   - [kortex_api-2.3.0.post34-py3-none-any.whl](https://artifactory.kinovaapps.com/ui/native/generic-public/kortex/API/2.3.0/kortex_api-2.3.0.post34-py3-none-any.whl).
 
 2. Install the downloaded package with `pip`:
 
-```
-$ pip install <path to kortex_api-2.3.0.post34-py3-none-any.whl>
-```
+	```
+	$ pip install <path to kortex_api-2.3.0.post34-py3-none-any.whl>
+	```
 
 3. Install the latest `rria-api` package with `pip`:
 
-```
-$ pip install rria-api
-```
+	```
+	$ pip install rria-api
+	```
 
 ### **Example**
 
-```
-from rria_api.robot_facade import *
+```python
+from rria_api.robot_object import RobotObject
+from rria_api.robot_enum import RobotEnum
 
 # Create gen3 RobotObject
-gen3_lite = RobotObject('172.22.64.105', 'gen3')
+gen3_lite = RobotObject('192.168.2.10', RobotEnum.GEN3_LITE)
 
 # Create Niryo NED RobotObject
-ned = RobotObject('169.254.200.200', 'ned')
+ned = RobotObject('169.254.200.200', RobotEnum.NED)
 
 gen3_lite.connect_robot()
 ned.connect_robot()
 
 gen3_lite.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 ned.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
```

### Comparing `rria_api-1.0.7/rria_api/gen3/action_gen3.py` & `rria_api-1.0.8/rria_api/gen3/action_gen3.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/gen3/api_gen3/device_connection.py` & `rria_api-1.0.8/rria_api/gen3/api_gen3/device_connection.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/gen3/api_gen3/gen3_api.py` & `rria_api-1.0.8/rria_api/gen3/api_gen3/gen3_api.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/gen3/connect_gen3.py` & `rria_api-1.0.8/rria_api/gen3/connect_gen3.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/ned/action_ned.py` & `rria_api-1.0.8/rria_api/ned/action_ned.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/poetry.lock` & `rria_api-1.0.8/rria_api/poetry.lock`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.7/rria_api/robot_object.py` & `rria_api-1.0.8/rria_api/robot_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,124 @@
 from rria_api.ned.connect_ned import ConnectNed
 from rria_api.ned.action_ned import ActionNed
 from rria_api.gen3.connect_gen3 import ConnectGen3
 from rria_api.gen3.action_gen3 import ActionGen3
+from robot_enum import RobotEnum
 from time import sleep
 
 
 class RobotObject:
     def __init__(self, ip_address, robot_type):
+        """
+        This class is used to initialize and use the robot object.
+        :param ip_address: string with the ip address of the robot
+        :param robot_type: enum with the type of the robot
+        """
         self.ip_address = ip_address
         self.robot_type = robot_type
 
         # This atribute is used to store the general robot instance
         self.robot_instance = None
 
         # This atribute is used to store the general connection instance
         self.connection_instance = None
 
-    def connect_robot(self):
+    def connect_robot(self) -> bool:
         """
         Connect robot depends on the robot type
         :rtype: bool
 
         """
 
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             try:
                 self.connection_instance = ConnectGen3(self.ip_address, ["admin", "admin"])
                 self.robot_instance = self.connection_instance.connect_robot()
 
                 return True
 
             except(Exception,):
                 print('The connection attempt failed. Check the physical connection to the robot and try again later.')
 
                 return False
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             try:
                 self.connection_instance = ConnectNed()
                 self.robot_instance = self.connection_instance.connect_robot(self.ip_address)
 
                 return True
 
             except(Exception,):
                 print('The connection attempt failed. Check the physical connection to the robot and try again later.')
 
                 return False
 
-        if self.robot_type == 'denso':
-            pass
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def disconnect_robot(self):
         """
         Close connection with robot
         :rtype: None
 
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             self.connection_instance.disconnect_robot()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             self.connection_instance.disconnect_robot()
 
-        if self.robot_type == 'denso':
-            pass
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def safe_disconnect(self):
         """
         Move robot for home position and close connection with robot. Home position dependes on robot type. For Gen3 is
         [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]  degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
         :rtype: None
 
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).move_to_zero()
             self.connection_instance.disconnect_robot()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).move_to_home()
             self.connection_instance.disconnect_robot()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     # Move Joints/Cartesian methods
-    def joints(self):
+    @property
+    def joints(self) -> list:
         return self.get_joints()
 
-    def get_joints(self):
+    def get_joints(self) -> list:
         """
         Get joints value in radians
         You can also use a getter ::
 
             joints = robot.get_joints()
             joints = robot.joints
 
         :return: List of joints value
         :rtype: list[float]
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             return ActionGen3(self.robot_instance).get_joints()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             return ActionNed(self.robot_instance).get_joints()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(0.5)
             return ['J1', 'J2', 'J3', 'J4', 'J5', 'J6']
 
     def move_joints(self, j1, j2, j3, j4, j5, j6):
         """
         Move robot joints. Joints are expressed in degrees.
 
@@ -141,53 +136,56 @@
         :type j4: float
         :param j5: joint 5,
         :type j5: float
         :param j6: joint 6,
         :type j6: float
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).move_joints([j1, j2, j3, j4, j5, j6])
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).move_joints(j1, j2, j3, j4, j5, j6)
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
-    def cartesian(self):
+    @property
+    def cartesian(self) -> list:
+        """
+        Get end effector link pose as [x, y, z, roll, pitch, yaw].
+        Call this method is equivalent to call get_cartesian() method.
+
+        :return: Robot pose list.
+        :rtype: list[float]
+        """
         return self.get_cartesian()
 
-    def get_cartesian(self):
+    def get_cartesian(self) -> list:
         """
         Get end effector link pose as [x, y, z, roll, pitch, yaw].
         x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
         You can also use a getter ::
 
-            pose = robot.get_pose()
-            pose = robot.pose
+            joints = robot.get_cartesian()
+            joints = robot.cartesian
 
-        :rtype: PoseObject
+        :return: Robot pose list.
+        :rtype: list[float]
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             return ActionGen3(self.robot_instance).get_cartesian()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             return ActionNed(self.robot_instance).get_cartesian()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
-            return True
+            return ['x', 'y', 'z', 'roll', 'pitch', 'yaw']
 
     def move_cartesian(self, x, y, z, roll, pitch, yaw):
         """
         Move robot end effector pose to a (x, y, z, roll, pitch, yaw, frame_name) pose
         in a particular frame (frame_name) if defined.
         x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
 
@@ -205,177 +203,150 @@
         :type roll: float
         :param pitch: rotation on y-axis,
         :type pitch: float
         :param yaw: rotation on z-axis,
         :type yaw: float
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             return ActionGen3(self.robot_instance).move_cartesian([x, y, z, roll, pitch, yaw])
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             return ActionNed(self.robot_instance).move_cartesian(x, y, z, roll, pitch, yaw)
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     # TODO: Pegar os valores de home do robot
     def move_to_home(self):
         """
         Move robot for home position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
         degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
 
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).move_to_home()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).move_to_home()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def move_to_zero(self):
         """
         Move robot for zero position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
         degrees and for Ned is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0] radians.
 
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).move_to_zero()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).move_to_zero()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def open_gripper(self):
         """
         Open gripper.
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).open_gripper()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).open_gripper()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def close_gripper(self):
         """
         Close gripper
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).close_gripper()
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).close_gripper()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     # TODO: Ver a função de aumento de velocidade para o Gen3
     def set_velocity(self, velocity):
         """
         Limit arm max velocity to a percentage of its maximum velocity. For Niryo one, velocity is a percentage of 100.
         For gen3, there are two types of velocities, an angular and a cartesian. The speed used in this method is
         angular.
 
         :param velocity: Should be between 1 & 100 for niryo
         :type velocity: int
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).set_velocity(velocity)
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).set_velocity(velocity)
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def calibrate(self):
         """
         Start an automatic motors calibration if motors are not calibrated yet
 
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             print('Gen3 NÃO necessita de calibração')
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).calibrate()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def go_to_sleep(self):
         """
         Go home pose and activate learning mode. The function is available only for Ned robot.
 
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ...
 
-        if self.robot_type == 'ned':
+        if self.robot_type == RobotEnum.NED:
             ActionNed(self.robot_instance).go_to_sleep()
 
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
 
     def apply_emergency_stop(self):
         """
         Apply emergency stop. The function is available only for Kinova Gen3.
 
         :rtype: None
         """
-        if self.robot_type == 'gen3':
+        if self.robot_type == RobotEnum.GEN3_LITE:
             ActionGen3(self.robot_instance).apply_emergency_stop()
 
-        if self.robot_type == 'ned':
-            ...
-
-        if self.robot_type == 'denso':
+        if self.robot_type == RobotEnum.NED:
             ...
 
-        if self.robot_type == 'test':
+        if self.robot_type == RobotEnum.DUMMY:
             sleep(1)
             return True
```

### Comparing `rria_api-1.0.7/PKG-INFO` & `rria_api-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rria-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: 
 Author: felipeadsm
 Author-email: 97059009+felipeadsm@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,41 +19,42 @@
 plans to support a Denso robot.
 
 ### **Requirements**
 
 - Python 3.9+
 - Kortex API .whl package
 
-### **Instalation**
+### **Installation**
 1. Download the v2.3.0 Kortex API .whl package (required for controlling the Kinova Gen3 and Gen3 lite):
 
-- [kortex_api-2.3.0.post34-py3-none-any.whl](https://artifactory.kinovaapps.com/ui/native/generic-public/kortex/API/2.3.0/kortex_api-2.3.0.post34-py3-none-any.whl).
+   - [kortex_api-2.3.0.post34-py3-none-any.whl](https://artifactory.kinovaapps.com/ui/native/generic-public/kortex/API/2.3.0/kortex_api-2.3.0.post34-py3-none-any.whl).
 
 2. Install the downloaded package with `pip`:
 
-```
-$ pip install <path to kortex_api-2.3.0.post34-py3-none-any.whl>
-```
+	```
+	$ pip install <path to kortex_api-2.3.0.post34-py3-none-any.whl>
+	```
 
 3. Install the latest `rria-api` package with `pip`:
 
-```
-$ pip install rria-api
-```
+	```
+	$ pip install rria-api
+	```
 
 ### **Example**
 
-```
-from rria_api.robot_facade import *
+```python
+from rria_api.robot_object import RobotObject
+from rria_api.robot_enum import RobotEnum
 
 # Create gen3 RobotObject
-gen3_lite = RobotObject('172.22.64.105', 'gen3')
+gen3_lite = RobotObject('192.168.2.10', RobotEnum.GEN3_LITE)
 
 # Create Niryo NED RobotObject
-ned = RobotObject('169.254.200.200', 'ned')
+ned = RobotObject('169.254.200.200', RobotEnum.NED)
 
 gen3_lite.connect_robot()
 ned.connect_robot()
 
 gen3_lite.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 ned.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
```

