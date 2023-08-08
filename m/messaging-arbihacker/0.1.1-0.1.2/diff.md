# Comparing `tmp/messaging_arbihacker-0.1.1.tar.gz` & `tmp/messaging_arbihacker-0.1.2.tar.gz`

## Comparing `messaging_arbihacker-0.1.1.tar` & `messaging_arbihacker-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.idea/messaging_arbihacker.iml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/src/messaging_arbihacker/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/README.MD
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.idea/messaging_arbihacker.iml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/src/messaging_arbihacker/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/README.MD
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 messaging_arbihacker-0.1.2/PKG-INFO
```

### Comparing `messaging_arbihacker-0.1.1/.github/workflows/python-publish.yml` & `messaging_arbihacker-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `messaging_arbihacker-0.1.1/src/messaging_arbihacker/__init__.py` & `messaging_arbihacker-0.1.2/src/messaging_arbihacker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         **kwargs,
     ):
         """
         :param update_entities: entities string are lowercase of table name of owning service by convention
         """
         super().__init__(main, broker=broker, backend=backend, **kwargs)
         # Create out special update queue with binding for each of `update_entities`
+        update_exchange = Exchange(ArbiCelery.UPDATE_Q, type="topic")
         if update_entities is not None:
-            update_exchange = Exchange(ArbiCelery.UPDATE_Q, type="topic")
             self.conf.task_queues = (
                 Queue(
                     bindings=[
                         binding(update_exchange, routing_key=f"{ArbiCelery.UPDATE_Q}.{entity}")
                         for entity in update_entities
                     ]
                 ),
```

### Comparing `messaging_arbihacker-0.1.1/LICENSE` & `messaging_arbihacker-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `messaging_arbihacker-0.1.1/pyproject.toml` & `messaging_arbihacker-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "messaging-arbihacker"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Sergei Aslamazov", email = "mrvisioo@gmail.com" },
 ]
 description = "Messaging utils"
 readme = "README.MD"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `messaging_arbihacker-0.1.1/PKG-INFO` & `messaging_arbihacker-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messaging-arbihacker
-Version: 0.1.1
+Version: 0.1.2
 Summary: Messaging utils
 Project-URL: Homepage, https://github.com/ArbiHacker/messaging-arbihacker
 Author-email: Sergei Aslamazov <mrvisioo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

