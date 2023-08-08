# Comparing `tmp/tentakel-4.0.0.tar.gz` & `tmp/tentakel-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentakel-4.0.0.tar", max compression
+gzip compressed data, was "tentakel-4.0.1.tar", max compression
```

## Comparing `tentakel-4.0.0.tar` & `tentakel-4.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1226 2021-02-26 14:54:35.000000 tentakel-4.0.0/README.md
--rw-r--r--   0        0        0      703 2023-01-30 17:29:01.567481 tentakel-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2019-06-21 14:46:57.000000 tentakel-4.0.0/src/tentakel/__init__.py
--rw-r--r--   0        0        0     9331 2023-01-30 16:33:28.669561 tentakel-4.0.0/src/tentakel/config.py
--rw-r--r--   0        0        0     1595 2021-02-26 11:13:11.000000 tentakel-4.0.0/src/tentakel/error.py
--rwxr-xr-x   0        0        0     4328 2023-01-30 16:38:30.569333 tentakel-4.0.0/src/tentakel/main.py
--rw-r--r--   0        0        0      803 2021-02-26 11:22:46.000000 tentakel-4.0.0/src/tentakel/plugins/__init__.py
--rw-r--r--   0        0        0     2445 2021-02-26 15:47:29.000000 tentakel-4.0.0/src/tentakel/plugins/rsh.py
--rw-r--r--   0        0        0     2194 2023-01-30 16:41:05.113783 tentakel-4.0.0/src/tentakel/plugins/ssh.py
--rw-r--r--   0        0        0     9602 2023-01-30 16:41:40.621341 tentakel-4.0.0/src/tentakel/remote.py
--rw-r--r--   0        0        0     3314 2021-02-26 16:02:56.000000 tentakel-4.0.0/src/tentakel/shell.py
--rw-r--r--   0        0        0    81427 2021-11-22 09:44:21.770218 tentakel-4.0.0/src/tentakel/tpg.py
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 tentakel-4.0.0/setup.py
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 tentakel-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1226 2021-02-26 14:54:35.000000 tentakel-4.0.1/README.md
+-rw-r--r--   0        0        0      858 2023-08-08 12:42:05.487869 tentakel-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2019-06-21 14:46:57.000000 tentakel-4.0.1/src/tentakel/__init__.py
+-rw-r--r--   0        0        0     9575 2023-05-29 13:41:54.362696 tentakel-4.0.1/src/tentakel/config.py
+-rw-r--r--   0        0        0     1653 2023-05-29 13:19:04.883835 tentakel-4.0.1/src/tentakel/error.py
+-rwxr-xr-x   0        0        0     4338 2023-05-29 13:33:34.851387 tentakel-4.0.1/src/tentakel/main.py
+-rw-r--r--   0        0        0      803 2021-02-26 11:22:46.000000 tentakel-4.0.1/src/tentakel/plugins/__init__.py
+-rw-r--r--   0        0        0     2445 2021-02-26 15:47:29.000000 tentakel-4.0.1/src/tentakel/plugins/rsh.py
+-rw-r--r--   0        0        0     2194 2023-01-30 16:41:05.113783 tentakel-4.0.1/src/tentakel/plugins/ssh.py
+-rw-r--r--   0        0        0     9630 2023-05-29 13:20:45.697081 tentakel-4.0.1/src/tentakel/remote.py
+-rw-r--r--   0        0        0     3314 2021-02-26 16:02:56.000000 tentakel-4.0.1/src/tentakel/shell.py
+-rw-r--r--   0        0        0    81427 2023-08-08 12:39:04.436503 tentakel-4.0.1/src/tentakel/tpg.py
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 tentakel-4.0.1/PKG-INFO
```

### Comparing `tentakel-4.0.0/README.md` & `tentakel-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tentakel-4.0.0/pyproject.toml` & `tentakel-4.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 [tool.poetry]
 name = "tentakel"
-version = "4.0.0"
+version = "4.0.1"
 description = "distributed command execution"
 license = "BSD"
 homepage = "https://github.com/sfermigier/tentakel"
 authors = [
   "Sebastian Stark, Marlon Berlin <cran@users.sourceforge.net, imaginat@users.sourceforge.net>",
   "Stefane Fermigier <sf@fermigier.com>",
 ]
 readme = "README.md"
-
 packages = [{ include = "tentakel", from = "src" }]
 
-
 [tool.poetry.scripts]
 tentakel = 'tentakel.main:main'
 
-
 [tool.poetry.dependencies]
 python = "^3.9"
 
-
 [tool.poetry.dev-dependencies]
-pytest = "*"
-
-abilian-devtools = "*"
-
+pytest = "^7.4.0"
+abilian-devtools = "^0.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-
 [tool.ruff]
 exclude = ["src/tentakel/tpg.py"]
+
+[tool.pyright]
+exclude = ['.nox', 'tests', 'sandbox', 'doc', 'scripts', 'tmp', "src/tentakel/tpg.py", "src/tentakel/plugins/rsh.py"]
+include = ["src"]
```

### Comparing `tentakel-4.0.0/src/tentakel/config.py` & `tentakel-4.0.1/src/tentakel/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 from __future__ import annotations
 
 import os
 import pwd
 import re
 import sys
 import tempfile
+from pathlib import Path
 
 from . import error, tpg
+from .error import Abort
 
 PARAMS = {
     "ssh_path": "/usr/bin/ssh",
     "rsh_path": "/usr/bin/rsh",
     "method": "ssh",
     "maxparallel": "0",
     "user": pwd.getpwuid(os.geteuid())[0],
@@ -66,15 +68,15 @@
 
 METHODS = ["ssh", "rsh"]
 
 __user_dir = os.path.join(os.environ["HOME"], ".tentakel")
 __user_plugin_dir = os.path.join(__user_dir, "plugins")
 
 
-class TConf(tpg.Parser):
+class ConfigParser(tpg.Parser):
     __doc__ = r"""
 
     set lexer = ContextSensitiveLexer
 
     token keyword  : '{keywords}'  str ;
     token eq       : '='      str ;
     token word     : '\w+'      str ;
@@ -145,14 +147,15 @@
         self["lists"] = []
 
     def __str__(self):
         groups = []
         for param in PARAMS.keys():
             if self[param]:
                 groups.append('{}="{}"'.format(param, re.sub('"', '""', self[param])))
+
         return f"group {self['name']} ({', '.join(groups)})"
 
 
 class ConfigBase(dict):
     """Store all configuration parameters.
 
     This class is used to hold a specific configuration state in a special
@@ -169,56 +172,62 @@
         super().__init__()
         self["groups"] = {}
         self["settings"] = PARAMS
 
     def parse(self, txt):
         """Parse a string containing configuration directives into the
         configuration tree."""
-        tp = TConf()
-        self.update(tp(txt))
+        parser = ConfigParser()
+        self.update(parser(txt))
 
-    def load(self, file):
+    def load(self, path: str | Path):
         """Load configuration from file."""
 
+        if isinstance(path, str):
+            path = Path(path)
+
         try:
-            self.parse("".join(file.readlines()))
+            self.parse(path.read_text())
         except tpg.SyntacticError as excerr:  # pragma: nocover
-            error.warn(f"in {file.name}: {excerr.msg}")
+            error.warn(f"in {path}: {excerr.msg}")
         except OSError:  # pragma: nocover
-            error.err(f"could not read from file: '{file.name}'")
+            raise Abort(f"could not read from file: '{path}'")
 
-    def dump(self, file):
+    def dump(self, path: str | Path):
         """Save configuration to file."""
 
+        if isinstance(path, str):
+            path = Path(path)
+
         comment = [
             "#\n",
             "# CURRENT CONFIGURATION\n",
             "#\n",
             "# You can change the configuration for the current session here.\n",
             "# Those changes will be lost after you quit tentakel.\n",
             "# No configuration file will be changed.\n",
             "#\n",
         ]
 
         try:
-            file.writelines(comment)
-            file.writelines(str(self))
+            text = "".join(comment) + "\n" + str(self)
+            path.write_text(text)
         except OSError:  # pragma: nocover
-            error.err(f"could not write to file: '{file.name}'")
+            raise Abort(f"could not write to file: '{path}'")
 
     def edit(self):
         """Interactively edit configuration."""
 
         tempedit = tempfile.NamedTemporaryFile()
         try:
             self.dump(tempedit)
             tempedit.seek(0, 0)
             editor = os.getenv("VISUAL") or os.getenv("EDITOR") or "vi"
             os.spawnvp(os.P_WAIT, editor, [editor, tempedit.name])
-            self.load(tempedit)
+            self.load(Path(tempedit.name))
         finally:
             tempedit.close()
 
     def __str__(self):
         """Pretty print configuration."""
 
         out = ""
@@ -238,33 +247,34 @@
         return out
 
     def get_groups(self) -> list[str]:
         """Return list of all group names."""
 
         return list(self["groups"].keys())
 
-    def _get_group(self, group_name):
+    def _get_group(self, group_name: str):
         """Return group specific configuration for group_name."""
 
         return self["groups"][group_name]
 
-    def get_group_members(self, group_name):
+    def get_group_members(self, group_name: str):
         """Return list of group_name members with sub lists expanded
         recursively."""
 
         group = self._get_group(group_name)
         out = [(x, self.get_group_params(group_name)) for x in group["hosts"]]
         for list in group["lists"]:
             try:
                 out += self.get_group_members(list)
             except (KeyError, RuntimeError):  # pragma: nocover
                 if sys.exc_info()[0] == KeyError:
                     error.warn(f"in group '{group_name}': no such group '{list}'")
                 if sys.exc_info()[0] == RuntimeError:
-                    error.err("runtime error: possible loop in configuration file")
+                    raise Abort("runtime error: possible loop in configuration file")
+
         return out
 
     def get_param(self, param: str, group=None):
         """Return the value for param.
 
         If group is specified, return the groups local value for param.
         If the group has no local value or group=None or group does not
```

### Comparing `tentakel-4.0.0/src/tentakel/error.py` & `tentakel-4.0.1/src/tentakel/error.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 """Error and user notification for tentakel."""
 
 import sys
 
 
-def err(errstring):
-    sys.stderr.write(f"tentakel error: {errstring}\n")
-    sys.exit(1)
+class Abort(SystemExit):
+    def __init__(self, message):
+        super().__init__(message)
+        sys.stderr.write(f"tentakel error: {message}\n")
 
 
 def warn(warnstring):
     sys.stderr.write(f"tentakel: {warnstring}\n")
```

### Comparing `tentakel-4.0.0/src/tentakel/main.py` & `tentakel-4.0.1/src/tentakel/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,34 +37,37 @@
 
 See tentakel(1) for more information
 """
 
 import getopt
 import os
 import sys
+from pathlib import Path
+
+from tentakel.error import Abort
 
 try:
     from importlib import metadata
 except ImportError:
     # Running on pre-3.8 Python; use importlib-metadata package
     import importlib_metadata as metadata  # type: ignore
 
-from tentakel import config, error, remote, shell
+from . import config, remote, shell
 
 
 def main():
     group_name = "default"
     flag_listgroups = 0
     override_config = ""
 
     try:
         opts, args = getopt.getopt(sys.argv[1:], "g:hlvc:D")
     except getopt.GetoptError:
         print_help()
-        error.err("parameter error")
+        raise Abort("parameter error")
 
     for o, v in opts:
         if o == "-h":
             print_help()
             sys.exit(0)
         if o == "-v":
             print(get_version())
@@ -85,34 +88,32 @@
     # check wether the user has chosen a specific configuration file
     # on the command line
     config_file = None
     if override_config:
         if os.path.isfile(override_config):
             config_file = override_config
         else:
-            error.err(f"no such file: '{override_config}'")
+            raise Abort(f"no such file: '{override_config}'")
     else:
         # look for configuration files from default locations
         configs = [
             os.path.join(config.__user_dir, "tentakel.conf"),
             "/etc/tentakel.conf",
         ]
         for c in configs:
             if os.path.isfile(c):
                 config_file = c
                 break
 
     if config_file is None:
-        error.err("no configuration file found")
-        sys.exit(1)
+        raise Abort("no configuration file found")
 
     # load configuration
     conf = config.ConfigBase()
-    with open(config_file) as f:
-        conf.load(f)
+    conf.load(Path(config_file))
 
     # process -g parameter
     if flag_listgroups:
         print("available groups:")
         for g in conf.get_groups():
             sys.stdout.write(g + " ")
         print()
```

### Comparing `tentakel-4.0.0/src/tentakel/plugins/__init__.py` & `tentakel-4.0.1/src/tentakel/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tentakel-4.0.0/src/tentakel/plugins/rsh.py` & `tentakel-4.0.1/src/tentakel/plugins/rsh.py`

 * *Files identical despite different names*

### Comparing `tentakel-4.0.0/src/tentakel/plugins/ssh.py` & `tentakel-4.0.1/src/tentakel/plugins/ssh.py`

 * *Files identical despite different names*

### Comparing `tentakel-4.0.0/src/tentakel/remote.py` & `tentakel-4.0.1/src/tentakel/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 import queue
 import sys
 import threading
 from abc import ABCMeta, abstractmethod
 
 from . import error, tpg
+from .error import Abort
 
 
 class FormatString(tpg.Parser):
     r"""
 
     token escape  : '\\[\\nt]'  str ;
     token fmtchar  : '%[%dost]'  str ;
@@ -145,15 +146,15 @@
         self.__class__.finished_objects.put(self)
 
     def get_result(self):
         """Return result from result queue."""
         return self._result_queue.get()
 
     def run(self):
-        while not self._stopevent.isSet():
+        while not self._stopevent.is_set():
             try:
                 command = self._command_queue.get(timeout=self._command_timeout)
                 if self.__maxparallel > 0:
                     self.slot.acquire()
                 result = self._rexec(command)
                 if self.__maxparallel > 0:
                     self.slot.release()
@@ -165,23 +166,23 @@
     def join(self, timeout=None):
         """Stop the thread."""
         self._stopevent.set()
         threading.Thread.join(self, self._command_timeout)
 
 
 def remote_command_factory(destination, params):
-    """Depending in the method, instantiate a corresponding RemoteCommand
+    """Depending on the method, instantiate a corresponding RemoteCommand
     derived object and return it."""
 
     method = params["method"]
     try:
         cls = _remote_command_plugins[method]
         return cls(destination, params)
     except KeyError:
-        error.err(f'Method not implemented: "{method}"')
+        raise Abort(f'Method not implemented: "{method}"')
 
 
 class RemoteCollator:
     """This class is meant to hold RemoteCommand instances each of which
     implements a specific way too execute a command on a remote host."""
 
     def __init__(self, conf, group_name):
```

### Comparing `tentakel-4.0.0/src/tentakel/shell.py` & `tentakel-4.0.1/src/tentakel/shell.py`

 * *Files identical despite different names*

### Comparing `tentakel-4.0.0/src/tentakel/tpg.py` & `tentakel-4.0.1/src/tentakel/tpg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1772,15 +1772,15 @@
             options = [ self.lexer_ignorecase,
                         self.lexer_locale,
                         self.lexer_multiline,
                         self.lexer_dotall,
                         self.lexer_verbose,
                         self.lexer_unicode,
                       ]
-            return "+".join([ "tpg.re.%s"%opt for opt in options if opt ]) or 0
+            return "+".join([ f"tpg.re.{opt}" for opt in options if opt ]) or 0
 
     class Empty:
         def empty(self):
             return True
 
     class NotEmpty:
         def empty(self):
```

### Comparing `tentakel-4.0.0/PKG-INFO` & `tentakel-4.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentakel
-Version: 4.0.0
+Version: 4.0.1
 Summary: distributed command execution
 Home-page: https://github.com/sfermigier/tentakel
 License: BSD
 Author: Sebastian Stark, Marlon Berlin
 Author-email: cran@users.sourceforge.net, imaginat@users.sourceforge.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

