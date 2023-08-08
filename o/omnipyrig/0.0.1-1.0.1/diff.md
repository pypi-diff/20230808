# Comparing `tmp/omnipyrig-0.0.1.tar.gz` & `tmp/omnipyrig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnipyrig-0.0.1.tar", last modified: Tue Aug  8 11:23:57 2023, max compression
+gzip compressed data, was "omnipyrig-1.0.1.tar", last modified: Tue Aug  8 13:09:30 2023, max compression
```

## Comparing `omnipyrig-0.0.1.tar` & `omnipyrig-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 11:23:57.812367 omnipyrig-0.0.1/
--rw-rw-rw-   0        0        0      640 2023-08-08 11:23:57.812367 omnipyrig-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-08-08 11:07:50.000000 omnipyrig-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 11:23:57.777479 omnipyrig-0.0.1/omnipyrig/
--rw-rw-rw-   0        0        0       36 2023-08-08 11:13:20.000000 omnipyrig-0.0.1/omnipyrig/__init__.py
--rw-rw-rw-   0        0        0     9652 2023-08-08 11:11:43.000000 omnipyrig-0.0.1/omnipyrig/omnipyrig.py
-drwxrwxrwx   0        0        0        0 2023-08-08 11:23:57.809379 omnipyrig-0.0.1/omnipyrig.egg-info/
--rw-rw-rw-   0        0        0      640 2023-08-08 11:23:57.000000 omnipyrig-0.0.1/omnipyrig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-08-08 11:23:57.000000 omnipyrig-0.0.1/omnipyrig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 11:23:57.000000 omnipyrig-0.0.1/omnipyrig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-08 11:23:57.000000 omnipyrig-0.0.1/omnipyrig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-08 11:23:57.000000 omnipyrig-0.0.1/omnipyrig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 11:23:57.813365 omnipyrig-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      948 2023-08-08 11:11:06.000000 omnipyrig-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:09:30.278385 omnipyrig-1.0.1/
+-rw-rw-rw-   0        0        0      548 2023-08-08 13:09:30.278385 omnipyrig-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-08-08 11:07:50.000000 omnipyrig-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 13:09:30.263192 omnipyrig-1.0.1/omnipyrig/
+-rw-rw-rw-   0        0        0       36 2023-08-08 11:13:20.000000 omnipyrig-1.0.1/omnipyrig/__init__.py
+-rw-rw-rw-   0        0        0     9768 2023-08-08 12:48:58.000000 omnipyrig-1.0.1/omnipyrig/omnipyrig.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:09:30.274987 omnipyrig-1.0.1/omnipyrig.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-08-08 13:09:30.000000 omnipyrig-1.0.1/omnipyrig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-08-08 13:09:30.000000 omnipyrig-1.0.1/omnipyrig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:09:30.000000 omnipyrig-1.0.1/omnipyrig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-08 13:09:30.000000 omnipyrig-1.0.1/omnipyrig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 13:09:30.000000 omnipyrig-1.0.1/omnipyrig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 13:09:30.278385 omnipyrig-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-08-08 13:09:15.000000 omnipyrig-1.0.1/setup.py
```

### Comparing `omnipyrig-0.0.1/PKG-INFO` & `omnipyrig-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: omnipyrig
-Version: 0.0.1
+Version: 1.0.1
 Summary: A python wrapper for Omni-Rig
 Author: 4Z1KD (Gil)
 Author-email: <4z1kd@iarc.org>
 Keywords: python,amateur radio,ham,omni-rig,omnirig,radio
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 A package that allows the deveplopment of amateur radio applications using the amazing Omni-Rig library
```

### Comparing `omnipyrig-0.0.1/omnipyrig/omnipyrig.py` & `omnipyrig-1.0.1/omnipyrig/omnipyrig.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,20 @@
     RIT_OFF = 0x00040000
     XIT_ON = 0x00080000
     XIT_OFF = 0x00100000
 
     #split
     SPLIT_ON = 0x00008000
     SPLIT_OFF = 0x00010000
+
+    #vfo
+    VFO_AA = 128
+    VFO_AB = 256
+    VFO_BB = 512
+    VFO_BA = 1024
     
 
     #c'tor
     def __init__(self):
         # create an instance of the service
         #self._omnirig = win32com.client.gencache.EnsureDispatch("Omnirig.OmnirigX")
         self._omnirig = win32com.client.Dispatch("Omnirig.OmnirigX")
@@ -168,27 +174,27 @@
                     pitch = int(pitch*10)
                     self._rig.Pitch = pitch
                 except ValueError:
                     return
 
     def setVfoA(self):
         time.sleep(self._timeout)
-        self._rig.Vfo = 128
+        self._rig.Vfo = self.VFO_AA
     
     def setVfoB(self):
         time.sleep(self._timeout)
-        self._rig.Vfo = 512
+        self._rig.Vfo = self.VFO_BB
     
     def setVfoAB(self):
         time.sleep(self._timeout)
-        self._rig.Vfo = 256
+        self._rig.Vfo = self.VFO_AB
     
     def setVfoBA(self):
         time.sleep(self._timeout)
-        self._rig.Vfo = 1024
+        self._rig.Vfo = self.VFO_BA
 
     def setActiveRig(self, index):
         if index == 1:
             self._rig = self._rig1
         elif index == 2:
             self._rig = self._rig2
```

### Comparing `omnipyrig-0.0.1/omnipyrig.egg-info/PKG-INFO` & `omnipyrig-1.0.1/omnipyrig.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: omnipyrig
-Version: 0.0.1
+Version: 1.0.1
 Summary: A python wrapper for Omni-Rig
 Author: 4Z1KD (Gil)
 Author-email: <4z1kd@iarc.org>
 Keywords: python,amateur radio,ham,omni-rig,omnirig,radio
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 A package that allows the deveplopment of amateur radio applications using the amazing Omni-Rig library
```

### Comparing `omnipyrig-0.0.1/setup.py` & `omnipyrig-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '1.0.1'
 DESCRIPTION = 'A python wrapper for Omni-Rig'
 LONG_DESCRIPTION = 'A package that allows the deveplopment of amateur radio applications using the amazing Omni-Rig library'
 
 # Setting up
 setup(
     name="omnipyrig",
     version=VERSION,
@@ -13,15 +13,13 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['pywin32'],
     keywords=['python', 'amateur radio', 'ham', 'omni-rig', 'omnirig', 'radio'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

