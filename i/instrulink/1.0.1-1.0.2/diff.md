# Comparing `tmp/instrulink-1.0.1.tar.gz` & `tmp/instrulink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instrulink-1.0.1.tar", last modified: Fri Aug  4 21:06:54 2023, max compression
+gzip compressed data, was "instrulink-1.0.2.tar", last modified: Tue Aug  8 20:20:33 2023, max compression
```

## Comparing `instrulink-1.0.1.tar` & `instrulink-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.744891 instrulink-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 21:06:44.000000 instrulink-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 21:06:44.000000 instrulink-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 21:06:54.744891 instrulink-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-04 21:06:44.000000 instrulink-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.740891 instrulink-1.0.1/instrulink/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/bk_2555.py
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/keysight_33500b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/keysight_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    43554 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/rigol_dg1022z.py
--rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/rigol_ds1054z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/si_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/sutter_mp285a.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/visa_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.740891 instrulink-1.0.1/instrulink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:06:44.000000 instrulink-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.744891 instrulink-1.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/list_visa_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_33500b.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_smoothed_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:06:54.744891 instrulink-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-04 21:06:44.000000 instrulink-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:20:33.036862 instrulink-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 20:20:22.000000 instrulink-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 20:20:22.000000 instrulink-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-08 20:20:33.036862 instrulink-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-08 20:20:22.000000 instrulink-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:20:33.032862 instrulink-1.0.2/instrulink/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/bk_2555.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/keysight_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/keysight_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58549 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/rigol_dg1022z.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/rigol_ds1054z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/si_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/sutter_mp285a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/visa_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-08-08 20:20:22.000000 instrulink-1.0.2/instrulink/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:20:33.036862 instrulink-1.0.2/instrulink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-08 20:20:33.000000 instrulink-1.0.2/instrulink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-08 20:20:33.000000 instrulink-1.0.2/instrulink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:20:33.000000 instrulink-1.0.2/instrulink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:20:32.000000 instrulink-1.0.2/instrulink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 20:20:33.000000 instrulink-1.0.2/instrulink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 20:20:33.000000 instrulink-1.0.2/instrulink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 20:20:22.000000 instrulink-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:20:33.036862 instrulink-1.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/list_visa_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-08 20:20:22.000000 instrulink-1.0.2/scripts/test_smoothed_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:20:33.036862 instrulink-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-08 20:20:22.000000 instrulink-1.0.2/setup.py
```

### Comparing `instrulink-1.0.1/LICENSE` & `instrulink-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/PKG-INFO` & `instrulink-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instrulink
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package to interface diverse laboratory instruments
 Home-page: https://github.com/tjjlemaire/instrulink
 Author: Theo Lemaire
 Author-email: theo.lemaire1@gmail.com
 License: MIT
 Keywords: laboratory instrument interface python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instrulink-1.0.1/README.md` & `instrulink-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/bk_2555.py` & `instrulink-1.0.2/instrulink/bk_2555.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/camera.py` & `instrulink-1.0.2/instrulink/camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/constants.py` & `instrulink-1.0.2/instrulink/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-07 17:11:50
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 11:43:32
+# @Last Modified time: 2023-08-08 15:13:27
 
 # Units conversion
 MHZ_TO_HZ = 1e6
 KHZ_TO_HZ = 1e3
 PA_TO_MPA = 1e-6
 S_TO_MS = 1e3
 MS_TO_S = 1e-3
 MV_TO_V = 1e-3
 KBS_TO_BS = 1e3
 S_TO_MS = 1e3
 CELSIUS_TO_KELVIN = 273.15
 
 # Default TTL pulse parameters
-TTL_PWIDTH = 1e-5  # width of a nominal TTL pulse (s)
-TTL_PAMP = 10.  # amplitude of a nominal TTL pulse (V)
+TTL_PWIDTH = 1e-4  # width of a nominal TTL pulse (s)
+TTL_PAMP = 5.  # amplitude of a nominal TTL pulse (V)
 
 # Regular expressions
 SI_REGEXP = '[+-]?\d\.\d+?[Ee][+-]?\d+'
 FLOAT_REGEXP = '[+-]?\d*[.]?\d+'
 INT_REGEXP = '\d+'
```

### Comparing `instrulink-1.0.1/instrulink/factory.py` & `instrulink-1.0.2/instrulink/factory.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/keysight_33500b.py` & `instrulink-1.0.2/instrulink/keysight_33500b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/keysight_e5061b.py` & `instrulink-1.0.2/instrulink/keysight_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/logger.py` & `instrulink-1.0.2/instrulink/logger.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/nidaq.py` & `instrulink-1.0.2/instrulink/nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/oscilloscope.py` & `instrulink-1.0.2/instrulink/oscilloscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-04-07 17:51:29
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 17:19:47
+# @Last Modified time: 2023-08-08 12:39:13
 # @Last Modified time: 2022-04-08 21:17:22
 
 import abc
 import re
 import io
 from PIL import Image
 import matplotlib.pyplot as plt
```

### Comparing `instrulink-1.0.1/instrulink/rigol_dg1022z.py` & `instrulink-1.0.2/instrulink/rigol_dg1022z.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-08 08:37:26
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-04 16:11:58
+# @Last Modified time: 2023-08-08 15:17:25
 
 import time
 import re
 from tqdm import tqdm
 import numpy as np
 
 from .waveform_generator import *
@@ -15,41 +15,62 @@
 from .constants import TTL_PWIDTH, TTL_PAMP, MV_TO_V
 from .utils import is_within
 from instrulink.wf_utils import *
 
 
 class RigolDG1022Z(WaveformGenerator):
 
+    # Miscellaneous
     USB_ID = 'DG1ZA\d+'  # USB identifier
     NO_ERROR_CODE = '0,"No error"'  # error code returned when no error
     ANGLE_UNITS = ('DEG')
     MAX_LEN_TEXT = 40
     WAVEFORM_TYPES = ('SIN', 'SQU', 'RAMP', 'PULS', 'NOIS', 'DC', 'USER')
     FMAX = 25e6  # max frequency (Hz)
     VMAX = 20.0  # max voltage (Vpp)
+    ANTIPHASE = 180  # degrees
+    CHANNELS = (1, 2)
+    PREFIX = ':'
+    # TIMEOUT_SECONDS = 20.  # long timeout to allow slow commands (e.g. waveform loading)
+
+    # Coupling
+    CPL_PATTERN = '^FREQ:(ON|OFF),PHASE:(ON|OFF),AMPL:(ON|OFF)$'
+    CPL_MODES = ('OFFS', 'RAT')  # coupling modes
+    CPL_AMP_RATIO_BOUNDS = (1e-3, 1e3)  # bounds for amplitude coupling ratio
+    CPL_AMP_DEV_BOUNDS = (-19.998, 19.998)  # bounds for amplitude coupling deviation
+    CPL_FREQ_RATIO_BOUNDS = (1e-6, 1e6)  # bounds for frequency coupling ratio
+    CPL_FREQ_DEV_BOUNDS = (-0.99 * FMAX, 0.99 * FMAX)  # bounds for frequency coupling deviation
+    CPL_PHASE_RATIO_BOUNDS = (1e-2, 1e2)  # bounds for phase coupling ratio
+    CPL_PHASE_DEV_BOUNDS = (-360, 360)  # bounds for phase coupling deviation
+
+    # Bursting
     BURST_MODES = ('TRIG', 'INF', 'GAT')
     BURST_IDLE_LEVELS = ('FPT', 'TOP', 'CENTER', 'BOTTOM')
     PULSE_HOLDS = ('WIDT', 'DUTY')
     MAX_BURST_PERIOD = 500. # s
+
+    # Modulation
     MOD_MODES = ('AM', 'FM', 'PM', 'ASK', 'FSK', 'PSK', 'PWM')
     MOD_VOLT_RANGE = (-5, 5)  # voltage range regulating modulation (V)
+    MOD_VOLT_MARGIN = 0.05  # margin on each side to ensure full range amplitude modulation (V)
     AM_DEPTH_RANGE = (0, 120)  # AM depth range (%)
     AM_FREQ_RANGE = (2e-3, 1e6)  # AM frequency range (Hz)
     MOD_SOURCES = ('INT', 'EXT')  # modulation sources
+
+    # Trigger
     TRIGGER_SOURCES = ('INT', 'EXT', 'MAN')
+
+    # Arbitrary waveform
     ARB_OUTPUT_MODES = ('FREQ', 'SRATE')
     ARB_SRATE_BOUNDS = (1e-6, 60e6)  # bounds for arbitrary waveform sample rate (Hz)
     ARB_WF_NPTS_BOUNDS = (8, 16384)  # bounds for arbitrary waveform number of points
     ARB_WF_MAXNPTS_PER_PACKET = 8192  # max number of points per packet for arbitrary waveform upload
     ARB_WF_DAC_RANGE = (0, 16383)  # integer range for arbitrary waveform DAC values
     ARB_WF_FLOAT_RANGE = (-1, 1)  # floating point range for arbitrary waveform values
-    CHANNELS = (1, 2)
-    PREFIX = ':'
     WAF_PATTERN = '^(ARB)(10?|[2-9])$'
-    # TIMEOUT_SECONDS = 20.  # long timeout to allow slow commands (e.g. waveform loading)
 
     def beep(self):
         ''' Issue a single beep immediately. '''
         self.write('SYST:BEEP:IMM')
     
     # --------------------- UNITS ---------------------
     
@@ -108,14 +129,328 @@
         time.sleep(1)
         self.disable_output_channel(1)
         time.sleep(1)
         self.enable_output()
         time.sleep(1)
         self.disable_output()
     
+    # --------------------- SYNC ---------------------
+    
+    def enable_output_sync(self, ich):
+        ''' Enable sync signal of specific channel on rear panel connector '''
+        self.check_channel_index(ich)
+        self.write(f'OUTP{ich}:SYNC ON')
+    
+    def disable_output_sync(self, ich):
+        ''' Disable sync signal of specific channel on rear panel connector '''
+        self.check_channel_index(ich)
+        self.write(f'OUTP{ich}:SYNC OFF')
+    
+    def is_output_sync_on(self, ich):
+        ''' Query whether sync signal is enabled for a specific channel '''
+        self.check_channel_index(ich)
+        out = self.query(f'OUTP{ich}:SYNC?')
+        return out == 'ON'
+
+    def set_output_sync_delay(self, ich, delay):
+        ''' 
+        Set sync signal delay for a specific channel 
+
+        :param ich: channel index
+        :param delay: delay (s)
+        '''
+        self.check_channel_index(ich)
+        T = 1 / self.get_waveform_freq(ich)
+        if not is_within(delay, (0, T)):
+            raise VisaError(f'invalid delay: {delay} (must be within [0, 1/f = {si_format(T, 2)}s])')
+        self.write(f'OUTP{ich}:SYNC:DEL {delay}')
+    
+    def get_output_sync_delay(self, ich):
+        ''' 
+        Get sync signal delay for a specific channel 
+
+        :param ich: channel index
+        :return: delay (s)
+        '''
+        self.check_channel_index(ich)
+        return float(self.query(f'OUTP{ich}:SYNC:DEL?'))
+    
+    def set_output_sync_polarity(self, ich, pol):
+        ''' 
+        Set sync signal polarity for a specific channel 
+
+        :param ich: channel index
+        :param pol: polarity ("POS" or "NEG")
+        '''
+        self.check_channel_index(ich)
+        if pol not in self.SLOPES:
+            raise VisaError(f'invalid polarity: "{pol}" (must be in {self.SLOPES})')
+        self.write(f'OUTP{ich}:SYNC:POL {pol}')
+
+    def get_output_sync_polarity(self, ich):
+        ''' 
+        Get sync signal polarity for a specific channel 
+
+        :param ich: channel index
+        :return: polarity ("POS" or "NEG")
+        '''
+        self.check_channel_index(ich)
+        return self.query(f'OUTP{ich}:SYNC:POL?')
+
+    # --------------------- COUPLING ---------------------
+
+    def enable_all_coupling(self):
+        ''' 
+        Enable frequency, phase and amplitude coupling across channels.
+        '''
+        self.write('COUP ON')
+    
+    def disable_all_coupling(self):
+        ''' 
+        Disable frequency, phase and amplitude coupling across channels.
+        '''
+        self.write('COUP OFF')
+    
+    def is_coupling_on(self):
+        ''' 
+        Query whether frequency, phase and amplitude coupling across channels are enabled.
+
+        :return: dictionary of coupling states
+        '''
+        out = self.query('COUP?')
+        mo = re.match(self.CPL_PATTERN, out)
+        if mo is None:
+            raise VisaError(f'invalid coupling query response: "{out}"')
+        cplstates = dict(zip(('FREQ', 'PHASE', 'AMPL'), mo.groups()))
+        return {k: v == 'ON' for k, v in cplstates.items()}
+
+    # --------------------- AMPLITUDE COUPLING ---------------------
+
+    def enable_amplitude_coupling(self):
+        ''' 
+        Enable amplitude coupling across channels.
+        '''
+        self.write('COUP:AMPL ON')
+    
+    def disable_amplitude_coupling(self):
+        ''' 
+        Disable amplitude coupling across channels.
+        '''
+        self.write('COUP:AMPL OFF')
+    
+    def is_amplitude_coupling_on(self):
+        ''' 
+        Query whether amplitude coupling across channels is enabled.
+
+        :return: boolean
+        '''
+        return self.query('COUP:AMPL?') == 'ON'
+
+    def set_amplitude_coupling_mode(self, mode):
+        ''' 
+        Set amplitude coupling mode across channels.
+
+        :param mode: amplitude coupling ("OFFS" for deviation or "RAT" for ratio)
+        '''
+        if mode not in self.CPL_MODES:
+            raise VisaError(f'invalid amplitude coupling mode: "{mode}" (must be one of {self.CPL_MODES})')
+        self.write(f'COUP:AMPL:MODE {mode}')
+    
+    def get_amplitude_coupling_mode(self):
+        ''' 
+        Get amplitude coupling mode across channels.
+
+        :return: amplitude coupling mode
+        '''
+        return self.query('COUP:AMPL:MODE?')
+
+    def set_amplitude_coupling_ratio(self, ratio):
+        ''' 
+        Set amplitude coupling ratio across channels.
+
+        :param ratio: amplitude coupling ratio
+        '''
+        if not is_within(ratio, self.CPL_AMP_RATIO_BOUNDS):
+            raise VisaError(f'invalid amplitude coupling ratio: "{ratio}" (must be within {self.CPL_AMP_RATIO_BOUNDS})')
+        self.write(f'COUP:AMPL:RAT {ratio}')
+    
+    def get_amplitude_coupling_ratio(self):
+        ''' 
+        Get amplitude coupling ratio across channels.
+
+        :return: amplitude coupling ratio
+        '''
+        return float(self.query('COUP:AMPL:RAT?'))
+
+    def set_amplitude_coupling_deviation(self, deviation):
+        ''' 
+        Set amplitude coupling deviation across channels.
+
+        :param deviation: amplitude coupling deviation
+        '''
+        if not is_within(deviation, self.CPL_AMP_DEV_BOUNDS):
+            raise VisaError(f'invalid amplitude coupling deviation: "{deviation}" (must be within {self.CPL_AMP_DEV_BOUNDS})')
+        self.write(f'COUP:AMPL:DEV {deviation}')
+    
+    def get_amplitude_coupling_deviation(self):
+        ''' 
+        Get amplitude coupling deviation across channels.
+
+        :return: amplitude coupling deviation
+        '''
+        return float(self.query('COUP:AMPL:DEV?'))
+    
+    # --------------------- FREQUENCY COUPLING ---------------------
+
+    def enable_frequency_coupling(self):
+        ''' 
+        Enable frequency coupling across channels.
+        '''
+        self.write('COUP:FREQ ON')
+
+    def disable_frequency_coupling(self):
+        ''' 
+        Disable frequency coupling across channels.
+        '''
+        self.write('COUP:FREQ OFF')
+
+    def is_frequency_coupling_on(self):
+        '''
+        Query whether frequency coupling across channels is enabled.
+        '''
+        return self.query('COUP:FREQ?') == 'ON'
+
+    def set_frequency_coupling_mode(self, mode):
+        ''' 
+        Set frequency coupling mode across channels.
+
+        :param mode: frequency coupling ("OFFS" for deviation or "RAT" for ratio)
+        '''
+        if mode not in self.CPL_MODES:
+            raise VisaError(f'invalid frequency coupling mode: "{mode}" (must be one of {self.CPL_MODES})')
+        self.write(f'COUP:FREQ:MODE {mode}')
+    
+    def get_frequency_coupling_mode(self):
+        ''' 
+        Get frequency coupling mode across channels.
+
+        :return: frequency coupling mode
+        '''
+        return self.query('COUP:FREQ:MODE?')
+
+    def set_frequency_coupling_ratio(self, ratio):
+        ''' 
+        Set frequency coupling ratio across channels.
+
+        :param ratio: frequency coupling ratio
+        '''
+        if not is_within(ratio, self.CPL_FREQ_RATIO_BOUNDS):
+            raise VisaError(f'invalid frequency coupling ratio: "{ratio}" (must be within {self.CPL_FREQ_RATIO_BOUNDS})')
+        self.write(f'COUP:FREQ:RAT {ratio}')
+    
+    def get_frequency_coupling_ratio(self):
+        ''' 
+        Get frequency coupling ratio across channels.
+
+        :return: frequency coupling ratio
+        '''
+        return float(self.query('COUP:FREQ:RAT?'))
+
+    def set_frequency_coupling_deviation(self, deviation):
+        ''' 
+        Set frequency coupling deviation across channels.
+
+        :param deviation: frequency coupling deviation
+        '''
+        if not is_within(deviation, self.CPL_FREQ_DEV_BOUNDS):
+            raise VisaError(f'invalid frequency coupling deviation: "{deviation}" (must be within {self.CPL_FREQ_DEV_BOUNDS})')
+        self.write(f'COUP:FREQ:DEV {deviation}')
+
+    def get_frequency_coupling_deviation(self):
+        ''' 
+        Get frequency coupling deviation across channels.
+
+        :return: frequency coupling deviation
+        '''
+        return float(self.query('COUP:FREQ:DEV?'))
+
+    # --------------------- PHASE COUPLING ---------------------
+
+    def enable_phase_coupling(self):
+        ''' 
+        Enable phase coupling across channels.
+        '''
+        self.write('COUP:PHAS ON')
+    
+    def disable_phase_coupling(self):
+        ''' 
+        Disable phase coupling across channels.
+        '''
+        self.write('COUP:PHAS OFF')
+    
+    def is_phase_coupling_on(self):
+        '''
+        Query whether phase coupling across channels is enabled.
+        '''
+        return self.query('COUP:PHAS?') == 'ON'
+
+    def set_phase_coupling_mode(self, mode):
+        ''' 
+        Set phase coupling mode across channels.
+
+        :param mode: phase coupling ("OFFS" for deviation or "RAT" for ratio)
+        '''
+        if mode not in self.CPL_MODES:
+            raise VisaError(f'invalid phase coupling mode: "{mode}" (must be one of {self.CPL_MODES})')
+        self.write(f'COUP:PHAS:MODE {mode}')
+    
+    def get_phase_coupling_mode(self):
+        ''' 
+        Get phase coupling mode across channels.
+
+        :return: phase coupling mode
+        '''
+        return self.query('COUP:PHAS:MODE?')
+    
+    def set_phase_coupling_ratio(self, ratio):
+        ''' 
+        Set phase coupling ratio across channels.
+
+        :param ratio: phase coupling ratio
+        '''
+        if not is_within(ratio, self.CPL_PHASE_RATIO_BOUNDS):
+            raise VisaError(f'invalid phase coupling ratio: "{ratio}" (must be within {self.CPL_PHASE_RATIO_BOUNDS})')
+        self.write(f'COUP:PHAS:RAT {ratio}')
+    
+    def get_phase_coupling_ratio(self):
+        ''' 
+        Get phase coupling ratio across channels.
+
+        :return: phase coupling ratio
+        '''
+        return float(self.query('COUP:PHAS:RAT?'))
+    
+    def set_phase_coupling_deviation(self, deviation):
+        ''' 
+        Set phase coupling deviation across channels.
+
+        :param deviation: phase coupling deviation
+        '''
+        if not is_within(deviation, self.CPL_PHASE_DEV_BOUNDS):
+            raise VisaError(f'invalid phase coupling deviation: "{deviation}" (must be within {self.CPL_PHASE_DEV_BOUNDS})')
+        self.write(f'COUP:PHAS:DEV {deviation}')
+    
+    def get_phase_coupling_deviation(self):
+        ''' 
+        Get phase coupling deviation across channels.
+
+        :return: phase coupling deviation
+        '''
+        return float(self.query('COUP:PHAS:DEV?'))
+
     # --------------------- BASIC WAVEFORM ---------------------
 
     def apply_waveform(self, wtype, ich, freq, amp, offset=0, phase=0):
         ''' Apply a waveform with specific parameters.
 
             :param wtype: waveform function
             :param ich: channel number
@@ -165,32 +500,44 @@
         self.check_channel_index(ich)
         self.check_amp(amp)
         self.write(f'SOUR{ich}:VOLT:LEV:IMM:AMPL {amp}')
 
     def get_waveform_amp(self, ich):
         self.check_channel_index(ich)
         return float(self.query(f'SOUR{ich}:VOLT:LEV:IMM:AMPL?'))
+    
+    def check_offset(self, offset, ich):
+        if np.absolute(offset) > self.VMAX - self.get_waveform_amp(ich) / 2:
+            raise VisaError(f'|VPP/2| + |Voffset| exceeds {self.VMAX} V')
 
     def set_waveform_offset(self, ich, offset):
         self.check_channel_index(ich)
-        self.check_offset(offset)
+        self.check_offset(offset, ich)
         self.write(f'SOUR{ich}:VOLT:LEV:IMM:OFFS {offset}')
 
     def get_waveform_offset(self, ich):
         self.check_channel_index(ich)
         return float(self.query(f'SOUR{ich}:VOLT:LEV:IMM:OFFS?'))
     
     def set_waveform_phase(self, ich, phase):
         self.check_channel_index(ich)
         self.check_phase(phase)
         self.write(f'SOUR{ich}:PHAS {phase}')
     
     def get_waveform_phase(self, ich):
         self.check_channel_index(ich)
         return float(self.query(f'SOUR{ich}:PHAS?'))  # degrees
+
+    def invert_waveform_phase(self, ich):
+        ''' Invert the phase of the waveform of the specified channel. '''
+        self.set_waveform_phase(ich, self.ANTIPHASE)
+    
+    def is_waveform_phase_inverted(self, ich):
+        ''' Query whether the phase of the waveform of the specified channel is inverted. '''
+        return self.get_waveform_phase(ich) == self.ANTIPHASE
     
     def set_square_duty_cycle(self, ich, DC):
         self.check_channel_index(ich)
         self.check_duty_cycle(DC)
         self.write(f'SOUR{ich}:FUNC:SQU:DCYC {DC}')
 
     def get_square_duty_cycle(self, ich):
@@ -345,26 +692,28 @@
     
     def write_binary_values(self, cmd, values, **kwargs):
         ''' Write binary values to instrument. '''
         logger.debug(f'{cmd} {values.size}')
         self.instrument_handle.write_binary_values(
             f'{self.PREFIX}{cmd}', values, **kwargs)
 
-    def upload_arbitrary_waveform(self, ich, y, dtype='dac16', precision=2, adapt_npoints=True):
+    def upload_arbitrary_waveform(self, ich, y, dtype='dac16', precision=2,
+                                  adapt_npoints=True, activate=False):
         ''' 
         Upload an arbitrary waveform into volatile memory of a specific channel
         
         :param ich: channel index
         :param y: waveform vector
         :param dtype: data type used to upload waveform vector (default: "dac16")
             - "float": floating point values between -1 and 1
             - "dac": decimal DAC values between 0 and 16383
             - "dac16": 16-bits binary DAC values between 0 and 16383
         :param precision: number of decimal digits to use for each sample (default: 2, only used with "float" data type)
         :param adapt_npoints: whether to adapt the waveform vector to match the reference number of points of instrument waveforms
+        :param activate: whether to set waveform type to arbitrary after upload (default: False)
         '''
         # Check channel index
         self.check_channel_index(ich)
 
         # Cast waveform vector to numpy array, and check waveform size
         y = np.asarray(y)
         
@@ -423,14 +772,18 @@
         # to avoid unwanted padding
         if y.size < self.ARB_WF_MAXNPTS_PER_PACKET:
             self.set_waveform_npoints(ich, y.size)
 
         # Set output mode to frequency to enable use as amplitude modulator
         self.set_arbitrary_output_mode(ich, 'FREQ')
 
+        # If specified, set waveform type to arbitrary
+        if activate:
+            self.set_waveform_type(ich, 'USER')
+
     @property
     def ARB_WF_DAC_MAX(self):
         ''' Maximum integer value for arbitrary waveform DAC. '''
         return self.ARB_WF_DAC_RANGE[1]
     
     def get_waveform_value(self, ich, idx):
         '''
@@ -865,17 +1218,17 @@
         '''
         if T is not None:
             self.set_burst_internal_period(ich, T)
         self.set_trigger_source(ich, 'INT')
     
     # --------------------- MULTI-LAYER PULSING ---------------------
     
-    def set_gating_pulse_train(self, ich, PRF, tburst, Vpp=None, T=None, trig_source='EXT'):
+    def set_trigger_pulse_train(self, ich, PRF, tburst, Vpp=None, T=None, trig_source='EXT'):
         '''
-        Set a gating pulse train on a specific channel
+        Set a train of TTL-type trigger pulses on a specific channel
         
         :param ich: channel index
         :param PRF: pulse repetition frequency (Hz)
         :param tburst: burst duration (s)
         :param Vpp: pulse amplitude in V, defaults to TTL pulse amplitude (5V)
         :param T: burst repetition period in s, only for internal trigger source (defaults to 2)
         :param trig_source: trigger source (default: external)
@@ -915,31 +1268,33 @@
         # Set burst repetition period, if any
         if T is not None:
             self.set_burst_internal_period(ich, T)  # s
         # Set burst duration
         self.set_burst_duration(ich, tburst)  # s
         # Enable burst mode on channel
         self.enable_burst(ich)
+        # Enable channel sync signal on rear panel connector
+        self.enable_output_sync(ich)
         # Set channel trigger source
         self.set_trigger_source(ich, trig_source)
     
-    def set_modulating_pulse_train(self, ich, PRF, DC, tburst, tramp=0, T=None, trig_source='EXT'):
+    def set_AM_pulse_train(self, ich, PRF, DC, tburst, tramp=0, T=None, trig_source='EXT'):
         '''
         Set an amplitude modulating pulse train on a specific channel
         
         :param ich: channel index
         :param PRF: pulse repetition frequency (Hz)
         :param DC: duty cycle (%)
         :param tburst: burst duration (s)
         :param tramp: nominal pulse ramping duration (s), defaults to 0
         :param T: burst repetition period in s, only for internal trigger source (defaults to 2)
         :param trig_source: trigger source (default: external)
         '''
         # Define default log message
-        s = f'setting channel {ich} to trigger {si_format(tburst, 2)}s long modulating pulse train with {si_format(PRF, 2)}Hz internal PRF'
+        s = f'setting channel {ich} to trigger {si_format(tburst, 2)}s long amplitude-modulating pulse train with {si_format(PRF, 2)}Hz internal PRF'
 
         # Add ramping time to log message if specified
         if tramp > 0:
             s = f'{s} and {si_format(tramp, 2)}s ramping time'
 
         # Complete log message based on trigger source
         if trig_source == 'INT':
@@ -957,82 +1312,88 @@
         logger.info(s)
 
         # If ramping time is specified
         if tramp > 0:
             # Design smoothed waveform with appropriate number of points
             npts = self.ARB_WF_MAXNPTS_PER_PACKET
             _, y = get_DC_smoothed_pulse_envelope(npts, PRF, DC, tramp=tramp, plot='all')
-            # Upload it to volatile memory of specified channel, and set waveform type to "user"
-            self.upload_arbitrary_waveform(ich, y)
-            self.set_waveform_type(ich, 'USER')
+            # Upload it to volatile memory of specified channel, 
+            # and set waveform type to "user"
+            self.upload_arbitrary_waveform(ich, y, activate=True)
         # Otherwise
         else:
             # Use standard rectangular pulse with specific duty cycle
             self.set_waveform_type(ich, 'SQU')
             self.set_square_duty_cycle(ich, DC)  # %
-            self.set_waveform_phase(ich, 180)  # set phase to 180 deg to avoid DC offset
+            self.invert_waveform_phase(ich)  # invert phase to avoid DC offset
 
-        # Set waveform amplitude to full AM range (+/- 5V)
-        self.set_waveform_amp(ich, self.MOD_VOLT_AMP)
+        # Set waveform amplitude to full AM range (with extra margin) and ensure zero offset
+        self.set_waveform_amp(ich, (1 + 2 * self.MOD_VOLT_MARGIN) * self.MOD_VOLT_AMP)
+        self.set_waveform_offset(ich, 0)
         # Apply waveform as burst with specific repetition frequency
         self.set_waveform_freq(ich, PRF)
         # Set channel trigger source to external (to avoid erroneous outputs upon setting)
         self.set_trigger_source(ich, 'EXT')
         # Set burst repetition period, if any
         if T is not None:
             self.set_burst_internal_period(ich, T)  # s
         # Set burst duration
         self.set_burst_duration(ich, tburst)  # s
         # Enable burst mode on channel
         self.enable_burst(ich)
+        # Enable channel sync signal on rear panel connector
+        self.enable_output_sync(ich)
+        # If waveform is phase-inverted, set sync polarity to negative
+        if self.is_waveform_phase_inverted(ich):
+            self.set_output_sync_polarity(ich, 'NEG')
         # Set channel trigger source
         self.set_trigger_source(ich, trig_source)
 
-    def set_gated_sine_burst(self, Fdrive, Vpp, tstim, PRF, DC, ich_gate=1, ich_carrier=2, **kwargs):
+    def set_triggered_sine_burst_train(self, Fdrive, Vpp, tstim, PRF, DC, ich_trig=1, ich_carrier=2, **kwargs):
         '''
-        Set sine burst on channel 2 gated by channel 1 (used for pulsed US stimulus)
+        Set a train of sine bursts on a specific channel, triggered by another channel. 
+        Used for pulsed sinusoidal waveform generation.
         
         :param Fdrive: driving frequency (Hz)
         :param Vpp: waveform amplitude (Vpp)
         :param tstim: total stimulus duration (s)
         :param PRF: pulse repetition frequency (Hz)
         :param DC: duty cycle (%)
         :param ich_gate: index of the gating channel
         :param ich_carrier: index of the carrier channel
         '''
         # Check that channels indexes are different
-        if ich_gate == ich_carrier:
-            raise VisaError('gating and carrier channels cannot be identical')
+        if ich_trig == ich_carrier:
+            raise VisaError('trigger and carrier channels cannot be identical')
         
         # Disable all outputs (carrier channel first to avoid erroneous outputs)
         self.disable_output_channel(ich_carrier)
-        self.disable_output_channel(ich_gate)
+        self.disable_output_channel(ich_trig)
         
-        # Set gating channel parameters
-        self.set_gating_pulse_train(ich_gate, PRF, tstim, **kwargs)
+        # Set trigger channel parameters
+        self.set_trigger_pulse_train(ich_trig, PRF, tstim, **kwargs)
 
-        # Set sinewave channel parameters
+        # Set carrier channel parameters
         tburst = DC / (100 * PRF)  # s
-        logger.info(f'setting channel {ich_carrier} to output {si_format(tburst, 2)}s long, ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave triggered externally by channel {ich_gate}')
+        logger.info(f'setting channel {ich_carrier} to output {si_format(tburst, 2)}s long, ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave triggered externally by channel {ich_trig}')
         self.apply_sine(ich_carrier, Fdrive, Vpp)
-        self.set_trigger_source(ich_carrier, 'EXT')
         self.set_burst_duration(ich_carrier, tburst)  # s
         self.enable_burst(ich_carrier)
         self.set_trigger_source(ich_carrier, 'EXT')
 
         # If carrier amplitude is > 0, enable all outputs 
         # (carrier channel last to avoid erroneous outputs)
         if Vpp > 0.:
-            self.enable_output_channel(ich_gate)
+            self.enable_output_channel(ich_trig)
             self.enable_output_channel(ich_carrier)
     
-    def set_modulated_sine_burst(self, Fdrive, Vpp, tstim, PRF, DC, tramp=0, ich_mod=1, ich_carrier=2, **kwargs):
+    def set_AM_sine_burst_train(self, Fdrive, Vpp, tstim, PRF, DC, tramp=0, ich_mod=1, ich_carrier=2, **kwargs):
         '''
-        Set sine burst on channel 2 amplitude modulated by channel 1.
-        Used for (smoothed) pulsed US stimulus.
+        Set a train of sine bursts on a specific channel, amplitude-modulated by another channel.
+        Used for pulsed sinusoidal waveform generation, with optional envelope smoothing.
         
         :param Fdrive: driving frequency (Hz)
         :param Vpp: waveform amplitude (Vpp)
         :param tstim: total stimulus duration (s)
         :param PRF: pulse repetition frequency (Hz)
         :param DC: duty cycle (%)
         :param tramp: nominal pulse ramping duration (s), defaults to 0
@@ -1044,67 +1405,119 @@
             raise VisaError('gating and carrier channels cannot be identical')
         
         # Disable all outputs (carrier channel first to avoid erroneous outputs)
         self.disable_output_channel(ich_carrier)
         self.disable_output_channel(ich_mod)
         
         # Set envelope modulating channel parameters
-        self.set_modulating_pulse_train(ich_mod, PRF, DC, tstim, tramp=tramp, **kwargs)
+        self.set_AM_pulse_train(ich_mod, PRF, DC, tstim, tramp=tramp, **kwargs)
 
         # Set sinewave channel parameters
-        logger.info(f'setting channel {ich_carrier} to output ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave amplitude modulated externally by channel {ich_mod}')
+        logger.info(f'setting channel {ich_carrier} to output ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave amplitude-modulated externally by channel {ich_mod}')
         self.apply_sine(ich_carrier, Fdrive, Vpp, 0)
         self.enable_am(ich_carrier)
         self.set_am_source(ich_carrier, 'EXT')
 
         # If carrier amplitude is > 0, enable all outputs 
         # (carrier channel last to avoid erroneous outputs)
         if Vpp > 0.:
             self.enable_output_channel(ich_mod)
             self.enable_output_channel(ich_carrier)
     
-    def set_looping_sine_burst(self, ich, Fdrive, Vpp=.1, ncycles=200, PRF=100., tramp=0, ich_trig=None):
+    def set_gated_sine_burst(self, *args, tramp=0, ich_gate=1, ich_carrier=2, gate_type='trig', **kwargs):
+        '''
+        Wrapper method to set up a train of sine bursts on a carrier channel, gated by
+        another channel with a specific gating method. Two gating methods are supported:
+        - "trigger" gating -> calls `set_triggered_sine_burst` method
+        - "mod" gating -> calls `set_AM_sine_burst` method
+        The "trigger" gating method is the default, but does not support envelope smoothing.
+        
+        :param tramp: nominal pulse ramping duration (s), defaults to 0
+        :param ich_gate: index of the gating channel
+        :param ich_carrier: index of the carrier channel
+        :param gate_type: gating type (default: "trigger")
+        '''
+        # Trigger gating
+        if gate_type == 'trig':
+            # Check that ramp time is 0
+            if tramp > 0:
+                raise VisaError('ramping time not supported for trigger gating')
+            # Call `set_triggered_sine_burst` method
+            self.set_triggered_sine_burst_train(
+                *args, ich_trig=ich_gate, ich_carrier=ich_carrier, **kwargs)
+        
+        # Modulation gating
+        elif gate_type == 'mod':
+            # Call `set_AM_sine_burst` method
+            self.set_AM_sine_burst_train(
+                *args, tramp=tramp, ich_mod=ich_gate, ich_carrier=ich_carrier, **kwargs)
+        
+        # Invalid gating type
+        else:
+            raise VisaError(f'invalid gating type: {gate_type}')
+    
+    def set_looping_sine_burst(self, ich, Fdrive, Vpp=.1, ncycles=200, PRF=100., tramp=0, 
+                               ich_trig=None, gate_type='trig'):
         '''
         Set an internally looping sine burst on a specific channel
         
         :param ich: channel index (1 or 2)
         :param Fdrive: driving frequency (Hz)
         :param Vpp: waveform amplitude (Vpp)
         :param ncycles: number of cycles per burst
         :param PRF: pulse repetition frequency (Hz)
         :param tramp: nominal pulse ramping duration (s), defaults to 0
         :param ich_trig (optional): triggering channel index
         '''
         # Cast number of cycles to integer
         ncycles = int(np.round(ncycles))
+        if ncycles < 1:
+            raise VisaError(f'invalid number of cycles: {ncycles} (must be >= 1)')
 
         # If trigger channel is different than signal channel
         if ich_trig is not None:
             # Compute nominal burst duration and duty cycle
             tburst = ncycles / Fdrive  # s
 
-            # If no ramp time is speficied
-            if tramp == 0:
-                # Use `set_gated_sine_burst` to set up loop
-                self.set_gated_sine_burst(
-                    Fdrive, Vpp, tburst, 1 / tburst, 100, 
-                    T=1. / PRF, ich_gate=ich_trig, ich_carrier=ich)
-                # Start trigger loop 
-                self.start_trigger_loop(ich_trig, T=1. / PRF)
+            # Compute modulation periodicity
+            mod_T = 1 / PRF  # s
 
-            # Otherwise
+            # Determine gating type
+            if gate_type not in ('trig', 'mod'):
+                raise ValueError(f'invalid gating type: {gate_type}')
+            if tramp > 0 and gate_type == 'trig':
+                logger.warning('ramping time not supported for trigger gating, switching to modulation gating')
+                gate_type = 'mod'
+
+            # Determine gate-type-dependent parameters
+            if gate_type == 'trig':
+                DC = 100  # %
+                tstim = tburst  # s
+                internal_PRF = 1 / tburst
             else:
-                # Compute DC
                 DC = PRF * tburst * 100  # %
                 if DC > 100:
                     raise ValueError(f'{si_format(tburst, 2)}s burst cannot be pulsed at {PRF:.2f} Hz')
-                # Use `set_modulated_sine_burst` to set up loop
-                self.set_modulated_sine_burst(
-                    Fdrive, Vpp, 2 / PRF, PRF, DC, tramp=tramp, 
-                    T=1. / PRF, ich_mod=ich_trig, ich_carrier=ich)
+                tstim = 2 / PRF  # s
+                internal_PRF = PRF
+
+            # Set up gated pulse train
+            self.set_gated_sine_burst(
+                Fdrive, Vpp, tstim, internal_PRF, DC, T=mod_T, 
+                tramp=tramp if gate_type == 'mod' else 0, 
+                ich_gate=ich_trig, ich_carrier=ich, gate_type=gate_type
+            )
+            
+            # Trigger mode: start trigger loop on trigger channel
+            if gate_type == 'trig':
+                self.start_trigger_loop(ich_trig, T=1. / PRF)
+            
+            # Modulation mode: disable burst mode on modulation channel to start
+            # infinite modulation loop
+            else:
                 self.disable_burst(ich_trig)
         
         # Otherwise, set up loop directly on signal channel
         else:
             # Check that ramping time is 0
             if tramp > 0:
                 raise VisaError('ramping time not supported for looping sine burst without trigger channel')
```

### Comparing `instrulink-1.0.1/instrulink/rigol_ds1054z.py` & `instrulink-1.0.2/instrulink/rigol_ds1054z.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/si_utils.py` & `instrulink-1.0.2/instrulink/si_utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/sutter_mp285a.py` & `instrulink-1.0.2/instrulink/sutter_mp285a.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/utils.py` & `instrulink-1.0.2/instrulink/utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/visa_instrument.py` & `instrulink-1.0.2/instrulink/visa_instrument.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/instrulink/waveform_generator.py` & `instrulink-1.0.2/instrulink/waveform_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-15 09:26:06
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-04 15:55:47
+# @Last Modified time: 2023-08-07 16:14:09
 
 import abc
 import numpy as np
 
 from .visa_instrument import *
 
 
@@ -231,18 +231,18 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_waveform_amp(self, *args, **kwargs):
         ''' Get the carrier signal amplitude '''
         raise NotImplementedError
     
-    def check_offset(self, offset):
+    @abc.abstractmethod
+    def check_offset(self, offset, *args, **kwargs):
         ''' Check the waveform voltage offset '''
-        if np.absolute(offset) > self.VMAX - self.get_voltage_amp() / 2:
-            raise VisaError(f'|VPP/2| + |Voffset| exceeds {self.VMAX} V')
+        raise NotImplementedError
     
     @abc.abstractmethod
     def set_waveform_offset(self, *args, **kwargs):
         ''' Set the waveform voltage offset (V). '''
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `instrulink-1.0.1/instrulink/wf_utils.py` & `instrulink-1.0.2/instrulink/wf_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-08-15 09:29:37
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-04 16:01:52
+# @Last Modified time: 2023-08-07 14:50:28
 
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
+from scipy.signal import welch
 
+from .logger import logger
 from .si_utils import si_prefixes, si_format
 
 
 def sigmoid_ramp(t, tramp=1, t0=0, dy=0.01):
     ''' 
     Sigmoidal ramp-up function with a specific ramp time and half-ramp point
     
@@ -64,14 +66,16 @@
     :param n: number of points in the ramp vector
     :param tramp: ramp time
     :param t0: half-ramp point
     :param kind: ramp-up function type ('sigmoid' or 'sine')
     :param direction: ramp direction ('up' or 'down')
     :return: time and sigmoid vectors
     '''
+    if tramp <= 0:
+        raise ValueError('tramp must be positive')
     # Get time vector
     t = np.linspace(0, tramp, n) + t0 - tramp / 2
     # Get ramp-up vector
     if kind == 'sigmoid':
         y = sigmoid_ramp(t, t0=t0, tramp=tramp, **kwargs)
     elif kind == 'sine':
         y = sine_ramp(t, t0=t0, tramp=tramp)
@@ -108,23 +112,34 @@
     # Compute characteristic times and total duration 
     tonset = 0
     toffset = tramp + thigh
     ttot = 2 * tramp + thigh + tlow
 
     # Derive number of points in ramp-up (and down) phases
     nramp = int(np.round(n * tramp / ttot)) + 1
+    dt = ttot / (n - 1)
 
     # Get data points for rising and falling edges
-    tr, yr = get_smooth_ramp(
-        nramp, tramp=tramp, t0=tonset + tramp / 2, direction='up', **kwargs)
-    tf, yf = get_smooth_ramp(
-        nramp, tramp=tramp, t0=toffset + tramp / 2, direction='down', **kwargs)
+    try:
+        tr, yr = get_smooth_ramp(
+            nramp, tramp=tramp, t0=tonset + tramp / 2, direction='up', **kwargs)
+        tf, yf = get_smooth_ramp(
+            nramp, tramp=tramp, t0=toffset + tramp / 2, direction='down', **kwargs)
+    except ValueError as e:
+        tr, yr = np.array([0.]), np.array([0.])
+        tf, yf = np.array([0.]), np.array([1.])
+    
+    # Check that ramp time is long enough to be resolved by the requested time step
+    if tr.size > 1:
+        dt = np.diff(tr)[0]
+    else:
+        logger.warning(
+            f'ramping time ({si_format(tramp, 2)}s) is too short to be resolved by the requested time step ({si_format(dt, 2)}s) -> switching to discrete transition')
     
     # Get data points for pulse "high" plateau
-    dt = np.diff(tr)[0]
     th = np.arange(tr[-1] + dt, toffset - dt / 2, dt)
     yh = np.ones(th.size)
 
     # If plateau is empty, remove first ramp-down point
     if th.size == 0:
         tf = tf[1:]
         yf = yf[1:]
@@ -259,44 +274,97 @@
     '''
     dt = np.diff(t)[0]  # s
     freqs = np.fft.rfftfreq(y.size, dt)  # Hz
     ps = np.abs(np.fft.rfft(y))**2  # power
     return freqs, ps
 
 
-def get_continous_intervals(t):
+def get_continous_intervals(t, refdt):
     '''
     Identify intervals of continuity in time vector.
 
     :param t: time vector (s)
+    :param refdt: expected time step in continous time vector (s)
     :return: list of (start, end) pairs for each identified continuous time interval
     '''
+    # Check that time vector contains at least 2 elements
+    if t.size < 2:
+        raise ValueError('Time vector must contain at least 2 elements')
+    # Check that time contains at least 1 continous segment
+    if not np.isclose(np.diff(t), refdt).any():
+        raise ValueError('No continuity detected in time vector')
+    
+    # Identify discontinuities
     dt2 = np.diff(t, 2)
     iscontdt = np.isclose(dt2, 0)
     idiscont = np.where(~iscontdt)[0]
+
+    # Identify index boundaries of continuous intervals
     istarts, iends = [0], []
     for i1, i2 in zip(idiscont[::2], idiscont[1::2]):
         if i2 != i1 + 1:
-            raise ValueError('Discontinuity detected in baseline')
+            raise ValueError(f'invalid discontinuity indices: {i1}, {i2}')
         iends.append(i2)
         istarts.append(i2 + 1)
     iends.append(t.size - 1)
+
+    # Extract corresponding start and end times for each continuity region
     tstarts, tends = t[istarts], t[iends]
+
+    # Return list of (start time, end time) pairs
     return np.array(list(zip(tstarts, tends)))
 
 
-def plot_smoothed_waveform(tenv, yenv, Fdrive, unit='ms', ax=None, **kwargs):
+def get_bounds_per_region(t, y):
+    ''' 
+    Identify ramp-up, plateau, ramp-down, and baseline regions in waveform vector
+    
+    :param t: time vector (s)
+    :param y: waveform vector
+    :return: dictionary of (start, end) pairs for each identified region
+    '''
+    # Check that time step is consistent
+    dt = np.unique(np.round(np.diff(t), 10))
+    if dt.size > 1:
+        raise ValueError(f'Inconsistent time step detected: {dt}')
+    dt = dt[0]
+
+    # Identify ramp-up, plateau, ramp-down, and baseline regions
+    tregions = {
+        'ramp-up': t[np.where(np.diff(y) > 0)],
+        'plateau': t[np.where(y == 1)],
+        'ramp-down': t[np.where(np.diff(y) < 0)],
+        'baseline': t[np.where(y == 0)][1:],
+    }
+
+    # Identify time bounds for each valid region
+    tbounds = {}
+    for key, tvec in tregions.items():
+        try:
+            tbounds[key] = get_continous_intervals(tvec, dt)
+        except ValueError as e:
+            logger.warning(f'{key}: {e}')
+    
+    # Return dictionary of time bounds for each identified region
+    return tbounds
+
+
+def plot_smoothed_waveform(tenv, yenv, Fdrive, unit='ms', ax=None, title=None, 
+                           label=None, mark_regs=True, **kwargs):
     ''' 
     Plot a smoothed waveform from a time vector, an envelope vector and a carrier frequency.
 
     :param t: time vector (s)
     :param yenv: envelope vector
     :param Fdrive: carrier frequency (Hz)
     :param unit: time unit for plotting (default = 'ms')
     :param ax: axis handle (default = None)
+    :param title: title for the plot (default = None)
+    :param label: label for the plotted waveform (default = None)
+    :param mark_regs: flag indicating whether to mark identified regions (default = True)
     :return: figure handle
     '''
     # Get figure and axis handles
     if ax is None:
         fig, ax = plt.subplots()
     else:
         fig = ax.get_figure()
@@ -304,95 +372,129 @@
 
     # Get dense time, waveform and envelope vectors
     tdense, ydense, yenvdense = get_full_waveform(tenv, yenv, Fdrive, **kwargs)
     tfactor = si_prefixes[unit[:-1]]
     tdense /= tfactor
 
     # Plot waveform and its envelope
-    ax.plot(tdense, ydense, label='waveform')
-    ax.plot(tdense, yenvdense, label='envelope')
+    lh, *_ = ax.plot(tdense, yenvdense, label=label if label is not None else 'envelope')
+    ax.plot(tdense, ydense, c=lh.get_color(), alpha=0.5, label='waveform' if label is None else None)
     ax.set_xlabel(f'time ({unit})')
     ax.set_ylabel('amplitude')
     ax.axhline(0, c='k', ls='--')
 
     # Identify ramp-up, plateau, ramp-down, and baseline regions
-    thigh = get_continous_intervals(tdense[np.where(yenvdense == 1)])
-    tlow = get_continous_intervals(tdense[np.where(yenvdense == 0)][1:])
-    assert thigh.shape[0] == tlow.shape[0], 'Number of plateau and baseline windows must be equal'
-    npulses = thigh.shape[0]
-    trampup, trampdown = [], []
-    tref = 0
-    for iw in range(npulses):
-        trampup.append((tref, thigh[iw, 0]))
-        trampdown.append((thigh[iw, 1], tlow[iw, 0]))
-        tref = tlow[iw, 1]
-    trampup, trampdown = np.array(trampup), np.array(trampdown)
-
-    # Add title with breakdown of characteristic waveform phases
-    tramp = np.diff(trampup[0])[0]
-    tplateau = np.diff(thigh[0])[0]
-    tbase = np.diff(tlow[0])[0]
-    title = f'tramp = {tramp:.2f} {unit}, tplateau = {tplateau:.2f} {unit}, tbase = {tbase:.2f} {unit}'
-    if npulses > 1:
-        title = f'{title}, {npulses} pulses'
+    tbounds = get_bounds_per_region(tdense, yenvdense)
+    
+    # Get number of pulses
+    npulses = max(v.shape[0] for v in tbounds.values())
+
+    # Generate title with breakdown of characteristic waveform phases if not provided
+    if title is None:
+        l = []
+        if 'ramp-up' in tbounds:
+            l.append(f'tramp = {np.diff(tbounds["ramp-up"][0])[0]:.2f} {unit}')
+        elif 'ramp-down' in tbounds:
+            l.append(f'tramp = {np.diff(tbounds["ramp-down"][0])[0]:.2f} {unit}')
+        if 'plateau' in tbounds:
+            l.append(f'tplateau = {np.diff(tbounds["plateau"][0])[0]:.2f} {unit}')
+        if 'baseline' in tbounds:
+            l.append(f'tbase = {np.diff(tbounds["baseline"][0])[0]:.2f} {unit}')
+        if npulses > 1:
+            l.append(f'{npulses} pulses')
+        title = ', '.join(l)
+
+    # Add title 
     ax.set_title(title)
 
-    # Mark ramp-up, plateau, ramp-down, and baseline regions
-    for phase, (color, tvec) in {
-        'ramp-up': ('g', trampup), 
-        'plateau': ('k', thigh),
-        'ramp-down': ('r', trampdown),
-        'baseline': ('dimgray', tlow)
-        }.items():
-        for i, (tstart, tend) in enumerate(tvec):
-            ax.axvspan(
-                tstart, tend, color=color, alpha=0.1, label=phase if i == 0 else None)
+    # Mark identified regions, if specified
+    if mark_regs:
+        colors_per_reg = {
+            'ramp-up': 'g',
+            'plateau': 'k',
+            'ramp-down': 'r',
+            'baseline': 'dimgray'
+        }
+        for reg, tvec in tbounds.items():
+            for i, (tstart, tend) in enumerate(tvec):
+                ax.axvspan(
+                    tstart, tend, color=colors_per_reg[reg], alpha=0.1, 
+                    label=reg if i == 0 else None)
 
     # Add legend
     ax.legend()
 
     # Return figure handle
     return fig
 
 
-def plot_waveform_spectrum(tenv, yenv, Fdrive, ax=None, **kwargs):
+def plot_waveform_spectrum(tenv, yenv, Fdrive, ax=None, label=None, mark_freqs=True, 
+                           title=None, get_PRF_val=False, color=None, plot=True, **kwargs):
     ''' 
     Plot a smoothed waveform from a time vector, an envelope vector and a carrier frequency.
 
     :param t: time vector (s)
     :param yenv: envelope vector
     :param Fdrive: carrier frequency (Hz)
     :param ax: axis handle (default = None)
-    :return: figure handle
+    :param label: label for the plotted spectrum (default = None)
+    :param mark_freqs: flag indicating whether to mark carrier and PRF frequencies (default = True)
+    :param title: title for the plot (default = None)
+    :param get_PRF_val: flag indicating whether to compute and return the log-spectrum value (in dB) at the waveform PRF (default = False)
+    :return: figure handle (and log-spectrum value if requested)
     '''
     # Get figure and axis handles
     if ax is None:
         fig, ax = plt.subplots()
     else:
         fig = ax.get_figure()
     sns.despine(ax=ax)
 
+    # Generate label if not provided
+    if label is None:
+        label = 'spectrum'
+    
+    # Add title
+    ax.set_title('waveform spectrum' if title is None else title)
+
     # Get dense time, waveform and envelope vectors
     tdense, ydense, yenvdense = get_full_waveform(tenv, yenv, Fdrive, **kwargs)
 
     # Extract and waveform frequency spectrum
     freqs, ps = get_power_spectrum(tdense, ydense)
     ps_decibel = 10 * np.log10(ps / ps.max())
-    ax.plot(freqs, ps_decibel)
+    if plot:
+        ax.plot(freqs, ps_decibel, label=label, c=color)
     ax.set_xlabel('frequency (Hz)')
     ax.set_ylabel('relative power (dB)')
     ax.set_xscale('log')
 
-    # Mark carrier frequency
-    ax.axvline(Fdrive, c='k', ls='--', label='carrier')
+    # Get number of pulses
+    tbounds = get_bounds_per_region(tdense, yenvdense)
+    nws = {k: v.shape[0] for k, v in tbounds.items()}
+    k, npulses = max(nws, key=nws.get), max(nws.values())
 
-    # In cases of multiple pulses, extract and mark PRF
-    thigh = get_continous_intervals(tdense[np.where(yenvdense == 1)])
-    if thigh.shape[0] > 1:
-        PRF = np.round(1 / (thigh[1, 0] - thigh[0, 0]), 2)  # Hz
-        ax.axvline(PRF, c='r', ls='--', label='PRF')
+    # In cases of multiple pulses, extract PRF and log-spectrum value at PRF
+    if npulses > 1:
+        logger.debug(f'identifying PRF from time difference between first 2 {k} onsets')
+        PRF = np.round(1 / (tbounds[k][1, 0] - tbounds[k][0, 0]), 2)
+        PRF_val = np.interp(PRF, freqs, ps_decibel)
+    else:
+        if get_PRF_val:
+            raise ValueError('Cannot compute PRF log-spectrum value for single-pulse waveform')
+        PRF = None
+
+    # Mark carrier and PRF frequencies, if specified
+    if mark_freqs:
+        ax.axvline(Fdrive, c='k', ls='--', label='carrier')
+        if PRF is not None:
+            ax.axvline(PRF, c='r', ls='--', label='PRF')
     
     # Add legend
-    ax.legend()
+    if plot:
+        ax.legend()
 
-    # Return figure handle
-    return fig
+    # Return figure handle (and log-spectrum value if requested)
+    if get_PRF_val:
+        return fig, PRF_val
+    else:
+        return fig
```

### Comparing `instrulink-1.0.1/instrulink.egg-info/PKG-INFO` & `instrulink-1.0.2/instrulink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instrulink
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package to interface diverse laboratory instruments
 Home-page: https://github.com/tjjlemaire/instrulink
 Author: Theo Lemaire
 Author-email: theo.lemaire1@gmail.com
 License: MIT
 Keywords: laboratory instrument interface python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instrulink-1.0.1/instrulink.egg-info/SOURCES.txt` & `instrulink-1.0.2/instrulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_33500b.py` & `instrulink-1.0.2/scripts/test_33500b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_camera.py` & `instrulink-1.0.2/scripts/test_camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_e5061b.py` & `instrulink-1.0.2/scripts/test_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_generator.py` & `instrulink-1.0.2/scripts/test_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-15 15:44:20
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-04 16:05:31
+# @Last Modified time: 2023-08-08 11:51:23
 
 ''' Initiate test sequence with Rigol waveform generator. '''
 
 import logging
 import time
 import argparse
 
 from instrulink import logger, grab_generator, VisaError
 
 logger.setLevel(logging.INFO)
 
 # Default waveform parameters
 Fdrive = 1e4  # carrier frequency (Hz)
 Vpp = 0.5  # signal amplitude (Vpp)
-tstim = 100e-3  # burst duration (s)
+tstim = 200e-3  # burst duration (s)
 PRF = 100.  # burst internal PRF (Hz)
 DC = 50.  # burst internal duty cycle (%)
 tramp = 0.  # nominal pulse ramp up time (s)
 
 # Parse command line arguments
 parser = argparse.ArgumentParser()
 parser.add_argument(
     '--icarrier', type=int, default=2, choices=(1, 2), help='Carrier channel index')
 parser.add_argument(
     '--igating', type=int, default=1, choices=(1, 2), help='Gating channel index')
 parser.add_argument(
+    '--gtype', default='trig', choices=('mod', 'trig'), 
+    help='Gating type, i.e. "mod" for modulation or "trig" for trigger (only if modulation period is specified)')
+parser.add_argument(
     '-s', '--source', type=str, default='int', choices=('int', 'man'), help='Trigger source (only if modulation period is specified)')
 parser.add_argument(
     '-f', '--frequency', type=float, default=Fdrive, help='Carrier frequency (Hz)')
 parser.add_argument(
     '--vpp', type=float, default=Vpp, help='Signal amplitude (Vpp)')
 parser.add_argument(
     '--tstim', type=float, default=tstim, help='Burst duration (s)')
@@ -42,15 +45,16 @@
     '--DC', type=float, default=DC, help='Burst internal duty cycle (%)')
 parser.add_argument(
     '--tramp', type=float, default=tramp, help='Nominal pulse ramp up time (ms)')
 parser.add_argument(
     '-T', type=float, default=-1., help='Modulation period (s, defaults to -1, i.e. continous looping)')
 args = parser.parse_args()
 ich_carrier = args.icarrier  # carrier channel
-ich_mod = args.igating  # gating channel
+ich_gate = args.igating  # gating channel
+gtype = args.gtype  # gating type
 trigger_source = args.source.upper()  # trigger source
 Fdrive = args.frequency  # carrier frequency (Hz)
 Vpp = args.vpp  # signal amplitude (Vpp)
 tstim = args.tstim  # burst duration (s)
 PRF = args.PRF  # burst internal PRF (Hz)
 DC = args.DC  # burst internal duty cycle (%)
 tramp = args.tramp * 1e-3  # nominal pulse ramp up time (s)
@@ -58,23 +62,20 @@
 
 try:
     # If modulation period is not specified
     if mod_T < 0:
         # Set modulation period to None
         mod_T = None
         # If manual trigger, check that signal and gating channels are different
-        if trigger_source == 'MAN' and ich_carrier == ich_mod:
+        if trigger_source == 'MAN' and ich_carrier == ich_gate:
             raise ValueError('Signal and gating channels must be different for single burst trigger')
     # Otherwise
     else:
-        # Check that trigger source is internal
-        if trigger_source != 'INT':
-            raise ValueError('Trigger source must be internal when modulation period is specified')
         # Check that signal and gating channels are different
-        if ich_carrier == ich_mod:
+        if ich_carrier == ich_gate:
             raise ValueError('Signal and gating channels must be different when modulation period is specified')
 except ValueError as e:
     logger.error(e)
     quit()
 
 try:
     # Grab function generator
@@ -82,42 +83,51 @@
 
     # If modulation period is not specified
     if mod_T is None:
         # If internal trigger is used, apply continous looping
         if trigger_source == 'INT':
             tburst = .01 * DC / PRF   # burst duration = pulse duration (s)
             wg.set_looping_sine_burst(
-                ich_carrier, Fdrive, Vpp=Vpp, ncycles=tburst * Fdrive, PRF=PRF, 
-                tramp=tramp, ich_trig=None if ich_mod == ich_carrier else ich_mod)
+                ich_carrier, Fdrive, Vpp=Vpp, ncycles=tburst * Fdrive, 
+                PRF=PRF, tramp=tramp, 
+                ich_trig=None if ich_gate == ich_carrier else ich_gate,
+                gate_type=gtype,
+            )
         
         # If manual trigger is used, apply single burst
         else:
             wg.set_gated_sine_burst(
                 Fdrive, Vpp, tstim, PRF, DC,
-                ich_carrier=ich_carrier, ich_mod=ich_mod,
-                trig_source=trigger_source
+                ich_carrier=ich_carrier, ich_gate=ich_gate,
+                trig_source=trigger_source,
+                tramp=tramp,
+                gate_type=gtype,
             )
             time.sleep(2)
-            wg.trigger_channel(ich_mod)
+            wg.trigger_channel(ich_gate)
     
     # If modulation period is specified
     else:
-        # Apply signal on signal channel gated/modulated by other channel
-        if tramp == 0:
-            wg.set_gated_sine_burst(
-                Fdrive, Vpp, tstim, PRF, DC,
-                ich_carrier=ich_carrier, ich_gate=ich_mod,
-                trig_source=trigger_source, T=mod_T
-            )
-        else:
-            wg.set_modulated_sine_burst(
-                Fdrive, Vpp, tstim, PRF, DC, tramp=tramp,
-                ich_carrier=ich_carrier, ich_mod=ich_mod,
-                trig_source=trigger_source, T=mod_T
-            )
+        # Apply signal on signal channel triggered/modulated by other channel
+        wg.set_gated_sine_burst(
+            Fdrive, Vpp, tstim, PRF, DC,
+            tramp=tramp,
+            ich_carrier=ich_carrier, ich_gate=ich_gate,
+            trig_source=trigger_source, T=mod_T,
+            gate_type=gtype
+        )
+        
+        # Manual trigger: set up infinite trigger loop at specified periodicity
+        if trigger_source == 'MAN':
+            while True:
+                wg.trigger_channel(ich_gate)
+                time.sleep(mod_T)
 
     # Unlock front panel
     wg.unlock_front_panel()
 
+    # Close connection
+    wg.disconnect()
+
 except VisaError as e:
     logger.error(e)
     quit()
```

### Comparing `instrulink-1.0.1/scripts/test_manipulator.py` & `instrulink-1.0.2/scripts/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_nidaq.py` & `instrulink-1.0.2/scripts/test_nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/scripts/test_scope.py` & `instrulink-1.0.2/scripts/test_scope.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.1/setup.py` & `instrulink-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Email: theo.lemaire@epfl.ch
 # @Date:   2017-06-13 09:40:02
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-04 16:54:26
+# @Last Modified time: 2023-08-08 16:18:18
 
 import os
 from setuptools import setup
 
 readme_file = 'README.md'
 req_file = 'requirements.txt'
 
@@ -21,15 +21,15 @@
         return f.readlines()
 
 def getFiles(path):
     return [f'{path}/{x}' for x in os.listdir(path)]
 
 setup(
     name='instrulink',
-    version='1.0.1',
+    version='1.0.2',
     description='Python package to interface diverse laboratory instruments',
     long_description_content_type='text/markdown',
     long_description=readme(),
     url='https://github.com/tjjlemaire/instrulink',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
```

