# Comparing `tmp/volttron_boptest-0.1.1rc3.tar.gz` & `tmp/volttron_boptest-0.1.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_boptest-0.1.1rc3.tar", max compression
+gzip compressed data, was "volttron_boptest-0.1.1rc4.tar", max compression
```

## Comparing `volttron_boptest-0.1.1rc3.tar` & `volttron_boptest-0.1.1rc4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11927 2023-07-17 18:43:01.662518 volttron_boptest-0.1.1rc3/LICENSE
--rw-r--r--   0        0        0    17236 2023-07-17 18:43:01.662518 volttron_boptest-0.1.1rc3/README.md
--rw-r--r--   0        0        0     1845 2023-07-17 18:44:31.405902 volttron_boptest-0.1.1rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/__init__.py
--rw-r--r--   0        0        0    15888 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/agent.py
--rw-r--r--   0        0        0     1525 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/README.md
--rw-r--r--   0        0        0       77 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpi_calculator.py
--rw-r--r--   0        0        0      499 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.config
--rw-r--r--   0        0        0     1152 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.py
--rw-r--r--   0        0        0    18520 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1rc3/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-08-08 17:49:51.614302 volttron_boptest-0.1.1rc4/LICENSE
+-rw-r--r--   0        0        0    17236 2023-08-08 17:49:51.614302 volttron_boptest-0.1.1rc4/README.md
+-rw-r--r--   0        0        0     1845 2023-08-08 17:51:18.892640 volttron_boptest-0.1.1rc4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/__init__.py
+-rw-r--r--   0        0        0    15888 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/agent.py
+-rw-r--r--   0        0        0     1525 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/README.md
+-rw-r--r--   0        0        0       77 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/__init__.py
+-rw-r--r--   0        0        0     1852 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/custom_kpi_calculator.py
+-rw-r--r--   0        0        0      499 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/custom_kpis_example.config
+-rw-r--r--   0        0        0     1152 2023-08-08 17:49:51.618302 volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/custom_kpis_example.py
+-rw-r--r--   0        0        0    18520 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1rc4/PKG-INFO
```

### Comparing `volttron_boptest-0.1.1rc3/LICENSE` & `volttron_boptest-0.1.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/README.md` & `volttron_boptest-0.1.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/pyproject.toml` & `volttron_boptest-0.1.1rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-boptest"
-version = "0.1.1rc3"
+version = "0.1.1rc4"
 description = "A Volttron agent that runs boptest simulation."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
@@ -37,15 +37,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-volttron-lib-boptest-integration = "^0.1.1rc3"
+volttron-lib-boptest-integration = "^0.1.1rc4"
 numpy = ">0.0.0"
 pandas = ">0.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.2.4"
 pytest-cov = ">=3.0.0"
 pytest-env = ">0.0.0"
```

### Comparing `volttron_boptest-0.1.1rc3/src/boptest/agent.py` & `volttron_boptest-0.1.1rc4/src/boptest/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/README.md` & `volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/README.md`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpi_calculator.py` & `volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/custom_kpi_calculator.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.py` & `volttron_boptest-0.1.1rc4/src/boptest/custom_kpi/custom_kpis_example.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc3/PKG-INFO` & `volttron_boptest-0.1.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-boptest
-Version: 0.1.1rc3
+Version: 0.1.1rc4
 Summary: A Volttron agent that runs boptest simulation.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,agent,boptest,simulation,application
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0)
-Requires-Dist: volttron-lib-boptest-integration (>=0.1.1rc3,<0.2.0)
+Requires-Dist: volttron-lib-boptest-integration (>=0.1.1rc4,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-boptest/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-boptest
 Description-Content-Type: text/markdown
 
 # boptest-agent
 
 The volttron-boptest-agent utilizes the volttron-lib-boptest-integration library to perform simulation control and
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1rc3 Summary: A
+Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1rc4 Summary: A
 Volttron agent that runs boptest simulation. Home-page: https://github.com/
 eclipse-volttron/volttron-boptest License: Apache-2.0 Keywords:
 volttron,agent,boptest,simulation,application Author: Kefei Mo Author-email:
 kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Home Automation Classifier:
 Topic :: Software Development :: Embedded Systems Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0) Requires-Dist: volttron-lib-boptest-integration
-(>=0.1.1rc3,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
+(>=0.1.1rc4,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
 volttron/volttron-boptest/issues Project-URL: Repository, https://github.com/
 eclipse-volttron/volttron-boptest Description-Content-Type: text/markdown #
 boptest-agent The volttron-boptest-agent utilizes the volttron-lib-boptest-
 integration library to perform simulation control and benchmark tasks. BOPTEST
 is designed to facilitate the performance evaluation and benchmarking of
 building control strategies, which contains these key components: 1. Run-Time
 Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API,
```

