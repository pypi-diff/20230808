# Comparing `tmp/flow-agent-package-0.0.8.tar.gz` & `tmp/flow-agent-package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-agent-package-0.0.8.tar", last modified: Wed Aug  2 20:57:52 2023, max compression
+gzip compressed data, was "flow-agent-package-0.0.9.tar", last modified: Thu Aug  3 23:05:09 2023, max compression
```

## Comparing `flow-agent-package-0.0.8.tar` & `flow-agent-package-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.263958 flow-agent-package-0.0.8/
--rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-08-02 20:57:52.262452 flow-agent-package-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.212789 flow-agent-package-0.0.8/flow_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.8/flow_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.252932 flow-agent-package-0.0.8/flow_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.8/flow_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-08-02 20:57:13.000000 flow-agent-package-0.0.8/flow_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0     3582 2023-08-02 20:45:32.000000 flow-agent-package-0.0.8/flow_agent_package/tools/get_flow_tool.py
--rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.8/flow_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.258452 flow-agent-package-0.0.8/flow_agent_package/yamls/
--rw-rw-rw-   0        0        0      520 2023-08-02 20:32:04.000000 flow-agent-package-0.0.8/flow_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      407 2023-08-02 20:31:48.000000 flow-agent-package-0.0.8/flow_agent_package/yamls/get_flow_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.235400 flow-agent-package-0.0.8/flow_agent_package.egg-info/
--rw-rw-rw-   0        0        0      106 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 20:57:52.263958 flow-agent-package-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-08-02 20:57:48.000000 flow-agent-package-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.261451 flow-agent-package-0.0.8/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.8/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.775802 flow-agent-package-0.0.9/
+-rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-08-03 23:05:09.773791 flow-agent-package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.641505 flow-agent-package-0.0.9/flow_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.9/flow_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.739793 flow-agent-package-0.0.9/flow_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.9/flow_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-08-02 20:57:13.000000 flow-agent-package-0.0.9/flow_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0     3682 2023-08-03 20:59:46.000000 flow-agent-package-0.0.9/flow_agent_package/tools/get_flow_tool.py
+-rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.9/flow_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.767802 flow-agent-package-0.0.9/flow_agent_package/yamls/
+-rw-rw-rw-   0        0        0      520 2023-08-02 20:32:04.000000 flow-agent-package-0.0.9/flow_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      407 2023-08-02 20:31:48.000000 flow-agent-package-0.0.9/flow_agent_package/yamls/get_flow_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.678503 flow-agent-package-0.0.9/flow_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-08-03 23:05:09.000000 flow-agent-package-0.0.9/flow_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-08-03 23:05:09.000000 flow-agent-package-0.0.9/flow_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 23:05:09.000000 flow-agent-package-0.0.9/flow_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-03 23:05:09.000000 flow-agent-package-0.0.9/flow_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-08-03 23:05:09.000000 flow-agent-package-0.0.9/flow_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 23:05:09.775802 flow-agent-package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-08-03 23:05:03.000000 flow-agent-package-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:05:09.770803 flow-agent-package-0.0.9/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.9/tests/test_my_tool_1.py
```

### Comparing `flow-agent-package-0.0.8/README.md` & `flow-agent-package-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.8/flow_agent_package/tools/agent_tool.py` & `flow-agent-package-0.0.9/flow_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.8/flow_agent_package/tools/get_flow_tool.py` & `flow-agent-package-0.0.9/flow_agent_package/tools/get_flow_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,13 +69,15 @@
                 "api_type": "azure",
                 "api_version": "2023-03-15-preview"
             }
         }
         connection_configs[connection_name] = config
     
     final_json = {
+        "flowName": correct_flow["flowName"],
+        "description": correct_flow["description"],
         "flowId": correct_flow["flowId"],
         "flow": graph,
         "batch_inputs": batch_inputs,
         "connections": connection_configs
     }
     return final_json
```

### Comparing `flow-agent-package-0.0.8/flow_agent_package/tools/utils.py` & `flow-agent-package-0.0.9/flow_agent_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.8/flow_agent_package/yamls/agent_tool.yaml` & `flow-agent-package-0.0.9/flow_agent_package/yamls/agent_tool.yaml`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.8/flow_agent_package.egg-info/SOURCES.txt` & `flow-agent-package-0.0.9/flow_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

