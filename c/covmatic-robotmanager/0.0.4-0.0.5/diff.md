# Comparing `tmp/covmatic_robotmanager-0.0.4.tar.gz` & `tmp/covmatic_robotmanager-0.0.5.tar.gz`

## Comparing `covmatic_robotmanager-0.0.4.tar` & `covmatic_robotmanager-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaHelper.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaLockThread.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/__init__.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/api.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/calibrator.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/config.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/gripper.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/main.py
--rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/movement.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/positions.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot.py
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot_manager.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/singleton.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/toolpath.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/__init__.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/common.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/test_manager_plate.py
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/test_robot_manager.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/LICENSE
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/README.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/EvaHelper.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/EvaLockThread.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/__init__.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/api.py
+-rw-r--r--   0        0        0     8399 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/calibrator.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/config.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/gripper.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/main.py
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/movement.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/positions.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/robot.py
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/robot_manager.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/setup.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/singleton.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/toolpath.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/templates/Covmatic-robotmanager_Icon.ico
+-rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/templates/Covmatic-robotmanager_Icon.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/templates/covmatic.desktop
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/test/common.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/test/test_manager_plate.py
+-rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/test/test_robot_manager.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/README.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.5/PKG-INFO
```

### Comparing `covmatic_robotmanager-0.0.4/CHANGELOG.md` & `covmatic_robotmanager-0.0.5/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Covmatic RobotManager
 
+## v0.0.5
+
+## Fixed
+- [calibrator] main *HOME* position can be saved directly.
+- [calibrator] create *positions.json* file if not found.
+
+## Added
+- [setup] Setup module for creation of desktop link to start *robotmanager-server*
+
 ## v0.0.4
 
 ## Fixed
 - [server] do not home when pick and drop plate are inside same machine
 
 ## Added
 - [server] Robot operation has *aborted* state in case of error during pick
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaHelper.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/EvaHelper.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaLockThread.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/EvaLockThread.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/api.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/api.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/calibrator.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/calibrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,22 +249,24 @@
 
 
 def main_loop():
     global quit_requested, initial_angles
 
     getch = _Getch()
 
-    robot = Robot(Config().eva_ip, Config().eva_token, Config().positions_filepath, logger)
+    robot = Robot(Config().eva_ip, Config().eva_token, Config().positions_filepath, calibration=True, logger=logger)
     owner = input("Insert name of target robot: ")
 
-    pos_name = input("Insert name of position for robot {}: ".format(owner))
+    if owner == "HOME":
+        pos_name = "HOME"
+    else:
+        slot_name = input("Insert name of slot for robot {}: ".format(owner))
+        check_default_positions_exist_for_owner(robot, owner, slot_name)
+        pos_name = "{}-{}".format(owner, slot_name)
 
-    check_default_positions_exist_for_owner(robot, owner, pos_name)
-
-    pos_name = "{}-{}".format(owner, pos_name)
     print("Actual position {}".format(pos_name))
 
     with robot._eva_helper.eva.lock():
         check_position_exist_and_load(robot, pos_name)
 
         while not quit_requested:
             print("Position: {}".format(pos_name))
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/config.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 
 """
 import argparse
 import configargparse
 import os
 import logging
 from .singleton import SingletonMeta
+from .utils import FunctionCaseStartWith
+
+
+desktop_file = FunctionCaseStartWith(os.sys.platform)
+
+@desktop_file.case('linux')
+def desktop_file_linux():
+    return os.path.expanduser("~/.local/share/applications/covmatic-robotmanager.desktop")
+
+
+@desktop_file.case(('win32', 'cygwin'))
+def desktop_file_win():
+    import winshell
+    return os.path.join(winshell.desktop(), "Covmatic Robotmanager server.lnk")
+
+
+@desktop_file.case('')  # all other
+def desktop_file_other():
+    return ""
 
 
 class Config(argparse.Namespace, metaclass=SingletonMeta):
     _logger = logging.getLogger("robotmanager.config")
 
     @classmethod
     def get_base_config_folder(cls):
@@ -30,14 +49,18 @@
         return os.path.join(cls.get_base_config_folder(), "robotmanager.conf")
 
     @classmethod
     def get_default_positions_file_path(cls) -> str:
         return os.path.join(cls.get_base_config_folder(), "positions.json")
 
     @classmethod
+    def get_desktop_file_path(cls) -> str:
+        return desktop_file()
+
+    @classmethod
     def parse(cls, description):
         cls._logger.info("Checking for arguments in config file {}".format(cls.get_config_file_path()))
         parser = configargparse.ArgParser(description=description,
                                           default_config_files=[cls.get_config_file_path()],
                                           add_config_file_help=True)
         parser.add_argument('-E', '--eva-ip', metavar='address',  required=True, help="Eva hostname or ip address")
         parser.add_argument('-T', '--eva-token', metavar='token', required=True, help="Eva token")
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/gripper.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/gripper.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/main.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/main.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/movement.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/movement.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 
 
 class MovementException(Exception):
     pass
 
 
 class Movement:
-    def __init__(self, position_filepath: str, logger=logging.getLogger("robotmanager.movement")):
+    def __init__(self,
+                 position_filepath: str,
+                 calibration: bool = False,
+                 logger=logging.getLogger("robotmanager.movement")):
         self._eva = EvaHelper().eva
-        self._positions = Positions(position_filepath)
+        self._positions = Positions(position_filepath, create_file=calibration)
         self._logger = logger
         self._eva_helper = EvaHelper()
         self._logger.info("Loaded Eva: {}".format(self._eva_helper.get_robot_info()))
 
     def move_to(self, position):
         xyz = self._positions.get_position(position)
         self._logger.info("going to position: {}".format(xyz))
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/positions.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/positions.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 import os
 import logging
 
 
 class Positions:
     def __init__(self,
                  positions_file_path: str,
+                 create_file: bool = False,
                  logger=logging.getLogger("robotmanager.positions")):
         self._logger = logger
         self._abs_path = os.path.abspath(positions_file_path)
         self._logger.info("Checking path {}...".format(self._abs_path))
 
         if not os.path.exists(self._abs_path):
-            raise Exception("Position file passed must exist: {}".format(self._abs_path))
+            if create_file:
+                self._logger.info("Position file not existing... Creating a new one.")
+                with open(self._abs_path, "w") as fp:
+                    json.dump(dict(), fp)
+            else:
+                raise Exception("Position file passed must exist: {}".format(self._abs_path))
 
         with open(self._abs_path, "r") as fp:
             self._positions = json.load(fp)
 
         self._logger.debug("Loaded positions: {}".format(self._positions))
 
     def save(self, name, field, data):
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 
 class RobotException(Exception):
     pass
 
 
 class Robot:
-    def __init__(self, eva_ip_address, token, position_filepath, logger=logging.getLogger("robotmanager.robot")):
+    def __init__(self, eva_ip_address, token, position_filepath,
+                 calibration: bool = False, logger=logging.getLogger("robotmanager.robot")):
         self._logger = logger
         self._eva_helper = EvaHelper()
         self._eva_helper.connect(eva_ip_address, token)
-        self._movement = Movement(position_filepath)
+        self._movement = Movement(position_filepath, calibration=calibration)
 
     def unlock(self):
         self._eva_helper.disconnect()
 
     def save_position(self, name: str, joints=None):
         self._movement.save_position(name, joints)
```

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot_manager.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/robot_manager.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/singleton.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/singleton.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/toolpath.py` & `covmatic_robotmanager-0.0.5/src/covmatic_robotmanager/toolpath.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/test/test_manager_plate.py` & `covmatic_robotmanager-0.0.5/test/test_manager_plate.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/test/test_robot_manager.py` & `covmatic_robotmanager-0.0.5/test/test_robot_manager.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/.gitignore` & `covmatic_robotmanager-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/LICENSE` & `covmatic_robotmanager-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.4/pyproject.toml` & `covmatic_robotmanager-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,38 @@
 
 [project]
 name = "covmatic-robotmanager"
 authors = [
     { name="Agostino Facotti", email="agostino.facotti@asst-bergamoest.it"},
 ]
 description = "Covmatic Robot Manager is a robotic arm manager for action requested by other robots"
+keywords = ["automation", "lab", "biology", "robotics"]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Development Status :: 4 - Beta"
 ]
 dynamic = ["version"]
 
 dependencies = [
     "configargparse",
     "evasdk",
     "flask",
     "flask-restful",
-    "waitress"
+    "waitress",
+    "winshell; platform_system == 'Windows'",
+    "pywin32; platform_system == 'Windows'"
 ]
 
-[project-urls]
-"Homepage" = "https://github.com/ASST-Bergamo-Est/covmatic-robotmanager"
+[project.urls]
+Homepage = "https://github.com/ASST-Bergamo-Est/covmatic-robotmanager"
+"Source Code" = "https://github.com/ASST-Bergamo-Est/covmatic-robotmanager"
 
 [tool.hatch.version]
 path = "src/covmatic_robotmanager/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
```

