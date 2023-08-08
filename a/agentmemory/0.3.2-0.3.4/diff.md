# Comparing `tmp/agentmemory-0.3.2.tar.gz` & `tmp/agentmemory-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.3.2.tar", last modified: Thu Aug  3 07:48:12 2023, max compression
+gzip compressed data, was "agentmemory-0.3.4.tar", last modified: Tue Aug  8 09:39:41 2023, max compression
```

## Comparing `agentmemory-0.3.2.tar` & `agentmemory-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:48:03.000000 agentmemory-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-08-03 07:48:12.768981 agentmemory-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-03 07:48:03.000000 agentmemory-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/agentmemory/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/agentmemory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:48:12.768981 agentmemory-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:48:03.000000 agentmemory-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:39:41.743025 agentmemory-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 09:39:32.000000 agentmemory-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-08-08 09:39:41.743025 agentmemory-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-08-08 09:39:32.000000 agentmemory-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:39:41.739025 agentmemory-0.3.4/agentmemory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-08 09:39:32.000000 agentmemory-0.3.4/agentmemory/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:39:41.743025 agentmemory-0.3.4/agentmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-08-08 09:39:41.000000 agentmemory-0.3.4/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 09:39:41.000000 agentmemory-0.3.4/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:39:41.000000 agentmemory-0.3.4/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 09:39:41.000000 agentmemory-0.3.4/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 09:39:41.000000 agentmemory-0.3.4/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:39:41.743025 agentmemory-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-08 09:39:32.000000 agentmemory-0.3.4/setup.py
```

### Comparing `agentmemory-0.3.2/LICENSE` & `agentmemory-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.2/PKG-INFO` & `agentmemory-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.2
+Version: 0.3.4
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -18,14 +18,16 @@
 
 
 Easy-to-use agent memory, powered by chromadb
 
 
 [![Lint and Test](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/agentmemory.svg)](https://badge.fury.io/py/agentmemory)
+[![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/AutonomousResearchGroup/easycompletion/blob/main/LICENSE)
+[![forks - easycompletion](https://img.shields.io/github/forks/AutonomousResearchGroup/easycompletion?style=social)](https://github.com/AutonomousResearchGroup/easycompletion)
 
 # Installation
 
 ```bash
 pip install agentmemory
 ```
 
@@ -662,10 +664,66 @@
 
 ```python
 events = get_events(1)
 for event in events:
     print(event["document"])
 ```
 
+# Clustering
+
+## Overview
+
+The `cluster` function in `agentmemory.clustering` provides an implementation of DBScan (Density-Based Spatial Clustering of Applications with Noise) clustering. It is designed to group memories in the agent's memory based on their similarity and proximity in the data space.
+
+## Function Signature
+
+```python
+def cluster(epsilon, min_samples, category, filter_metadata=None, unique=False)
+```
+
+## Parameters
+
+- `epsilon` (float): The maximum distance between two samples for one to be considered as in the neighborhood of the other.
+- `min_samples` (int): The number of samples (or total weight) in a neighborhood for a point to be considered as a core point.
+- `category` (str): The category of the collection to be clustered.
+- `filter_metadata` (dict, optional): Additional metadata for filtering the memories before clustering. Defaults to None.
+- `unique` (bool, optional): Whether to return only unique memories. Defaults to False.
+
+## Memory Clustering
+
+The `cluster` function updates memories directly with their cluster ID by performing the DBScan clustering algorithm. Memories with similar content and metadata will be grouped together into clusters. The clustering result will be reflected in the metadata of the memories.
+
+## Memory Marking
+
+- Memories with less than `min_samples` neighbors within a distance of `epsilon` will be marked as noise, and their cluster ID in the metadata will be set to "noise."
+- Memories belonging to a cluster will have their cluster ID stored in the "cluster" field of the metadata.
+
+## Usage
+
+To perform clustering on a specific category of memories, call the `cluster` function with appropriate parameters:
+
+```python
+from agentmemory.clustering import cluster
+
+# Example usage
+epsilon = 0.1
+min_samples = 3
+category = "conversation"
+filter_metadata = {"speaker": "HAL"}  # Optional metadata filter
+unique = False  # Whether to return only unique memories
+
+cluster(epsilon, min_samples, category, filter_metadata=filter_metadata, unique=unique)
+```
+
+## Note
+
+- The clustering operation will directly update the memories' metadata in the specified category. Please make sure to have a backup of the data before performing clustering if necessary.
+
+## References
+
+For more information about DBScan clustering, refer to the original paper:
+[DBScan Paper](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)
+
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
+
```

### Comparing `agentmemory-0.3.2/README.md` & `agentmemory-0.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# agentmemory <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a>
+# agentmemory <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a> <a href="https://github.com/AutonomousResearchGroup/agentmemory/stargazers"><img style="float: right; padding: 5px;" src="https://img.shields.io/github/stars/AutonomousResearchGroup/agentmemory?style=social" alt=""></a>
 
 Easy-to-use agent memory, powered by chromadb
 
 <img src="resources/image.jpg">
 
 [![Lint and Test](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/agentmemory.svg)](https://badge.fury.io/py/agentmemory)
+[![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/AutonomousResearchGroup/easycompletion/blob/main/LICENSE)
+[![forks - easycompletion](https://img.shields.io/github/forks/AutonomousResearchGroup/easycompletion?style=social)](https://github.com/AutonomousResearchGroup/easycompletion)
 
 # Installation
 
 ```bash
 pip install agentmemory
 ```
 
@@ -646,12 +648,67 @@
 
 ```python
 events = get_events(1)
 for event in events:
     print(event["document"])
 ```
 
+# Clustering
+
+## Overview
+
+The `cluster` function in `agentmemory.clustering` provides an implementation of DBScan (Density-Based Spatial Clustering of Applications with Noise) clustering. It is designed to group memories in the agent's memory based on their similarity and proximity in the data space.
+
+## Function Signature
+
+```python
+def cluster(epsilon, min_samples, category, filter_metadata=None, unique=False)
+```
+
+## Parameters
+
+- `epsilon` (float): The maximum distance between two samples for one to be considered as in the neighborhood of the other.
+- `min_samples` (int): The number of samples (or total weight) in a neighborhood for a point to be considered as a core point.
+- `category` (str): The category of the collection to be clustered.
+- `filter_metadata` (dict, optional): Additional metadata for filtering the memories before clustering. Defaults to None.
+- `unique` (bool, optional): Whether to return only unique memories. Defaults to False.
+
+## Memory Clustering
+
+The `cluster` function updates memories directly with their cluster ID by performing the DBScan clustering algorithm. Memories with similar content and metadata will be grouped together into clusters. The clustering result will be reflected in the metadata of the memories.
+
+## Memory Marking
+
+- Memories with less than `min_samples` neighbors within a distance of `epsilon` will be marked as noise, and their cluster ID in the metadata will be set to "noise."
+- Memories belonging to a cluster will have their cluster ID stored in the "cluster" field of the metadata.
+
+## Usage
+
+To perform clustering on a specific category of memories, call the `cluster` function with appropriate parameters:
+
+```python
+from agentmemory.clustering import cluster
+
+# Example usage
+epsilon = 0.1
+min_samples = 3
+category = "conversation"
+filter_metadata = {"speaker": "HAL"}  # Optional metadata filter
+unique = False  # Whether to return only unique memories
+
+cluster(epsilon, min_samples, category, filter_metadata=filter_metadata, unique=unique)
+```
+
+## Note
+
+- The clustering operation will directly update the memories' metadata in the specified category. Please make sure to have a backup of the data before performing clustering if necessary.
+
+## References
+
+For more information about DBScan clustering, refer to the original paper:
+[DBScan Paper](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)
+
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
-<img src="resources/youcreatethefuture.jpg">
+<img src="resources/youcreatethefuture.jpg">
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
-# agentmemory  Easy-to-use agent memory, powered by chromadb [resources/
+# agentmemory   Easy-to-use agent memory, powered by chromadb [resources/
 image.jpg] [![Lint and Test](https://github.com/AutonomousResearchGroup/
 agentmemory/actions/workflows/test.yml/badge.svg)](https://github.com/
 AutonomousResearchGroup/agentmemory/actions/workflows/test.yml) [![PyPI
 version](https://badge.fury.io/py/agentmemory.svg)](https://badge.fury.io/py/
-agentmemory) # Installation ```bash pip install agentmemory ``` # Quickstart
+agentmemory) [![License](https://img.shields.io/badge/License-MIT-blue)](https:
+//github.com/AutonomousResearchGroup/easycompletion/blob/main/LICENSE) [![forks
+- easycompletion](https://img.shields.io/github/forks/AutonomousResearchGroup/
+easycompletion?style=social)](https://github.com/AutonomousResearchGroup/
+easycompletion) # Installation ```bash pip install agentmemory ``` # Quickstart
 ```python from agentmemory import create_memory, search_memory # create a
 memory create_memory("conversation", "I can't do that, Dave.", metadata=
 {"speaker": "HAL", "some_other_key": "some value, could be a number or
 string"}) # search for a memory memories = search_memory("conversation",
 "Dave") # category, search term print(str(memories)) # memories is a list of
 dictionaries [ { "id": int, "document": string, "metadata": dict{...values},
 "embeddings": (Optional) list[float] | None }, { ... } ] ``` # Debugging You
@@ -177,12 +181,43 @@
 `embedding` (object, optional): An optional embedding for the event. **Usage:**
 ```python create_event(text, metadata={}, embedding=None) ``` **Example:**
 ```python create_event("This is a test event", metadata={"test": "test"}) ``` -
 -- ## `get_events(epoch=None, filter_metadata=None, n_results=10)` The
 `get_events` function retrieves events from the agent's memory. **Arguments:**
 - `epoch` (int, optional): If specified, only retrieve events from this epoch.
 **Usage:** ```python get_events(epoch=None) ``` **Example:** ```python events =
-get_events(1) for event in events: print(event["document"]) ``` # Contributions
-Welcome If you like this library and want to contribute in any way, please feel
-free to submit a PR and I will review it. Please note that the goal here is
-simplicity and accesibility, using common language and few dependencies.
-[resources/youcreatethefuture.jpg]
+get_events(1) for event in events: print(event["document"]) ``` # Clustering ##
+Overview The `cluster` function in `agentmemory.clustering` provides an
+implementation of DBScan (Density-Based Spatial Clustering of Applications with
+Noise) clustering. It is designed to group memories in the agent's memory based
+on their similarity and proximity in the data space. ## Function Signature
+```python def cluster(epsilon, min_samples, category, filter_metadata=None,
+unique=False) ``` ## Parameters - `epsilon` (float): The maximum distance
+between two samples for one to be considered as in the neighborhood of the
+other. - `min_samples` (int): The number of samples (or total weight) in a
+neighborhood for a point to be considered as a core point. - `category` (str):
+The category of the collection to be clustered. - `filter_metadata` (dict,
+optional): Additional metadata for filtering the memories before clustering.
+Defaults to None. - `unique` (bool, optional): Whether to return only unique
+memories. Defaults to False. ## Memory Clustering The `cluster` function
+updates memories directly with their cluster ID by performing the DBScan
+clustering algorithm. Memories with similar content and metadata will be
+grouped together into clusters. The clustering result will be reflected in the
+metadata of the memories. ## Memory Marking - Memories with less than
+`min_samples` neighbors within a distance of `epsilon` will be marked as noise,
+and their cluster ID in the metadata will be set to "noise." - Memories
+belonging to a cluster will have their cluster ID stored in the "cluster" field
+of the metadata. ## Usage To perform clustering on a specific category of
+memories, call the `cluster` function with appropriate parameters: ```python
+from agentmemory.clustering import cluster # Example usage epsilon = 0.1
+min_samples = 3 category = "conversation" filter_metadata = {"speaker": "HAL"}
+# Optional metadata filter unique = False # Whether to return only unique
+memories cluster(epsilon, min_samples, category,
+filter_metadata=filter_metadata, unique=unique) ``` ## Note - The clustering
+operation will directly update the memories' metadata in the specified
+category. Please make sure to have a backup of the data before performing
+clustering if necessary. ## References For more information about DBScan
+clustering, refer to the original paper: [DBScan Paper](https://www.aaai.org/
+Papers/KDD/1996/KDD96-037.pdf) # Contributions Welcome If you like this library
+and want to contribute in any way, please feel free to submit a PR and I will
+review it. Please note that the goal here is simplicity and accesibility, using
+common language and few dependencies. [resources/youcreatethefuture.jpg]
```

### Comparing `agentmemory-0.3.2/agentmemory/__init__.py` & `agentmemory-0.3.4/agentmemory/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 )
 
 from .client import (
     get_chroma_client,
     set_chroma_client,
 )
 
+from .clustering import (
+    cluster,
+)
+
 __all__ = [
     "create_memory",
     "create_unique_memory",
     "get_memories",
     "search_memory",
     "get_memory",
     "update_memory",
@@ -63,8 +67,9 @@
     "get_persistent_directory",
     "create_event",
     "get_epoch",
     "get_events",
     "increment_epoch",
     "reset_epoch",
     "set_epoch",
+    "cluster",
 ]
```

### Comparing `agentmemory-0.3.2/agentmemory/client.py` & `agentmemory-0.3.4/agentmemory/client.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.2/agentmemory/events.py` & `agentmemory-0.3.4/agentmemory/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     """
     Retrieves the current epoch value from the agent's memory.
 
     Returns:
         int: The current epoch value.
     """
     memories = get_memories("epoch")
+    if len(memories) == 0:
+        create_memory("epoch", str(1))
+        return 1
     memory = memories[0]
     return int(memory["document"])
 
 
 def create_event(text, metadata={}, embedding=None):
     """
     Creates a new event in the agent's memory.
```

### Comparing `agentmemory-0.3.2/agentmemory/helpers.py` & `agentmemory-0.3.4/agentmemory/helpers.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.2/agentmemory/main.py` & `agentmemory-0.3.4/agentmemory/main.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.2/agentmemory/persistence.py` & `agentmemory-0.3.4/agentmemory/persistence.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.2/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.3.4/agentmemory.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.2
+Version: 0.3.4
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -18,14 +18,16 @@
 
 
 Easy-to-use agent memory, powered by chromadb
 
 
 [![Lint and Test](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentmemory/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/agentmemory.svg)](https://badge.fury.io/py/agentmemory)
+[![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/AutonomousResearchGroup/easycompletion/blob/main/LICENSE)
+[![forks - easycompletion](https://img.shields.io/github/forks/AutonomousResearchGroup/easycompletion?style=social)](https://github.com/AutonomousResearchGroup/easycompletion)
 
 # Installation
 
 ```bash
 pip install agentmemory
 ```
 
@@ -662,10 +664,66 @@
 
 ```python
 events = get_events(1)
 for event in events:
     print(event["document"])
 ```
 
+# Clustering
+
+## Overview
+
+The `cluster` function in `agentmemory.clustering` provides an implementation of DBScan (Density-Based Spatial Clustering of Applications with Noise) clustering. It is designed to group memories in the agent's memory based on their similarity and proximity in the data space.
+
+## Function Signature
+
+```python
+def cluster(epsilon, min_samples, category, filter_metadata=None, unique=False)
+```
+
+## Parameters
+
+- `epsilon` (float): The maximum distance between two samples for one to be considered as in the neighborhood of the other.
+- `min_samples` (int): The number of samples (or total weight) in a neighborhood for a point to be considered as a core point.
+- `category` (str): The category of the collection to be clustered.
+- `filter_metadata` (dict, optional): Additional metadata for filtering the memories before clustering. Defaults to None.
+- `unique` (bool, optional): Whether to return only unique memories. Defaults to False.
+
+## Memory Clustering
+
+The `cluster` function updates memories directly with their cluster ID by performing the DBScan clustering algorithm. Memories with similar content and metadata will be grouped together into clusters. The clustering result will be reflected in the metadata of the memories.
+
+## Memory Marking
+
+- Memories with less than `min_samples` neighbors within a distance of `epsilon` will be marked as noise, and their cluster ID in the metadata will be set to "noise."
+- Memories belonging to a cluster will have their cluster ID stored in the "cluster" field of the metadata.
+
+## Usage
+
+To perform clustering on a specific category of memories, call the `cluster` function with appropriate parameters:
+
+```python
+from agentmemory.clustering import cluster
+
+# Example usage
+epsilon = 0.1
+min_samples = 3
+category = "conversation"
+filter_metadata = {"speaker": "HAL"}  # Optional metadata filter
+unique = False  # Whether to return only unique memories
+
+cluster(epsilon, min_samples, category, filter_metadata=filter_metadata, unique=unique)
+```
+
+## Note
+
+- The clustering operation will directly update the memories' metadata in the specified category. Please make sure to have a backup of the data before performing clustering if necessary.
+
+## References
+
+For more information about DBScan clustering, refer to the original paper:
+[DBScan Paper](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)
+
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
+
```

### Comparing `agentmemory-0.3.2/setup.py` & `agentmemory-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.3.2',
+    version='0.3.4',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

