# Comparing `tmp/dyn_rm-1.0.2.tar.gz` & `tmp/dyn_rm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn_rm-1.0.2.tar", last modified: Tue Aug  8 11:00:31 2023, max compression
+gzip compressed data, was "dyn_rm-1.0.3.tar", last modified: Tue Aug  8 11:38:43 2023, max compression
```

## Comparing `dyn_rm-1.0.2.tar` & `dyn_rm-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.229701 dyn_rm-1.0.2/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     3391 2023-06-22 07:27:11.000000 dyn_rm-1.0.2/README.md
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/dyn_rm/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.2/dyn_rm/__init__.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22535 2023-08-08 07:57:51.000000 dyn_rm-1.0.2/dyn_rm/dynamic_resource_manager.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36868 2023-07-25 13:30:50.000000 dyn_rm-1.0.2/dyn_rm/hpc_system.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.2/dyn_rm/my_pmix.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.2/dyn_rm/my_pmix_constants.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.2/dyn_rm/plotter.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.2/dyn_rm/setup.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.2/dyn_rm/util.py
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/dyn_rm.egg-info/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/SOURCES.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/dependency_links.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/entry_points.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/requires.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/top_level.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-08-08 11:00:31.229701 dyn_rm-1.0.2/setup.cfg
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      551 2023-08-08 10:53:07.000000 dyn_rm-1.0.2/setup.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:38:43.733953 dyn_rm-1.0.3/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:38:43.733953 dyn_rm-1.0.3/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     3391 2023-06-22 07:27:11.000000 dyn_rm-1.0.3/README.md
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:38:43.733953 dyn_rm-1.0.3/dyn_rm/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.3/dyn_rm/__init__.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22536 2023-08-08 11:32:45.000000 dyn_rm-1.0.3/dyn_rm/dynamic_resource_manager.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36868 2023-07-25 13:30:50.000000 dyn_rm-1.0.3/dyn_rm/hpc_system.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.3/dyn_rm/my_pmix.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.3/dyn_rm/my_pmix_constants.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.3/dyn_rm/plotter.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.3/dyn_rm/setup.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.3/dyn_rm/util.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:38:43.733953 dyn_rm-1.0.3/dyn_rm.egg-info/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/entry_points.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/requires.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:38:43.000000 dyn_rm-1.0.3/dyn_rm.egg-info/top_level.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-08-08 11:38:43.733953 dyn_rm-1.0.3/setup.cfg
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      551 2023-08-08 11:38:36.000000 dyn_rm-1.0.3/setup.py
```

### Comparing `dyn_rm-1.0.2/README.md` & `dyn_rm-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.2/dyn_rm/dynamic_resource_manager.py` & `dyn_rm-1.0.3/dyn_rm/dynamic_resource_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         pid = -1
         if name == "PRRTE":
             v_print("Starting PRRTE", 1, self.verbosity_level)
             filename = None
             if None != self.tmpdir:
                 filename = os.path.join(self.tmpdir, "pid")
             else:
-                filename = os.pah.join(os.getcwd(), "pid")
+                filename = os.path.join(os.getcwd(), "pid")
             # Start PRRTE
             os.system("prterun --report-pid "+filename+" --max-vm-size 4 --daemonize --mca ras timex --host "+hosts)
 
             start = time.time()
             # get the pid of the PRRTE Master
             while pid < 0:
                 if time.time() - start > timeout:
```

### Comparing `dyn_rm-1.0.2/dyn_rm/hpc_system.py` & `dyn_rm-1.0.3/dyn_rm/hpc_system.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.2/dyn_rm/my_pmix.py` & `dyn_rm-1.0.3/dyn_rm/my_pmix.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.2/dyn_rm/my_pmix_constants.py` & `dyn_rm-1.0.3/dyn_rm/my_pmix_constants.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.2/dyn_rm/plotter.py` & `dyn_rm-1.0.3/dyn_rm/plotter.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.2/setup.py` & `dyn_rm-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='dyn_rm',
-    version='1.0.2',
+    version='1.0.3',
     description='A Dynamic Resource Manager for Dyn_PRRTE, Dyn_PMIx and Dyn_OMPI',
     author='Dominik Huber',
     author_email='domi.huber@tum.de',
     url='https://gitlab.inria.fr/dynres/dyn-procs/dyn_rm',
     packages=find_packages(),
     install_requires=[
         # List any dependencies your package requires
```

