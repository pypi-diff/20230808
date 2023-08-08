# Comparing `tmp/toolforge-weld-1.1.1.tar.gz` & `tmp/toolforge-weld-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-1.1.1.tar", last modified: Mon Jul  3 11:53:15 2023, max compression
+gzip compressed data, was "toolforge-weld-1.2.0.tar", last modified: Tue Aug  8 15:18:27 2023, max compression
```

## Comparing `toolforge-weld-1.1.1.tar` & `toolforge-weld-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-07-03 11:47:16.000000 toolforge-weld-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.756692 toolforge-weld-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.756692 toolforge-weld-1.1.1/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3503 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7730 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3684 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 11:53:07.000000 toolforge-weld-1.1.1/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:18:27.875789 toolforge-weld-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-08-08 15:18:27.875789 toolforge-weld-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 15:18:27.875789 toolforge-weld-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:18:27.871789 toolforge-weld-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:18:27.871789 toolforge-weld-1.2.0/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7730 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4275 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:18:27.875789 toolforge-weld-1.2.0/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:18:19.000000 toolforge-weld-1.2.0/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-08-08 15:09:46.000000 toolforge-weld-1.2.0/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:18:27.875789 toolforge-weld-1.2.0/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-08-08 15:18:27.000000 toolforge-weld-1.2.0/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2023-08-08 15:18:27.000000 toolforge-weld-1.2.0/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:18:27.000000 toolforge-weld-1.2.0/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-08-08 15:18:27.000000 toolforge-weld-1.2.0/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-08 15:18:27.000000 toolforge-weld-1.2.0/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-1.1.1/LICENSE` & `toolforge-weld-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/PKG-INFO` & `toolforge-weld-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.1.1
+Version: 1.2.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.1.1/setup.py` & `toolforge-weld-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="1.1.1",
+    version="1.2.0",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
     long_description=(this_directory / "README.md").read_text(),
```

### Comparing `toolforge-weld-1.1.1/tests/test_api_client.py` & `toolforge-weld-1.2.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/tests/test_config.py` & `toolforge-weld-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/tests/test_kubernetes_config.py` & `toolforge-weld-1.2.0/tests/test_kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/api_client.py` & `toolforge-weld-1.2.0/toolforge_weld/api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/config.py` & `toolforge-weld-1.2.0/toolforge_weld/config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/errors.py` & `toolforge-weld-1.2.0/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/kubernetes.py` & `toolforge-weld-1.2.0/toolforge_weld/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/kubernetes_config.py` & `toolforge-weld-1.2.0/toolforge_weld/kubernetes_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,22 +35,38 @@
 
     @classmethod
     def from_path(cls, path: Path) -> "Kubeconfig":
         data = yaml.safe_load(path.read_text())
         current_context = _find_cfg_obj(data, "contexts", data["current-context"])
         current_cluster = _find_cfg_obj(data, "clusters", current_context["cluster"])
         current_user = _find_cfg_obj(data, "users", current_context["user"])
+        # TODO: handle when the contents of the cert are embedded in the kubeconfig
+        client_cert_file = (
+            _resolve_file_path(path.parent, current_user["client-certificate"])
+            if current_user.get("client-certificate", None)
+            else None
+        )
+        # TODO: handle when the contents of the key are embedded in the kubeconfig
+        client_key_file = (
+            _resolve_file_path(path.parent, current_user["client-key"])
+            if current_user.get("client-key", None)
+            else None
+        )
+        token = current_user.get("token", None)
+
+        if not token and (not client_cert_file or not client_key_file):
+            raise ToolforgeKubernetesConfigError(
+                "Either token or both client-cert and client-key must be provided in the kubeconfig."
+            )
+
         return cls(
             current_server=current_cluster["server"],
-            # TODO: handle when the contents of the cert are embedded in the kubeconfig
-            client_cert_file=_resolve_file_path(
-                path.parent, current_user["client-certificate"]
-            ),
-            # TODO: handle when the contents of the key are embedded in the kubeconfig
-            client_key_file=_resolve_file_path(path.parent, current_user["client-key"]),
+            client_cert_file=client_cert_file,
+            client_key_file=client_key_file,
+            token=current_user.get("token", None),
             current_namespace=current_context["namespace"],
         )
 
     @classmethod
     def load(cls, path: Optional[Path] = None) -> "Kubeconfig":
         """Load the kubeconfig file from the given path or environment and standard locations."""
         if path is None:
```

### Comparing `toolforge-weld-1.1.1/toolforge_weld/logs/__init__.py` & `toolforge-weld-1.2.0/toolforge_weld/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-1.2.0/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld/logs/source.py` & `toolforge-weld-1.2.0/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.1/toolforge_weld.egg-info/PKG-INFO` & `toolforge-weld-1.2.0/toolforge_weld.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.1.1
+Version: 1.2.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.1.1/toolforge_weld.egg-info/SOURCES.txt` & `toolforge-weld-1.2.0/toolforge_weld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

