# Comparing `tmp/smartdash-0.0.1.dev8.tar.gz` & `tmp/smartdash-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev8.tar", last modified: Tue Jul 18 09:31:42 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev9.tar", last modified: Tue Aug  8 05:17:46 2023, max compression
```

## Comparing `smartdash-0.0.1.dev8.tar` & `smartdash-0.0.1.dev9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:31:42.940430 smartdash-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 09:31:42.940430 smartdash-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:31:42.940430 smartdash-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:31:42.940430 smartdash-0.0.1.dev8/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 09:31:24.000000 smartdash-0.0.1.dev8/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:31:42.940430 smartdash-0.0.1.dev8/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:31:42.000000 smartdash-0.0.1.dev8/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:17:46.528368 smartdash-0.0.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-08 05:17:46.528368 smartdash-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 05:17:46.528368 smartdash-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:17:46.528368 smartdash-0.0.1.dev9/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-08-08 05:17:31.000000 smartdash-0.0.1.dev9/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:17:46.528368 smartdash-0.0.1.dev9/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 05:17:46.000000 smartdash-0.0.1.dev9/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev8/PKG-INFO` & `smartdash-0.0.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartdash-0.0.1.dev8/setup.py` & `smartdash-0.0.1.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev8"
+VERSION = "0.0.1.dev9"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly", "gevent", "falcon", "gunicorn"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartdash-0.0.1.dev8/smartdash/__init__.py` & `smartdash-0.0.1.dev9/smartdash/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev8/smartdash/dash.py` & `smartdash-0.0.1.dev9/smartdash/dash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Importing required libraries
 import streamlit as st
 import pandas as pd
 import requests
 import os
 import json
 import plotly.express as px
 from datetime import datetime
@@ -36,14 +35,21 @@
 
     return sorted(tags), sorted(levels), sorted(stages)
 
 
 # Main function to run the Streamlit app
 def main():
     st.set_page_config(page_title="SmartDash", layout="wide")
+    hide_streamlit_style = """
+            <style>
+            #MainMenu {visibility: hidden;}
+            footer {visibility: hidden;}
+            </style>
+            """
+    st.markdown(hide_streamlit_style, unsafe_allow_html=True) 
 
     st.sidebar.title("SmartDash - App Dashboard")
 
     try:
         # Dropdowns for app_name and last_n_hours in the sidebar
         st.sidebar.markdown("## Settings")
         app_name = st.sidebar.selectbox(
@@ -133,32 +139,40 @@
                 y="time_taken",
                 color="stage",
                 title="Time taken by each stage",
             )
             graphs.append(stage_time_line)
 
         if data_by_uid:
-            # Pie chart showing number of failed, success, and in-process uids
-            metrics_pie = px.pie(
-                values=[
-                    sum([1 for uid, data in data_by_uid.items() if data["success"]]),
-                    sum([1 for uid, data in data_by_uid.items() if data["in_process"]]),
-                    sum([1 for uid, data in data_by_uid.items() if data["failed"]]),
-                    sum(
-                        [1 for uid, data in data_by_uid.items() if data["long_running"]]
-                    ),
-                ],
-                names=["Success", "In Process", "Failed", "Long running"],
-                title="Uids by Status",
-            )
+            metrics_df = pd.DataFrame({
+                    "status": ["Success" if data["success"] 
+                                else "In Process" if data["in_process"]
+                                else "Failed" if data["failed"] 
+                                else "Long running"
+                                for uid, data in data_by_uid.items()],
+                })
+
+            metrics_pie = px.pie(metrics_df, 
+                        names='status', 
+                        title="Uids by Status", 
+                        color='status',
+                        color_discrete_map={
+                            "Success": "green",
+                            "In Process": "yellow",
+                            "Failed": "red",
+                            "Long running": "lightcoral"
+                        })
+            
+            metrics_pie.update_traces(textposition='inside', textinfo='percent+label')
+
             graphs.append(metrics_pie)
 
         cols = st.columns(2, gap="small")
         for i, graph in enumerate(graphs):
-            cols[i % 2].write(graph)
+            cols[i % 2].plotly_chart(graph)
 
         with st.expander("Show/hide logs"):
             logs_data = []
             for uid, data in data_by_uid.items():
                 logs_data.extend(data["logs"])
                 if data["success"]:
                     logs_data[-1]["status"] = "Success"
@@ -192,14 +206,15 @@
                 if filter_uid:
                     logs_data = [log for log in logs_data if log["u_id"] == filter_uid]
 
                 logs_df = pd.DataFrame(logs_data)
                 st.dataframe(logs_df)
 
     except Exception as e:
+        print(e)
         st.warning(
             "No Apps uploaded logs yet. Please upload logs using the smartlogger CLI."
         )
         st.stop()
 
 
 if __name__ == "__main__":
```

### Comparing `smartdash-0.0.1.dev8/smartdash/smartdash_server.py` & `smartdash-0.0.1.dev9/smartdash/smartdash_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 METRICS_INDEX = DefinedIndex(
     f"metrics_index",
     schema={"app_name": "", "metric": "", "value": 0, "timestamp": 0},
     db_path=db_path,
     auto_key=True,
 )
 
+class HealthCheck(object):
+    def on_get(self, req, resp):
+        resp.media = {"status": "ok"}
+
 
 class GetDashMetrics(object):
     def on_get(self, req, resp):
         eight_hours_ago = (
             time.time() - float(req.params.get("last_n_hours", 8)) * 60 * 60
         )
         long_running_if_greater_than = (
@@ -111,14 +115,18 @@
             page_size=1000,
         ):
             if ml_inputs_outputs["u_id"] not in data_by_id:
                 data_by_id[log["u_id"]] = {
                     "logs": [],
                     "ml_inputs_outputs": [],
                     "stage_wise_times": {},
+                    "success": None,
+                    "failed": None,
+                    "in_process": None,
+                    "long_running": False,
                 }
 
             data_by_id[log["u_id"]]["ml_inputs_outputs"].append(ml_inputs_outputs)
 
         # Calculate stage wise timers
         for u_id, data in data_by_id.items():
             stage_timers = {}
@@ -201,14 +209,15 @@
     )
 
     app.add_route("/logs", AddLogs())
     app.add_route("/metrics", AddMetrics())
     app.add_route("/ml_inputs_outputs", AddMLInputsOutputs())
     app.add_route("/app_names", AppNames())
     app.add_route("/get_dash_metrics", GetDashMetrics())
+    app.add_route("/health", HealthCheck())
 
     import gunicorn.app.base
 
     class StandaloneApplication(gunicorn.app.base.BaseApplication):
         def __init__(self, app, options=None):
             self.options = options or {}
             self.application = app
```

### Comparing `smartdash-0.0.1.dev8/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev9/smartdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

