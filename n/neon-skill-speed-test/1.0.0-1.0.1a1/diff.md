# Comparing `tmp/neon-skill-speed_test-1.0.0.tar.gz` & `tmp/neon-skill-speed_test-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-speed_test-1.0.0.tar", last modified: Wed Jun 28 23:18:40 2023, max compression
+gzip compressed data, was "neon-skill-speed_test-1.0.1a1.tar", last modified: Mon Aug  7 23:12:23 2023, max compression
```

## Comparing `neon-skill-speed_test-1.0.0.tar` & `neon-skill-speed_test-1.0.1a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/locale/en-us/dialog/notify_testing.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/locale/en-us/dialog/results.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/locale/en-us/dialog/start_test.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/locale/en-us/intent/run_speed_test.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-28 23:18:39.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-28 23:18:40.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 23:18:39.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-28 23:18:39.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 23:18:39.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 23:18:39.000000 neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:18:40.009068 neon-skill-speed_test-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-28 23:18:34.000000 neon-skill-speed_test-1.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.415410 neon-skill-speed_test-1.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.415410 neon-skill-speed_test-1.0.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/locale/en-us/dialog/notify_testing.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/locale/en-us/dialog/results.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/locale/en-us/dialog/start_test.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/locale/en-us/intent/run_speed_test.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 23:12:23.000000 neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:12:23.419410 neon-skill-speed_test-1.0.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 23:12:19.000000 neon-skill-speed_test-1.0.1a1/version.py
```

### Comparing `neon-skill-speed_test-1.0.0/LICENSE.md` & `neon-skill-speed_test-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.0/PKG-INFO` & `neon-skill-speed_test-1.0.1a1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed_test
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.0/README.md` & `neon-skill-speed_test-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.0/__init__.py` & `neon-skill-speed_test-1.0.1a1/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,22 +35,28 @@
 
 from mycroft.skills import intent_file_handler
 
 
 class SpeedTestSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
-        self.test = speedtest.Speedtest()
+        self._test = None
         try:
             server = self.test.get_best_server()
             LOG.debug(f"Selected: {server}")
         except Exception as e:
             LOG.exception(e)
         # TODO: Support configured server
 
+    @property
+    def test(self):
+        # TODO: Handle 403 errors
+        self._test = self._test or speedtest.Speedtest()
+        return self._test
+
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
                                    requires_network=True,
```

### Comparing `neon-skill-speed_test-1.0.0/neon_skill_speed_test.egg-info/PKG-INFO` & `neon-skill-speed_test-1.0.1a1/neon_skill_speed_test.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed-test
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.0/setup.py` & `neon-skill-speed_test-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.0/skill.json` & `neon-skill-speed_test-1.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.0/test/test_skill.py` & `neon-skill-speed_test-1.0.1a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.0/version.py` & `neon-skill-speed_test-1.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1a1"
```

