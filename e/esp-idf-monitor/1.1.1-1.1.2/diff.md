# Comparing `tmp/esp-idf-monitor-1.1.1.tar.gz` & `tmp/esp-idf-monitor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-rhl95jpb/esp-idf-monitor-1.1.1.tar", last modified: Tue Jun 20 14:17:18 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-fw1bt1vc/esp-idf-monitor-1.1.2.tar", last modified: Tue Aug  8 13:30:32 2023, max compression
```

## Comparing `esp-idf-monitor-1.1.1.tar` & `esp-idf-monitor-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/ansi_color_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/chip_specific_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/coredump.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/gdbhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/line_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/pc_address_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/rom_elf_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/gdb_panic_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17723 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/idf_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/ansi_color_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/chip_specific_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/console_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/console_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/coredump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/gdbhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/line_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/pc_address_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/rom_elf_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/serial_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/base/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/gdb_panic_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18870 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/esp_idf_monitor/idf_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:30:32.000000 esp-idf-monitor-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-08 13:30:13.000000 esp-idf-monitor-1.1.2/setup.py
```

### Comparing `esp-idf-monitor-1.1.1/LICENSE` & `esp-idf-monitor-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/PKG-INFO` & `esp-idf-monitor-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.1.1/README.md` & `esp-idf-monitor-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/ansi_color_converter.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/ansi_color_converter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/argument_parser.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/argument_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # SPDX-FileCopyrightText: 2015-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import os
+import sys
 
 from .constants import (DEFAULT_PRINT_FILTER, DEFAULT_TOOLCHAIN_PREFIX,
                         PANIC_DECODE_BACKTRACE, PANIC_DECODE_DISABLE)
 from .coredump import COREDUMP_DECODE_DISABLE, COREDUMP_DECODE_INFO
 
 
 def get_parser():  # type: () -> argparse.ArgumentParser
     parser = argparse.ArgumentParser('idf_monitor - a serial output monitor for esp-idf')
 
     parser.add_argument(
         '--port', '-p',
-        help='Serial port device',
-        default=os.environ.get('ESPTOOL_PORT', '/dev/ttyUSB0')
+        help='Serial port device. If not set, a connected port will be used.' +
+        (' Defaults to `/dev/ttyUSB0` if connected.' if sys.platform == 'linux' else ''),
+        default=os.environ.get('ESPTOOL_PORT', None)
     )
 
     parser.add_argument(
         '--no-reset',
         help='Do not reset the chip on monitor startup',
         action='store_true'
     )
```

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/chip_specific_config.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/chip_specific_config.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_parser.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/console_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_reader.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/console_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/constants.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/constants.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/coredump.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/coredump.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/gdbhelper.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/gdbhelper.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/line_matcher.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/line_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/logger.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/logger.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/output_helpers.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/output_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/pc_address_matcher.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/rom_elf_getter.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/rom_elf_getter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_handler.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/serial_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self.target = target
         self._force_line_print = force_line_print
         self.start_cmd_sent = start_cmd_sent
         self.serial_instance = serial_instance
         self.encrypted = encrypted
         self.reset = reset
         self.elf_file = elf_file
+        self.decode_error_cnt = 0
 
     def splitdata(self, data):  # type: (bytes) -> List[bytes]
         """
         Split data into lines, while keeping newlines, and move unfinished line for future processing
         """
         # if data is empty fallback to empty string for easier concatenation with last line
         sp = data.splitlines(keepends=True) or [b'']
@@ -106,17 +107,26 @@
         for line in sp:
             line_strip = line.strip()
             if self._serial_check_exit and line_strip == console_parser.exit_key.encode('latin-1'):
                 raise SerialStopException()
             if gdb_helper:
                 self.check_panic_decode_trigger(line_strip, gdb_helper)
             with coredump.check(line_strip):
-                if self._force_line_print or line_matcher.match(line_strip.decode(errors='ignore')):
+                try:
+                    decoded_line = line.decode()
+                    self.decode_error_cnt = 0
+                except UnicodeDecodeError:
+                    decoded_line = line_strip.decode(errors='ignore')
+                    self.decode_error_cnt += 1
+                    if self.decode_error_cnt >= 3:
+                        yellow_print('Multiple decode errors occured: Try checking the baud rate and XTAL frequency setting in menuconfig')
+                        self.decode_error_cnt = 0
+                if self._force_line_print or line_matcher.match(decoded_line):
                     self.logger.print(line)
-                    self.compare_elf_sha256(line.decode(errors='ignore'))
+                    self.compare_elf_sha256(decoded_line)
                     self.logger.handle_possible_pc_address_in_line(line_strip)
             check_gdb_stub_and_run(line_strip)
             self._force_line_print = False
 
         if self._last_line_part.startswith(CONSOLE_STATUS_QUERY):
             self.logger.print(CONSOLE_STATUS_QUERY)
             self._last_line_part = self._last_line_part[len(CONSOLE_STATUS_QUERY):]
```

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_reader.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/serial_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import queue  # noqa: F401
 import subprocess  # noqa: F401
 import sys
 import time
 
 import serial
+from serial.tools import list_ports
 
 from .constants import (CHECK_ALIVE_FLAG_TIMEOUT, MINIMAL_EN_LOW_DELAY,
                         RECONNECT_DELAY, TAG_SERIAL)
 from .output_helpers import red_print, yellow_print
 from .stoppable_thread import StoppableThread
 
 
@@ -46,15 +47,21 @@
             high = False
             low = True
 
             self.serial.dtr = low      # Non reset state
             self.serial.rts = high     # IO0=HIGH
             self.serial.dtr = self.serial.dtr   # usbser.sys workaround
             # Current state not reset the target!
-            self.serial.open()
+            try:
+                self.serial.open()
+            except serial.serialutil.SerialException:
+                # if connection to port fails suggest other available ports
+                port_list = '\n'.join([p.device for p in list_ports.comports()])
+                yellow_print(f'Connection to {self.serial.portstr} failed. Available ports:\n{port_list}')
+                return
             if not self.gdb_exit and self.reset:
                 self.serial.dtr = high     # Set dtr to reset state (affected by rts)
                 self.serial.rts = low      # Set rts/dtr to the reset state
                 self.serial.dtr = self.serial.dtr   # usbser.sys workaround
 
                 # Add a delay to meet the requirements of minimal EN low time (2ms for ESP32-C3)
                 time.sleep(MINIMAL_EN_LOW_DELAY)
```

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/stoppable_thread.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/base/web_socket_client.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/base/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/gdb_panic_server.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/gdb_panic_server.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor/idf_monitor.py` & `esp-idf-monitor-1.1.2/esp_idf_monitor/idf_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 import subprocess
 import sys
 import threading
 import time
 from typing import Any, List, Optional, Type, Union  # noqa: F401
 
 import serial
-import serial.tools.list_ports
-from serial.tools import miniterm
+from serial.tools import list_ports, miniterm
 
 # Windows console stuff
 from esp_idf_monitor.base.ansi_color_converter import get_ansi_converter
 from esp_idf_monitor.base.argument_parser import get_parser
 from esp_idf_monitor.base.console_parser import ConsoleParser
 from esp_idf_monitor.base.console_reader import ConsoleReader
 from esp_idf_monitor.base.constants import (CTRL_C, CTRL_H,
@@ -244,25 +243,33 @@
 class SerialMonitor(Monitor):
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:  # type: ignore
         """ Use 'with self' to temporarily disable monitoring behaviour """
         self.console_reader.start()
         if self.elf_exists:
             self.serial_reader.gdb_exit = self.gdb_helper.gdb_exit  # type: ignore # write gdb_exit flag
         self.serial_reader.start()
+        self.timeout_cnt = 0
 
     def _pre_start(self) -> None:
         super()._pre_start()
         if self.elf_exists:
             self.gdb_helper.gdb_exit = False  # type: ignore
         self.serial_handler.start_cmd_sent = False
 
     def serial_write(self, *args: str, **kwargs: str) -> None:
         self.serial: serial.Serial
         try:
             self.serial.write(*args, **kwargs)
+            self.timeout_cnt = 0
+        except serial.SerialTimeoutException:
+            self.timeout_cnt += 1
+            if self.timeout_cnt >= 3:
+                yellow_print('Writing to serial is timing out. Please make sure that your application supports '
+                             'an interactive console and that you have picked the correct console for serial communication.')
+                self.timeout_cnt = 0
         except serial.SerialException:
             pass  # this shouldn't happen, but sometimes port has closed in serial thread
         except UnicodeEncodeError:
             pass  # this can happen if a non-ascii character was passed, ignoring
 
     def check_gdb_stub_and_run(self, line: bytes) -> None:  # type: ignore # The base class one is a None value
         if self.gdb_helper and self.gdb_helper.check_gdb_stub_trigger(line):
@@ -300,14 +307,29 @@
     parser = get_parser()
     args = parser.parse_args()
 
     # The port name is changed in cases described in the following lines. Use a local argument and
     # avoid the modification of args.port.
     port = args.port
 
+    # if no port was set, detect connected ports and use one of them
+    if port is None:
+        try:
+            port_list = list_ports.comports()
+            port = port_list[-1].device
+            # keep the `/dev/ttyUSB0` default port on linux if connected
+            # TODO: This can be removed in next major release
+            if sys.platform == 'linux':
+                for p in port_list:
+                    if p.device == '/dev/ttyUSB0':
+                        port = p.device
+                        break
+            yellow_print(f'--- Using autodetected port {port}')
+        except IndexError:
+            sys.exit('No serial ports detected.')
     # GDB uses CreateFile to open COM port, which requires the COM name to be r'\\.\COMx' if the COM
     # number is larger than 10
     if os.name == 'nt' and port.startswith('COM'):
         port = port.replace('COM', r'\\.\COM')
         yellow_print('--- WARNING: GDB cannot open serial ports accessed as COMx')
         yellow_print('--- Using %s instead...' % port)
     elif port.startswith('/dev/tty.') and sys.platform == 'darwin':
@@ -345,14 +367,15 @@
             serial_instance = None
             cls = LinuxMonitor
             yellow_print('--- idf_monitor on linux ---')
         else:
             serial_instance = serial.serial_for_url(port, args.baud, do_not_open=True)
             serial_instance.dtr = False
             serial_instance.rts = False
+            serial_instance.write_timeout = 0.3
 
             # Pass the actual used port to callee of idf_monitor (e.g. idf.py/cmake) through `ESPPORT` environment
             # variable.
             # Note that the port must be original port argument without any replacement done in IDF Monitor (idf.py
             # has a check for this).
             # To make sure the key as well as the value are str type, by the requirements of subprocess
             espport_val = str(args.port)
```

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/PKG-INFO` & `esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/SOURCES.txt` & `esp-idf-monitor-1.1.2/esp_idf_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.1/setup.py` & `esp-idf-monitor-1.1.2/setup.py`

 * *Files identical despite different names*

