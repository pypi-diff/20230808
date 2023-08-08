# Comparing `tmp/taranis_story_clustering-0.1.0.tar.gz` & `tmp/taranis_story_clustering-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taranis_story_clustering-0.1.0.tar", last modified: Tue Aug  8 12:04:47 2023, max compression
+gzip compressed data, was "taranis_story_clustering-0.1.1.tar", last modified: Tue Aug  8 14:02:27 2023, max compression
```

## Comparing `taranis_story_clustering-0.1.0.tar` & `taranis_story_clustering-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-08-08 12:04:47.546516 taranis_story_clustering-0.1.0/
--rw-r--r--   0 ben       (1000) ben       (1000)    13827 2023-08-01 10:42:01.000000 taranis_story_clustering-0.1.0/LICENSE.md
--rw-r--r--   0 ben       (1000) ben       (1000)    16939 2023-08-08 12:04:47.546516 taranis_story_clustering-0.1.0/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      137 2023-08-01 06:58:56.000000 taranis_story_clustering-0.1.0/README.md
--rw-r--r--   0 ben       (1000) ben       (1000)     1156 2023-08-08 12:04:15.000000 taranis_story_clustering-0.1.0/pyproject.toml
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-08-08 12:04:47.546516 taranis_story_clustering-0.1.0/setup.cfg
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-08-08 12:04:47.545516 taranis_story_clustering-0.1.0/story_clustering/
--rw-r--r--   0 ben       (1000) ben       (1000)       44 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-08-01 09:16:19.000000 taranis_story_clustering-0.1.0/story_clustering/__main__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     4857 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/clustering.py
--rw-r--r--   0 ben       (1000) ben       (1000)     7375 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/document_representation.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2709 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/event_organizer.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8519 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/eventdetector.py
--rw-r--r--   0 ben       (1000) ben       (1000)    25866 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/keywords_organizer.py
--rw-r--r--   0 ben       (1000) ben       (1000)      283 2023-08-08 06:46:53.000000 taranis_story_clustering-0.1.0/story_clustering/nlp_utils.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14930 2023-08-08 06:49:12.000000 taranis_story_clustering-0.1.0/story_clustering/story_maker.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-08-08 12:04:47.545516 taranis_story_clustering-0.1.0/story_clustering/tests/
--rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-08-01 10:55:51.000000 taranis_story_clustering-0.1.0/story_clustering/tests/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       14 2023-08-01 10:56:00.000000 taranis_story_clustering-0.1.0/story_clustering/tests/conftest.py
--rw-r--r--   0 ben       (1000) ben       (1000)       41 2023-08-01 11:00:41.000000 taranis_story_clustering-0.1.0/story_clustering/tests/test_clustering.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-08-08 12:04:47.546516 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)    16939 2023-08-08 12:04:47.000000 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      690 2023-08-08 12:04:47.000000 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-08-08 12:04:47.000000 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       99 2023-08-08 12:04:47.000000 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       17 2023-08-08 12:04:47.000000 taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/story_clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/document_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/event_organizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/eventdetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25866 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/keywords_organizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/nlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/story_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/story_clustering/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 14:02:15.000000 taranis_story_clustering-0.1.1/story_clustering/tests/test_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:02:27.613736 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-08-08 14:02:27.000000 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-08 14:02:27.000000 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:02:27.000000 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 14:02:27.000000 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 14:02:27.000000 taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/top_level.txt
```

### Comparing `taranis_story_clustering-0.1.0/LICENSE.md` & `taranis_story_clustering-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/PKG-INFO` & `taranis_story_clustering-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taranis_story_clustering
-Version: 0.1.0
+Version: 0.1.1
 Summary: Story Clustering Bot for Taranis-NG
 Maintainer-email: AIT <benjamin.akhras@ait.ac.at>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `taranis_story_clustering-0.1.0/pyproject.toml` & `taranis_story_clustering-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "taranis_story_clustering"
 description = "Story Clustering Bot for Taranis-NG"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = {file = "LICENSE.md"}
 maintainers = [{ name = "AIT", email = "benjamin.akhras@ait.ac.at" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -43,8 +43,8 @@
 line-length = "142"
 target-version = ["py311"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:.*_app_ctx_stack.*:DeprecationWarning",
     "ignore::DeprecationWarning"
-]
+]
```

### Comparing `taranis_story_clustering-0.1.0/story_clustering/clustering.py` & `taranis_story_clustering-0.1.1/story_clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/story_clustering/document_representation.py` & `taranis_story_clustering-0.1.1/story_clustering/document_representation.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/story_clustering/event_organizer.py` & `taranis_story_clustering-0.1.1/story_clustering/event_organizer.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/story_clustering/eventdetector.py` & `taranis_story_clustering-0.1.1/story_clustering/eventdetector.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/story_clustering/keywords_organizer.py` & `taranis_story_clustering-0.1.1/story_clustering/keywords_organizer.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/story_clustering/story_maker.py` & `taranis_story_clustering-0.1.1/story_clustering/story_maker.py`

 * *Files identical despite different names*

### Comparing `taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/PKG-INFO` & `taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taranis-story-clustering
-Version: 0.1.0
+Version: 0.1.1
 Summary: Story Clustering Bot for Taranis-NG
 Maintainer-email: AIT <benjamin.akhras@ait.ac.at>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `taranis_story_clustering-0.1.0/taranis_story_clustering.egg-info/SOURCES.txt` & `taranis_story_clustering-0.1.1/taranis_story_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

