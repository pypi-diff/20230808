# Comparing `tmp/ngcpp-0.0.2.tar.gz` & `tmp/ngcpp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngcpp-0.0.2.tar", max compression
+gzip compressed data, was "ngcpp-0.0.3.tar", max compression
```

## Comparing `ngcpp-0.0.2.tar` & `ngcpp-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      173 2023-08-08 01:57:21.970742 ngcpp-0.0.2/README.md
--rw-r--r--   0        0        0      884 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cli/cluster_info.py
--rw-r--r--   0        0        0     4146 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cluster.py
--rw-r--r--   0        0        0     1154 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/cluster.yaml
--rw-r--r--   0        0        0      383 2023-08-08 01:57:21.970742 ngcpp-0.0.2/ngcpp/utils.py
--rw-r--r--   0        0        0      666 2023-08-08 01:57:23.109734 ngcpp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 ngcpp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      574 2023-08-08 03:18:20.306765 ngcpp-0.0.3/README.md
+-rw-r--r--   0        0        0     1331 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cli/cluster_info.py
+-rw-r--r--   0        0        0     6920 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cli/job_info.py
+-rw-r--r--   0        0        0     4656 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cluster.py
+-rw-r--r--   0        0        0     1154 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cluster.yaml
+-rw-r--r--   0        0        0      383 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/utils.py
+-rw-r--r--   0        0        0      717 2023-08-08 03:18:24.076802 ngcpp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 ngcpp-0.0.3/PKG-INFO
```

### Comparing `ngcpp-0.0.2/ngcpp/cli/cluster_info.py` & `ngcpp-0.0.3/ngcpp/cli/cluster_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,9 +40,28 @@
     """
     List all available cluster aliases
     """
     for k, v in ALIAS_TO_CLUSTER.items():
         print(f"{k} : {v}")
 
 
+@app.command()
+def list(  # pylint: disable=redefined-builtin
+    alias: str = typer.Argument(
+        "10",
+        help="cluster alias, e.g. 10 for prd10, "
+        "use alias command to list all available aliases",
+    )
+):
+    """
+    List user jobs
+    """
+    cluster = Cluster(alias)
+    df = cluster.jobs()
+    del df["Team"]
+    del df["Status Details"]
+    df = df.sort_values(by=["Status", "Id"])
+    print(df.to_string(index=False))
+
+
 def main():
     app()
```

### Comparing `ngcpp-0.0.2/ngcpp/cluster.py` & `ngcpp-0.0.3/ngcpp/cluster.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,7 +104,23 @@
 
         # Sorting the result by Replicas usage in descending order
         df = df.sort_values(by="Replicas", ascending=False)
 
         # Displaying the result
         print(df.to_string(index=False))
         return df
+
+    def jobs(
+        self,
+    ):
+        _, stderr = run_simple_command(
+            f"ngc batch list --format_type csv --team {self.team} --ace {self.ace}"
+            f" > /tmp/ngcpp_{self.name}.csv"
+        )
+        if stderr:
+            logging.info(stderr)
+            raise RuntimeError("ngc batch list error")
+        df = pd.read_csv(f"/tmp/ngcpp_{self.name}.csv").dropna(subset=["Id"])
+        df["Id"] = df["Id"].astype(int)
+        df = df.sort_values("Id", ascending=False)
+
+        return df
```

### Comparing `ngcpp-0.0.2/ngcpp/cluster.yaml` & `ngcpp-0.0.3/ngcpp/cluster.yaml`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.2/pyproject.toml` & `ngcpp-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngcpp"
-version = "0.0.2"
+version = "0.0.3"
 description = "A toolkit for ngc"
 authors = ["Qinsheng <qsh.zh27@gmail.com>"]
 readme = "README.md"
 keywords = ["jam", "experiment", "ngc"]
 license = "MIT"
 packages = [
     {include = "ngcpp"},
@@ -13,21 +13,23 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 typer = "^0.3.2"
 loguru = "^0.7.0"
 hydra-core = "^1.1.0"
 pyfzf = "^0.2.2"
 pandas = "^1.5.3"
+tqdm = "^4.65.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pre-commit = "^2.13.0"
 black = "^21.5b1"
 isort = "^5.8.0"
 pylint = "^2.8.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ngc_cluster="ngcpp.cli.cluster_info:main"
+ngc_job="ngcpp.cli.job_info:main"
```

### Comparing `ngcpp-0.0.2/PKG-INFO` & `ngcpp-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngcpp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A toolkit for ngc
 License: MIT
 Keywords: jam,experiment,ngc
 Author: Qinsheng
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,33 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: hydra-core (>=1.1.0,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyfzf (>=0.2.2,<0.3.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
-# support
+# Install
+
+```shell
+pip install ngcpp
+sudo apt intall fzf # iteractive fuzzy finder
+```
+
+# Feature
+
+## cluster `ngc_cluster --help`
 
 * `ngc_cluster usage --help`: List user usage
 * `ngc_cluster hang --help`: List all hanging jobs
+* `ngc_cluster list --help`: List all jobs in one cluster
 * `ngc_cluster alias --help`: List all available cluster aliases
 
+## job `ngc_job --help`
+
+* `ngc_job kill --help`: kill jobs interactively
+* `ngc_job result --help`: download results for jobs interactively
+* `ngc_job bash --help`: exec bash for one selected job~(support autoresuming)
+
```

