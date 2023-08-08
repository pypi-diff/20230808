# Comparing `tmp/pyed-1.1.0.tar.gz` & `tmp/pyed-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyed-1.1.0.tar", last modified: Fri Aug  4 13:44:04 2023, max compression
+gzip compressed data, was "pyed-1.2.0.tar", last modified: Tue Aug  8 08:33:19 2023, max compression
```

## Comparing `pyed-1.1.0.tar` & `pyed-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1069 2023-07-17 06:32:44.000000 pyed-1.1.0/LICENSE.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       19 2023-07-17 06:32:44.000000 pyed-1.1.0/MANIFEST.in
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-04 13:44:04.265254 pyed-1.1.0/PKG-INFO
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)    16844 2023-08-04 13:40:53.000000 pyed-1.1.0/README.adoc
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.261254 pyed-1.1.0/pyed/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      136 2023-07-24 07:40:55.000000 pyed-1.1.0/pyed/__init__.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/pyed/core/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/__init__.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1270 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/constants.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4365 2023-07-24 07:54:54.000000 pyed-1.1.0/pyed/core/node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      452 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/utils.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      837 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/xml_item.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/pyed/elements/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      264 2023-08-04 08:30:26.000000 pyed-1.1.0/pyed/elements/__init__.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4653 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/edge.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2564 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/generic_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     6354 2023-08-04 09:52:41.000000 pyed-1.1.0/pyed/elements/graph.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7196 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/group.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4285 2023-07-17 12:11:14.000000 pyed-1.1.0/pyed/elements/label.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      851 2023-08-04 12:42:07.000000 pyed-1.1.0/pyed/elements/resource.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1368 2023-07-17 13:40:49.000000 pyed-1.1.0/pyed/elements/shape_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1320 2023-08-04 08:30:26.000000 pyed-1.1.0/pyed/elements/svg_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     3886 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/table_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1339 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/uml_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7257 2023-07-24 07:41:12.000000 pyed-1.1.0/pyed/utils.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       22 2023-08-04 13:43:51.000000 pyed-1.1.0/pyed/version.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.261254 pyed-1.1.0/pyed.egg-info/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/PKG-INFO
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      648 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/SOURCES.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        1 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/dependency_links.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       18 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/requires.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        5 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/top_level.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1610 2023-08-04 13:40:53.000000 pyed-1.1.0/pypi.md
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      105 2023-07-17 06:32:44.000000 pyed-1.1.0/pyproject.toml
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      508 2023-08-04 13:44:04.265254 pyed-1.1.0/setup.cfg
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      174 2023-07-17 06:32:44.000000 pyed-1.1.0/setup.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-08 08:33:19.475080 pyed-1.2.0/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1069 2023-07-17 06:32:44.000000 pyed-1.2.0/LICENSE.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       19 2023-07-17 06:32:44.000000 pyed-1.2.0/MANIFEST.in
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-08 08:33:19.475080 pyed-1.2.0/PKG-INFO
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2141 2023-08-04 16:30:37.000000 pyed-1.2.0/README.adoc
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-08 08:33:19.471080 pyed-1.2.0/pyed/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      195 2023-08-08 07:42:36.000000 pyed-1.2.0/pyed/__init__.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-08 08:33:19.471080 pyed-1.2.0/pyed/core/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/core/__init__.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1270 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/core/constants.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2315 2023-08-08 08:26:04.000000 pyed-1.2.0/pyed/core/dict_parser.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4365 2023-07-24 07:54:54.000000 pyed-1.2.0/pyed/core/node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      452 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/core/utils.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      837 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/core/xml_item.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-08 08:33:19.475080 pyed-1.2.0/pyed/elements/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      264 2023-08-04 08:30:26.000000 pyed-1.2.0/pyed/elements/__init__.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4653 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/elements/edge.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2564 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/elements/generic_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     6354 2023-08-04 09:52:41.000000 pyed-1.2.0/pyed/elements/graph.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7196 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/elements/group.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4285 2023-07-17 12:11:14.000000 pyed-1.2.0/pyed/elements/label.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      851 2023-08-04 12:42:07.000000 pyed-1.2.0/pyed/elements/resource.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1368 2023-07-17 13:40:49.000000 pyed-1.2.0/pyed/elements/shape_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1320 2023-08-04 08:30:26.000000 pyed-1.2.0/pyed/elements/svg_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     3886 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/elements/table_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1339 2023-07-17 06:32:44.000000 pyed-1.2.0/pyed/elements/uml_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     6471 2023-08-08 07:42:36.000000 pyed-1.2.0/pyed/utils.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       22 2023-08-08 08:18:40.000000 pyed-1.2.0/pyed/version.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-08 08:33:19.471080 pyed-1.2.0/pyed.egg-info/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-08 08:33:19.000000 pyed-1.2.0/pyed.egg-info/PKG-INFO
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      673 2023-08-08 08:33:19.000000 pyed-1.2.0/pyed.egg-info/SOURCES.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        1 2023-08-08 08:33:19.000000 pyed-1.2.0/pyed.egg-info/dependency_links.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       25 2023-08-08 08:33:19.000000 pyed-1.2.0/pyed.egg-info/requires.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        5 2023-08-08 08:33:19.000000 pyed-1.2.0/pyed.egg-info/top_level.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1610 2023-08-04 13:40:53.000000 pyed-1.2.0/pypi.md
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      105 2023-07-17 06:32:44.000000 pyed-1.2.0/pyproject.toml
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      516 2023-08-08 08:33:19.475080 pyed-1.2.0/setup.cfg
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      174 2023-07-17 06:32:44.000000 pyed-1.2.0/setup.py
```

### Comparing `pyed-1.1.0/LICENSE.txt` & `pyed-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/PKG-INFO` & `pyed-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyed
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Python Yed Simple Graph generator"
 Home-page: https://github.com/ccossou/Pyed
 Author: "Christophe Cossou"
 Author-email: "ccossou@gmail.com"
 Platform: ["Linux"
 Platform: "Mac OS X"]
 Requires-Python: >=3.9
```

### Comparing `pyed-1.1.0/pyed/core/constants.py` & `pyed-1.2.0/pyed/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/core/node.py` & `pyed-1.2.0/pyed/core/node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/core/xml_item.py` & `pyed-1.2.0/pyed/core/xml_item.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/edge.py` & `pyed-1.2.0/pyed/elements/edge.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/generic_node.py` & `pyed-1.2.0/pyed/elements/generic_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/graph.py` & `pyed-1.2.0/pyed/elements/graph.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/group.py` & `pyed-1.2.0/pyed/elements/group.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/label.py` & `pyed-1.2.0/pyed/elements/label.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/resource.py` & `pyed-1.2.0/pyed/elements/resource.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/shape_node.py` & `pyed-1.2.0/pyed/elements/shape_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/svg_node.py` & `pyed-1.2.0/pyed/elements/svg_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/table_node.py` & `pyed-1.2.0/pyed/elements/table_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/elements/uml_node.py` & `pyed-1.2.0/pyed/elements/uml_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.1.0/pyed/utils.py` & `pyed-1.2.0/pyed/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,20 +172,18 @@
         if isinstance(v, collections.abc.Mapping):
             d[k] = update_dict(d.get(k, {}), v)
         else:
             d[k] = v
     return d
 
 
-def init_log(log="pyed.log", stdout_loglevel="INFO", file_loglevel="DEBUG", extra_config=None):
+def init_log(level="INFO", extra_config=None):
     """
 
-    :param str log: filename where to store logs. By default "pipeline.log"
-    :param str stdout_loglevel: log level for standard output (ERROR, WARNING, INFO, DEBUG)
-    :param str file_loglevel: log level for log file (ERROR, WARNING, INFO, DEBUG)
+    :param str level: log level for standard output (ERROR, WARNING, INFO, DEBUG)
     :param dict extra_config: [optional] Set of extra properties to be added to the dict_config for logging
     :return:
     :rtype:
     """
 
     import logging.config
 
@@ -194,44 +192,31 @@
         "formatters":
             {
                 "form01":
                     {
                         "format": "%(asctime)s %(levelname)-8s %(message)s",
                         "datefmt": "%H:%M:%S"
                     },
-                "form02":
-                    {
-                        "format": "%(asctime)s [%(processName)s/%(name)s] %(levelname)s - %(message)s",
-                        "datefmt": "%H:%M:%S"
-                    },
             },
         "handlers":
             {
                 "console":
                     {
                         "class": "logging.StreamHandler",
                         "formatter": "form01",
-                        "level": stdout_loglevel,
+                        "level": level,
                         "stream": "ext://sys.stdout",
                     },
-                "file":
-                    {
-                        "class": "logging.FileHandler",
-                        "formatter": "form02",
-                        "level": file_loglevel,
-                        "filename": log,
-                        "mode": "w",  # Overwrite file if it exists
-                    },
             },
         "loggers":
             {
                 "":
                     {
                         "level": "NOTSET",
-                        "handlers": ["console", "file"],
+                        "handlers": ["console"],
                     },
             },
         "disable_existing_loggers": False,
     }
 
     if extra_config is not None:
         log_config = update_dict(log_config, extra_config)
```

### Comparing `pyed-1.1.0/pyed.egg-info/PKG-INFO` & `pyed-1.2.0/pyed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyed
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Python Yed Simple Graph generator"
 Home-page: https://github.com/ccossou/Pyed
 Author: "Christophe Cossou"
 Author-email: "ccossou@gmail.com"
 Platform: ["Linux"
 Platform: "Mac OS X"]
 Requires-Python: >=3.9
```

### Comparing `pyed-1.1.0/pyed.egg-info/SOURCES.txt` & `pyed-1.2.0/pyed.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pyed.egg-info/PKG-INFO
 pyed.egg-info/SOURCES.txt
 pyed.egg-info/dependency_links.txt
 pyed.egg-info/requires.txt
 pyed.egg-info/top_level.txt
 pyed/core/__init__.py
 pyed/core/constants.py
+pyed/core/dict_parser.py
 pyed/core/node.py
 pyed/core/utils.py
 pyed/core/xml_item.py
 pyed/elements/__init__.py
 pyed/elements/edge.py
 pyed/elements/generic_node.py
 pyed/elements/graph.py
```

### Comparing `pyed-1.1.0/pypi.md` & `pyed-1.2.0/pypi.md`

 * *Files identical despite different names*

