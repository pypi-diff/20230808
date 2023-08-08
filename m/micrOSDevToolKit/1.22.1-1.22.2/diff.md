# Comparing `tmp/micrOSDevToolKit-1.22.1.tar.gz` & `tmp/micrOSDevToolKit-1.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.22.1.tar", last modified: Tue Aug  8 19:16:51 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.22.2.tar", last modified: Tue Aug  8 21:51:17 2023, max compression
```

## Comparing `micrOSDevToolKit-1.22.1.tar` & `micrOSDevToolKit-1.22.2.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.758831 micrOSDevToolKit-1.22.1/
--rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.22.1/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-08 19:16:51.758227 micrOSDevToolKit-1.22.1/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45495 2023-08-05 00:33:02.000000 micrOSDevToolKit-1.22.1/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.22.1/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.296434 micrOSDevToolKit-1.22.1/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.290121 micrOSDevToolKit-1.22.1/env/driver_cp210x/
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.330894 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/
--rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
--rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
--rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
--rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.331702 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
--rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.333421 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
--rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
--rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
--rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.335664 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
--rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.337667 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
--rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.350082 micrOSDevToolKit-1.22.1/env/driver_cp210x/macOS_VCP_Driver/
--rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
--rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.360253 micrOSDevToolKit-1.22.1/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.1/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.1/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.362273 micrOSDevToolKit-1.22.1/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.22.1/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.397904 micrOSDevToolKit-1.22.1/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.22.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.22.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.532375 micrOSDevToolKit-1.22.1/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.22.1/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.22.1/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.22.1/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.1/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.22.1/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6916 2023-08-07 15:52:09.000000 micrOSDevToolKit-1.22.1/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11532 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.1/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.22.1/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_aht10.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    19504 2023-08-04 14:14:52.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_rgbcct.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.1/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.22.1/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.22.1/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.22.1/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.22.1/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11571 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.1/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-08-06 19:01:22.000000 micrOSDevToolKit-1.22.1/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.22.1/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.1/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.22.1/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.22.1/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.22.1/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.22.1/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.548917 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-08 19:16:50.000000 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-08 19:16:51.000000 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-08 19:16:50.000000 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-08 19:16:50.000000 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-08 19:16:50.000000 micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-08 19:16:51.759059 micrOSDevToolKit-1.22.1/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-08 16:29:05.000000 micrOSDevToolKit-1.22.1/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.568471 micrOSDevToolKit-1.22.1/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.22.1/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.22.1/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.22.1/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12260 2023-08-08 17:08:28.000000 micrOSDevToolKit-1.22.1/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.22.1/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.586944 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.591621 micrOSDevToolKit-1.22.1/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.22.1/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5813 2023-08-08 18:52:11.000000 micrOSDevToolKit-1.22.1/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6221 2023-08-08 16:07:16.000000 micrOSDevToolKit-1.22.1/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.22.1/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.22.1/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.609463 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.640435 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.22.1/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.641291 micrOSDevToolKit-1.22.1/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.22.1/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.641667 micrOSDevToolKit-1.22.1/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.642065 micrOSDevToolKit-1.22.1/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 19:16:51.755665 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4147 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_aht10.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6207 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-08 09:53:34.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rgbcct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3760 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5714 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.218020 micrOSDevToolKit-1.22.2/
+-rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.22.2/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-08 21:51:17.217369 micrOSDevToolKit-1.22.2/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45495 2023-08-05 00:33:02.000000 micrOSDevToolKit-1.22.2/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.22.2/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.533012 micrOSDevToolKit-1.22.2/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.517811 micrOSDevToolKit-1.22.2/env/driver_cp210x/
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.568754 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/
+-rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
+-rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
+-rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
+-rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.570372 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
+-rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.572742 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
+-rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
+-rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
+-rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.586975 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
+-rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.603155 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
+-rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.637531 micrOSDevToolKit-1.22.2/env/driver_cp210x/macOS_VCP_Driver/
+-rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
+-rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.656899 micrOSDevToolKit-1.22.2/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.2/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.2/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.676327 micrOSDevToolKit-1.22.2/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.22.2/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:16.837740 micrOSDevToolKit-1.22.2/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.22.2/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.22.2/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.024364 micrOSDevToolKit-1.22.2/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.22.2/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.22.2/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.22.2/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.2/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.22.2/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6916 2023-08-07 15:52:09.000000 micrOSDevToolKit-1.22.2/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11532 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.2/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.22.2/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_aht10.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19504 2023-08-04 14:14:52.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_rgbcct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.2/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.22.2/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.22.2/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.22.2/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.22.2/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11571 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.2/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-08-06 19:01:22.000000 micrOSDevToolKit-1.22.2/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.22.2/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.2/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.22.2/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.22.2/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.22.2/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.22.2/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.027925 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-08 21:51:16.000000 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-08 21:51:16.000000 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-08 21:51:16.000000 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-08 21:51:16.000000 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-08 21:51:16.000000 micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-08 21:51:17.218162 micrOSDevToolKit-1.22.2/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-08 21:43:16.000000 micrOSDevToolKit-1.22.2/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.041585 micrOSDevToolKit-1.22.2/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.22.2/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.22.2/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.22.2/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12260 2023-08-08 17:08:28.000000 micrOSDevToolKit-1.22.2/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.22.2/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.067667 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.074215 micrOSDevToolKit-1.22.2/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.22.2/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5813 2023-08-08 18:52:11.000000 micrOSDevToolKit-1.22.2/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6221 2023-08-08 16:07:16.000000 micrOSDevToolKit-1.22.2/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.22.2/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.22.2/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.094602 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.131798 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16981 2023-08-08 21:44:49.000000 micrOSDevToolKit-1.22.2/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.132401 micrOSDevToolKit-1.22.2/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.22.2/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.132886 micrOSDevToolKit-1.22.2/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.133643 micrOSDevToolKit-1.22.2/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-08 21:51:17.215558 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4147 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_aht10.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6207 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-08 09:53:34.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rgbcct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3760 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5714 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-08 09:53:35.000000 micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.22.1/PKG-INFO` & `micrOSDevToolKit-1.22.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.22.1
+Version: 1.22.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.22.1/README.md` & `micrOSDevToolKit-1.22.2/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/devToolKit.py` & `micrOSDevToolKit-1.22.2/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt` & `micrOSDevToolKit-1.22.2/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/media/dnd.png` & `micrOSDevToolKit-1.22.2/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/media/logo.png` & `micrOSDevToolKit-1.22.2/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/media/logo_mini.png` & `micrOSDevToolKit-1.22.2/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.22.2/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.2/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.2/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.22.2/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.22.2/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.2/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.22.2/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Common.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.22.2/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Debug.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.22.2/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.22.2/micrOS/source/InterpreterShell.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.22.2/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_aht10.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_aht10.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_rgbcct.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_rgbcct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.22.2/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Network.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Notify.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.22.2/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.22.2/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/Time.py` & `micrOSDevToolKit-1.22.2/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.22.2/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.22.2/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.22.2/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOS/source/urequests.py` & `micrOSDevToolKit-1.22.2/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.22.1
+Version: 1.22.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.22.1/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.22.2/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/setup.py` & `micrOSDevToolKit-1.22.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.22.1',
+    version='1.22.2',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.22.1/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.22.2/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.22.2/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.22.2/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/Gateway.py` & `micrOSDevToolKit-1.22.2/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.22.2/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.22.2/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.22.2/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.22.2/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.22.2/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.22.2/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.22.2/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.22.2/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.22.2/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/socketClient.py` & `micrOSDevToolKit-1.22.2/toolkit/socketClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,28 +125,28 @@
     @staticmethod
     def save_micrOS_device_cache():
         ConnectionData.read_micrOS_device_cache()
         cache_path = ConnectionData.DEVICE_CACHE_PATH
         print("Write micrOS device cache: {}".format(cache_path))
         with open(cache_path, 'w') as f:
             ConnectionData.DEFAULT_CONFIG_FRAGMNENT.update(ConnectionData.MICROS_DEVICES)
-            json.dump(ConnectionData.MICROS_DEVICES, f, indent=4)
+            json.dump(ConnectionData.DEFAULT_CONFIG_FRAGMNENT, f, indent=4)
 
     @staticmethod
     def read_micrOS_device_cache():
         cache_path = ConnectionData.DEVICE_CACHE_PATH
         if os.path.isfile(cache_path):
             print("Load micrOS device cache: {}".format(cache_path))
             with open(cache_path, 'r') as f:
                 cache_content = json.load(f)
                 cache_content.update(ConnectionData.MICROS_DEVICES)
                 ConnectionData.MICROS_DEVICES = cache_content
         else:
             print("Load micrOS device cache not found: {}".format(cache_path))
-            ConnectionData.MICROS_DEVICES = ConnectionData.DEFAULT_CONFIG_FRAGMNENT
+            #ConnectionData.MICROS_DEVICES = ConnectionData.DEFAULT_CONFIG_FRAGMNENT
         return ConnectionData.MICROS_DEVICES
 
     @staticmethod
     def select_device(device_tag=None):
         """
         :param device_tag: uid or devip or fuid
         :return: IP, PORT, FID
```

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_aht10.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_aht10.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_rgbcct.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_rgbcct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.22.1/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.22.2/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

