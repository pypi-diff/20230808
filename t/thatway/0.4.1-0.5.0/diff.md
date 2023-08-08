# Comparing `tmp/thatway-0.4.1.tar.gz` & `tmp/thatway-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thatway-0.4.1.tar", last modified: Tue Aug  8 15:51:56 2023, max compression
+gzip compressed data, was "thatway-0.5.0.tar", last modified: Tue Aug  8 18:26:10 2023, max compression
```

## Comparing `thatway-0.4.1.tar` & `thatway-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.954287 thatway-0.4.1/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.4.1/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)     6004 2023-08-08 15:51:56.954086 thatway-0.4.1/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     5630 2023-08-08 15:49:41.000000 thatway-0.4.1/README.rst
--rw-r--r--   0 jlorieau   (501) staff       (20)      819 2023-08-08 15:51:25.000000 thatway-0.4.1/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 15:51:56.954372 thatway-0.4.1/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.951531 thatway-0.4.1/tests/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6020 2023-08-08 15:17:21.000000 thatway-0.4.1/tests/test_base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.952235 thatway-0.4.1/thatway/
--rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 15:51:14.000000 thatway-0.4.1/thatway/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11450 2023-08-08 14:44:07.000000 thatway-0.4.1/thatway/base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.953746 thatway-0.4.1/thatway.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6004 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/top_level.txt
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.037705 thatway-0.5.0/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.5.0/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6382 2023-08-08 18:26:10.037453 thatway-0.5.0/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6008 2023-08-08 18:25:02.000000 thatway-0.5.0/README.rst
+-rw-r--r--   0 jlorieau   (501) staff       (20)      819 2023-08-08 15:51:25.000000 thatway-0.5.0/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 18:26:10.037799 thatway-0.5.0/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.034547 thatway-0.5.0/tests/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6629 2023-08-08 18:20:16.000000 thatway-0.5.0/tests/test_base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.035353 thatway-0.5.0/thatway/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 18:25:38.000000 thatway-0.5.0/thatway/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13169 2023-08-08 18:20:09.000000 thatway-0.5.0/thatway/base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.037096 thatway-0.5.0/thatway.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6382 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/top_level.txt
```

### Comparing `thatway-0.4.1/LICENSE` & `thatway-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thatway-0.4.1/PKG-INFO` & `thatway-0.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: thatway
-Version: 0.4.1
-Author: Justin Lorieau
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 ThatWay
 =======
 .. image:: https://img.shields.io/pypi/v/thatway.svg
     :target: https://pypi.org/project/thatway/
     :alt: PyPI version
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -224,7 +211,25 @@
       a: 1
     b: name  # The 'b' setting
     nested:
       c: true
 
 And `yaml <https://yaml.org>`_ strings or files can be loaded with
 ``config.loads_yaml(string)`` and ``config.load_yaml(filepath)``, respectively.
+
+3. Toml processing
+~~~~~~~~~~~~~~~~~~
+
+Settings can be dumped in `toml <https://toml.io/en/>`_.
+
+``config.dumps_toml()``
+
+.. code-block:: toml
+
+    [Obj]
+      a = 1
+    b = name  # The 'b' setting
+    [nested]
+      c = true
+
+And `toml <https://toml.io/en/>`_ strings or files can be loaded with
+``config.loads_toml(string)`` and ``config.load_toml(filepath)``, respectively.
```

### Comparing `thatway-0.4.1/README.rst` & `thatway-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: thatway
+Version: 0.5.0
+Author: Justin Lorieau
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 ThatWay
 =======
 .. image:: https://img.shields.io/pypi/v/thatway.svg
     :target: https://pypi.org/project/thatway/
     :alt: PyPI version
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -211,7 +224,25 @@
       a: 1
     b: name  # The 'b' setting
     nested:
       c: true
 
 And `yaml <https://yaml.org>`_ strings or files can be loaded with
 ``config.loads_yaml(string)`` and ``config.load_yaml(filepath)``, respectively.
+
+3. Toml processing
+~~~~~~~~~~~~~~~~~~
+
+Settings can be dumped in `toml <https://toml.io/en/>`_.
+
+``config.dumps_toml()``
+
+.. code-block:: toml
+
+    [Obj]
+      a = 1
+    b = name  # The 'b' setting
+    [nested]
+      c = true
+
+And `toml <https://toml.io/en/>`_ strings or files can be loaded with
+``config.loads_toml(string)`` and ``config.load_toml(filepath)``, respectively.
```

### Comparing `thatway-0.4.1/pyproject.toml` & `thatway-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thatway-0.4.1/tests/test_base.py` & `thatway-0.5.0/tests/test_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -228,7 +228,31 @@
         config.loads_toml(toml_string)
     elif mode == "file":
         tmp_file = tmp_path / "settings.toml"
         tmp_file.write_text(toml_string)
         config.load_toml(tmp_file)
 
     assert Obj.a == 2
+
+
+def test_config_dumps_toml(config):
+    """Test the config.dumps_toml method for generating toml strings"""
+
+    # Setup a config
+    class Obj:
+        a = Setting(1)
+        b = Setting((1, 2, 3))
+        c = Setting("my message")
+        d = Setting(True, desc="my true setting")
+
+    # Retrieve and compare the yaml string
+    toml = config.dumps_toml()
+    assert toml == (
+        "[Obj]\n"
+        "  a = 1\n"
+        "  b = [1, 2, 3]\n"
+        "  c = 'my message'\n"
+        "  d = true  # my true setting\n"
+    )
+
+    # The string can be loaded back without exception
+    config.loads_toml(toml)
```

### Comparing `thatway-0.4.1/thatway/base.py` & `thatway-0.5.0/thatway/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,17 +317,63 @@
             else:
                 # Only Config and Setting objects should be in here
                 raise ConfigException(f"Unknown config type for entry '{v}'")
         return string
 
     # toml methods
 
+    @staticmethod
+    def _to_toml(value) -> str:
+        """Convert a value to a string formatted for yaml"""
+        if isinstance(value, bool):
+            return str(value).lower()
+        elif isinstance(value, str):
+            return f"'{value}'"
+        elif isinstance(value, list) or isinstance(value, tuple):
+            return f"[{', '.join(map(Config._to_toml, value))}]"
+        else:
+            return str(value)
+
     def loads_toml(self, string: str) -> None:
         """Load settings from a toml string into the config"""
         d = tomllib.loads(string)
         self.update(d)
 
     def load_toml(self, filepath: str) -> None:
         """Load settings from a toml file into the config"""
         with open(filepath, "rb") as f:
             d = tomllib.load(f)
         self.update(d)
+
+    def dumps_toml(self, level: int = 0, indent: int = 2) -> str:
+        """Dump settings from the config into a toml string
+
+        Parameters
+        ----------
+        level
+            The current level of the config for nested configs
+        indent
+            The number of spaces to indent each level
+
+        Returns
+        -------
+        yaml
+            A yaml-formatted string
+        """
+        string = ""
+        for k, v in self.__dict__.items():
+            spacer = " " * indent * level
+            if isinstance(v, Setting):
+                # Format the setting value and, optionally, its description
+                comment = f"  # {v.desc}" if v.desc else ""
+                value = self._to_toml(v.value)
+                string += f"{spacer}{k} = {value}{comment}\n"
+
+            elif isinstance(v, Config):
+                # Print the config as a new section then use the config's corresponding
+                # dump method to get its values
+                string += f"{spacer}[{k}]\n"
+                string += v.dumps_toml(level=level + 1, indent=indent)  # this method
+            else:
+                # Only Config and Setting objects should be in here
+                raise ConfigException(f"Unknown config type for entry '{v}'")
+        return string
```

### Comparing `thatway-0.4.1/thatway.egg-info/PKG-INFO` & `thatway-0.5.0/thatway.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thatway
-Version: 0.4.1
+Version: 0.5.0
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
@@ -224,7 +224,25 @@
       a: 1
     b: name  # The 'b' setting
     nested:
       c: true
 
 And `yaml <https://yaml.org>`_ strings or files can be loaded with
 ``config.loads_yaml(string)`` and ``config.load_yaml(filepath)``, respectively.
+
+3. Toml processing
+~~~~~~~~~~~~~~~~~~
+
+Settings can be dumped in `toml <https://toml.io/en/>`_.
+
+``config.dumps_toml()``
+
+.. code-block:: toml
+
+    [Obj]
+      a = 1
+    b = name  # The 'b' setting
+    [nested]
+      c = true
+
+And `toml <https://toml.io/en/>`_ strings or files can be loaded with
+``config.loads_toml(string)`` and ``config.load_toml(filepath)``, respectively.
```

