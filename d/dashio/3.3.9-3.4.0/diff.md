# Comparing `tmp/dashio-3.3.9.tar.gz` & `tmp/dashio-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.9.tar", last modified: Tue Jul 25 06:05:07 2023, max compression
+gzip compressed data, was "dashio-3.4.0.tar", last modified: Tue Aug  8 05:15:37 2023, max compression
```

## Comparing `dashio-3.3.9.tar` & `dashio-3.4.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 06:04:55.000000 dashio-3.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-25 06:05:07.595159 dashio-3.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-07-25 06:04:55.000000 dashio-3.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.579159 dashio-3.3.9/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.583159 dashio-3.3.9/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.591159 dashio-3.3.9/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.583159 dashio-3.3.9/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 06:04:55.000000 dashio-3.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 06:05:07.599159 dashio-3.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-25 06:04:55.000000 dashio-3.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_zqmconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-25 06:04:55.000000 dashio-3.3.9/utilities/c64_decode
--rwxr-xr-x   0 runner    (1001) docker     (123)     1726 2023-07-25 06:04:55.000000 dashio-3.3.9/utilities/c64_encode
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.156818 dashio-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 05:15:25.000000 dashio-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-08 05:15:37.156818 dashio-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-08-08 05:15:25.000000 dashio-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.128817 dashio-3.4.0/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.132817 dashio-3.4.0/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.144817 dashio-3.4.0/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-08 05:15:25.000000 dashio-3.4.0/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.128817 dashio-3.4.0/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-08 05:15:37.000000 dashio-3.4.0/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-08 05:15:37.000000 dashio-3.4.0/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:15:37.000000 dashio-3.4.0/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:15:36.000000 dashio-3.4.0/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 05:15:37.000000 dashio-3.4.0/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 05:15:37.000000 dashio-3.4.0/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 05:15:25.000000 dashio-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-08 05:15:37.156818 dashio-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 05:15:25.000000 dashio-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.152818 dashio-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:25.000000 dashio-3.4.0/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:15:37.156818 dashio-3.4.0/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-08-08 05:15:25.000000 dashio-3.4.0/utilities/c64_decode
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1726 2023-08-08 05:15:25.000000 dashio-3.4.0/utilities/c64_encode
```

### Comparing `dashio-3.3.9/LICENSE` & `dashio-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/PKG-INFO` & `dashio-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.9
+Version: 3.4.0
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6.0
+Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
```

### Comparing `dashio-3.3.9/README.md` & `dashio-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/__init__.py` & `dashio-3.4.0/dashio/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/action_station.py` & `dashio-3.4.0/dashio/action_station.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import logging
 import threading
 import time
 import sys
 import shortuuid
 import zmq
 
-
-from .constants import CONNECTION_PUB_URL, MEMORY_REQ_URL, TASK_PULL
+from . import ip
+from .constants import CONNECTION_PUB_URL, TASK_MEMORY_PORT_OFFSET, TASK_PULL_PORT_OFFSET, TASK_CONN_PORT_OFFSET, TCP_URL
 from .action_station_services.task_service import TaskService
 from .action_station_services.timer_service import TimerService, make_timer_config
 from .action_station_services.as_servicel import make_test_config
 from .action_station_services.modbus_service import ModbusService, make_modbus_config
 from .action_station_services.clock_servicel import ClockService, make_clock_config
 from .load_config import CONTROL_INSTANCE_DICT, CONFIG_INSTANCE_DICT, decode_cfg64, encode_cfg64
 
@@ -116,15 +116,15 @@
             if isinstance(control_list, list):
                 for control in control_list:
                     key = f"{control_type}\t{control['controlID']}"
                     if self.device.is_control_loaded(control_type, control['controlID']):
                         modified = True
                         logging.debug("Deleting layouts: %s, %s", control_type, control['controlID'])
                         try:
-                            self.device.controls_dict[key].del_configs_columnar()
+                            self.device.controls_dict[key].del_config()
                         except KeyError:
                             logging.debug("Error deleting layout: %s, %s", control_type, control['controlID'])
         return modified
 
     def _update_gui_controls(self, cfg_dict: dict):
         new_cfg_dict = {}
         new_cfg_dict["CFG"] = self.device._cfg
@@ -134,15 +134,15 @@
             if isinstance(control_list, list):
                 for control in control_list:
                     key = f"{control_type}\t{control['controlID']}"
                     if self.device.is_control_loaded(control_type, control['controlID']):
                         # load new config into control
                         logging.debug("Adding layouts: %s, %s", control_type, control['controlID'])
                         cfg = CONFIG_INSTANCE_DICT[control_type].from_dict(control)
-                        self.device.controls_dict[key].add_config_columnar(cfg)
+                        self.device.controls_dict[key].add_config(cfg)
                         modified = True
                         if key in added_control_ids:
                             # Add the next config to the control
                             new_cfg_dict[control_type].append(control)
                     else:
                         # Create a new control.
                         g_control = CONTROL_INSTANCE_DICT[control_type].from_cfg_dict(control)
@@ -216,19 +216,19 @@
             'msgType': 'disconnect',
             'deviceID': device_id
         }
         logging.debug("AS DISCONNECT: %s", device_id)
         self.tx_zmq_pub.send_multipart([b"COMMAND", json.dumps(msg_dict).encode()])
 
     def _start_control(self, t_object: dict):
-        if t_object['uuid'] in self.thread_dicts:
-            self.thread_dicts[t_object['uuid']].close()
+        if t_object["uuid"] in self.thread_dicts:
+            self.thread_dicts[t_object["uuid"]].close()
             time.sleep(0.1)
-        logging.debug("INIT TASK %s", t_object['uuid'])
-        self.thread_dicts[t_object['uuid']] = self.service_objects_defs[t_object['objectType']](self.device_id, self.zmq_service_uuid, t_object, self.context)
+        logging.debug("INIT TASK %s", t_object["uuid"])
+        self.thread_dicts[t_object['uuid']] = self.service_objects_defs[t_object['objectType']](self.device_id, self.local_port, t_object, self.context)
         return True
 
     def _list_command(self, data):
         j_object_list = []
         for j_object in self.configured_services.values():
             action_pair = {
                 "name": j_object['name'],
@@ -236,35 +236,36 @@
                 "objectType": j_object['objectType'],
                 "revision": j_object.get('revision', 1)
             }
             j_object_list.append(action_pair)
         # TODO delete this for loop
         for j_object in self.configs.values():
             action_pair = {
-                "name": j_object['name'],
-                "uuid": j_object['uuid'],
-                "objectType": j_object['objectType'],
-                "revision": j_object.get('revision', 1)
+                "name": j_object.name,
+                "uuid": j_object.uuid,
+                "objectType": j_object.objectType,
+                "revision": j_object.revision
             }
             j_object_list.append(action_pair)
         result = {
             'objectType': "LIST_RESULT",
             'list': j_object_list
         }
         reply = f"\t{self.device_id}\tACTN\tLIST\t{json.dumps(result)}\n"
         return reply
 
     def _list_configs_command(self, data):
-        j_object_list = []
-        for j_object in self.configs.values():
-            if j_object['objectType'] == "CONFIG":
-                j_object_list.append(j_object)
+        config_list = []
+        for config in self.configs.values():
+            if config.objectType == "CONFIG":
+                config_list.append(config.dict())
+                logging.debug("Conf: %s", config.objectName)
         result = {
             'objectType': "LIST_RESULT",
-            'list': j_object_list
+            'list': config_list
         }
         reply = f"\t{self.device_id}\tACTN\tLIST_CONFIGS\t{json.dumps(result)}\n"
         return reply
 
     def _list_tasks_command(self, data):
         j_object_list = []
         for j_object in self.configured_services.values():
@@ -352,24 +353,28 @@
     def __init__(self, device, max_actions=100, number_timers=10, memory_storage_size=0, context: zmq.Context = None):
         """Action Station"""
         threading.Thread.__init__(self, daemon=True)
         self.context = context or zmq.Context.instance()
         self.device_id = device.device_id
         self.device = device
         self._json_filename = f"{self.device_id}_Actions.json"
-
+        self.local_port = 7654
         self.configured_services = {}
         self.configs = {}
         self.memory_tasks = {}
         self.remote_device_ids = []
         self.connections_list = []
         self._action_station_layout = None
         self.action_station_dict = self.load_action(self._json_filename)
         self.max_actions = max_actions
 
+        while ip.is_port_in_use("127.0.0.1", self.local_port):
+            # increment port until we find one that is free.
+            self.local_port += 1
+
         self.service_objects_defs = {
             'TASK': TaskService,
             'TMR': TimerService,
             'MDBS': ModbusService,
             'CLK': ClockService
         }
         self.thread_dicts = {}  # For the Instantiated control and task objects.
@@ -383,19 +388,19 @@
             "UPDATE": self._update_command,
             "RUN": self._run_command
         }
         timer_cfg = make_timer_config(number_timers)
         test_cfg = make_test_config(1)
         modbus_cfg = make_modbus_config(1)
         clock_cfg = make_clock_config(1)
-        self.configs[timer_cfg['uuid']] = timer_cfg
-        self.configs[test_cfg['uuid']] = test_cfg
-        self.configs[modbus_cfg['uuid']] = modbus_cfg
-        self.configs[clock_cfg['uuid']] = clock_cfg
-        self.zmq_service_uuid = "SRVC:" + shortuuid.uuid()
+        self.configs[timer_cfg.uuid] = timer_cfg
+        self.configs[test_cfg.uuid] = test_cfg
+        self.configs[modbus_cfg.uuid] = modbus_cfg
+        self.configs[clock_cfg.uuid] = clock_cfg
+        # self.zmq_service_uuid = "SRVC:" + shortuuid.uuid()
         if not self.action_station_dict:
             self.zmq_connection_uuid = "ACTN:" + shortuuid.uuid()
             self.action_station_dict['actionStationID'] = self.zmq_connection_uuid
             self.action_station_dict['services'] = self.configured_services
             self.action_station_dict['tasksMemory'] = self.memory_tasks
         else:
             try:
@@ -407,16 +412,15 @@
 
         self.running = True
         self.start()
 
     def run(self):
 
         self.zmq_service_pub = self.context.socket(zmq.PUB)
-
-        self.zmq_service_pub.bind(CONNECTION_PUB_URL.format(id=self.zmq_service_uuid))
+        self.zmq_service_pub.bind(TCP_URL.format(port=self.local_port + TASK_CONN_PORT_OFFSET))
 
         self.tx_zmq_pub = self.context.socket(zmq.PUB)
         self.tx_zmq_pub.bind(CONNECTION_PUB_URL.format(id=self.zmq_connection_uuid))
 
         self.device_zmq_sub = self.context.socket(zmq.SUB)
         #  Subscribe on ALL, and my connection
         self.device_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "ALL")
@@ -425,18 +429,18 @@
         #  rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "ANNOUNCE")
         self.connection_zmq_sub = self.context.socket(zmq.SUB)
         self.connection_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "COMMAND")
         self.connection_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "\t")  # - All valid DashIO messaging
 
         #  Socket to receive messages on
         task_receiver = self.context.socket(zmq.PULL)
-        task_receiver.bind(TASK_PULL.format(id=self.zmq_service_uuid))
+        task_receiver.bind(TCP_URL.format(port=self.local_port + TASK_PULL_PORT_OFFSET))
 
         memory_socket = self.context.socket(zmq.REP)
-        memory_socket.bind(MEMORY_REQ_URL.format(id=self.device_id))
+        memory_socket.bind(TCP_URL.format(port=self.local_port + TASK_MEMORY_PORT_OFFSET))
 
         poller = zmq.Poller()
         poller.register(self.device_zmq_sub, zmq.POLLIN)
         poller.register(self.connection_zmq_sub, zmq.POLLIN)
         poller.register(task_receiver, zmq.POLLIN)
         poller.register(memory_socket, zmq.POLLIN)
 
@@ -466,15 +470,16 @@
                 # logging.debug("ActionStation Connection RX:\n%s, %s", msg_from, msg.decode())
                 if msg[0] == b"COMMAND":
                     self._rx_command(msg_from)
                     continue
                 if msg.startswith(f"\t{self.device_id}\tACTN".encode()):
                     self._service_actn_commands(msg, msg_from)
                     continue
-                self.zmq_service_pub.send_multipart([msg, msg_from])
+                for sub_msg in msg.split(b'\n'):
+                    self.zmq_service_pub.send_multipart([sub_msg, msg_from])
 
             if task_receiver in socks:
                 msg_to, msg = task_receiver.recv_multipart()
                 self.tx_zmq_pub.send_multipart([msg_to, msg])
                 if msg_to == b'COMMAND':
                     msg_dict = json.loads(msg)
                     if msg_dict['msgType'] == 'connect':
```

### Comparing `dashio-3.3.9/dashio/action_station_services/as_servicel.py` & `dashio-3.4.0/dashio/action_station_services/as_servicel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,108 @@
 """Memory Class"""
 import logging
 import threading
 import zmq
+import shortuuid
 
-from ..constants import CONNECTION_PUB_URL, TASK_PULL
+from ..constants import TASK_CONN_PORT_OFFSET, TASK_PULL_PORT_OFFSET, TCP_URL
 from .action_station_service_config import (ActionServiceCFG,
                                             BoolParameterSpec,
                                             FloatParameterSpec,
                                             IntParameterSpec,
                                             ListParameterSpec,
                                             SelectorParameterSpec,
                                             SliderParameterSpec,
                                             StringParameterSpec)
 
 
 def make_test_config(num_tests):
     """Make a timer config"""
     provisioning_list = [
-        SelectorParameterSpec("A Selector", ["Selection 1", "Selection2", "Selection3"], "Selection 1"),
-        IntParameterSpec("An Int", 0, 100, "jiggers", 42),
-        StringParameterSpec("A String", "Little Bo Peep...."),
-        FloatParameterSpec("A Float", 2.71828, 299792458.0, "jiffies", 1.4142),
-        BoolParameterSpec("A bool", True),
-        SliderParameterSpec("A Slider", 1.0, 10.0, 1.0, 5.0),
+        SelectorParameterSpec(name="A Selector", selection=["Selection1", "Selection2", "Selection3"], value="Selection1", uuid=shortuuid.uuid()),
+        IntParameterSpec(name="An Int", min=0, max=100, units="jiggers", value=42, uuid=shortuuid.uuid()),
+        StringParameterSpec(name="A String", value="Little Bo Peep....", uuid=shortuuid.uuid()),
+        FloatParameterSpec(name="A Float", min=2.71828, max=299792458.0, units="jiffies", value=1.4142, uuid=shortuuid.uuid()),
+        BoolParameterSpec(name="A bool", value=True, uuid=shortuuid.uuid()),
+        SliderParameterSpec(name="A Slider", min=1.0, max=10.0, step=1.0, value=5.0, uuid=shortuuid.uuid()),
         ListParameterSpec(
-            "List of Things",
-            "Create a list",
-            [
+            name="List of Things",
+            text="Create a list",
+            uuid=shortuuid.uuid(),
+            param_list=[
                 IntParameterSpec(
-                    "Add a uint_16",
-                    0,
-                    65535,
-                    "",
-                    0
+                    name="Add a uint_16",
+                    min=0,
+                    max=65535,
+                    units="",
+                    value=0,
+                    uuid=shortuuid.uuid()
                 ),
                 SelectorParameterSpec(
-                    "Choose a thing", [
+                    name="Choose a thing",
+                    selection=[
                         "Thing One",
                         "Thing Two",
                         "The Lorax",
                         "The Grinch",
                         "Horton",
                         "Sam-I-Am",
                         "Thidwick",
                         "Yertle the Turtle",
                         "Lord Droon"
                     ],
-                    "Horton",
+                    value="Horton",
+                    uuid=shortuuid.uuid()
                 )
             ]
         )
 
     ]
     parameter_list = []
 
     timer_cfg = ActionServiceCFG(
-        "TST",
-        "Test",
-        "Test with all provisioning types",
-        "TST",
-        num_tests,
-        True,
-        True,
-        provisioning_list,
-        parameter_list
+        objectName="TST",
+        name="Test",
+        text="Test with all provisioning types",
+        uuid=shortuuid.uuid(),
+        controlID="TST",
+        numAvail=num_tests,
+        isTrigger=True,
+        isIO=True,
+        provisioning=provisioning_list,
+        parameters=parameter_list
         #  parameter_list_out
     )
-    return timer_cfg.__json__()
+    return timer_cfg
 
 
 class ASService(threading.Thread):
     """Action Station Template Class"""
 
     def send_message(self, out_message=""):
         """Send the message"""
         self.task_sender.send_multipart([b"ALL", out_message.encode('utf-8')])
 
     def close(self):
         """Close the thread"""
         self.running = False
 
-    def __init__(self, device_id: str, action_station_id: str, control_config_dict: dict, context: zmq.Context) -> None:
+    def __init__(self, device_id: str, local_port: int, control_config_dict: dict, context: zmq.Context) -> None:
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context
         self.running = True
 
         self.control_id = control_config_dict['controlID']
         self.name = control_config_dict['name']
         self.control_type = control_config_dict['objectType']
         # provision_list = control_config_dict['provisioning']
 
-        self.sub_url = CONNECTION_PUB_URL.format(id=action_station_id)
-
-        self.push_url = TASK_PULL.format(id=action_station_id)
+        self.sub_url = TCP_URL.format(port=local_port + TASK_CONN_PORT_OFFSET)
+        self.push_url = TCP_URL.format(port=local_port + + TASK_PULL_PORT_OFFSET)
         self.task_sender = self.context.socket(zmq.PUSH)
         self.task_sender.connect(self.push_url)
 
         self.control_msg = f"\t{device_id}\t{self.control_type}\t{self.control_id}"
         logging.debug("Init Class: %s, %s", self.control_type, self.name)
 
         self.start()
```

### Comparing `dashio-3.3.9/dashio/action_station_services/clock_servicel.py` & `dashio-3.4.0/dashio/action_station_services/clock_servicel.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,45 +20,46 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import datetime
 import logging
 import threading
 import time
-
+import shortuuid
 import zmq
 from astral import LocationInfo
 from astral.sun import sun
 from dateutil import tz
 
-from ..constants import TASK_PULL, CONNECTION_PUB_URL
+from ..constants import TASK_PULL_PORT_OFFSET, TASK_CONN_PORT_OFFSET, TCP_URL
 from .action_station_service_config import ActionServiceCFG, FloatParameterSpec
 
 
 def make_clock_config(num_tests):
     """Make a timer config"""
     provisioning_list = [
-        FloatParameterSpec("Latitude", -90.0, 90.0, "degs", -43.5256),
-        FloatParameterSpec("Longitude", -180.0, 180.0, "degs", 172.6398),
+        FloatParameterSpec(name="Latitude", min=-90.0, max=90.0, units="degs", value=-43.5256, uuid=shortuuid.uuid()),
+        FloatParameterSpec(name="Longitude", min=-180.0, max=180.0, units="degs", value=172.6398, uuid=shortuuid.uuid()),
     ]
     parameter_list = []
 
     clock_cfg = ActionServiceCFG(
-        "CLK",
-        "Local Clock",
-        "Send local time and SunUp or SunDown every minute.",
-        "CLK1",
-        num_tests,
-        True,
-        True,
-        provisioning_list,
-        parameter_list
+        objectName="CLK",
+        name="Local Clock",
+        uuid=shortuuid.uuid(),
+        text="Send local time and SunUp or SunDown every minute.",
+        controlID="CLK1",
+        numAvail=num_tests,
+        isTrigger=True,
+        isIO=True,
+        provisioning=provisioning_list,
+        parameters=parameter_list
         #  parameter_list_out
     )
-    return clock_cfg.__json__()
+    return clock_cfg
 
 
 class ClockThread(threading.Thread):
     """Watch keeping thread returns every minute"""
     def __init__(self, callback) -> None:
         threading.Thread.__init__(self, daemon=True)
         self.running = True
@@ -101,15 +102,15 @@
         self.task_sender.send_multipart([b"ALL", out_message.encode('utf-8')])
 
     def close(self):
         """Close the thread"""
         self.clock.close()
         self.running = False
 
-    def __init__(self, device_id: str, action_station_id: str, control_config_dict: dict, context: zmq.Context) -> None:
+    def __init__(self, device_id: str, local_port: int, control_config_dict: dict, context: zmq.Context) -> None:
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context
         self.running = True
 
         self.control_id = control_config_dict['controlID']
         self.name = control_config_dict['name']
@@ -121,17 +122,16 @@
         latitude = provision_list[0]['value']
         longitude = provision_list[1]['value']
         self.location_info = LocationInfo('name', 'region', 'timezone/name', latitude, longitude)
         tstamp = datetime.datetime.now()
         self.day = tstamp.day
         self.sun_time = sun(self.location_info.observer, date=datetime.datetime.now(tz=tz.tzlocal()))
 
-        self.push_url = TASK_PULL.format(id=action_station_id)
-
-        self.sub_url = CONNECTION_PUB_URL.format(id=action_station_id)
+        self.sub_url = TCP_URL.format(port=local_port + TASK_CONN_PORT_OFFSET)
+        self.push_url = TCP_URL.format(port=local_port + TASK_PULL_PORT_OFFSET)
 
         self.task_sender = self.context.socket(zmq.PUSH)
         self.task_sender.connect(self.push_url)
         self.clock = ClockThread(self.clock_message)
         logging.debug("Clock Started")
         self.start()
```

### Comparing `dashio-3.3.9/dashio/action_station_services/modbus_service.py` & `dashio-3.4.0/dashio/action_station_services/modbus_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Modbus"""
 import glob
 import logging
 import sys
 import threading
-
+import shortuuid
 import serial
 import zmq
 
-from ..constants import TASK_PULL, CONNECTION_PUB_URL
+from ..constants import TASK_PULL_PORT_OFFSET, TASK_CONN_PORT_OFFSET, TCP_URL
 from .action_station_service_config import (
     ActionServiceCFG,
     IntParameterSpec,
     ListParameterSpec,
     SelectorParameterSpec
 )
 
@@ -48,115 +48,124 @@
 def make_modbus_config(num_tests):
     """Make a timer config"""
     s_ports = serial_ports()
     default = ""
     if len(s_ports) > 0:
         default = s_ports[0]
     provisioning_list = [
-        SelectorParameterSpec("Serial Port", s_ports, default),
-        SelectorParameterSpec("Baud", ["1200", "2400", "4800", "9600", "19200", "38400", "57600", "115200"], "9600"),
-        SelectorParameterSpec("Modbus Type", ["RTU", "ASCII"], "RTU"),
+        SelectorParameterSpec(name="Serial Port", selection=s_ports, value=default, uuid=shortuuid.uuid()),
+        SelectorParameterSpec(name="Baud", selection=["1200", "2400", "4800", "9600", "19200", "38400", "57600", "115200"], value="9600", uuid=shortuuid.uuid()),
+        SelectorParameterSpec(name="Modbus Type", selection=["RTU", "ASCII"], value="RTU", uuid=shortuuid.uuid()),
         ListParameterSpec(
-            "Read Registers",
-            "Create a list of registers to read data from.",
-            [
+            name="Read Registers",
+            text="Create a list of registers to read data from.",
+            uuid=shortuuid.uuid(),
+            param_list=[
                 IntParameterSpec(
-                    "Read Register Base Address",
-                    0,
-                    65535,
-                    "",
-                    0
+                    name="Read Register Base Address",
+                    min=0,
+                    max=65535,
+                    units="",
+                    value=0,
+                    uuid=shortuuid.uuid()
                 ),
                 SelectorParameterSpec(
-                    "Register Type", [
+                    name="Register Type",
+                    selection=[
                         "char",
                         "int_8",
                         "uint_8",
                         "int_16",
                         "uint_16",
                         "int_32",
                         "uint_32",
                         "int_64",
                         "uint_64"
                     ],
-                    "uint_16",
+                    value="uint_16",
+                    uuid=shortuuid.uuid()
                 ),
                 IntParameterSpec(
-                    "Number of register to read from base address (Optional).",
-                    0,
-                    65535,
-                    "",
-                    2
+                    name="Number of register to read from base address (Optional).",
+                    min=0,
+                    max=65535,
+                    units="",
+                    value=2,
+                    uuid=shortuuid.uuid()
                 )
             ]
         ),
         ListParameterSpec(
-            "Read a Bit",
-            "Create a list of registers to read data from.",
-            [
+            name="Read a Bit",
+            text="Create a list of registers to read data from.",
+            uuid=shortuuid.uuid(),
+            param_list=[
                 IntParameterSpec(
-                    "Read Register Base Address",
-                    0,
-                    65535,
-                    "",
-                    0
+                    name="Read Register Base Address",
+                    min=0,
+                    max=65535,
+                    units="",
+                    value=0,
+                    uuid=shortuuid.uuid()
                 ),
                 IntParameterSpec(
-                    "Bit Mask",
-                    0,
-                    65535,
-                    "",
-                    0
+                    name="Bit Mask",
+                    min=0,
+                    max=65535,
+                    units="",
+                    value=0,
+                    uuid=shortuuid.uuid()
                 )
             ]
         )
 
     ]
     parameter_list_in = []
     # parameter_list_out = []
     timer_cfg = ActionServiceCFG(
-        "MDBS",
-        "Modbus Test",
-        "Modbus - Test provisioning of list",
-        "TST$",
-        num_tests,
-        True,
-        True,
-        provisioning_list,
-        parameter_list_in
+        objectName="MDBS",
+        name="Modbus Test",
+        uuid=shortuuid.uuid(),
+        text="Modbus - Test provisioning of list",
+        controlID="TST",
+        num_tests=num_tests,
+        numAvail=1,
+        isTrigger=True,
+        isIO=True,
+        provisioning=provisioning_list,
+        parameters=parameter_list_in
         #  parameter_list_out
     )
-    return timer_cfg.__json__()
+    return timer_cfg
 
 
 class ModbusService(threading.Thread):
     """Action Station Template Class"""
 
     def send_message(self, out_message=""):
         """Send the message"""
         self.task_sender.send_multipart([b"ALL", out_message.encode('utf-8')])
 
     def close(self):
         """Close the thread"""
         self.running = False
 
-    def __init__(self, device_id: str, action_station_id: str, control_config_dict: dict, context: zmq.Context) -> None:
+    def __init__(self, device_id: str, local_port: int, control_config_dict: dict, context: zmq.Context) -> None:
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context
         self.running = True
 
         self.control_id = control_config_dict['controlID']
         self.name = control_config_dict['name']
         self.control_type = control_config_dict['objectType']
         # provision_list = control_config_dict['provisioning']
 
-        self.push_url = TASK_PULL.format(id=action_station_id)
-
-        self.sub_url = CONNECTION_PUB_URL.format(id=action_station_id)
+        self.sub_url = TCP_URL.format(port=local_port + TASK_CONN_PORT_OFFSET)
+        self.push_url = TCP_URL.format(port=local_port + TASK_PULL_PORT_OFFSET)
 
         self.task_sender = self.context.socket(zmq.PUSH)
         self.task_sender.connect(self.push_url)
 
         self.control_msg = f"\t{device_id}\t{self.control_type}\t{self.control_id}"
         logging.debug("Init Class: %s, %s", self.control_type, self.name)
```

### Comparing `dashio-3.3.9/dashio/action_station_services/task_service.py` & `dashio-3.4.0/dashio/mqttconnection.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,216 +19,229 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import json
 import logging
+import ssl
 import threading
+import time
 
+import paho.mqtt.client as mqtt
+import shortuuid
 import zmq
 
-from ..constants import CONNECTION_PUB_URL, MEMORY_REQ_URL, TASK_PULL
+from .constants import CONNECTION_PUB_URL
 
+from .iotcontrol.enums import ConnectionState
 
-def num(s_num: str):
-    try:
-        return int(s_num)
-    except ValueError:
-        return float(s_num)
-
-
-def _read_control_task(data, task):
-    logging.debug("READ_CONTROL: %s", data)
-    return data[+3]
-
-
-def _if_task(data, task):
-    logging.debug("IF: %s", data)
-    return ""
-
-
-def _endif_task(data, task):
-    logging.debug("ENDIF: %s", data)
-    return ''
-
-
-def _send_alarm_task(data, task):
-    logging.debug("SEND_ALARM: %s", data)
-    return ''
-
-
-def _write_control_task(data, task):
-    logging.debug("WRITE_CONTROL: %s", data)
-    return ""
-
-
-MESSAGE_FORMAT_INPUTS = {
-    "AVD": ["url"],
-    "BTTN": ["button_state", "icon_name", "text"],
-    "TEXT": ["text"],
-    "GRPH": ["line_id", "line_data"],
-    "DIAL": ["data"],
-    "CLR": ["rgb"],
-    "TGRPH": ["time_stamp", "data"],
-    "KNOB": ["data"],
-    "KBDL": ["data"],
-    "SLCTR": ["url"],
-    "SLDR": ["url"],
-    "DIR": ["url"],
-    "LOG": ["url"],
-    "LBL": ["url"],
-}
-
-MESSAGE_FORMAT_OUTPUTS = {
-    "AVD": "\t{device_id}\tAVD\t{control_id}\t{url}",
-    "BTTN": "\t{device_id}\tBTTN\t{control_id}\t{url}",
-    "TEXT": "\t{device_id}\tTEXT\t{control_id}\t{url}",
-    "GRPH": "\t{device_id}\tGRPH\t{control_id}\t{url}",
-    "DIAL": "\t{device_id}\tDIAL\t{control_id}\t{url}",
-    "CLR": "\t{device_id}\tCLR\t{control_id}\t{url}",
-    "TGRPH": "\t{device_id}\tTGRPH\t{control_id}\t{url}",
-    "KNOB": "\t{device_id}\tKNOB\t{control_id}\t{url}",
-    "KBDL": "\t{device_id}\tKBDL\t{control_id}\t{url}",
-    "SLCTR": "\t{device_id}\tSLCTR\t{control_id}\t{url}",
-    "SLDR": "\t{device_id}\tSLDR\t{control_id}\t{url}",
-    "DIR": "\t{device_id}\tDIR\t{control_id}\t{url}",
-    "LOG": "\t{device_id}\tLOG\t{control_id}\t{url}",
-    "LBL": "\t{device_id}\tLBL\t{control_id}\t{url}",
-}
-
-
-class TaskService(threading.Thread):
-    """Task Class"""
-
-    def send_message(self, out_message=""):
-        """Send the message"""
-        self.task_sender.send_multipart([b"ALL", out_message.encode()])
 
-    def close(self):
-        """Close the thread"""
-        self.running = False
-
-    def _task_store_mem(self, mem_loc, data):
-        self.task_memory[mem_loc] = data
+class MQTTConnection(threading.Thread):
+    """Setups and manages a connection thread to the MQTT Server."""
 
-    def _task_get_mem(self, mem_loc):
-        return self.task_memory.get(mem_loc, "")
-
-    def _send_alarm(self, alarm_id: str, header: str, body: str):
-        msg = f"\t{self.device_id}\tALM\t{alarm_id}\t{header}\t{body}\n"
-        self.send_message(msg)
-
-    def _read_control_action(self, action, msg: bytearray):
-        logging.debug("READ_CONTROL: %s", msg.decode())
-
-    def _send_alarm_action(self, action, msg):
-        logging.debug("SEND_ALARM: %s", msg)
-        self._send_alarm(action['alarmID'], action['title'], action['body'])
-
-    def _write_control_action(self, action, msg):
-        logging.debug("WRITE_CONTROL: %s", msg.decode())
-
-    def _read_mem_action(self, action, msg):
-        logging.debug("READ_MEM memType: %s", action["memType"])
-        if action["memType"] == "Local":
-            pass
-        elif action["memType"] == "Task":
-            reply = self._task_get_mem(action['memoryID'])
-            logging.debug("Task read mem: %s", reply)
-        elif action["memType"] == "Global":
-            self.device_mem_socket.send_multipart([b'GET', action['memoryID'].encode(), b'0'])
-            reply = self.device_mem_socket.recv_multipart()
+    def _on_connect(self, client, userdata, flags, msg):
+        if msg == 0:
+            self._connection_state = ConnectionState.CONNECTED
+            for device_id in self._device_id_list:
+                control_topic = f"{self.username}/{device_id}/control"
+                self.mqttc.subscribe(control_topic, 0)
+            for device_id in self._device_id_rx_list:
+                data_topic = f"{self.username}/{device_id}/data"
+                self.mqttc.subscribe(data_topic, 0)
+            self._send_dash_announce()
+            logging.debug("connected OK")
         else:
-            logging.debug("READ_MEM unknown memType: %s", action["memType"])
+            logging.debug("Bad connection Returned code=%s", msg)
 
-    def _write_mem_action(self, action, msg):
-        logging.debug("WRITE_MEM memType: %s", action["memType"])
-        if action["memType"] == "Local":
-            pass
-        elif action["memType"] == "Task":
-            self._task_store_mem(action['memoryID'], action['thing'])
-        elif action["memType"] == "Global":
-            self.device_mem_socket.send_multipart([b'SET', action['memoryID'].encode(), action['thing'].encode()])
-            reply = self.device_mem_socket.recv_multipart()
-            logging.debug("Task write mem: %s", reply)
-        else:
-            logging.debug("WRITE_MEM unknown memType: %s", action["memType"])
-
-    def _connect_device_id(self, device_id):
-        msg_dict = {
-            'msgType': 'connect',
-            'deviceID': device_id
+    def _on_disconnect(self, client, userdata, msg):
+        logging.debug("disconnecting reason  %s", msg)
+        self._connection_state = ConnectionState.DISCONNECTED
+
+    def _on_message(self, client, obj, msg):
+        data = str(msg.payload, "utf-8").strip()
+        logging.debug("MQTT RX:\n%s", data)
+        self.tx_zmq_pub.send_multipart([msg.payload, self.b_connection_id])
+
+    def _on_subscribe(self, client, obj, mid, granted_qos):
+        logging.debug("Subscribed: %s %s", str(mid), str(granted_qos))
+
+    def _on_log(self, client, obj, level, string):
+        logging.debug(string)
+
+    def add_device(self, device):
+        """Add a Device to the connextion
+
+        Parameters
+        ----------
+            device (Device):
+                The Device to add.
+        """
+        if device.device_id not in self._device_id_list:
+            self._device_id_list.append(device.device_id)
+            device.register_connection(self)
+            if self._connection_state == ConnectionState.CONNECTED:
+                control_topic = f"{self.username}/{device.device_id}/control"
+                self.mqttc.subscribe(control_topic, 0)
+                self._send_dash_announce()
+
+    def _add_device_rx(self, msg_dict):
+        """Connect to another device"""
+        device_id = msg_dict["deviceID"]
+        logging.debug("MQTT DEVICE CONNECT: %s", device_id)
+        if device_id not in self._device_id_rx_list:
+            self._device_id_rx_list.append(device_id)
+            data_topic = f"{self.username}/{device_id}/data"
+            self.mqttc.subscribe(data_topic, 0)
+
+    def _del_device_rx(self, msg_dict):
+        device_id = msg_dict["deviceID"]
+        if device_id in self._device_id_rx_list:
+            data_topic = f"{self.username}/{device_id}/data"
+            self.mqttc.unsubscribe(data_topic)
+            logging.debug("MQTT DEVICE_DISCONNECT: %s", device_id)
+            del self._device_id_rx_list[device_id]
+
+    def _send_dash_announce(self):
+        msg = {
+            'msgType': 'send_announce',
+            'connectionUUID': self.zmq_connection_uuid
         }
-        logging.debug("AS CONNECT: %s", device_id)
-        self.task_sender.send_multipart([b"COMMAND", json.dumps(msg_dict).encode()])
+        logging.debug("MQTT SEND ANNOUNCE: %s", msg)
+        self.tx_zmq_pub.send_multipart([b"COMMAND", json.dumps(msg).encode()])
+
+    def close(self):
+        """Close the connection."""
+        self.running = False
+
+    def __init__(self, host, port, username="", password="", use_ssl=False, context: zmq.Context = None):
+        """
+        Setups and manages a connection thread to the MQTT Server.
+
+        Parameters
+        ---------
+            host : str
+                The server name of the mqtt host.
+            port :int
+                Port number to connect to.
+            username : str
+                username for the mqtt connection.
+            password : str
+                password for the mqtt connection.
+
+        Keyword Parameters
+        -----------------
+            use_ssl : bool
+                Whether to use ssl for the connection or not. (default: {False})
+        """
 
-    def __init__(self, device_id: str, action_station_id: str, task_config_dict: dict, context: zmq.Context) -> None:
         threading.Thread.__init__(self, daemon=True)
-        self.context = context
-        self.running = True
-        self.timer_type = None
-        self.device_id = device_id
-        self.control_type = "TASK"
-        self.task_memory = {}
-
-        self.action_function_dict = {
-            "READ_CONTROL": self._read_control_action,
-            "SEND_ALARM": self._send_alarm_action,
-            "WRITE_CONTROL": self._write_control_action,
-            "READ_MEM": self._read_mem_action,
-            "WRITE_MEM": self._write_mem_action,
-        }
 
-        self.task_id = task_config_dict['uuid']
-        self.actions = task_config_dict['actions']
-        self.name = task_config_dict['name']
-        self.sub_msg = None
-        rx_device_id = ""
-        if len(self.actions) == 0:
-            return
+        self.context = context or zmq.Context.instance()
+        self.zmq_connection_uuid = "MQTT:" + shortuuid.uuid()
+        self.b_connection_id = self.zmq_connection_uuid.encode('utf-8')
+        self._connection_state = ConnectionState.DISCONNECTED
+        self.connection_topic_list = []
+        self._device_id_list = []
+        self._device_id_rx_list = []
+        self.host = host
+        self.port = port
+        # self.last_will = "OFFLINE"
+        self.running = True
+        self.username = username
+        self.mqttc = mqtt.Client()
+        # Assign event callbacks
+        self.mqttc.on_message = self._on_message
+        self.mqttc.on_connect = self._on_connect
+        self.mqttc.on_disconnect = self._on_disconnect
+        self.mqttc.on_subscribe = self._on_subscribe
+
+        if use_ssl:
+            self.mqttc.tls_set(
+                ca_certs=None,
+                certfile=None,
+                keyfile=None,
+                cert_reqs=ssl.CERT_REQUIRED,
+                tls_version=ssl.PROTOCOL_TLSv1_2,
+                ciphers=None,
+            )
+            self.mqttc.tls_insecure_set(False)
+
+        self.mqttc.on_log = self._on_log
+        # self.mqttc.will_set(self.data_topic, self.last_will, qos=1, retain=False)
+        # Connect
+        if username and password:
+            self.mqttc.username_pw_set(username, password)
         try:
-            rx_device_id = self.actions[0]["deviceID"]
-            rx_control_type = self.actions[0]["controlType"]
-            rx_control_id = self.actions[0]["controlID"]
-        except KeyError:
-            return
-        self.sub_msg = f"\t{rx_device_id}\t{rx_control_type}\t{rx_control_id}"
-        self.push_url = TASK_PULL.format(id=action_station_id)
-        self.sub_url = CONNECTION_PUB_URL.format(id=action_station_id)
+            self.mqttc.connect(self.host, self.port)
+            self._connection_state = ConnectionState.CONNECTING
+        except mqtt.socket.gaierror as error:
+            logging.debug("No connection to internet: %s", str(error))
+        # Start subscribe, with QoS level 0
+        self._disconnect_timeout = 1.0
+        self.start()
 
-        self.device_mem_socket = self.context.socket(zmq.REQ)
-        self.device_mem_socket.connect(MEMORY_REQ_URL.format(id=self.device_id))
+    def _mqtt_command(self, msg_dict: dict):
+        logging.debug("MQTT CMD: %s", msg_dict)
+        if msg_dict['msgType'] == 'connect':
+            self._add_device_rx(msg_dict)
+        if msg_dict['msgType'] == 'disconnect':
+            self._del_device_rx(msg_dict)
 
-        self.task_sender = self.context.socket(zmq.PUSH)
-        self.task_sender.connect(self.push_url)
+    def run(self):
+        self.mqttc.loop_start()
 
-        if rx_device_id != device_id:
-            self._connect_device_id(rx_device_id)
-        self.start()
+        self.tx_zmq_pub = self.context.socket(zmq.PUB)
+        self.tx_zmq_pub.bind(CONNECTION_PUB_URL.format(id=self.zmq_connection_uuid))
 
-    # Do a simple test case to check messaging.
-    def _do_actions(self, msg):
-        for action in self.actions:
-            self.action_function_dict[action['objectType']](action, msg)
+        self.rx_zmq_sub = self.context.socket(zmq.SUB)
+        self.tx_zmq_pub = self.context.socket(zmq.PUB)
 
-    def run(self):
-        task_receiver = self.context.socket(zmq.SUB)
-        task_receiver.connect(self.sub_url)
-        task_receiver.setsockopt_string(zmq.SUBSCRIBE, self.sub_msg)
+        #  Subscribe on ALL, and my connection
+        self.rx_zmq_sub.setsockopt(zmq.SUBSCRIBE, b"ALL")
+        self.rx_zmq_sub.setsockopt(zmq.SUBSCRIBE, b"MQTT")
+        self.rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, self.zmq_connection_uuid)
 
         poller = zmq.Poller()
-        poller.register(task_receiver, zmq.POLLIN)
+        poller.register(self.rx_zmq_sub, zmq.POLLIN)
 
         while self.running:
             try:
-                socks = dict(poller.poll(15))
+                socks = dict(poller.poll(50))
             except zmq.error.ContextTerminated:
                 break
-            if task_receiver in socks:
-                message, _ = task_receiver.recv_multipart()
-                if message:
-                    logging.debug("TASK: %s\t%s RX:%s", self.name, self.task_id, message.decode())
-                    self._do_actions(message)
-        self.task_sender.close()
-        task_receiver.close()
-        self.device_mem_socket.close()
+            if self.rx_zmq_sub in socks:
+                try:
+                    [msg_to, data] = self.rx_zmq_sub.recv_multipart()
+                except ValueError:
+                    logging.debug("MQTT value error")
+                    continue
+                if not data:
+                    logging.debug("MQTT no data error")
+                    continue
+                # logging.debug("DASH: %s ,%s", msg_to, data)
+                if msg_to == b'COMMAND':
+                    logging.debug("MQTT RX COMMAND")
+                    self._mqtt_command(json.loads(data))
+                    continue
+                msg_l = data.split(b'\t')
+                try:
+                    device_id = msg_l[1].decode().strip()
+                except IndexError:
+                    continue
+                data_topic = f"{self.username}/{device_id}/data"
+                if self._connection_state == ConnectionState.CONNECTED:
+                    logging.debug("MQTT TX:\n%s", data.decode().rstrip())
+                    self.mqttc.publish(data_topic, data.decode())
+            if self._connection_state == ConnectionState.DISCONNECTED:
+                self._disconnect_timeout = min(self._disconnect_timeout, 900)
+                time.sleep(self._disconnect_timeout)
+                try:
+                    self.mqttc.connect(self.host, self.port)
+                    self._connection_state = ConnectionState.CONNECTING
+                except mqtt.socket.gaierror as error:
+                    logging.debug("No connection to internet: %s", str(error))
+                self._disconnect_timeout = self._disconnect_timeout * 2
+
+        self.mqttc.loop_stop()
+        self.tx_zmq_pub.close()
+        self.rx_zmq_sub.close()
```

### Comparing `dashio-3.3.9/dashio/action_station_services/timer_service.py` & `dashio-3.4.0/dashio/action_station_services/timer_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,49 +19,49 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import logging
 import threading
-
+import shortuuid
 import zmq
 
-from ..constants import CONNECTION_PUB_URL, TASK_PULL
+from ..constants import TASK_CONN_PORT_OFFSET, TASK_PULL_PORT_OFFSET, TCP_URL
 from .action_station_service_config import (
     ActionServiceCFG,
     IntParameterSpec,
     SelectorParameterSpec
 )
 
 
 # This defines the provisioning for the TIMER
 def make_timer_config(num_timers):
     """Make a timer config"""
     provisioning_list = [
-        SelectorParameterSpec("Timer Type", ["Repeat", "OneShot"], "Repeat"),
-        IntParameterSpec("Timeout", 100, 600000, "ms", 1000)
+        SelectorParameterSpec(name="Timer Type", selection=["Repeat", "OneShot"], value="Repeat", uuid=shortuuid.uuid()),
+        IntParameterSpec(name="Timeout", min=100, max=600000, units="ms", value=1000, uuid=shortuuid.uuid())
     ]
     parameter_in_list = []
     #  parameter_out_list = []
 
     timer_cfg = ActionServiceCFG(
-        "TMR",
-        "Timer",
-        "A timer control.",
-        "TMR",
-        num_timers,
-        True,
-        True,
-        provisioning_list,
-        parameter_in_list
+        objectName="TMR",
+        name="Timer",
+        uuid=shortuuid.uuid(),
+        text="A timer control.",
+        controlID="TMR",
+        numAvail=num_timers,
+        isTrigger=True,
+        isIO=True,
+        provisioning=provisioning_list,
+        parameters=parameter_in_list
         #  parameter_out_list
     )
-    return timer_cfg.__json__()
-
+    return timer_cfg
 
 class RepeatTimer(threading.Timer):
     """The timer"""
     def run(self):
         while not self.finished.wait(self.interval):
             self.function(*self.args, **self.kwargs)
 
@@ -83,29 +83,29 @@
         """Send the message"""
         self.task_sender.send_multipart([b"ALL", out_message.encode('utf-8')])
 
     def close(self):
         """Close the thread"""
         self.running = False
 
-    def __init__(self, device_id: str, action_station_id: str, control_config_dict: dict, context: zmq.Context) -> None:
+    def __init__(self, device_id: str, local_port: int, control_config_dict: dict, context: zmq.Context) -> None:
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context
         self.running = True
         self.timer_type = None
 
         self.control_id = control_config_dict['controlID']
         self.name = control_config_dict['name']
         self.control_type = control_config_dict['objectType']
         provision_list = control_config_dict['provisioning']
 
-        self.sub_url = CONNECTION_PUB_URL.format(id=action_station_id)
+        self.sub_url = TCP_URL.format(port=local_port + TASK_CONN_PORT_OFFSET)
+        self.push_url = TCP_URL.format(port=local_port + TASK_PULL_PORT_OFFSET)
 
-        self.push_url = TASK_PULL.format(id=action_station_id)
         self.task_sender = self.context.socket(zmq.PUSH)
         self.task_sender.connect(self.push_url)
 
         self.timer_time = int(provision_list[1]['value']) / 1000.0
         self.timer_type = provision_list[0]['value']
 
         self.control_msg = f"\t{device_id}\t{self.control_type}\t{self.control_id}"
```

### Comparing `dashio-3.3.9/dashio/bleconnection.py` & `dashio-3.4.0/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/constants.py` & `dashio-3.4.0/dashio/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 CONNECTION_PUB_URL = "inproc://DASHIO_CONN_PUB_{id}"
-MEMORY_REQ_URL = "inproc://DASHIO_MEM_REQ_{id}"
-TASK_PULL = "inproc://DASHIO_TASK_PULL_{id}"
+TCP_URL = "tcp://127.0.0.1:{port}"
+TASK_CONN_PORT_OFFSET = 1
+TASK_PULL_PORT_OFFSET = 2
+TASK_MEMORY_PORT_OFFSET = 3
 
 BAD_CHARS = {ord(i): None for i in '\t\n'}
```

### Comparing `dashio-3.3.9/dashio/dashconnection.py` & `dashio-3.4.0/dashio/dashconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,16 +278,16 @@
         # self.dash_c.will_set(self.data_topic, self.LWD, qos=1, retain=False)
         # Connect
         if username and password:
             self._dash_c.username_pw_set(username, password)
             try:
                 self._dash_c.connect(host, port)
                 self._connection_state = ConnectionState.CONNECTING
-            except mqtt.socket.gaierror as error:
-                logging.debug("No connection to internet: %s", str(error))
+            except (mqtt.socket.gaierror, ConnectionRefusedError) as error:
+                logging.debug("No connection to server: %s", str(error))
         # Start subscribe, with QoS level 0
         self.rx_zmq_sub = self.context.socket(zmq.SUB)
         self._disconnect_timeout = 1.0
         self.start()
 
     def close(self):
         """Close the connection."""
@@ -353,14 +353,14 @@
                     self._dash_c.publish(data_topic, data.decode())
             if self._connection_state == ConnectionState.DISCONNECTED:
                 self._disconnect_timeout = min(self._disconnect_timeout, 900)
                 time.sleep(self._disconnect_timeout)
                 try:
                     self._dash_c.connect(self.host, self.port)
                     self._connection_state = ConnectionState.CONNECTING
-                except mqtt.socket.gaierror as error:
-                    logging.debug("No connection to internet: %s", str(error))
+                except (mqtt.socket.gaierror, ConnectionRefusedError) as error:
+                    logging.debug("No connection to server: %s", str(error))
                 self._disconnect_timeout = self._disconnect_timeout * 2
 
         self._dash_c.loop_stop()
         self.tx_zmq_pub.close()
         self.rx_zmq_sub.close()
```

### Comparing `dashio-3.3.9/dashio/device.py` & `dashio-3.4.0/dashio/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,31 +213,36 @@
         self.tx_zmq_pub.send_multipart([b"DASH", payload.encode('utf-8')])
 
     def is_control_loaded(self, control_type, control_id: str) -> bool:
         """Is the control loaded in the device?"""
         key = f"{control_type}\t{control_id}"
         return key in self.controls_dict
 
-    def add_all_c64_controls(self, c64_dict: dict):
+    def add_all_c64_controls(self, c64_dict: dict, column_no=1):
         """Loads all the controls in cfg_dict into the device.
 
         Parameters
         ----------
         c64_dict : Dict
             dictionary of the CFG loaded by decode_cfg from a CFG64 or json
+        column_no: Int From 1 to 3 (default 1).
+            The DashIO app reports the size of the screen in no of columns. You can load a seperate
+            config for each reported column number.
         """
+        if not 1 <= column_no <= 3:
+            column_no = 1
         for control_type, control_list in c64_dict.items():
             if isinstance(control_list, list):
                 for control in control_list:
                     key = f"{control_type}\t{control['controlID']}"
                     if self.is_control_loaded(control_type, control['controlID']):
                         cfg = CONFIG_INSTANCE_DICT[control_type].from_dict(control)
-                        self.controls_dict[key].add_config_columnar(cfg)
+                        self.controls_dict[key].add_config(cfg, column_no=column_no)
                     else:
-                        new_control = CONTROL_INSTANCE_DICT[control_type].from_cfg_dict(control)
+                        new_control = CONTROL_INSTANCE_DICT[control_type].from_cfg_dict(control, column_no=column_no)
                         self.add_control(new_control)
 
     def add_control(self, iot_control):
         """Add a control to the device.
 
         Parameters
         ----------
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/__init__.py` & `dashio-3.4.0/dashio/iotcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/iotcontrol/alarm.py` & `dashio-3.4.0/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.4.0/dashio/iotcontrol/audio_visual_display.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     """
 
     def __init__(
         self,
         control_id: str,
         title="A Audio visual display",
         title_position=TitlePosition.BOTTOM,
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """AudioVisualDisplay
         Set the URL for IoTDashboard to play the media pointed to by the URL
 
         Parameters
         ----------
         control_id : str
@@ -47,19 +48,19 @@
             Title of the control, by default None
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         title_position : TitlePosition, optional
             Position of the title when displayed on the iotdashboard app, by default None
         """
         super().__init__("AVD", control_id)
-        self._cfg_columnar.append(ControlConfig(control_id, title, control_position, title_position))
+        self._app_columns_cfg[str(column_no)].append(ControlConfig(control_id, title, control_position, title_position))
         self.url = ""
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Button from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -67,15 +68,16 @@
         -------
         Button
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         """get_state is called by iotdashboard
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/button.py` & `dashio-3.4.0/dashio/iotcontrol/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,18 +131,19 @@
         title_position=TitlePosition.BOTTOM,
         button_enabled=True,
         style=ButtonStyle.BASIC,
         icon_name=Icon.NONE,
         on_color=Color.BLUE,
         off_color=Color.RED,
         text="",
-        control_position: ControlPosition = None
+        control_position: ControlPosition = None,
+        column_no=1
     ):
         super().__init__("BTTN", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             ButtonConfig(
                 control_id,
                 title,
                 title_position,
                 button_enabled,
                 style,
                 icon_name,
@@ -153,15 +154,15 @@
             )
         )
         self._btn_state = ButtonState.OFF
         self._text = text.translate(BAD_CHARS)
         self._icon_name = icon_name
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Button from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -175,15 +176,16 @@
             _get_title_position(cfg_dict["titlePosition"]),
             cfg_dict["buttonEnabled"],
             _get_button_style(cfg_dict.get("style", 'basic')),
             _get_icon(cfg_dict["iconName"]),
             _get_color(cfg_dict["onColor"]),
             _get_color(cfg_dict["offColor"]),
             cfg_dict["text"],
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         """get_state is called by iotdashboard
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/button_group.py` & `dashio-3.4.0/dashio/iotcontrol/button_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         title="A Button Group",
         text="A Button group with Text",
         title_position=TitlePosition.BOTTOM,
         style=ButtonGroupStyle.BASIC,
         icon=Icon.MENU,
         grid_view=True,
         control_position=None,
+        column_no=1
     ):
         """ButtonGroup control that shows a popup of buttons.
 
         Parameters
         ----------
             control_id : str
                 An unique control identity string. The control identity string must be a unique string for each control per device
@@ -120,18 +121,18 @@
                 [description]. Defaults to Icon.MENU.
             grid_view (bool, optional):
                 [description]. Defaults to True.
             control_position (ControlPosition, optional):
                 [description]. Defaults to None.
         """
         super().__init__("BTGP", control_id)
-        self._cfg_columnar.append(ButtonGroupConfig(control_id, title, text, style, icon, grid_view, control_position, title_position))
+        self._app_columns_cfg[str(column_no)].append(ButtonGroupConfig(control_id, title, text, style, icon, grid_view, control_position, title_position))
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates ButtonGroup from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -143,15 +144,16 @@
             cfg_dict["controlID"],
             cfg_dict.get("title", ""),
             cfg_dict.get("text", ""),
             _get_title_position(cfg_dict.get("titlePosition", "Bottom")),
             _get_button_group_style(cfg_dict.get("style", "basic")),
             _get_icon(cfg_dict.get("iconName", "None")),
             cfg_dict.get("gridView", True),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def add_button(self, control):
         """[summary]
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/chart.py` & `dashio-3.4.0/dashio/iotcontrol/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         y_axis_min=0.0,
         y_axis_max=1000.0,
         y_axis_num_bars=5,
         y_axis_label_rt="",
         y_axis_min_rt=0.0,
         y_axis_max_rt=1000.0,
         control_position=None,
+        column_no=1
     ):
         """A Chart Control
 
         Parameters
         ----------
         control_id : str
             A unique identifier for this control
@@ -185,15 +186,15 @@
             Max value for the Y axis, by default 100.0
         y_axis_num_bars : int, optional
             Number of bars on the Y axis, by default 5
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         """
         super().__init__("CHRT", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             ChartConfig(
                 control_id,
                 title,
                 title_position,
                 x_axis_label,
                 x_axis_min,
                 x_axis_max,
@@ -256,15 +257,15 @@
 
     @property
     def y_axis_num_bars(self):
         """Returns the y axis number of bars"""
         return self.y_axis_num_bars
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Chart from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -284,15 +285,16 @@
             cfg_dict["yAxisLabel"],
             cfg_dict["yAxisMin"],
             cfg_dict["yAxisMax"],
             cfg_dict["yAxisNumBars"],
             cfg_dict.get("yAxisLabelRt", ''),
             cfg_dict.get("yAxisMinRt", 0.0),
             cfg_dict.get("yAxisMaxRt", 1000.0),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def add_line(self, line_id: str, gline: ChartLine):
         """Add a line to the chart
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/color_picker.py` & `dashio-3.4.0/dashio/iotcontrol/color_picker.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self,
         control_id: str,
         title="A Color Picker",
         title_position=TitlePosition.BOTTOM,
         style=ColorPickerStyle.WHEEL,
         send_only_on_release=True,
         control_position=None,
+        column_no=1
     ):
         """ColorPicker
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -94,28 +95,28 @@
         picker_style: ColorPickerStyle, optional
             The style of color picker to use.
         send_only_on_release: Boolean
             send only on release, by default True
 
         """
         super().__init__("CLR", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             ColorPickerConfig(
                 control_id,
                 title,
                 title_position,
                 style,
                 send_only_on_release,
                 control_position
             )
         )
         self._color_value = "#4F5GA2"
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates ColorPicker from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -125,15 +126,16 @@
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
             _get_color_picker_style(cfg_dict["pickerStyle"]),
             cfg_dict["sendOnlyOnRelease"],
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         return self._control_hdr_str + f"{self._color_value}\n"
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/control.py` & `dashio-3.4.0/dashio/iotcontrol/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -296,20 +296,22 @@
         """
         cfg_list = []
         try:
             num_columns = int(data[3])
             dashboard_id = data[2]
         except (IndexError, ValueError):
             return cfg_list
-        if num_columns >= self._cfg_full_page_no_columns and self._cfg_full_page:
-            for cfg in self._cfg_full_page:
-                cfg_list.append(f"\tCFG\t{dashboard_id}\t{self.cntrl_type}\t{cfg.get_cfg_json()}")
-        else:
-            for control_cfg in self._cfg_columnar:
-                cfg_list.append(f"\tCFG\t{dashboard_id}\t{self.cntrl_type}\t{control_cfg.get_cfg_json()}")
+        if 1 <= num_columns <= self._cfg_max_no_columns:
+            while num_columns >= 1:
+                cfgs = self._app_columns_cfg[str(num_columns)]
+                if cfgs:
+                    for cfg in cfgs:
+                        cfg_list.append(f"\tCFG\t{dashboard_id}\t{self.cntrl_type}\t{cfg.get_cfg_json()}")
+                    break
+                num_columns = num_columns - 1
         return cfg_list
 
     def get_cfg64(self, data) -> list:
         """Returns the CFG dict for the control called when the iotdashboard app asks for a CFG
 
         Parameters
         ----------
@@ -322,35 +324,29 @@
             The CFG dict for this control
         """
         cfg_list = []
         try:
             num_columns = int(data[3])
         except (IndexError, ValueError):
             return []
-        if num_columns >= self._cfg_full_page_no_columns and self._cfg_full_page:
-            for cfg in self._cfg_full_page:
-                cfg_list.append(cfg.get_cfg64())
-        else:
-            for cfg in self._cfg_columnar:
-                cfg_list.append(cfg.get_cfg64())
+        if 1 <= num_columns <= self._cfg_max_no_columns:
+            while num_columns >= 1:
+                cfgs = self._app_columns_cfg[str(num_columns)]
+                if cfgs:
+                    for cfg in cfgs:
+                        cfg_list.append(cfg.get_cfg64())
+                    break
+                num_columns = num_columns - 1
         return cfg_list
 
-    def add_config_columnar(self, config):
-        """Add a duplicate Config for the columnar view"""
+    def add_config(self, config, column_no=1):
+        """Add a duplicate Config for dashio Apps with wider screens"""
         config.cfg["controlID"] = self.control_id
-        self._cfg_columnar.append(config)
-
-    def add_config_full_page(self, config):
-        """Add a duplicate Config for the full page view"""
-        config.cfg["controlID"] = self.control_id
-        self._cfg_full_page.append(config)
-
-    def set_no_culumns_full_page(self, no_columns: int):
-        """Set the number of columns that the full page view uses."""
-        self._cfg_full_page_no_columns = no_columns
+        if 1 <= column_no <= self._cfg_max_no_columns:
+            self._app_columns_cfg[str(column_no)].append(config)
 
     def add_receive_message_callback(self, callback):
         """Add a callback to receive incoming messages to the control."""
         self._message_rx_event += callback
 
     def remove_receive_message_callback(self, callback):
         """Remaove a callback from receive incoming messages to the control."""
@@ -370,35 +366,34 @@
         Parameters
         ----------
         cntrl_type : str
             The type of control to implement
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
         """
-        # Dictionary to store CFG json
-        self._cfg_columnar = []
-        self._cfg_full_page = []
-        self._cfg_full_page_no_columns = 0
+        # List to store control CFG json
+        self._app_columns_cfg = {
+            '1': [],
+            '2': [],
+            '3': []
+        }
+        self._cfg_max_no_columns = 3
         self.cntrl_type = cntrl_type.translate(BAD_CHARS)
         self.control_id = control_id.translate(BAD_CHARS)
         if not self.control_id:
             raise ValueError('control_id cannot be an empty string')
         self._message_rx_event = Event()
         self._message_tx_event = Event()
         # This may break things but makes all controls able to be setup from tasks.
         self._message_rx_event += self._message_tx_event
         self._control_hdr_str = f"\t{{device_id}}\t{self.cntrl_type}\t{self.control_id}\t"
 
-    def del_configs_columnar(self):
+    def del_config(self, column_no=1):
         """Deletes all the columnar config layout entries"""
-        self._cfg_columnar = []
-
-    def del_configs_full_page(self):
-        """Deletes all the full page config layout entries"""
-        self._cfg_columnar = []
+        self._app_columns_cfg[str(column_no)] = []
 
     @property
     def state_str(self) -> str:
         """The current state of the control
 
         Returns
         -------
@@ -409,21 +404,25 @@
 
     @state_str.setter
     def state_str(self, val):
         self._message_tx_event(val)
 
     #  Use getter, setter properties to store the settings in the config dictionary
     @property
-    def parent_id(self, index=0) -> str:
+    def parent_id(self, index=0, column_no=1) -> str:
         """The parent control or deviceview this control belongs to
 
         Returns
         -------
         str
             The parent_id
         """
-        return self._cfg_columnar[index]["parentID"]
+        if not 1 <= column_no <= self._cfg_max_no_columns:
+            column_no = 1
+        return self._app_columns_cfg[str(column_no)][index]["parentID"]
 
     @parent_id.setter
-    def parent_id(self, val: str, index=0):
+    def parent_id(self, val: str, index=0, column_no=1):
         _val = val.translate(BAD_CHARS)
-        self._cfg_columnar[index].parent_id = _val
+        if not 1 <= column_no <= self._cfg_max_no_columns:
+            column_no = 1
+        self._app_columns_cfg[str(column_no)][index].parent_id = _val
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/device_view.py` & `dashio-3.4.0/dashio/iotcontrol/device_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,19 @@
         control_color=Color.WHITE_SMOKE,
         control_border_color=Color.WHITE_SMOKE,
         control_background_color=Color.BLACK,
         control_title_font_size=16,
         control_max_font_size=20,
         control_background_transparency=0,
         num_grid_columns=22,
-        num_grid_rows=32
+        num_grid_rows=32,
+        column_no=1
     ):
         super().__init__("DVVW", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             DeviceViewConfig(
                 control_id,
                 title,
                 style,
                 icon,
                 color,
                 share_column,
@@ -189,15 +190,15 @@
                 num_grid_columns,
                 num_grid_rows
             )
         )
         self._state_str = ""
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates DeviceView from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -218,15 +219,16 @@
             _get_color(cfg_dict["ctrlColor"]),
             _get_color(cfg_dict["ctrlBorderColor"]),
             _get_color(cfg_dict["ctrlBkgndColor"]),
             cfg_dict["ctrlTitleFontSize"],
             cfg_dict["ctrlMaxFontSize"],
             cfg_dict["ctrlBkgndTransparency"],
             cfg_dict["gridColumns"],
-            cfg_dict["gridRows"]
+            cfg_dict["gridRows"],
+            column_no
         )
 
     def add_control(self, control):
         """Add a control to the DeviceView
 
         Parameters
         ----------
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/dial.py` & `dashio-3.4.0/dashio/iotcontrol/dial.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,29 +89,21 @@
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
 
 class Dial(Control):
     """Dial Control"""
 
-    def add_config_columnar(self, config: DialConfig):
+    def add_config(self, config: DialConfig, column_no=1):
         if isinstance(config, DialConfig):
             config.cfg["min"] = self.dial_min
             config.cfg["max"] = self.dial_max
             config.cfg["redValue"] = self.red_value
             config.cfg["ControlID"] = self.control_id
-            self._cfg_columnar.append(config)
-
-    def add_config_full_page(self, config: DialConfig):
-        if isinstance(config, DialConfig):
-            config.cfg["min"] = self.dial_min
-            config.cfg["max"] = self.dial_max
-            config.cfg["redValue"] = self.red_value
-            config.cfg["ControlID"] = self.control_id
-            self._cfg_columnar.append(config)
+            self._app_columns_cfg[str(column_no)].append(config)
 
     def __init__(
         self,
         control_id: str,
         title="A Dial",
         title_position=TitlePosition.BOTTOM,
         dial_min=0.0,
@@ -120,15 +112,16 @@
         dial_fill_color=Color.RED,
         pointer_color=Color.BLUE,
         number_position=DialNumberPosition.LEFT,
         show_min_max=False,
         style=DialStyle.PIE,
         precision=Precision.OFF,
         units="",
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """Dial
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -156,15 +149,15 @@
             Dial style, by default DialStyle.PIE
         precision : Precision, optional
             Precision of the displayed number, by default Precision.OFF
         units : str, optional
             Units of the dial position, by default ""
         """
         super().__init__("DIAL", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             DialConfig(
                 control_id,
                 title,
                 title_position,
                 dial_min,
                 dial_max,
                 red_value,
@@ -195,15 +188,15 @@
 
     @property
     def red_value(self):
         """Return the red value for the dial"""
         return self._red_value
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Dial from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -222,15 +215,16 @@
             _get_color(cfg_dict["dialFillColor"]),
             _get_color(cfg_dict["pointerColor"]),
             _get_dial_number_position(cfg_dict["numberPosition"]),
             cfg_dict["showMinMax"],
             _get_dial_style(cfg_dict["style"]),
             _get_precision(cfg_dict["precision"]),
             cfg_dict["units"],
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         return self._control_hdr_str + f"{self._dial_value}\n"
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/direction.py` & `dashio-3.4.0/dashio/iotcontrol/direction.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,37 +74,32 @@
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
 
 class Direction(Control):
     """Direction control"""
 
-    def add_config_columnar(self, config: DirectionConfig):
+    def add_config(self, config: DirectionConfig, column_no=1):
         if isinstance(config, DirectionConfig):
             config.cfg["calAngle"] = self.cal_angle
             config.cfg["ControlID"] = self.control_id
-            self._cfg_columnar.append(config)
-
-    def add_config_full_page(self, config: DirectionConfig):
-        if isinstance(config, DirectionConfig):
-            config.cfg["calAngle"] = self.cal_angle
-            config.cfg["ControlID"] = self.control_id
-            self._cfg_full_page.append(config)
+            self._app_columns_cfg[str(column_no)]
 
     def __init__(
         self,
         control_id: str,
         title="A Control",
         style=DirectionStyle.DEG,
         title_position=TitlePosition.BOTTOM,
         pointer_color=Color.GREEN,
         units="",
         precision=Precision.OFF,
         calibration_angle=0,
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """Direction Control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -122,15 +117,15 @@
             Units to be displayed with the value, by default ""
         precision : Precision, optional
             Precision of the value displayed, by default Precision.OFF
         calibration_angle : int, optional
             Calibration angle offset, by default 0
         """
         super().__init__("DIR", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             DirectionConfig(
                 control_id,
                 title,
                 style,
                 title_position,
                 pointer_color,
                 units,
@@ -145,15 +140,15 @@
 
     @property
     def cal_angle(self):
         """Retturns the calibration angle"""
         return self._cal_angle
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Direction from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -166,15 +161,16 @@
             cfg_dict["title"],
             _get_direction_style(cfg_dict["style"]),
             _get_title_position(cfg_dict["titlePosition"]),
             _get_color(cfg_dict["pointerColor"]),
             cfg_dict["units"],
             _get_precision(cfg_dict["precision"]),
             cfg_dict["calAngle"],
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         if self._direction_text:
             s_str = self._control_hdr_str + f"{self._direction_value}\t{self._direction_text}\n"
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/enums.py` & `dashio-3.4.0/dashio/iotcontrol/enums.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/iotcontrol/event.py` & `dashio-3.4.0/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/iotcontrol/event_log.py` & `dashio-3.4.0/dashio/iotcontrol/event_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,23 @@
         return header
 
 
 class EventLog(Control):
     """EventLog control
     """
 
-    def __init__(self,
-                 control_id: str,
-                 title="An Event Log",
-                 title_position=TitlePosition.BOTTOM,
-                 control_position=None,
-                 max_log_entries=100):
+    def __init__(
+        self,
+        control_id: str,
+        title="An Event Log",
+        title_position=TitlePosition.BOTTOM,
+        control_position=None,
+        max_log_entries=100,
+        column_no=1
+    ):
         """An EventLog control
 
         Parameters
         ----------
 
         control_id : str
             A unique identifier for this control
@@ -102,22 +105,22 @@
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         max_log_entries : int, optional
             The EventLog usues a ring buffer for data entries this dfines the number of
             entries before over wrting older entires, by default 100
         """
         super().__init__("LOG", control_id)
-        self._cfg_columnar.append(ControlConfig(control_id, title, control_position, title_position))
+        self._app_columns_cfg[str(column_no)].append(ControlConfig(control_id, title, control_position, title_position))
 
         self._message_rx_event = Event()
         self._message_rx_event += self._get_log_from_timestamp
         self.log = RingBuffer(max_log_entries)
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Menu from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -125,15 +128,16 @@
         -------
         Menu
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def _get_log_from_timestamp(self, msg):
         data_str = ""
         try:
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/knob.py` & `dashio-3.4.0/dashio/iotcontrol/knob.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,29 +86,21 @@
         return tmp_cls
 
 
 class Knob(Control):
     """A Knob control
     """
 
-    def add_config_columnar(self, config: KnobConfig):
+    def add_config_columnar(self, config: KnobConfig, column_no=1):
         if isinstance(config, KnobConfig):
             config.cfg["min"] = self.dial_min
             config.cfg["max"] = self.dial_max
             config.cfg["redValue"] = self.red_value
             config.cfg["ControlID"] = self.control_id
-            self._cfg_columnar.append(config)
-
-    def add_config_full_page(self, config: KnobConfig):
-        if isinstance(config, KnobConfig):
-            config.cfg["min"] = self.dial_min
-            config.cfg["max"] = self.dial_max
-            config.cfg["redValue"] = self.red_value
-            config.cfg["ControlID"] = self.control_id
-            self._cfg_columnar.append(config)
+            self._app_columns_cfg[str(column_no)]
 
     def __init__(
         self,
         control_id,
         title="A Knob",
         title_position=TitlePosition.BOTTOM,
         knob_style=KnobStyle.NORMAL,
@@ -116,15 +108,16 @@
         dial_max=100.0,
         red_value=75.0,
         show_min_max=False,
         send_only_on_release=True,
         dial_follows_knob=False,
         dial_color=Color.BLUE,
         knob_color=Color.RED,
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """A Knob control is a control with a dial and knob.
 
         Parameters
         ----------
         control_id : str
             A unique identifier for this control
@@ -150,15 +143,15 @@
             Color of the Dial, by default Color.BLUE
         knob_color : Color, optional
             Color of the Knob, by default Color.RED
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         """
         super().__init__("KNOB", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             KnobConfig(
                 control_id,
                 title,
                 title_position,
                 knob_style,
                 dial_min,
                 dial_max,
@@ -195,15 +188,15 @@
 
     @property
     def red_value(self):
         """Return the red value for the dial"""
         return self._red_value
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Knob from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -220,15 +213,16 @@
             cfg_dict["max"],
             cfg_dict["redValue"],
             cfg_dict["showMinMax"],
             cfg_dict["sendOnlyOnRelease"],
             cfg_dict["dialFollowsKnob"],
             _get_color(cfg_dict["dialColor"]),
             _get_color(cfg_dict["knobColor"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         return self._knob_dial_state_str
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/label.py` & `dashio-3.4.0/dashio/iotcontrol/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self,
         control_id: str,
         title="A label",
         title_position=TitlePosition.BOTTOM,
         color=Color.WHITE,
         style=LabelStyle.BASIC,
         control_position=None,
+        column_no=1
     ):
         """Label
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -99,19 +100,19 @@
             control_id,
             title,
             title_position,
             color,
             style,
             control_position
         )
-        self._cfg_columnar.append(control_config)
+        self._app_columns_cfg[str(column_no)].append(control_config)
         self._state_str = ""
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates a label from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -121,11 +122,12 @@
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
             _get_color(cfg_dict["color"]),
             _get_label_style(cfg_dict["style"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/map.py` & `dashio-3.4.0/dashio/iotcontrol/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,16 @@
     """
 
     def __init__(
         self,
         control_id,
         title="A Map",
         title_position=TitlePosition.BOTTOM,
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """A Map control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device.
@@ -158,23 +159,23 @@
             Title of the control, by default "A Map"
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         title_position : TitlePosition, optional
             Position of the title when displayed on the iotdashboard app, by default None
         """
         super().__init__("MAP", control_id)
-        self._cfg_columnar.append(ControlConfig(control_id, title, control_position, title_position))
+        self._app_columns_cfg[str(column_no)].append(ControlConfig(control_id, title, control_position, title_position))
         self.tracks = {}
         self.tracks["DEFAULT"] = self.default_track
 
         self._message_rx_event = Event()
         self._message_rx_event += self._get_tracks_from_timestamp
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Map from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -182,15 +183,16 @@
         -------
         Map
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def _get_tracks_from_timestamp(self, msg):
         reply = ""
         try:
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/menu.py` & `dashio-3.4.0/dashio/iotcontrol/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         self,
         control_id: str,
         title="A Menu",
         title_position=TitlePosition.BOTTOM,
         text="A Menu with Text",
         style=MenuStyle.BASIC,
         icon_name=Icon.MENU,
-        control_position=None
+        control_position=None,
+        column_no=1
     ):
         """A Menu control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -101,28 +102,28 @@
             Position of the title when displayed on the iotdashboard app, by default None
         text : str, optional
             Menu text, by default "A Menu with Text"
         icon : Icon, optional
             Menu icon, by default Icon.MENU
         """
         super().__init__("MENU", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             MenuConfig(
                 control_id,
                 title,
                 title_position,
                 text,
                 style,
                 icon_name,
                 control_position
             )
         )
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Menu from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -133,15 +134,16 @@
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict.get("title", ""),
             _get_title_position(cfg_dict.get("titlePosition", "Bottom")),
             cfg_dict.get("text", ""),
             _get_menu_style(cfg_dict.get("style", "basic")),
             _get_icon(cfg_dict.get("iconName", "None")),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def add_control(self, control):
         """Add a control to the menu
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/ring_buffer.py` & `dashio-3.4.0/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/iotcontrol/selector.py` & `dashio-3.4.0/dashio/iotcontrol/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,42 +26,49 @@
 from .enums import TitlePosition
 
 
 class Selector(Control):
     """A Selector control
     """
 
-    def __init__(self, control_id: str, title="A Selector", title_position=TitlePosition.BOTTOM, control_position=None):
+    def __init__(
+        self,
+        control_id: str,
+        title="A Selector",
+        title_position=TitlePosition.BOTTOM,
+        control_position=None,
+        column_no=1
+    ):
         """A Selector control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
         title : str, optional
             Title of the control, by default "A Selector"
         control_position : ControlPosition, optional
             The position of the control on a DeviceView, by default None
         title_position : TitlePosition, optional
             Position of the title when displayed on the iotdashboard app, by default None
         """
         super().__init__("SLCTR", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             ControlConfig(
                 control_id,
                 title,
                 control_position,
                 title_position
             )
         )
         self._position = 0
         self.selection_list = []
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Selector from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -69,15 +76,16 @@
         -------
         Selector
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         _state_str = self._control_hdr_str + f"{self.position}\t"
         _state_str += "\t".join(map(str, self.selection_list))
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/slider.py` & `dashio-3.4.0/dashio/iotcontrol/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         slider_enabled=True,
         send_only_on_release=True,
         bar_follows_slider=False,
         bar_color=Color.BLUE,
         knob_color=Color.RED,
         bar_style=SliderBarStyle.SEG,
         control_position=None,
+        column_no=1
     ):
         """[summary]
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -156,15 +157,15 @@
             bar color, by default Color.BLUE
         knob_color : Color, optional
             knob color, by default Color.RED
         bar_style : SliderBarStyle, optional
             bar style, by default SliderBarStyle.SEGMENTED
         """
         super().__init__("SLDR", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             SliderConfig(
                 control_id,
                 title,
                 title_position,
                 bar_min,
                 bar_max,
                 red_value,
@@ -205,15 +206,15 @@
 
     @property
     def red_value(self):
         """Returns the red value"""
         return self._red_value
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates Slider from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -231,15 +232,16 @@
             cfg_dict["showMinMax"],
             cfg_dict["sliderEnabled"],
             cfg_dict["sendOnlyOnRelease"],
             cfg_dict["barFollowsSlider"],
             _get_color(cfg_dict["barColor"]),
             _get_color(cfg_dict["knobColor"]),
             _get_bar_style(cfg_dict["barStyle"]),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         return self._bar_slider_state_str
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/textbox.py` & `dashio-3.4.0/dashio/iotcontrol/textbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         text_align=TextAlignment.LEFT,
         text_format=TextFormat.NONE,
         units="",
         precision=Precision.OFF,
         keyboard_type=Keyboard.ALL,
         close_keyboard_on_send=True,
         control_position=None,
+        column_no=1
     ):
         """A TextBox control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -124,15 +125,15 @@
             precision, by default Precision.OFF
         keyboard_type : Keyboard, optional
             Keyboard type for the textbox, by default Keyboard.ALL
         close_keyboard_on_send : bool, optional
             Set to True to close keyboard on close, by default True
         """
         super().__init__("TEXT", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             TextBoxConfig(
                 control_id,
                 title,
                 title_position,
                 text,
                 text_align,
                 text_format,
@@ -145,15 +146,15 @@
         )
         self.text = text.translate(BAD_CHARS)
 
     def get_state(self):
         return self._control_hdr_str + f"{self.text}\n"
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates TextBox from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -168,15 +169,16 @@
             "",
             _get_text_align(cfg_dict["textAlign"]),
             _get_text_format(cfg_dict["format"]),
             cfg_dict["units"],
             _get_precision(cfg_dict["precision"]),
             _get_keyboard_type(cfg_dict["kbdType"]),
             cfg_dict["closeKbdOnSend"],
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     @property
     def text(self) -> str:
         """TextBox text
```

### Comparing `dashio-3.3.9/dashio/iotcontrol/time_graph.py` & `dashio-3.4.0/dashio/iotcontrol/time_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
         y_axis_min=0.0,
         y_axis_max=1000.0,
         y_axis_num_bars=5,
         y_axis_label_rt='',
         y_axis_min_rt=0.0,
         y_axis_max_rt=1000.0,
         control_position=None,
+        column_no=1
     ):
         """A Timegraph control
 
         Parameters
         ----------
         control_id : str
             An unique control identity string. The control identity string must be a unique string for each control per device
@@ -237,15 +238,15 @@
             Min value for the Y axis, by default 0.0
         y_axis_max : float, optional
             Max value for the Y axis, by default 100.0
         y_axis_num_bars : int, optional
             The number of bars to display on the graph, by default 5
         """
         super().__init__("TGRPH", control_id)
-        self._cfg_columnar.append(
+        self._app_columns_cfg[str(column_no)].append(
             TimeGraphConfig(
                 control_id,
                 title,
                 title_position,
                 y_axis_label,
                 y_axis_min,
                 y_axis_max,
@@ -288,15 +289,15 @@
 
     @property
     def y_axis_num_bars(self):
         """Returns the y axis number of bars"""
         return self.y_axis_num_bars
 
     @classmethod
-    def from_cfg_dict(cls, cfg_dict: dict):
+    def from_cfg_dict(cls, cfg_dict: dict, column_no=1):
         """Instatiates TimeGraph from cfg dictionary
 
         Parameters
         ----------
         cfg_dict : dict
             A dictionary usually loaded from a config json from IoTDashboard App
 
@@ -311,15 +312,16 @@
             cfg_dict["yAxisLabel"],
             cfg_dict["yAxisMin"],
             cfg_dict["yAxisMax"],
             cfg_dict["yAxisNumBars"],
             cfg_dict.get("yAxisLabelRt", ''),
             cfg_dict.get("yAxisMinRt", 0.0),
             cfg_dict.get("yAxisMaxRt", 1000.0),
-            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
+            ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
+            column_no
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def get_state(self):
         state_str = ""
         for key, line in self.line_dict.items():
```

### Comparing `dashio-3.3.9/dashio/ip.py` & `dashio-3.4.0/dashio/ip.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,19 +20,29 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import socket
 
 
-def get_local_ip_address():
+def get_local_ip_v4_address():
     """Find the external IP address."""
     test_s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't even have to be reachable
         test_s.connect(('10.255.255.255', 1))
         i_address = test_s.getsockname()[0]
     except socket.error:
         i_address = '127.0.0.1'
     finally:
         test_s.close()
     return i_address
+
+
+def get_local_ip_v6_address():
+    """Find the external IP address."""
+    i_address = socket.getaddrinfo(socket.gethostname(), None, socket.AF_INET6)[1][4][0]
+    return i_address
+
+def is_port_in_use(ip_address, port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as port_s:
+        return port_s.connect_ex((ip_address, port)) == 0
```

### Comparing `dashio-3.3.9/dashio/load_config.py` & `dashio-3.4.0/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/serialconnection.py` & `dashio-3.4.0/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/dashio/tcpconnection.py` & `dashio-3.4.0/dashio/tcpconnection.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,19 +56,14 @@
             Add a device to the connection.
         """
         if device.device_id not in self.local_device_id_list:
             device.register_connection(self)
             self.local_device_id_list.append(device.device_id)
             self.z_conf.add_device(device.device_id)
 
-    @staticmethod
-    def _is_port_in_use(ip_address, port):
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as port_s:
-            return port_s.connect_ex((ip_address, port)) == 0
-
     def __init__(self, ip_address="*", port=5650, use_zero_conf=True, context: zmq.Context = None):
         """TCP Connection
 
         Parameters
         ---------
             ip_address : str, optional
                 IP Address to use. Defaults to "*" - forces The TCP connection to find the ip address attached to the local network.
@@ -83,22 +78,22 @@
         threading.Thread.__init__(self, daemon=True)
         self.context = context or zmq.Context.instance()
         self.zmq_connection_uuid = "TCP:" + shortuuid.uuid()
         self.b_zmq_connection_uuid = self.zmq_connection_uuid.encode('utf-8')
         self.use_zeroconf = use_zero_conf
 
         if ip_address == "*":
-            self.local_ip = ip.get_local_ip_address()
+            self.local_ip = ip.get_local_ip_v4_address()
         else:
             self.local_ip = ip_address
         self.local_port = port
-        while self._is_port_in_use(self.local_ip, self.local_port) and use_zero_conf:
+        while ip.is_port_in_use(self.local_ip, self.local_port) and use_zero_conf:
             # increment port until we find one that is free.
             self.local_port += 1
-        self.ext_url = "tcp://" + self.local_ip + ":" + str(self.local_port)
+        self.ext_url = "tcp://*:" + str(self.local_port)
 
         self.socket_ids = []
         self.local_device_id_list = []
         self.remote_connection_dict = {}
         self.remote_device_con_dict = {}
         self.remote_device_id_msg_dict = {}
         self._device_id_action_station_list = []
@@ -121,27 +116,27 @@
 
         if self.use_zeroconf:
             self.z_conf.close()
         self.running = False
 
     def _connect_remote_device(self, msg: dict):
         """Connect to remote device"""
-        ip_address = msg['address']
+        server = msg['server']
         port = msg['port']
-        url = f"tcp://{ip_address}:{port}"
+        url = f"tcp://{server}:{port}"
         self.tcpsocket.connect(url)
         socket_id = self.tcpsocket.getsockopt(zmq.IDENTITY)
-        ip_b = ip_address + ':' + port
+        ip_b = server + ':' + port
         if ip_b not in self.tcp_ip_2_id_dict:
             try:
                 logging.debug("Sending WHO to ID: %s", socket_id.hex())
                 self.tcpsocket.send(socket_id, zmq.SNDMORE)
                 self.tcpsocket.send_string('\tWHO\n')
-                self.tcp_id_2_ip_dict[socket_id] = ip_address + ':' + port
-                self.tcp_ip_2_id_dict[ip_address + ':' + port] = socket_id
+                self.tcp_id_2_ip_dict[socket_id] = ip_b
+                self.tcp_ip_2_id_dict[ip_b] = socket_id
             except zmq.error.ZMQError:
                 logging.debug("Sending TX Error.")
                 self.tcpsocket.send(b'')
         time.sleep(0.1)
         if socket_id not in self.socket_ids:
             logging.debug("Added Socket ID: %s", socket_id.hex())
             self.socket_ids.append(socket_id)
@@ -153,17 +148,17 @@
             self.tcpsocket.send(self.tcp_ip_2_id_dict[ip_key], zmq.SNDMORE)
             self.tcpsocket.send(b'', zmq.NOBLOCK)
             del self.tcp_ip_2_id_dict[ip_key]
 
     def _send_remote_device(self, r_device_id, msg):
         if r_device_id in self.remote_device_id_msg_dict:
             remote = self.remote_device_id_msg_dict[r_device_id]
-            ip_address = remote['address']
+            server = msg['server']
             port = remote['port']
-            url = f"tcp://{ip_address}:{port}"
+            url = f"tcp://{server}:{port}"
             self.tcpsocket.connect(url)
             socket_id = self.tcpsocket.getsockopt(zmq.IDENTITY)
             self.tcpsocket.send(socket_id, zmq.SNDMORE)
             self.tcpsocket.send(msg)
             self.tcpsocket.send(socket_id, zmq.SNDMORE)
             self.tcpsocket.send(b'', zmq.NOBLOCK)
 
@@ -264,23 +259,23 @@
         message = self.tcpsocket.recv()
         if tcp_id not in self.socket_ids and tcp_id not in self.tcp_id_2_ip_dict:
             logging.debug("Added Socket ID: %s", tcp_id.hex())
             self.socket_ids.append(tcp_id)
         if message:
             logging.debug("TCP RX: %s\n%s", tcp_id.hex(), message.decode().rstrip())
             msg_from = self.b_zmq_connection_uuid + b":" + tcp_id
-            tx_zmq_pub.send_multipart([message, msg_from])
+            for sub_msg in message.split(b'\n'):
+                tx_zmq_pub.send_multipart([sub_msg, msg_from])
         else:
             if tcp_id in self.socket_ids:
                 logging.debug("Removed Socket ID: %s", tcp_id.hex())
                 self.socket_ids.remove(tcp_id)
 
     def run(self):
         self.tcpsocket = self.context.socket(zmq.STREAM)
-
         self.rx_zmq_sub = self.context.socket(zmq.SUB)
         # Subscribe on ALL, COMMAND, and my zmq_connection_uuid
         self.rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "ALL")
         self.rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "COMMAND")
         self.rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, "TCP")
         self.rx_zmq_sub.setsockopt_string(zmq.SUBSCRIBE, self.zmq_connection_uuid)
```

### Comparing `dashio-3.3.9/dashio/zeroconf_service.py` & `dashio-3.4.0/dashio/zeroconf_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
         self.zmq_socket.send(json.dumps(msg).encode())
 
     def _send_info(self, connection_uuid, info):
         try:
             device_ids = info.properties[b'deviceID'].decode()
         except KeyError:
             device_ids = ''
+        logging.debug("Zcon INFO: %s", info)
         for address in info.addresses:
             msg = {
                 'objectType': 'zeroConfUpdate',
+                'server': str(info.server),
                 'address': socket.inet_ntoa(address),
                 'deviceID': device_ids,
                 'connectionID': connection_uuid,
                 'port': str(info.port)
             }
             self._send_msg(msg)
```

### Comparing `dashio-3.3.9/dashio/zmqconnection.py` & `dashio-3.4.0/dashio/zmqconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self.b_zmq_connection_id = self.zmq_connection_uuid.encode('utf-8')
 
         host_name = socket.gethostname()
         host_list = host_name.split(".")
         # rename for .local mDNS advertising
         self.host_name = f"{host_list[0]}.local"
 
-        self.local_ip = ip.get_local_ip_address()
+        self.local_ip = ip.get_local_ip_v4_address()
         self.zeroconf = Zeroconf(ip_version=IPVersion.V4Only)
         self._zconf_publish_zmq(sub_port, pub_port)
         self.start()
 
     def _add_device_rx(self, msg_dict):
         """Connect to another device"""
         device_id = msg_dict["deviceID"]
```

### Comparing `dashio-3.3.9/dashio.egg-info/PKG-INFO` & `dashio-3.4.0/dashio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.9
+Version: 3.4.0
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6.0
+Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
```

### Comparing `dashio-3.3.9/dashio.egg-info/SOURCES.txt` & `dashio-3.4.0/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/setup.cfg` & `dashio-3.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = dashio
 description = DashIO interface library
 author = James Boulton
 author_email = "james@dashio.com"
 license = MIT
 license_files = LICENSE
 classifiers = 
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
 	Operating System :: OS Independent
 url = "https://dashio.io"
 download_url = "https://github.com/dashio-connect/python-dashio"
 long_description = long_description
 long_description_content_type = "text/markdown"
 
 [options]
@@ -20,15 +20,16 @@
 	paho-mqtt
 	pyzmq
 	python-dateutil
 	zeroconf
 	shortuuid
 	pyserial
 	astral
-python_requires = >=3.6
+	pydantic
+python_requires = >=3.7.0
 zip_safe = no
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
 	pytest-cov>=2.0
 	flake8>=3.9
```

### Comparing `dashio-3.3.9/setup.py` & `dashio-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.9",
+    version="3.4.0",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
     packages=find_packages(),
     license="MIT",
-    classifiers=["Programming Language :: Python :: 3.6", "Operating System :: OS Independent"],
-    install_requires=["paho-mqtt", "pyzmq", "python-dateutil", "zeroconf", "shortuuid", "pyserial", "astral"],
-    python_requires='>3.6.0',
+    classifiers=["Programming Language :: Python :: 3.7", "Operating System :: OS Independent"],
+    install_requires=["paho-mqtt", "pyzmq", "python-dateutil", "zeroconf", "shortuuid", "pyserial", "astral", "pydantic"],
+    python_requires='>3.7.0',
     scripts=['utilities/c64_encode', 'utilities/c64_decode'],
 )
```

### Comparing `dashio-3.3.9/tests/test_button.py` & `dashio-3.4.0/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_button_group.py` & `dashio-3.4.0/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_chart.py` & `dashio-3.4.0/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_dashdevice.py` & `dashio-3.4.0/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_device_view.py` & `dashio-3.4.0/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_dial.py` & `dashio-3.4.0/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_direction.py` & `dashio-3.4.0/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_event_log.py` & `dashio-3.4.0/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_knob.py` & `dashio-3.4.0/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_label.py` & `dashio-3.4.0/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_map.py` & `dashio-3.4.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_menu.py` & `dashio-3.4.0/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_selector.py` & `dashio-3.4.0/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_slider.py` & `dashio-3.4.0/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_textbox.py` & `dashio-3.4.0/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/tests/test_time_graph.py` & `dashio-3.4.0/tests/test_time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/utilities/c64_decode` & `dashio-3.4.0/utilities/c64_decode`

 * *Files identical despite different names*

### Comparing `dashio-3.3.9/utilities/c64_encode` & `dashio-3.4.0/utilities/c64_encode`

 * *Files identical despite different names*

