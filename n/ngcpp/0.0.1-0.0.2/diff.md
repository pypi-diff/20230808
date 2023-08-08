# Comparing `tmp/ngcpp-0.0.1.tar.gz` & `tmp/ngcpp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngcpp-0.0.1.tar", max compression
+gzip compressed data, was "ngcpp-0.0.2.tar", max compression
```

## Comparing `ngcpp-0.0.1.tar` & `ngcpp-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      173 2023-08-08 01:10:21.779194 ngcpp-0.0.1/README.md
--rw-r--r--   0        0        0      884 2023-08-08 01:30:40.839493 ngcpp-0.0.1/ngcpp/cli/cluster_info.py
--rw-r--r--   0        0        0     4026 2023-08-08 01:34:55.148955 ngcpp-0.0.1/ngcpp/cluster.py
--rw-r--r--   0        0        0     1154 2023-08-08 01:10:21.779194 ngcpp-0.0.1/ngcpp/cluster.yaml
--rw-r--r--   0        0        0      383 2023-08-08 01:30:08.160425 ngcpp-0.0.1/ngcpp/utils.py
--rw-r--r--   0        0        0      666 2023-08-08 01:10:21.779194 ngcpp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 ngcpp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      173 2023-08-08 01:57:21.970742 ngcpp-0.0.2/README.md
+-rw-r--r--   0        0        0      884 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cli/cluster_info.py
+-rw-r--r--   0        0        0     4146 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cluster.py
+-rw-r--r--   0        0        0     1154 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cluster.yaml
+-rw-r--r--   0        0        0      383 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/utils.py
+-rw-r--r--   0        0        0      666 2023-08-08 01:57:23.109734 ngcpp-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 ngcpp-0.0.2/PKG-INFO
```

### Comparing `ngcpp-0.0.1/ngcpp/cli/cluster_info.py` & `ngcpp-0.0.2/ngcpp/cli/cluster_info.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.1/ngcpp/cluster.py` & `ngcpp-0.0.2/ngcpp/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
             f" --status RUNNING > /tmp/ngcpp_{self.name}.csv"
         )
         if stderr:
             logging.info(stderr)
             raise RuntimeError("ngc batch list error")
         df = pd.read_csv(f"/tmp/ngcpp_{self.name}.csv").dropna(subset=["Id"])
         df["Id"] = df["Id"].astype(int)
+        # if df is empty, return
+        if df.empty:
+            logging.info("No running jobs")
+            return df
         # get id of running jobs
         for _, row in df.iterrows():
             cur_id = row["Id"]
             dir_fp = f"/tmp/ngcpp/{cur_id}"
             if not os.path.exists(dir_fp):
                 os.makedirs(dir_fp)
             _, stderr = run_simple_command(
```

### Comparing `ngcpp-0.0.1/ngcpp/cluster.yaml` & `ngcpp-0.0.2/ngcpp/cluster.yaml`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.1/pyproject.toml` & `ngcpp-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngcpp"
-version = "0.0.1"
+version = "0.0.2"
 description = "A toolkit for ngc"
 authors = ["Qinsheng <qsh.zh27@gmail.com>"]
 readme = "README.md"
 keywords = ["jam", "experiment", "ngc"]
 license = "MIT"
 packages = [
     {include = "ngcpp"},
```

### Comparing `ngcpp-0.0.1/PKG-INFO` & `ngcpp-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngcpp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolkit for ngc
 License: MIT
 Keywords: jam,experiment,ngc
 Author: Qinsheng
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

