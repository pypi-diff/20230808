# Comparing `tmp/torchapp-0.3.2.tar.gz` & `tmp/torchapp-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchapp-0.3.2.tar", max compression
+gzip compressed data, was "torchapp-0.3.3.tar", max compression
```

## Comparing `torchapp-0.3.2.tar` & `torchapp-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11345 2023-08-02 01:47:15.130976 torchapp-0.3.2/LICENSE
--rw-r--r--   0        0        0     6537 2023-08-02 01:47:15.130976 torchapp-0.3.2/README.rst
--rw-r--r--   0        0        0     2142 2023-08-02 01:47:15.134976 torchapp-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/__init__.py
--rw-r--r--   0        0        0    33403 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/apps.py
--rw-r--r--   0        0        0     2141 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/fastai.bib
--rw-r--r--   0        0        0      633 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/mlflow.bib
--rw-r--r--   0        0        0      426 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/optuna.bib
--rw-r--r--   0        0        0      470 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/skopt.bib
--rw-r--r--   0        0        0      244 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/torchapp.bib
--rw-r--r--   0        0        0      185 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/wandb.bib
--rw-r--r--   0        0        0      420 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/blocks.py
--rw-r--r--   0        0        0       84 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/__init__.py
--rw-r--r--   0        0        0     4116 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/mlflow.py
--rw-r--r--   0        0        0      717 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/wandb.py
--rw-r--r--   0        0        0     1937 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/citations.py
--rw-r--r--   0        0        0     2215 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/download.py
--rw-r--r--   0        0        0     1904 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/enums.py
--rw-r--r--   0        0        0        0 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/__init__.py
--rw-r--r--   0        0        0    12563 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/diffusion.py
--rw-r--r--   0        0        0     6750 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/image_classifier.py
--rw-r--r--   0        0        0      738 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/iris.bib
--rw-r--r--   0        0        0     1512 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/iris.py
--rwxr-xr-x   0        0        0     1809 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/logistic_regression.py
--rw-r--r--   0        0        0     1053 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/mlp.py
--rw-r--r--   0        0        0     2435 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/main.py
--rw-r--r--   0        0        0      638 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/metrics.py
--rw-r--r--   0        0        0     1161 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/params.py
--rw-r--r--   0        0        0    15534 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/testing.py
--rw-r--r--   0        0        0        0 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/__init__.py
--rw-r--r--   0        0        0     2763 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/optuna.py
--rw-r--r--   0        0        0     5376 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/skopt.py
--rw-r--r--   0        0        0     3794 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/wandb.py
--rw-r--r--   0        0        0     3704 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/util.py
--rw-r--r--   0        0        0     3384 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/vision.py
--rw-r--r--   0        0        0     8479 1970-01-01 00:00:00.000000 torchapp-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-08-08 08:55:38.758574 torchapp-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6537 2023-08-08 08:55:38.758574 torchapp-0.3.3/README.rst
+-rw-r--r--   0        0        0     2142 2023-08-08 08:55:38.762574 torchapp-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/__init__.py
+-rw-r--r--   0        0        0    33403 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/apps.py
+-rw-r--r--   0        0        0     2141 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/fastai.bib
+-rw-r--r--   0        0        0      633 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/mlflow.bib
+-rw-r--r--   0        0        0      426 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/optuna.bib
+-rw-r--r--   0        0        0      470 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/skopt.bib
+-rw-r--r--   0        0        0      244 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/torchapp.bib
+-rw-r--r--   0        0        0      185 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/bibtex/wandb.bib
+-rw-r--r--   0        0        0      420 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/blocks.py
+-rw-r--r--   0        0        0       84 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/callbacks/__init__.py
+-rw-r--r--   0        0        0     4116 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/callbacks/mlflow.py
+-rw-r--r--   0        0        0      717 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/callbacks/wandb.py
+-rw-r--r--   0        0        0     1937 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/citations.py
+-rw-r--r--   0        0        0     2215 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/download.py
+-rw-r--r--   0        0        0     1904 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/enums.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/__init__.py
+-rw-r--r--   0        0        0    12563 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/diffusion.py
+-rw-r--r--   0        0        0     6750 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/image_classifier.py
+-rw-r--r--   0        0        0      738 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/iris.bib
+-rw-r--r--   0        0        0     1512 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/iris.py
+-rwxr-xr-x   0        0        0     1809 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/logistic_regression.py
+-rw-r--r--   0        0        0     1053 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/examples/mlp.py
+-rw-r--r--   0        0        0     2435 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/main.py
+-rw-r--r--   0        0        0      638 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/metrics.py
+-rw-r--r--   0        0        0     1161 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/params.py
+-rw-r--r--   0        0        0    14104 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/testing.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/tuning/__init__.py
+-rw-r--r--   0        0        0     2763 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/tuning/optuna.py
+-rw-r--r--   0        0        0     5376 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/tuning/skopt.py
+-rw-r--r--   0        0        0     3794 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/tuning/wandb.py
+-rw-r--r--   0        0        0     3704 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/util.py
+-rw-r--r--   0        0        0     3384 2023-08-08 08:55:38.766574 torchapp-0.3.3/torchapp/vision.py
+-rw-r--r--   0        0        0     8479 1970-01-01 00:00:00.000000 torchapp-0.3.3/PKG-INFO
```

### Comparing `torchapp-0.3.2/LICENSE` & `torchapp-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/README.rst` & `torchapp-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/pyproject.toml` & `torchapp-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torchapp"
-version = "0.3.2"
+version = "0.3.3"
 description = "A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning."
 authors = ["Robert Turnbull <robert.turnbull@unimelb.edu.au>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/rbturnbull/torchapp"
 documentation = "https://rbturnbull.github.io/torchapp/"
 homepage = "https://github.com/rbturnbull/torchapp"
```

### Comparing `torchapp-0.3.2/torchapp/apps.py` & `torchapp-0.3.3/torchapp/apps.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/bibtex/fastai.bib` & `torchapp-0.3.3/torchapp/bibtex/fastai.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/bibtex/mlflow.bib` & `torchapp-0.3.3/torchapp/bibtex/mlflow.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/callbacks/mlflow.py` & `torchapp-0.3.3/torchapp/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/callbacks/wandb.py` & `torchapp-0.3.3/torchapp/callbacks/wandb.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/citations.py` & `torchapp-0.3.3/torchapp/citations.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/download.py` & `torchapp-0.3.3/torchapp/download.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/enums.py` & `torchapp-0.3.3/torchapp/enums.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/diffusion.py` & `torchapp-0.3.3/torchapp/examples/diffusion.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/image_classifier.py` & `torchapp-0.3.3/torchapp/examples/image_classifier.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/iris.bib` & `torchapp-0.3.3/torchapp/examples/iris.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/iris.py` & `torchapp-0.3.3/torchapp/examples/iris.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/logistic_regression.py` & `torchapp-0.3.3/torchapp/examples/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/examples/mlp.py` & `torchapp-0.3.3/torchapp/examples/mlp.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/main.py` & `torchapp-0.3.3/torchapp/main.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/metrics.py` & `torchapp-0.3.3/torchapp/metrics.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/params.py` & `torchapp-0.3.3/torchapp/params.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/testing.py` & `torchapp-0.3.3/torchapp/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         return re.sub(r"\s+", " ", obj)
     if isinstance(obj, dict):
         return {k:strip_whitespace_recursive(v) for k,v in obj.items()}
 
     return obj
 
 
-def assert_output(file: Path, interactive: bool, params: dict, output, expected, regenerate: bool = False):
+def assert_output(file: Path, interactive: bool, params: dict, output, expected, regenerate: bool = False, threshold:float=0.9):
     """
     Tests to see if the output is the same as the expected data and allows for saving a new version of the expected files if needed.
 
     Args:
         file (Path): The path to the expected file in yaml format.
         interactive (bool): Whether or not to prompt for replacing the expected file.
         params (dict): The dictionary of parameters to store in the expected file.
@@ -109,22 +109,18 @@
     """
     if expected == output:
         return
 
     # if expected and output are both strings, check to see if they are equal when normalizing whitespace
     expected_cleaned = strip_whitespace_recursive(expected)
     output_cleaned = strip_whitespace_recursive(output)
+
     if expected_cleaned == output_cleaned:
         return
 
-    print(' ----------------------\n')
-    print('expected_cleaned ----------------------\n', expected_cleaned)
-    print('output_cleaned ----------------------\n', output_cleaned)
-    print(' ----------------------\n')
-
     if isinstance(expected, dict) and isinstance(output, dict):
         keys = set(expected.keys()) | set(output.keys())
         diff = {}
         for key in keys:
             diff[key] = get_diff(expected.get(key, ""), output.get(key, ""))
             if diff[key]:
                 console.print(diff[key])
@@ -366,45 +362,30 @@
 
     def test_one_batch_output_size(self, interactive: bool):
         self.perform_subtests(interactive=interactive, name=sys._getframe().f_code.co_name)
 
     def test_one_batch_loss(self, interactive: bool):
         self.perform_subtests(interactive=interactive, name=sys._getframe().f_code.co_name)
 
-    def test_cli(self, interactive: bool):
-        app = self.get_app()
-        regenerate = False
-        name = sys._getframe().f_code.co_name
 
-        if interactive:
-            if not self.subtest_files(name):
-                prompt_response = input(
-                    f"\nNo expected files for '{name}' when testing '{app}'.\n"
-                    "Should default expected files be automatically generated? (y/N) "
-                )
-                if prompt_response.lower() == "y":
-                    regenerate = True
-                    directory = self.subtest_dir(name)
-                    default_commands = ["train", "predict", "show-batch", "tune"]
-                    for command in default_commands:
-                        with open(directory / f"{command}_help.yaml", "w") as f:
-                            data = OrderedDict(
-                                params=[command, "--help"], output=""
-                            )  # The output will be autogenerated later
-                            yaml.dump(data, f)
-                    plain_commands = ["bibtex", "bibliography"]
-                    for command in plain_commands:
-                        with open(directory / f"{command}.yaml", "w") as f:
-                            data = OrderedDict(params=[command], output="")  # The output will be autogenerated later
-                            yaml.dump(data, f)
+    def cli_commands_to_test(self):
+        return [
+            "--help",
+            "train --help",
+            "infer --help",
+            "show-batch --help",
+            "tune --help",
+            "bibtex",
+            "bibliography",
+        ]
 
+    def test_cli(self):
+        app = self.get_app()
         runner = CliRunner()
-        for params, expected_output, file in self.subtests(app, name):
-            result = runner.invoke(app.cli(), params)
-            output = dict(
-                stdout=literal(result.stdout),
-                exit_code=result.exit_code,
-            )
+        for command in self.cli_commands_to_test():
+            print(command)
+            result = runner.invoke(app.cli(), command.split())
+            assert result.exit_code == 0
+            assert result.stdout
 
-            assert_output(file, interactive, params, output, expected_output, regenerate=regenerate)
```

### Comparing `torchapp-0.3.2/torchapp/tuning/optuna.py` & `torchapp-0.3.3/torchapp/tuning/optuna.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/tuning/skopt.py` & `torchapp-0.3.3/torchapp/tuning/skopt.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/tuning/wandb.py` & `torchapp-0.3.3/torchapp/tuning/wandb.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/util.py` & `torchapp-0.3.3/torchapp/util.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/torchapp/vision.py` & `torchapp-0.3.3/torchapp/vision.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.2/PKG-INFO` & `torchapp-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchapp
-Version: 0.3.2
+Version: 0.3.3
 Summary: A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning.
 Home-page: https://github.com/rbturnbull/torchapp
 License: Apache-2.0
 Keywords: fastai,pytorch,deep learning,command-line interface
 Author: Robert Turnbull
 Author-email: robert.turnbull@unimelb.edu.au
 Requires-Python: >=3.8,<3.12
```

