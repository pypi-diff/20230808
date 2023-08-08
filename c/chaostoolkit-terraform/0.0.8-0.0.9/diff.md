# Comparing `tmp/chaostoolkit-terraform-0.0.8.tar.gz` & `tmp/chaostoolkit-terraform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.8.tar", last modified: Mon Jul  3 12:57:10 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.9.tar", last modified: Tue Aug  8 10:50:51 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.8.tar` & `chaostoolkit-terraform-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.592165 chaostoolkit-terraform-0.0.8/chaosterraform/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-03 12:57:04.000000 chaostoolkit-terraform-0.0.8/chaosterraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/chaosterraform/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/chaosterraform/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.592165 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-03 12:57:04.000000 chaostoolkit-terraform-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5578 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5289 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/chaosterraform/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-08-08 10:50:45.000000 chaostoolkit-terraform-0.0.9/chaosterraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/chaosterraform/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/chaosterraform/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5578 2023-08-08 10:50:51.000000 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-08-08 10:50:51.000000 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:50:51.000000 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-08 10:50:51.000000 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-08 10:50:51.000000 chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-08 10:50:45.000000 chaostoolkit-terraform-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:50:51.515193 chaostoolkit-terraform-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-08 10:50:29.000000 chaostoolkit-terraform-0.0.9/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.8/LICENSE` & `chaostoolkit-terraform-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.8/PKG-INFO` & `chaostoolkit-terraform-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChaosToolkit Terraform
@@ -27,16 +27,17 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
-you need to define it in your experiment files (or settings):
+**chaostoolkit-terraform** provides a control to deploy Terraform modules. The control will automatically create the resources defined in the Terraform stack before experiment execution and destroy them once the experiment is completed.
+
+To activate the `chaosterraform.control` for your experiments you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
@@ -51,15 +52,15 @@
 
 By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
-| **Configure control** | Initialize the Terraform driver |
+| **Configure control** | Initialize the Terraform driver in Chaos Toolkit|
 | **Before experiment** | Initialize and apply the selected Terraform module |
 | **After experiment**  | Run terraform destroy unless specifically asked to retain the created resources |
 
 ## Configuration
 
 You can configure the Terraform control either via *control arguments* or using Chaos Toolkit parameters with the `tf_conf__` prefix:
 
@@ -85,43 +86,41 @@
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
 ```
 
-> When both options are supplied **configuration parameters supplied via the experiment configuration will
+> When both options are provided **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
-| **chdir** | Instruct Terraform to change its working directory before running subcommands |
+| **chdir** | Instruct Terraform to change its working directory |
 
 ## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using the `variables`
-argument for the control:
+You can override input variables defined in the Terraform module from within the experiment using the `variables` argument for the control:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
       arguments:
         variables:
           vpc_id: "vpc-0000000000"
           number_of_azs: 2
 ```
 
-Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
-already defined in Chaos Toolkit configuration:
+Alternatively, you can provide input variables from Chaos Toolkit configuration by referencing a parameter name already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
   env_name: "live"
   ...
 
 controls:
@@ -169,7 +168,22 @@
       tolerance: 200
       provider:
         type: http
         url: "http://${tf_out__alb_dns_name}"
         method: "GET"
         timeout: 3
 ```
+
+In addition, we can ask the `chaosterraform.control` to map Terraform output values to new Chaos Toolkit configuration variables or override existing ones using the `outputs` argument:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        outputs:
+            alb_dns_name: "application_dns_name"
+```
+
+In the example above, the control will map the output value `alb_dns_name` into a new Chaos Toolkit configuration `application_dns_name` that can be referenced in the experiment template using the `${application_dns_name}` notation.
```

### Comparing `chaostoolkit-terraform-0.0.8/README.md` & `chaostoolkit-terraform-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
-you need to define it in your experiment files (or settings):
+**chaostoolkit-terraform** provides a control to deploy Terraform modules. The control will automatically create the resources defined in the Terraform stack before experiment execution and destroy them once the experiment is completed.
+
+To activate the `chaosterraform.control` for your experiments you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
@@ -42,15 +43,15 @@
 
 By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
-| **Configure control** | Initialize the Terraform driver |
+| **Configure control** | Initialize the Terraform driver in Chaos Toolkit|
 | **Before experiment** | Initialize and apply the selected Terraform module |
 | **After experiment**  | Run terraform destroy unless specifically asked to retain the created resources |
 
 ## Configuration
 
 You can configure the Terraform control either via *control arguments* or using Chaos Toolkit parameters with the `tf_conf__` prefix:
 
@@ -76,43 +77,41 @@
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
 ```
 
-> When both options are supplied **configuration parameters supplied via the experiment configuration will
+> When both options are provided **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
-| **chdir** | Instruct Terraform to change its working directory before running subcommands |
+| **chdir** | Instruct Terraform to change its working directory |
 
 ## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using the `variables`
-argument for the control:
+You can override input variables defined in the Terraform module from within the experiment using the `variables` argument for the control:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
       arguments:
         variables:
           vpc_id: "vpc-0000000000"
           number_of_azs: 2
 ```
 
-Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
-already defined in Chaos Toolkit configuration:
+Alternatively, you can provide input variables from Chaos Toolkit configuration by referencing a parameter name already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
   env_name: "live"
   ...
 
 controls:
@@ -160,7 +159,22 @@
       tolerance: 200
       provider:
         type: http
         url: "http://${tf_out__alb_dns_name}"
         method: "GET"
         timeout: 3
 ```
+
+In addition, we can ask the `chaosterraform.control` to map Terraform output values to new Chaos Toolkit configuration variables or override existing ones using the `outputs` argument:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        outputs:
+            alb_dns_name: "application_dns_name"
+```
+
+In the example above, the control will map the output value `alb_dns_name` into a new Chaos Toolkit configuration `application_dns_name` that can be referenced in the experiment template using the `${application_dns_name}` notation.
```

### Comparing `chaostoolkit-terraform-0.0.8/chaosterraform/__init__.py` & `chaostoolkit-terraform-0.0.9/chaosterraform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from chaoslib.discovery.discover import discover_actions, discover_activities, initialize_discovery_result
 from chaoslib.types import DiscoveredActivities, Discovery
 
 name = "chaosterraform"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
```

### Comparing `chaostoolkit-terraform-0.0.8/chaosterraform/control.py` & `chaostoolkit-terraform-0.0.9/chaosterraform/control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Terraform control module
 
 This module allows Chaos Toolkit users to create infrastructure resources using Terraform scripts
 for the experiment execution.
 """
-from typing import Any, Dict, List
+from typing import Any, Dict
 
 from chaoslib.exceptions import InterruptExecution
 from chaoslib.types import Configuration, Experiment, Journal, Secrets, Settings
 from logzero import logger
 
 from .driver import Terraform
 
@@ -16,36 +16,37 @@
 EXPORT_VAR_PREFIX = "tf_out__"
 
 
 def configure_control(
     silent: bool = True,
     retain: bool = False,
     chdir: str = None,
-    variables: List = None,
+    variables: Dict = None,
     outputs: Dict = None,
     configuration: Configuration = None,
     secrets: Secrets = None,
     settings: Settings = None,
     experiment: Experiment = None,
 ):
     """
     Configure terraform control for the experiment execution
 
     Parameters
     ----------
     silent: bool
         suppress Terraform logs in ChaosToolkit experiment logs
     retain: bool
-        retain created resources at the end of the experiment
+        retain created resources after the end of the experiment
     chdir: str
         change the Terraform working directory
-    variables: List
+    variables: Dict
         input variables configuration for Terraform
     outputs: Dict
-       configuration to map Terraform outputs to ChaosToolkit variables
+       defines how to map Terraform outputs to ChaosToolkit variables. By default
+       output values are always mapped using the "tf_out__" prefix.
 
     Raises
     ------
     InterruptExecution
         If terraform init fails we interrupt the experiment execution immediately
     """
     # pylint: disable=unused-argument
```

### Comparing `chaostoolkit-terraform-0.0.8/chaosterraform/driver.py` & `chaostoolkit-terraform-0.0.9/chaosterraform/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,28 @@
             if not os.path.exists(self.chdir):
                 raise InterruptExecution(f"Terraform: chdir [{self.chdir}] does not exists")
             if not os.path.isdir(self.chdir):
                 raise InterruptExecution(f"Terraform: chdir [{self.chdir}] is not a directory")
             return ["terraform", f"-chdir={self.chdir}"]
         return ["terraform"]
 
+    def _get_var_overrides(self, args=None):
+        _args = deepcopy(self.args)
+        if args:
+            _args.update(args)
+
+        var_overrides = []
+        for key, value in _args.items():
+            string_value = str(value)
+            if isinstance(value, bool):
+                string_value = str(value).lower()
+            var_overrides.extend(["-var", f"{key}={string_value}"])
+
+        return var_overrides
+
     def terraform_init(self):
         """
         Initialize Terraform modules
 
         Raises
         ------
         InterruptExecution
@@ -107,23 +121,15 @@
 
         Raises
         ------
         InterruptExecution
             Interrupts the experiment execution if the Terraform stack failed to create
         """
 
-        args = deepcopy(self.args)
-        args.update(kwargs)
-
-        var_overrides = []
-        for key, value in args.items():
-            string_value = value
-            if isinstance(value, bool):
-                string_value = str(value).lower()
-            var_overrides.extend(["-var", f"{key}={string_value}"])
+        var_overrides = self._get_var_overrides(kwargs)
 
         result = _run(
             self._terraform,
             ["apply", "-auto-approve"],
             var_overrides,
             capture_output=self.silent,
         )
@@ -145,12 +151,14 @@
         outputs = json.loads(result.stdout)
         return outputs
 
     def destroy(self):
         """
         Destroy the resources created by the Terraform stack
         """
+        var_overrides = self._get_var_overrides()
         _run(
             self._terraform,
             ["destroy", "-auto-approve"],
+            var_overrides,
             capture_output=self.silent,
         )
```

### Comparing `chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/PKG-INFO` & `chaostoolkit-terraform-0.0.9/chaostoolkit_terraform.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChaosToolkit Terraform
@@ -27,16 +27,17 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
-you need to define it in your experiment files (or settings):
+**chaostoolkit-terraform** provides a control to deploy Terraform modules. The control will automatically create the resources defined in the Terraform stack before experiment execution and destroy them once the experiment is completed.
+
+To activate the `chaosterraform.control` for your experiments you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
@@ -51,15 +52,15 @@
 
 By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
-| **Configure control** | Initialize the Terraform driver |
+| **Configure control** | Initialize the Terraform driver in Chaos Toolkit|
 | **Before experiment** | Initialize and apply the selected Terraform module |
 | **After experiment**  | Run terraform destroy unless specifically asked to retain the created resources |
 
 ## Configuration
 
 You can configure the Terraform control either via *control arguments* or using Chaos Toolkit parameters with the `tf_conf__` prefix:
 
@@ -85,43 +86,41 @@
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
 ```
 
-> When both options are supplied **configuration parameters supplied via the experiment configuration will
+> When both options are provided **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
-| **chdir** | Instruct Terraform to change its working directory before running subcommands |
+| **chdir** | Instruct Terraform to change its working directory |
 
 ## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using the `variables`
-argument for the control:
+You can override input variables defined in the Terraform module from within the experiment using the `variables` argument for the control:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
       arguments:
         variables:
           vpc_id: "vpc-0000000000"
           number_of_azs: 2
 ```
 
-Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
-already defined in Chaos Toolkit configuration:
+Alternatively, you can provide input variables from Chaos Toolkit configuration by referencing a parameter name already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
   env_name: "live"
   ...
 
 controls:
@@ -169,7 +168,22 @@
       tolerance: 200
       provider:
         type: http
         url: "http://${tf_out__alb_dns_name}"
         method: "GET"
         timeout: 3
 ```
+
+In addition, we can ask the `chaosterraform.control` to map Terraform output values to new Chaos Toolkit configuration variables or override existing ones using the `outputs` argument:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        outputs:
+            alb_dns_name: "application_dns_name"
+```
+
+In the example above, the control will map the output value `alb_dns_name` into a new Chaos Toolkit configuration `application_dns_name` that can be referenced in the experiment template using the `${application_dns_name}` notation.
```

### Comparing `chaostoolkit-terraform-0.0.8/pyproject.toml` & `chaostoolkit-terraform-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "chaostoolkit-terraform"
 description = "A Chaos Toolkit module to deploy terraform stacks"
 readme = "README.md"
-version = "0.0.8"
+version = "0.0.9"
 authors = [ { name = "Manuel Castellin" } ]
 dependencies = [
     'chaostoolkit',
     'chaostoolkit-lib',
 ]
 
 [project.urls]
```

### Comparing `chaostoolkit-terraform-0.0.8/tests/test_control.py` & `chaostoolkit-terraform-0.0.9/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.8/tests/test_driver.py` & `chaostoolkit-terraform-0.0.9/tests/test_driver.py`

 * *Files identical despite different names*

