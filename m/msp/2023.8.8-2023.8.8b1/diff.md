# Comparing `tmp/msp-2023.8.8.tar.gz` & `tmp/msp-2023.8.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msp-2023.8.8.tar", last modified: Tue Aug  8 01:52:37 2023, max compression
+gzip compressed data, was "msp-2023.8.8b1.tar", last modified: Tue Aug  8 03:40:10 2023, max compression
```

## Comparing `msp-2023.8.8.tar` & `msp-2023.8.8b1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 01:52:37.374956 msp-2023.8.8/
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     1090 2023-08-08 01:33:29.000000 msp-2023.8.8/LICENSE
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      408 2023-08-08 01:52:37.374738 msp-2023.8.8/PKG-INFO
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        9 2023-08-08 01:33:29.000000 msp-2023.8.8/README.md
-drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 01:52:37.365273 msp-2023.8.8/msp/
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)       25 2023-08-08 01:45:53.000000 msp-2023.8.8/msp/__init__.py
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     3360 2023-08-08 01:49:11.000000 msp-2023.8.8/msp/inference.py
-drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 01:52:37.374297 msp-2023.8.8/msp.egg-info/
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      408 2023-08-08 01:52:37.000000 msp-2023.8.8/msp.egg-info/PKG-INFO
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      193 2023-08-08 01:52:37.000000 msp-2023.8.8/msp.egg-info/SOURCES.txt
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        1 2023-08-08 01:52:37.000000 msp-2023.8.8/msp.egg-info/dependency_links.txt
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      135 2023-08-08 01:52:37.000000 msp-2023.8.8/msp.egg-info/requires.txt
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        4 2023-08-08 01:52:37.000000 msp-2023.8.8/msp.egg-info/top_level.txt
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)       38 2023-08-08 01:52:37.375004 msp-2023.8.8/setup.cfg
--rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     1146 2023-08-08 01:50:40.000000 msp-2023.8.8/setup.py
+drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 03:40:10.078447 msp-2023.8.8b1/
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     1090 2023-08-08 01:33:29.000000 msp-2023.8.8b1/LICENSE
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      410 2023-08-08 03:40:10.078161 msp-2023.8.8b1/PKG-INFO
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        9 2023-08-08 01:33:29.000000 msp-2023.8.8b1/README.md
+drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 03:40:10.065044 msp-2023.8.8b1/msp/
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)       27 2023-08-08 03:39:21.000000 msp-2023.8.8b1/msp/__init__.py
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     3361 2023-08-08 02:41:48.000000 msp-2023.8.8b1/msp/inference.py
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 03:39:25.000000 msp-2023.8.8b1/msp/model.py
+drwxr-xr-x   0 1112988  (839067945) SKT\Domain Users (1437349805)        0 2023-08-08 03:40:10.077536 msp-2023.8.8b1/msp.egg-info/
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      410 2023-08-08 03:40:10.000000 msp-2023.8.8b1/msp.egg-info/PKG-INFO
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      206 2023-08-08 03:40:10.000000 msp-2023.8.8b1/msp.egg-info/SOURCES.txt
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        1 2023-08-08 03:40:10.000000 msp-2023.8.8b1/msp.egg-info/dependency_links.txt
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)      135 2023-08-08 03:40:10.000000 msp-2023.8.8b1/msp.egg-info/requires.txt
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)        4 2023-08-08 03:40:10.000000 msp-2023.8.8b1/msp.egg-info/top_level.txt
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)       38 2023-08-08 03:40:10.078516 msp-2023.8.8b1/setup.cfg
+-rw-r--r--   0 1112988  (839067945) SKT\Domain Users (1437349805)     1146 2023-08-08 01:50:40.000000 msp-2023.8.8b1/setup.py
```

### Comparing `msp-2023.8.8/LICENSE` & `msp-2023.8.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `msp-2023.8.8/msp/inference.py` & `msp-2023.8.8b1/msp/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 }
 MSP_MODEL_VERSION = os.environ.get("MSP_MODEL_VERSION", "NONE")
 
 import model
 
 carrier = None
 
+
 def traced(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         global carrier
         with trace.get_tracer(f.__module__).start_as_current_span(
             f.__name__, context=extract(carrier=carrier), kind=trace.SpanKind.SERVER
         ):
```

### Comparing `msp-2023.8.8/setup.py` & `msp-2023.8.8b1/setup.py`

 * *Files identical despite different names*

