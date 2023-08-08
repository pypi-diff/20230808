# Comparing `tmp/kizano-1.0.1.tar.gz` & `tmp/kizano-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kizano-1.0.1.tar", last modified: Fri Apr  7 21:53:28 2023, max compression
+gzip compressed data, was "kizano-1.0.2.tar", last modified: Tue Aug  8 00:08:03 2023, max compression
```

## Comparing `kizano-1.0.1.tar` & `kizano-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/
--rw-r--r--   0 markizano  (1000) kizano    (1006)      581 2023-04-07 21:53:28.744200 kizano-1.0.1/PKG-INFO
--rw-r--r--   0 markizano  (1000) kizano    (1006)      363 2022-06-30 22:20:03.000000 kizano-1.0.1/README.md
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/kizano.egg-info/
--rw-r--r--   0 markizano  (1000) kizano    (1006)      581 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/PKG-INFO
--rw-r--r--   0 markizano  (1000) kizano    (1006)      221 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/SOURCES.txt
--rw-r--r--   0 markizano  (1000) kizano    (1006)        1 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/dependency_links.txt
--rw-r--r--   0 markizano  (1000) kizano    (1006)        7 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/top_level.txt
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/kizano/
--rw-r--r--   0 markizano  (1000) kizano    (1006)     1502 2023-04-07 19:36:24.000000 kizano-1.0.1/lib/kizano/__init__.py
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/kizano/logger/
--rw-r--r--   0 markizano  (1000) kizano    (1006)     1863 2022-07-05 02:20:07.000000 kizano-1.0.1/lib/kizano/logger/__init__.py
--rw-r--r--   0 markizano  (1000) kizano    (1006)     3346 2023-04-07 19:44:54.000000 kizano-1.0.1/lib/kizano/utils.py
--rw-r--r--   0 markizano  (1000) kizano    (1006)      313 2023-04-07 21:53:28.744200 kizano-1.0.1/setup.cfg
--rwxr-xr-x   0 markizano  (1000) kizano    (1006)     1709 2023-04-07 21:53:23.000000 kizano-1.0.1/setup.py
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-08-08 00:08:03.656931 kizano-1.0.2/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      582 2023-08-08 00:08:03.656931 kizano-1.0.2/PKG-INFO
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      363 2022-06-30 22:20:03.000000 kizano-1.0.2/README.md
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-08-08 00:08:03.656931 kizano-1.0.2/kizano.egg-info/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      582 2023-08-08 00:08:03.000000 kizano-1.0.2/kizano.egg-info/PKG-INFO
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      221 2023-08-08 00:08:03.000000 kizano-1.0.2/kizano.egg-info/SOURCES.txt
+-rw-r--r--   0 markizano  (1000) kizano    (1006)        1 2023-08-08 00:08:03.000000 kizano-1.0.2/kizano.egg-info/dependency_links.txt
+-rw-r--r--   0 markizano  (1000) kizano    (1006)        7 2023-08-08 00:08:03.000000 kizano-1.0.2/kizano.egg-info/top_level.txt
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-08-08 00:08:03.656931 kizano-1.0.2/lib/
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-08-08 00:08:03.656931 kizano-1.0.2/lib/kizano/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     1538 2023-04-08 02:21:14.000000 kizano-1.0.2/lib/kizano/__init__.py
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-08-08 00:08:03.656931 kizano-1.0.2/lib/kizano/logger/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     2213 2023-04-23 17:11:56.000000 kizano-1.0.2/lib/kizano/logger/__init__.py
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     3346 2023-04-07 19:44:54.000000 kizano-1.0.2/lib/kizano/utils.py
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      313 2023-08-08 00:08:03.656931 kizano-1.0.2/setup.cfg
+-rwxr-xr-x   0 markizano  (1000) kizano    (1006)     1710 2023-04-08 02:20:25.000000 kizano-1.0.2/setup.py
```

### Comparing `kizano-1.0.1/PKG-INFO` & `kizano-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kizano
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kizano code for quick access to functions.
 Home-page: https://markizano.net/
 Author: Markizano Draconus
 Author-email: markizano@markizano.net
 License: GNU
-Description: This is a core library that should allow one to import and run with pre-built libraries. Common features like logging and configuration management should not need to be re-created in every project. This aimsto minimize this by providing a core library of swiss army knife ofcommon functionality.
+Description: This is a core library that should allow one to import and run with pre-built libraries. Common features like logging and configuration management should not need to be re-created in every project. This aims to minimize this by providing a core library of swiss army knife ofcommon functionality.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kizano-1.0.1/kizano.egg-info/PKG-INFO` & `kizano-1.0.2/kizano.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kizano
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kizano code for quick access to functions.
 Home-page: https://markizano.net/
 Author: Markizano Draconus
 Author-email: markizano@markizano.net
 License: GNU
-Description: This is a core library that should allow one to import and run with pre-built libraries. Common features like logging and configuration management should not need to be re-created in every project. This aimsto minimize this by providing a core library of swiss army knife ofcommon functionality.
+Description: This is a core library that should allow one to import and run with pre-built libraries. Common features like logging and configuration management should not need to be re-created in every project. This aims to minimize this by providing a core library of swiss army knife ofcommon functionality.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kizano-1.0.1/lib/kizano/__init__.py` & `kizano-1.0.2/lib/kizano/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
+import os
 from kizano.logger import getLogger
 import kizano.utils as utils
+log = getLogger(__name__)
 
 class Config(object):
     '''
     Configuration object that tracks config in /etc/${APP_NAME}/config.yml and
     in ~/.config/${APP_NAME}/config.yml
 
     Returns a cached version of the config if we've asked the filesystem for it before for
```

### Comparing `kizano-1.0.1/lib/kizano/logger/__init__.py` & `kizano-1.0.2/lib/kizano/logger/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             while len(mesg) > maxlen:
                 record.msg = mesg[0:maxlen]
                 SysLogHandler.emit(self, record)
                 mesg = mesg[maxlen:]
         else:
             SysLogHandler.emit(self, record)
 
-def getLogger(name, log_level=None):
+def getLogger(name, log_level=None, log_format='standard'):
     '''
     Get a logger by the name provided. Set the log_level if you provide the second argument.
     If not, ask the environment for $LOG_LEVEL. If not, default to DEBUG.
     Also attaches a syslog handler that will handle large strings and stream the message
     to the syslog endpoint.
     @param log_level {enum:string} One of the logger levels.
     @return {@logging.getLogger()}
@@ -33,14 +33,20 @@
     log_level_map = dict([ (_ll, getattr(logging, _ll)) for _ll in log_levels ])
     if not log_level:
         #@throws KeyError if $LOG_LEVEL is set to invalid log level as described
         # by above array $log_level_map
         log_level = log_level_map[ os.getenv('LOG_LEVEL', 'DEBUG').upper() ]
     logger = logging.getLogger(name)
     logger.setLevel(log_level)
-    logging.basicConfig(format='%(asctime)s %(name)s.%(funcName)s(PID=%(process)d, %(levelname)s) %(message)s')
+    logFormats = {
+      'standard': '%(asctime)s %(name)s.%(funcName)s(PID=%(process)d %(levelname)-8s) %(message)s',
+      'json': '{ "time": "%(asctime)s", "function": "%(name)s.%(funcName)s", "pid": "%(process)d", "level": "%(levelname)s", "message", "%(message)s" }',
+      'csv': '%(asctime)s,%(name)s.%(funcName)s,%(levelname)s,%(message)s',
+    }
+    logging.basicConfig(format=logFormats.get(log_format, logFormats['standard']))
 
     syslog_handler = LocalSyslogHandler()
     syslog_handler.setLevel(log_level)
     logger.addHandler(syslog_handler)
 
     return logger
+
```

### Comparing `kizano-1.0.1/lib/kizano/utils.py` & `kizano-1.0.2/lib/kizano/utils.py`

 * *Files identical despite different names*

### Comparing `kizano-1.0.1/setup.py` & `kizano-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from setuptools import setup
 
 sys.path.insert(0, os.path.abspath('lib'))
 
 setup_opts = {
     'name'                : 'kizano',
     # We change this default each time we tag a release.
-    'version'             : '1.0.1',
+    'version'             : '1.0.2',
     'description'         : 'Kizano code for quick access to functions.',
     'long_description'    : ('This is a core library that should allow one to import and run with '
                             'pre-built libraries. Common features like logging and configuration '
-                            'management should not need to be re-created in every project. This aims'
+                            'management should not need to be re-created in every project. This aims '
                             'to minimize this by providing a core library of swiss army knife of'
                             'common functionality.'),
     'long_description_content_type': 'text/markdown',
     'author'              : 'Markizano Draconus',
     'author_email'        : 'markizano@markizano.net',
     'url'                 : 'https://markizano.net/',
     'license'             : 'GNU',
```

