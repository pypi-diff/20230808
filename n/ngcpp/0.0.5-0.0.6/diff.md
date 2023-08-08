# Comparing `tmp/ngcpp-0.0.5.tar.gz` & `tmp/ngcpp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngcpp-0.0.5.tar", max compression
+gzip compressed data, was "ngcpp-0.0.6.tar", max compression
```

## Comparing `ngcpp-0.0.5.tar` & `ngcpp-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      732 2023-08-08 04:05:20.134723 ngcpp-0.0.5/README.md
--rw-r--r--   0        0        0     1331 2023-08-08 04:05:20.134723 ngcpp-0.0.5/ngcpp/cli/cluster_info.py
--rw-r--r--   0        0        0     6920 2023-08-08 04:05:20.134723 ngcpp-0.0.5/ngcpp/cli/job_info.py
--rw-r--r--   0        0        0     4656 2023-08-08 04:05:20.134723 ngcpp-0.0.5/ngcpp/cluster.py
--rw-r--r--   0        0        0     1154 2023-08-08 04:05:20.135723 ngcpp-0.0.5/ngcpp/cluster.yaml
--rw-r--r--   0        0        0      383 2023-08-08 04:05:20.135723 ngcpp-0.0.5/ngcpp/utils.py
--rw-r--r--   0        0        0      717 2023-08-08 04:05:23.811759 ngcpp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 ngcpp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      732 2023-08-08 17:19:56.420280 ngcpp-0.0.6/README.md
+-rw-r--r--   0        0        0     1331 2023-08-08 17:19:56.420280 ngcpp-0.0.6/ngcpp/cli/cluster_info.py
+-rw-r--r--   0        0        0     6920 2023-08-08 17:19:56.420280 ngcpp-0.0.6/ngcpp/cli/job_info.py
+-rw-r--r--   0        0        0     4952 2023-08-08 17:19:56.420280 ngcpp-0.0.6/ngcpp/cluster.py
+-rw-r--r--   0        0        0     1154 2023-08-08 17:19:56.420280 ngcpp-0.0.6/ngcpp/cluster.yaml
+-rw-r--r--   0        0        0      383 2023-08-08 17:19:56.421280 ngcpp-0.0.6/ngcpp/utils.py
+-rw-r--r--   0        0        0      717 2023-08-08 17:20:00.216713 ngcpp-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 ngcpp-0.0.6/PKG-INFO
```

### Comparing `ngcpp-0.0.5/README.md` & `ngcpp-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.5/ngcpp/cli/cluster_info.py` & `ngcpp-0.0.6/ngcpp/cli/cluster_info.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.5/ngcpp/cli/job_info.py` & `ngcpp-0.0.6/ngcpp/cli/job_info.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.5/ngcpp/cluster.py` & `ngcpp-0.0.6/ngcpp/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from loguru import logger as logging
 from omegaconf import OmegaConf
 
 from ngcpp.utils import run_simple_command
 
 __all__ = ["Cluster", "CLUSTER_SETTING"]
 
+pd.set_option("display.max_colwidth", 150)
 
 CLUSTER_SETTING = OmegaConf.load(
     os.path.join(os.path.dirname(__file__), "cluster.yaml")
 )
 
 ALIAS_TO_CLUSTER = {v.alias: k for k, v in CLUSTER_SETTING.items()}
 
@@ -58,36 +59,41 @@
             latest_value = telemetry_data["GPU_FI_PROF_PIPE_TENSOR_ACTIVE"].iloc[-1]
 
             # If the latest value is non-zero, the hang time is zero
             if latest_value > 0.01:
                 hang_time = timedelta(0)
             else:
                 # Finding the timestamp of the latest non-zero 'GPU_FI_PROF_PIPE_TENSOR_ACTIVE'
-                latest_non_zero_time = telemetry_data.loc[
-                    telemetry_data["GPU_FI_PROF_PIPE_TENSOR_ACTIVE"] < 0.01, "Time"
-                ].iloc[-1]
+                non_zero = telemetry_data.loc[
+                    telemetry_data["GPU_FI_PROF_PIPE_TENSOR_ACTIVE"] > 0.01, "Time"
+                ]
+                if non_zero.empty:
+                    latest_non_zero_time = telemetry_data["Time"].iloc[0]
+                else:
+                    latest_non_zero_time = non_zero.iloc[-1]
 
                 # Finding the timestamp of the latest entry in the data
                 latest_time = telemetry_data["Time"].iloc[-1]
 
                 # Calculating the duration from now to the latest non-zero 'GPU_FI_PROF_PIPE_TENSOR_ACTIVE'
                 hang_time = latest_time - latest_non_zero_time
 
             # add hang time to df
             df.loc[df["Id"] == cur_id, "HangTime"] = hang_time
+            df.loc[df["Id"] == cur_id, "TensorCore"] = latest_value
         # filter out non-hangs
         _df = df[df["HangTime"] > timedelta(0)]
         # if no hangs, return
         if _df.empty:
             logging.info("No hanging jobs")
         else:
             print(
-                _df[["Id", "Name", "HangTime", "Duration", "Replicas"]].to_string(
-                    index=False
-                )
+                _df[
+                    ["Id", "Name", "HangTime", "TensorCore", "Duration", "Replicas"]
+                ].to_string(index=False)
             )
         return df
 
     def report_user_usage(self):
         _, stderr = run_simple_command(
             f"ngc batch list --all --format_type csv --team {self.team} --ace {self.ace} "
             f"--status RUNNING > /tmp/ngcpp_{self.name}.csv"
```

### Comparing `ngcpp-0.0.5/ngcpp/cluster.yaml` & `ngcpp-0.0.6/ngcpp/cluster.yaml`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.5/pyproject.toml` & `ngcpp-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngcpp"
-version = "0.0.5"
+version = "0.0.6"
 description = "A toolkit for ngc"
 authors = ["Qinsheng <qsh.zh27@gmail.com>"]
 readme = "README.md"
 keywords = ["jam", "experiment", "ngc"]
 license = "MIT"
 packages = [
     {include = "ngcpp"},
```

### Comparing `ngcpp-0.0.5/PKG-INFO` & `ngcpp-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngcpp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolkit for ngc
 License: MIT
 Keywords: jam,experiment,ngc
 Author: Qinsheng
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

