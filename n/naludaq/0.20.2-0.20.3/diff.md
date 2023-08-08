# Comparing `tmp/naludaq-0.20.2.tar.gz` & `tmp/naludaq-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.20.2.tar", last modified: Wed Jul 26 22:14:44 2023, max compression
+gzip compressed data, was "naludaq-0.20.3.tar", last modified: Tue Aug  8 02:11:03 2023, max compression
```

## Comparing `naludaq-0.20.2.tar` & `naludaq-0.20.3.tar`

### file list

```diff
@@ -1,261 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.249231 naludaq-0.20.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-26 22:14:27.000000 naludaq-0.20.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-26 22:14:44.249231 naludaq-0.20.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-26 22:14:27.000000 naludaq-0.20.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-26 22:14:27.000000 naludaq-0.20.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:14:44.249231 naludaq-0.20.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-26 22:14:27.000000 naludaq-0.20.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.189230 naludaq-0.20.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.197230 naludaq-0.20.2/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.197230 naludaq-0.20.2/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.201230 naludaq-0.20.2/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.201230 naludaq-0.20.2/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38000 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.201230 naludaq-0.20.2/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (123)    30012 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.205230 naludaq-0.20.2/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.205230 naludaq-0.20.2/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.205230 naludaq-0.20.2/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.209231 naludaq-0.20.2/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.209231 naludaq-0.20.2/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.209231 naludaq-0.20.2/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/asocv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.209231 naludaq-0.20.2/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.213230 naludaq-0.20.2/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.213230 naludaq-0.20.2/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.213230 naludaq-0.20.2/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.217231 naludaq-0.20.2/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.217231 naludaq-0.20.2/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.221231 naludaq-0.20.2/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.221231 naludaq-0.20.2/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.221231 naludaq-0.20.2/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.225231 naludaq-0.20.2/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.225231 naludaq-0.20.2/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.225231 naludaq-0.20.2/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.229231 naludaq-0.20.2/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.229231 naludaq-0.20.2/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.233231 naludaq-0.20.2/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.233231 naludaq-0.20.2/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.237231 naludaq-0.20.2/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.237231 naludaq-0.20.2/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.237231 naludaq-0.20.2/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.237231 naludaq-0.20.2/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.241231 naludaq-0.20.2/src/naludaq/tools/lookup_table/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/lookup_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/lookup_table/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/lookup_table/lookup_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.241231 naludaq-0.20.2/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/bayesian_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.241231 naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.245231 naludaq-0.20.2/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.245231 naludaq-0.20.2/src/naludaq/tools/pedestals/_new/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/_new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/_new/aav3.py
--rw-r--r--   0 runner    (1001) docker     (123)    25319 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/_new/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/_new/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_acq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.245231 naludaq-0.20.2/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/threshold_scan/threshold_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.249231 naludaq-0.20.2/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.249231 naludaq-0.20.2/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-26 22:14:27.000000 naludaq-0.20.2/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.197230 naludaq-0.20.2/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-26 22:14:44.000000 naludaq-0.20.2/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-26 22:14:44.000000 naludaq-0.20.2/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:14:44.000000 naludaq-0.20.2/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-26 22:14:44.000000 naludaq-0.20.2/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 22:14:44.000000 naludaq-0.20.2/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:14:44.249231 naludaq-0.20.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-26 22:14:27.000000 naludaq-0.20.2/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-08 02:10:43.000000 naludaq-0.20.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-08-08 02:11:03.146258 naludaq-0.20.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-08-08 02:10:43.000000 naludaq-0.20.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 02:10:43.000000 naludaq-0.20.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:11:03.146258 naludaq-0.20.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 02:10:43.000000 naludaq-0.20.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.114257 naludaq-0.20.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38000 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (123)    30012 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.122257 naludaq-0.20.3/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.122257 naludaq-0.20.3/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.122257 naludaq-0.20.3/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.126258 naludaq-0.20.3/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.130257 naludaq-0.20.3/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.130257 naludaq-0.20.3/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.130257 naludaq-0.20.3/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.130257 naludaq-0.20.3/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.130257 naludaq-0.20.3/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.134258 naludaq-0.20.3/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.134258 naludaq-0.20.3/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.134258 naludaq-0.20.3/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.134258 naludaq-0.20.3/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.134258 naludaq-0.20.3/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.138258 naludaq-0.20.3/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.138258 naludaq-0.20.3/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.138258 naludaq-0.20.3/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.138258 naludaq-0.20.3/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/bayesian_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.142258 naludaq-0.20.3/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/src/naludaq/tools/pedestals/_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/_new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/_new/aav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25319 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/_new/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/_new/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/threshold_scan/threshold_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-08 02:10:43.000000 naludaq-0.20.3/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.118257 naludaq-0.20.3/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-08-08 02:11:03.000000 naludaq-0.20.3/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-08-08 02:11:03.000000 naludaq-0.20.3/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:11:03.000000 naludaq-0.20.3/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-08 02:11:03.000000 naludaq-0.20.3/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 02:11:03.000000 naludaq-0.20.3/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:03.146258 naludaq-0.20.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 02:10:43.000000 naludaq-0.20.3/tests/test_naludaq.py
```

### Comparing `naludaq-0.20.2/LICENSE.txt` & `naludaq-0.20.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/PKG-INFO` & `naludaq-0.20.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.20.2
+Version: 0.20.3
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.20.2/README.md` & `naludaq-0.20.3/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/pyproject.toml` & `naludaq-0.20.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/setup.py` & `naludaq-0.20.3/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/client.py` & `naludaq-0.20.3/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/context.py` & `naludaq-0.20.3/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/exceptions.py` & `naludaq-0.20.3/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.20.3/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/managers/config.py` & `naludaq-0.20.3/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/managers/connection.py` & `naludaq-0.20.3/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/managers/io.py` & `naludaq-0.20.3/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/models/acquisition.py` & `naludaq-0.20.3/src/naludaq/backend/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/backend/models/device.py` & `naludaq-0.20.3/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/__init__.py` & `naludaq-0.20.3/src/naludaq/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/board_inits.py` & `naludaq-0.20.3/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.20.3/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.20.3/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/_UART.py` & `naludaq-0.20.3/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/_USB.py` & `naludaq-0.20.3/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/base_connection.py` & `naludaq-0.20.3/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.20.3/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/tcp.py` & `naludaq-0.20.3/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/connections/udp.py` & `naludaq-0.20.3/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/__init__.py` & `naludaq-0.20.3/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.20.3/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.20.3/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.20.3/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.20.3/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.20.3/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.20.3/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.20.3/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/board/params.py` & `naludaq-0.20.3/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/__init__.py` & `naludaq-0.20.3/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/_chip.py` & `naludaq-0.20.3/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/_common.py` & `naludaq-0.20.3/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/_fpga.py` & `naludaq-0.20.3/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/analog_registers.py` & `naludaq-0.20.3/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/chip_selection.py` & `naludaq-0.20.3/src/naludaq/communication/chip_selection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/control_registers.py` & `naludaq-0.20.3/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/digital_registers.py` & `naludaq-0.20.3/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/i2c.py` & `naludaq-0.20.3/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/i2c_registers.py` & `naludaq-0.20.3/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/communication/registers.py` & `naludaq-0.20.3/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.20.3/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.20.3/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/board/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 All functions to communicate with the Nalu boards are
 collected here. The Facade naludaq is intended to simplify
 the interface for general use.
 """
 import logging
 
 from .aodsoc import BoardControllerAodsoc
-from .asocv3 import BoardControllerAsocv3
 from .default import BoardController
 from .hdsoc import HDSoCBoardController
 from .oleas import BoardControllerOleas
 from .trbhm import TrbhmBoardController
 from .udc import UDCBoardController
 from .upac import UpacBoardController
 from .upac96 import UPAC96BoardController
@@ -26,15 +25,14 @@
         board (Board): the board object.
 
     Returns:
         The appropriate BoardController for the given board.
     """
     return {
         # 'aodsoc_aods': BoardControllerAodsoc,
-        "asocv3": BoardControllerAsocv3,
         "aodsoc_aods": BoardControllerOleas,
         "aodsoc_asoc": BoardControllerAodsoc,
         "hdsocv1": HDSoCBoardController,
         "hdsocv1_evalr1": HDSoCBoardController,
         "hdsocv1_evalr2": HDSoCBoardController,
         "trbhm": TrbhmBoardController,
         "udc16": UDCBoardController,
```

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/default.py` & `naludaq-0.20.3/src/naludaq/controllers/board/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
     It is the interface between the application and the board.
     The Analytics package or the GUI uses this class to communicate with the
     hardware. Keeps track of all registers etc.
     It doesn't receive continous data, the data acquisition module should be used for that.
     """
 
+    def __init__(self, board):
+        super().__init__(board)
+        self._trigger_wait_cycles = board.params.get("ext_trig_cycles", 3)
+
     def start_readout(
         self,
         trig="self",
         lb="trigrel",
         acq="raw",
         dig_head=False,
         ped="zero",
@@ -203,27 +207,32 @@
         """Toggles the "stopacq" signal on the readout module.
 
         It's equivalent of asking it nicely to stop reading.
         """
         self._write_control_register("stopacq", True)
         self._write_control_register("stopacq", False)
 
-    def toggle_trigger(self):
+    def toggle_trigger(self, cycles: int = None):
         """Toggles the ext trigger using software.
 
-        Sends the entire toggle as a single command, since individual
-        register writes hold the pin high for too long, causing
-        too many triggers.
+        Args:
+            cycles (int): number of cycles to hold the trigger high for.
+                If not provided, a default value is used.
         """
-        cr = ControlRegisters(self.board)
-        wait_cmd = "AE000001"
-        exttrig_high_cmd = cr.generate_write("exttrig", True)
-        exttrig_low_cmd = cr.generate_write("exttrig", False)
-        toggle_cmd = wait_cmd + exttrig_high_cmd + exttrig_low_cmd
-        self._send_command(toggle_cmd)
+        if cycles is None:
+            cycles = self._trigger_wait_cycles
+        if not isinstance(cycles, int):
+            raise TypeError(f'"cycles" must be an int')
+        if cycles < 1:
+            raise ValueError(f'"cycles" must be at least 1, got {cycles}')
+        if cycles > 2**16 - 1:
+            raise ValueError(
+                f'"cycles" must be at most {2**16 - 1} (16-bits), got {cycles}'
+            )
+        self._send_command(f"C000{cycles:04X}")
 
     def reset_board(self):
         """Try and reset the board.
 
         In case the FPGA get stuck this can help reset the state.
         """
         time.sleep(0.02)
```

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/board/hdsoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,25 +58,14 @@
         """Toggles the "stopacq" signal on the readout module.
 
         It's equivalent of asking it nicely to stop reading.
         """
         super().stop_readout()
         self.clear_buffer()
 
-    def toggle_trigger(self, cycles=3):
-        """Toggles the ext trigger using software."""
-        if not isinstance(cycles, int):
-            raise TypeError('"cycles" must be an int')
-        if cycles < 1:
-            raise ValueError('"cycles" must be at least 1')
-        if cycles > 2**16 - 1:
-            raise ValueError(f'"cycles" must be at most {2**16 - 1} (16-bits)')
-        cmd = f"C000{cycles:04X}"
-        self._send_command(cmd)
-
     def digital_reset(self):
         """Toggles the "reset" port on the readout module.
 
         Forcibly returns the chip to default state.
         """
         self._write_control_register("idig_rst", True)
         self._write_control_register("idig_rst", False)
```

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/oleas.py` & `naludaq-0.20.3/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.20.3/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/udc.py` & `naludaq-0.20.3/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/upac.py` & `naludaq-0.20.3/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/board/upac96.py` & `naludaq-0.20.3/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.20.3/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/connection/upac.py` & `naludaq-0.20.3/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.20.3/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/aardvarcv3.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.20.3/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.20.3/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.20.3/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.20.3/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/project_controller.py` & `naludaq-0.20.3/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.20.3/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/readout/default.py` & `naludaq-0.20.3/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.20.3/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.20.3/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/tia/base.py` & `naludaq-0.20.3/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/default.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.20.3/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/__init__.py` & `naludaq-0.20.3/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/debugdaq.py` & `naludaq-0.20.3/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/lightdaq.py` & `naludaq-0.20.3/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/preprocess.py` & `naludaq-0.20.3/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/__init__.py` & `naludaq-0.20.3/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.20.3/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.20.3/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.20.3/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.20.3/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.20.3/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.20.3/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.20.3/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.20.3/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/devices/eeprom.py` & `naludaq-0.20.3/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/devices/i2c_device.py` & `naludaq-0.20.3/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/devices/ltc2990.py` & `naludaq-0.20.3/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/decorators.py` & `naludaq-0.20.3/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/exceptions.py` & `naludaq-0.20.3/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/helper_functions.py` & `naludaq-0.20.3/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/register_cache.py` & `naludaq-0.20.3/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/semiton.py` & `naludaq-0.20.3/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/helpers/validations.py` & `naludaq-0.20.3/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/io/__init__.py` & `naludaq-0.20.3/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/io/csv_writer.py` & `naludaq-0.20.3/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/io/hdf5.py` & `naludaq-0.20.3/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/io/io_manager.py` & `naludaq-0.20.3/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/models/acq_converters.py` & `naludaq-0.20.3/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/models/acquisition.py` & `naludaq-0.20.3/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/naludaq.py` & `naludaq-0.20.3/src/naludaq/naludaq.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if not self.board.using_new_backend:
             self.daq = DataAcquisitionController(board, working_dir, start_workers)
             self.daq.preprocess = Preprocess(board)
 
         self.readout_settings = {
             "trig": "ext",
             "lb": "trigrel",
-            "acq": "ped",
+            "acq": "raw",
             "ped": "zero",
             "readoutEn": True,
             "singleEv": False,
         }
 
         self.is_capturing = False
         self.is_connected = False
```

### Comparing `naludaq-0.20.2/src/naludaq/parsers/__init__.py` & `naludaq-0.20.3/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/answer_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/base.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/siread.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.20.3/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/parser.py` & `naludaq-0.20.3/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/udc_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/parsers/upac_parser.py` & `naludaq-0.20.3/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.20.3/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.20.3/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.20.3/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.20.3/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/autoaction.py` & `naludaq-0.20.3/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.20.3/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/board_backup.py` & `naludaq-0.20.3/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.20.3/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/data_collector.py` & `naludaq-0.20.3/src/naludaq/tools/data_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             `TimeoutError` if no data is captured in `timeout` retries.
         """
 
         rdt_controller = get_readout_controller(self.board)
         readout_settings = {
             "trig": trig_type,
             "lb": lb_type,
-            "acq": "pedsub",  # Hardcoded because all simple readouts use this mode
+            "acq": "raw",  # Hardcoded because all simple readouts use this mode
             "ped": "zero",  # Hardcoded because all simple readouts use this mode
             "readoutEn": True,  # This should always be on since we always want ethernet readout
             "singleEv": True,  # Always on, make sure `amount` counter is used by FW.
         }
 
         window_settings = {
             "windows": windows,
@@ -367,14 +367,18 @@
             evt_waiter.timeout = self.timeout
             for attempt in range(num_attempts):
                 try:
                     bc.toggle_trigger()
                     evt_waiter.start()
                 except TimeoutError:
                     continue
+                # If there's no timeout error, the output buffer got a new event
+                if "data" not in self._daq.output_buffer[-1].keys():
+                    self._daq.output_buffer.pop()
+                    continue
                 if attempt + 1 == num_attempts:
                     bc.stop_readout()
                     self._daq.stop_capture()
                     raise TimeoutError(
                         f"Unable to capture events after {num_attempts} attempts"
                     )
                 break
```

### Comparing `naludaq-0.20.2/src/naludaq/tools/features.py` & `naludaq-0.20.3/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/ft60x.py` & `naludaq-0.20.3/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/ftdi.py` & `naludaq-0.20.3/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/lookup_table/lookup_table.py` & `naludaq-0.20.3/src/naludaq/tools/lookup_table/lookup_table.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/lookup_table/lookup_table_generator.py` & `naludaq-0.20.3/src/naludaq/tools/lookup_table/lookup_table_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/metadata.py` & `naludaq-0.20.3/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.20.3/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/__init__.py` & `naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py` & `naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/optimizers/conversion_ramp/upac96.py` & `naludaq-0.20.3/src/naludaq/tools/optimizers/conversion_ramp/upac96.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             max_progress = 80
             _update_progress(
                 self.progress,
                 10 + (max_progress - min_progress) * step_idx / len(isel_currents),
                 f"Capturing Calibration Data:",
             )
             LOGGER.debug(
-                "Capturing Calibration Data for isel_current_ramp: {}", isel_current
+                "Capturing Calibration Data for isel_current_ramp: %d", isel_current
             )
             # Get slope between lowest and highest cap select values
             slope, yint = self._get_slope_for_current_state(isel_current, channels)
             # finds suggested cap select that result in an event average of 500
             value = self._get_suggested_cap_from_isel_lin(slope, yint)
             values.append(value)
```

### Comparing `naludaq-0.20.2/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.20.3/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/_new/__init__.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/_new/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/_new/aav3.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/_new/aav3.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class PedestalsGeneratorAardvarcv3New(PedestalsGeneratorNew):
     def _start_readout(self):
         """Start a readout"""
         readout_settings = {
             "trig": "ext",
             "lb": "forced",
-            "acq": "pedsub",
+            "acq": "raw",
             "dig_head": False,
             "ped": "zero",
             "readoutEn": True,
             "singleEv": False,
         }
         get_board_controller(self.board).start_readout(**readout_settings)
```

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/_new/default.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/_new/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/_new/hdsoc.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/_new/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         return True
 
     def _start_capture(self):
         """Start board and daq capture"""
         readout_settings = {
             "trig": "ext",
             "lb": "forced",
-            "acq": "pedsub",
+            "acq": "raw",
             "dig_head": False,
             "ped": "zero",
             "readoutEn": True,
             "singleEv": False,
         }
         self._daq.start_capture()
         get_board_controller(self.board).start_readout(**readout_settings)
```

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_acq.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_acq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_controller.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/udc16_pedestals_generator.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/udc16_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/pedestals/upac96_pedestals_generator.py` & `naludaq-0.20.3/src/naludaq/tools/pedestals/upac96_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.20.3/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.20.3/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.20.3/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.20.3/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.20.3/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.20.3/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.20.3/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.20.2/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.20.3/src/naludaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.20.2
+Version: 0.20.3
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.20.2/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.20.3/src/naludaq.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 src/naludaq/controllers/controller.py
 src/naludaq/controllers/project_controller.py
 src/naludaq/controllers/si5341_controller.py
 src/naludaq/controllers/biasing_mode/__init__.py
 src/naludaq/controllers/biasing_mode/udc16.py
 src/naludaq/controllers/board/__init__.py
 src/naludaq/controllers/board/aodsoc.py
-src/naludaq/controllers/board/asocv3.py
 src/naludaq/controllers/board/default.py
 src/naludaq/controllers/board/hdsoc.py
 src/naludaq/controllers/board/oleas.py
 src/naludaq/controllers/board/trbhm.py
 src/naludaq/controllers/board/udc.py
 src/naludaq/controllers/board/upac.py
 src/naludaq/controllers/board/upac96.py
```

