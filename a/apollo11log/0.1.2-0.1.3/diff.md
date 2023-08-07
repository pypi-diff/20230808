# Comparing `tmp/apollo11log-0.1.2.tar.gz` & `tmp/apollo11log-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo11log-0.1.2.tar", max compression
+gzip compressed data, was "apollo11log-0.1.3.tar", max compression
```

## Comparing `apollo11log-0.1.2.tar` & `apollo11log-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      763 2023-08-06 00:50:06.136189 apollo11log-0.1.2/README.md
--rw-r--r--   0        0        0     1065 2023-08-06 01:31:18.758272 apollo11log-0.1.2/apollo11log/__main__.py
--rw-r--r--   0        0        0   818263 2023-08-06 00:30:42.777437 apollo11log-0.1.2/apollo11log/log.txt
--rw-r--r--   0        0        0      454 2023-08-06 01:31:51.138407 apollo11log-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1485 2023-08-06 01:32:03.269189 apollo11log-0.1.2/setup.py
--rw-r--r--   0        0        0     1192 2023-08-06 01:32:03.269450 apollo11log-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      763 2023-08-06 00:50:06.136189 apollo11log-0.1.3/README.md
+-rw-r--r--   0        0        0     1285 2023-08-07 23:00:49.020787 apollo11log-0.1.3/apollo11log/__main__.py
+-rw-r--r--   0        0        0   818263 2023-08-06 00:30:42.777437 apollo11log-0.1.3/apollo11log/log.txt
+-rw-r--r--   0        0        0      454 2023-08-07 23:02:09.849772 apollo11log-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1485 2023-08-07 23:03:30.592070 apollo11log-0.1.3/setup.py
+-rw-r--r--   0        0        0     1192 2023-08-07 23:03:30.592218 apollo11log-0.1.3/PKG-INFO
```

### Comparing `apollo11log-0.1.2/README.md` & `apollo11log-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `apollo11log-0.1.2/apollo11log/log.txt` & `apollo11log-0.1.3/apollo11log/log.txt`

 * *Files identical despite different names*

### Comparing `apollo11log-0.1.2/setup.py` & `apollo11log-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['apollo11log = apollo11log:__main__.main']}
 
 setup_kwargs = {
     'name': 'apollo11log',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Prints Apollo 11 Logs is realtime',
     'long_description': "### Install\n```sh\nsudo pip3 install apollo11log #to install system wide\n```\n\n### Run as a CLI app\n```\n$ apollo11log\n[CDR] 00 00:00:04 Roger. Clock.\n[CDR] 00 00:00:13 Roger. We got a roll program.\n[CMP] 00 00:00:15 Roger. Roll.\n[CDR] 00 00:00:34 Roll's complete an\n```\n\n### Run as a systemd service\n\nCreate a unit file - such as `/etc/systemd/system/apollo11.service`\nwith the contents like\n```\n[Unit]\nDescription=apollo11\nAfter=syslog.target\n\n[Service]\nExecStart=/usr/local/bin/apollo11log\nRestart=always\nRestartSec=120\nSyslogIdentifier=apollo11\n\n[Install]\nWantedBy=multi-user.target\n```\n\nThe enable and start the service\n```\nsudo systemctl enable apollo11.service\nsudo systemctl start apollo11.service\n```\n\n### Watch the logs\n```\njournalctl -u apollo11 -f -n\n```",
     'author': 'xss',
     'author_email': 'michaela@michaela.lgbt',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/xssfox/apollo11log',
```

### Comparing `apollo11log-0.1.2/PKG-INFO` & `apollo11log-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo11log
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prints Apollo 11 Logs is realtime
 Home-page: https://github.com/xssfox/apollo11log
 Author: xss
 Author-email: michaela@michaela.lgbt
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

