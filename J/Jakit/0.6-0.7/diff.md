# Comparing `tmp/Jakit-0.6.tar.gz` & `tmp/Jakit-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jakit-0.6.tar", last modified: Tue Aug  8 09:11:02 2023, max compression
+gzip compressed data, was "Jakit-0.7.tar", last modified: Tue Aug  8 11:51:34 2023, max compression
```

## Comparing `Jakit-0.6.tar` & `Jakit-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.570613 Jakit-0.6/
-drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.546615 Jakit-0.6/Jakit/
--rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.6/Jakit/__init__.py
--rw-rw-rw-   0        0        0      139 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/app.py
--rw-rw-rw-   0        0        0        0 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/error_handler.py
--rw-rw-rw-   0        0        0     5429 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/jakit_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.567615 Jakit-0.6/Jakit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      420 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.6/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-08 09:11:02.569613 Jakit-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-08-08 09:11:02.570613 Jakit-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1595 2023-08-08 09:10:55.000000 Jakit-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:51:34.708500 Jakit-0.7/
+drwxrwxrwx   0        0        0        0 2023-08-08 11:51:34.693500 Jakit-0.7/Jakit/
+-rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.7/Jakit/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-08-08 09:04:41.000000 Jakit-0.7/Jakit/app.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:04:41.000000 Jakit-0.7/Jakit/error_handler.py
+-rw-rw-rw-   0        0        0     4965 2023-08-08 11:41:35.000000 Jakit-0.7/Jakit/jakit_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:51:34.705512 Jakit-0.7/Jakit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-08 11:51:34.000000 Jakit-0.7/Jakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-08 11:51:34.000000 Jakit-0.7/Jakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 11:51:34.000000 Jakit-0.7/Jakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      420 2023-08-08 11:51:34.000000 Jakit-0.7/Jakit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 11:51:34.000000 Jakit-0.7/Jakit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.7/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-08 11:51:34.707505 Jakit-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 11:51:34.709503 Jakit-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2023-08-08 11:49:11.000000 Jakit-0.7/setup.py
```

### Comparing `Jakit-0.6/Jakit/jakit_jobs.py` & `Jakit-0.7/Jakit/jakit_jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,14 @@
 Tools_coll = 'Tools'
 
 ConnectionStringJakit = pymongo.MongoClient(Jakit_client)
 DatabaseJakit = ConnectionStringJakit[Jakit_conn]
 CollectionReports = DatabaseJakit[Reports_coll]
 CollectionTools = DatabaseJakit[Tools_coll]
 
-hvqk_client =  'mongodb://HVQK_rw:6Ot2kUj8nJr4h1y@p1ir1mon019.ger.corp.intel.com:7181,p2ir1mon019.ger.corp.intel.com:7181,p3ir1mon019.ger.corp.intel.com:7181/HVQK?ssl=true&replicaSet=mongo7181'
-hvqk_conn = 'HVQK'
-hvqk_coll = 'ReportSummaries'
-
-ConnectionStringHVQK = pymongo.MongoClient(hvqk_client)
-DatabaseHVQK = ConnectionStringHVQK[hvqk_conn]
-CollectionReportSummaries = DatabaseHVQK[hvqk_coll]
-
 class JakitJobs:
     """Jobs class"""
 
     def __init__(self):
         '''Initialize jobids'''
 
     def get_jobs(self,jobids):
@@ -124,16 +116,15 @@
                 "PassingItems" : PassingItems,
                 "FailingItems" : FailingItems,
                 "WarningItems" : WarningItems,
                 "DateCreated" :datetime.datetime.now(),
                 "ReportID": reportid
             }
         
-        # push to mongo
-        CollectionReportSummaries.insert_one(results)
+        return results
 
     def get_summary(self, reportid):
         summary = CollectionReportSummaries.find_one({"ReportID": reportid})
         if summary is not None:
             summary.pop('_id', None)  # Remove _id if it exists in the dictionary
         return summary
```

### Comparing `Jakit-0.6/Jakit.egg-info/PKG-INFO` & `Jakit-0.7/Jakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.6
+Version: 0.7
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.6/LICENSE` & `Jakit-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Jakit-0.6/PKG-INFO` & `Jakit-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.6
+Version: 0.7
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.6/setup.py` & `Jakit-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Jakit",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     author="Idriss Animashaun",
     author_email="idriss.animashaun@intel.com",
     description="Just Another Kappa Information Tool",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/iddy-ani/Jakit",
```

