# Comparing `tmp/dyn_rm-1.0.1.tar.gz` & `tmp/dyn_rm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn_rm-1.0.1.tar", last modified: Fri Jun 23 10:32:25 2023, max compression
+gzip compressed data, was "dyn_rm-1.0.2.tar", last modified: Tue Aug  8 11:00:31 2023, max compression
```

## Comparing `dyn_rm-1.0.1.tar` & `dyn_rm-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.688238 dyn_rm-1.0.1/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     3391 2023-06-22 07:27:11.000000 dyn_rm-1.0.1/README.md
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/dyn_rm/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.1/dyn_rm/__init__.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22366 2023-06-22 07:23:15.000000 dyn_rm-1.0.1/dyn_rm/dynamic_resource_manager.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36301 2023-06-21 14:24:56.000000 dyn_rm-1.0.1/dyn_rm/hpc_system.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.1/dyn_rm/my_pmix.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.1/dyn_rm/my_pmix_constants.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.1/dyn_rm/plotter.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.1/dyn_rm/setup.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.1/dyn_rm/util.py
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/dyn_rm.egg-info/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/SOURCES.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/dependency_links.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/entry_points.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/requires.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/top_level.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-06-23 10:32:25.688238 dyn_rm-1.0.1/setup.cfg
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      551 2023-06-23 10:31:52.000000 dyn_rm-1.0.1/setup.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.229701 dyn_rm-1.0.2/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     3391 2023-06-22 07:27:11.000000 dyn_rm-1.0.2/README.md
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/dyn_rm/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.2/dyn_rm/__init__.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22535 2023-08-08 07:57:51.000000 dyn_rm-1.0.2/dyn_rm/dynamic_resource_manager.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36868 2023-07-25 13:30:50.000000 dyn_rm-1.0.2/dyn_rm/hpc_system.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.2/dyn_rm/my_pmix.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.2/dyn_rm/my_pmix_constants.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.2/dyn_rm/plotter.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.2/dyn_rm/setup.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.2/dyn_rm/util.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-08-08 11:00:31.225701 dyn_rm-1.0.2/dyn_rm.egg-info/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/entry_points.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/requires.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-08-08 11:00:31.000000 dyn_rm-1.0.2/dyn_rm.egg-info/top_level.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-08-08 11:00:31.229701 dyn_rm-1.0.2/setup.cfg
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      551 2023-08-08 10:53:07.000000 dyn_rm-1.0.2/setup.py
```

### Comparing `dyn_rm-1.0.1/README.md` & `dyn_rm-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.1/dyn_rm/dynamic_resource_manager.py` & `dyn_rm-1.0.2/dyn_rm/dynamic_resource_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,30 @@
     process_managers=dict()
     job_mix = []
     verbosity_level = 0
     event_loop = asyncio.new_event_loop()
     my_pmix = My_PMIx()
     registered_event_handlers = dict()
     _lock = Lock()
-    start_time = time.time() 
+    start_time = time.time()
+    tmpdir = None
 
     def __new__(cls, *args, **kwargs):
         with cls._lock:
             if not cls._instance:
                 cls._instance = super().__new__(cls)
         return cls._instance
 
-    def __init__(self, verbosity_level = None, outputfile = None):
+    def __init__(self, verbosity_level = None, outputfile = None, tmpdir=None):
         if verbosity_level != None:
             self.verbosity_level = verbosity_level
         if None != outputfile:
             self.output = outputfile
+        if None != tmpdir:
+            self.tmpdir=tmpdir
     
     def add_job_mix(self, job_file):
 
         # Using readlines()
         file1 = open(job_file, 'r')
         lines = file1.readlines()
 
@@ -49,34 +52,36 @@
             self.job_mix.append(json.loads(line))
         
     # Start the process manager
     def start_process_manager(self, name, hosts, timeout=1):
         
         pid = -1
         if name == "PRRTE":
+            v_print("Starting PRRTE", 1, self.verbosity_level)
+            filename = None
+            if None != self.tmpdir:
+                filename = os.path.join(self.tmpdir, "pid")
+            else:
+                filename = os.pah.join(os.getcwd(), "pid")
             # Start PRRTE
-            temp_dir = tempfile.gettempdir()
-            #os.system("prterun --report-pid "+os.path.dirname(os.path.abspath(__file__))+"/pid --mca ras timex --host "+hosts+" ./../test_applications/build/dummy_job_release 0 &")
-            os.system("prterun --report-pid "+os.path.join(temp_dir, "pid")+" --max-vm-size 4 --daemonize --mca ras timex --host "+hosts)
+            os.system("prterun --report-pid "+filename+" --max-vm-size 4 --daemonize --mca ras timex --host "+hosts)
 
-            # Let the application shrink before we connect
-            #sleep(1)
-
-            i = 0
+            start = time.time()
             # get the pid of the PRRTE Master
             while pid < 0:
-                if i * 0.1 > timeout:
+                if time.time() - start > timeout:
                     raise Exception("PRRTE startup timed out!") 
                 
                 try:
-                    pid = int(open(os.path.join(temp_dir, "pid"), 'r').readlines()[0])
+                    pid = int(open(filename, 'r').readlines()[0])
                 except FileNotFoundError:
                     sleep(0.1)
             try: 
-                os.system("rm "+os.path.join(temp_dir, "pid"))
+                if os.path.exists(filename):
+                    os.remove(filename)
             except Exception:
                 pass
 
         else:
             raise Exception("Process Manager not supported!")
         
         self.process_managers[name] = pid
@@ -440,14 +445,15 @@
             app['env'] = env
             
             app['argv'] = args
             app['info'] = job_infos
 
             # PMIx_Spawn
             rc, jobid = self.my_pmix.my_tool.spawn(job_infos, [app])
+
             if rc == PMIX_SUCCESS:
                 job = Job(jobid)
                 self.my_system.add_jobs([job])
 
                 nodes = self.my_pmix.get_node_map(jobid)
                 ppn = self.my_pmix.get_proc_map(jobid)
 
@@ -487,14 +493,15 @@
     parser.add_argument('--server_pid', type=int, required=False)
     parser.add_argument('--verbosity_level', type=int, required=False)
     parser.add_argument('--sched_interval', type=float, required=False)
     parser.add_argument('--hosts', type=str, required=True)
     parser.add_argument('--jobs', type=str, required=True)
     parser.add_argument('--output', type=str, required=False)
     parser.add_argument('--policy', type=str, required=False, choices=['default', 'dmr'])
+    parser.add_argument('--tmpdir', type=str, required=False)
 
     args = parser.parse_args()
 
     pid = -1
     if args.server_pid is not None:
         pid = args.server_pid
 
@@ -511,23 +518,25 @@
 
     policy = 'default'
     if args.policy is not None:
         policy = args.policy
     
     output = args.output
 
-    return pid, verbosity_level, sched_interval, hosts, jobs, output, policy
+    tmpdir = args.tmpdir
+
+    return pid, verbosity_level, sched_interval, hosts, jobs, output, policy, tmpdir
 
 
 def main():
 
-    pid, verbosity_level, interval, hosts, jobs, output, policy = get_parameters()
+    pid, verbosity_level, interval, hosts, jobs, output, policy, tmpdir = get_parameters()
 
     # Create our resource Manager instance
-    resource_manager = ResourceManager(verbosity_level=verbosity_level, outputfile=output)
+    resource_manager = ResourceManager(verbosity_level=verbosity_level, outputfile=output, tmpdir=tmpdir)
 
     # If no server pid was specified, we start the Process Manager by ourself
     if pid < 0:
         pid = resource_manager.start_process_manager("PRRTE", hosts)
         
     
     # Initialize our connection to the Process Manager's PMIx server
```

### Comparing `dyn_rm-1.0.1/dyn_rm/hpc_system.py` & `dyn_rm-1.0.2/dyn_rm/hpc_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,15 +542,15 @@
         for info in self.info:
             if info['key'] == "mpi_num_procs_pref":
                 return int(info['value'])
         return -1
 
 
     def toString(self):
-        return "Setop: op = "+str(self.op)+", job = "+str(self.jobid)+", input = "+str(self.input)+", output = "+str(self.output)+", info = "+str(self.info)
+        return "Setop: op = "+str(self.op)+", job = "+str(self.jobid)+", input = "+str(self.input)+", output = "+str(self.output)+", info = "+str(self.info)+", nodelist = "+str(self.nodelist)+", additional_info = "+str(self.additional_info)
 
     
 
 class SchedulingPolicy:
 
     def __init__(self, name, verbosity_level = 0):
         self.name = name
@@ -652,15 +652,14 @@
 class DMR_Scheduler(SchedulingPolicy):
 
     def scheduling_function(self, my_system: System, params: list) ->dict:
         super().scheduling_function(my_system, params)
 
         jobs_to_start = []
         setops_to_execute = []
-
         #blocked_nodes = []
 
         cur_free_slots = my_system.get_num_free_slots()
         cur_free_nodes = my_system.get_free_nodes()
         if len(my_system.queue) > 0:
             v_print("1. Checking if jobs from queue can be scheduled", 2, self.verbosity_level)
             for waiting_job in my_system.queue:
@@ -738,25 +737,30 @@
                                         
                                         v_print("         Free slots = "+str(cur_free_slots)+" requested procs = "+str(num_procs)+" ==> GRANTED", 4, self.verbosity_level)
                                         setop.set_processed()
                                         setop.additional_info.append({'key' : "mpi_num_procs_add", 'flags': 0, 'value' : str(0), 'val_type' : PMIX_STRING})
                                         setop.additional_info.append({'key' : "mpi_num_procs_sub", 'flags': 0, 'value' : str(num_procs), 'val_type' : PMIX_STRING})
                                         setops_to_execute.append(setop)
                                         setop.nodelist = [node for node in my_system.jobs[setop.jobid].node_names]
-                                        num_to_add = num_procs
-                                        for node in cur_free_nodes:
-                                            if num_to_add > 0:
-                                                setop.nodelist.append(node)
-                                                num_to_add -= my_system.node_pool[node].num_slots
-                                            else:
-                                                break
-                                            
-                                        my_system.apply_placeholder_setop(setop)
-                                        cur_free_slots -= num_procs
+                                        #num_to_add = num_procs
+                                        #occupied_nodes = []
+                                        #for node in cur_free_nodes:
+                                        #    if num_to_add > 0:
+                                        #        setop.nodelist.append(node)
+                                        #        occupied_nodes.append(node)
+                                        #        num_to_add -= my_system.node_pool[node].num_slots
+                                        #    else:
+                                        #        break
+#
+                                        #for node in occupied_nodes:
+                                        #    cur_free_nodes.remove(node)    
+                                        #my_system.apply_placeholder_setop(setop)
+                                        #cur_free_slots -= num_procs
                                         #else:
+
                                     #always execute setops which do not require resource changes
                                 #    setops_to_execute.append(setop)
                                 elif setop.op == PMIX_PSETOP_NULL:
                                     rm_setops.append(setop)
                                     setop.additional_info.append({'key' : "PMIX_PSETOP_CANCELED", 'flags': 0, 'value' : True, 'val_type' : PMIX_BOOL})
                                     setop.set_processed()
                                     setops_to_execute.append(setop)
@@ -783,46 +787,50 @@
                         v_print("     Checking if Setop '"+str(setop.id)+"' in job '"+job.name+"' can be executed", 3, self.verbosity_level)
 
                         if setop.op == PMIX_PSETOP_REPLACE:
                             v_print("         Setop '"+str(setop.id)+"' in job '"+job.name+"' is an addition. Checking slots", 3, self.verbosity_level)
                             max_procs = setop.get_proc_max()
                             cur_procs = my_system.psets[setop.input[0]].size
 
-                            
                             gathered_slots = 0
                             aux_cur = cur_procs
-                            while aux_cur < cur_free_slots:
+                            while aux_cur <= cur_free_slots:
                                 aux_cur  = aux_cur * 2
                                 if aux_cur > max_procs:
                                     aux_cur /= 2
                                     break
-                                
                             if aux_cur == cur_procs: # then check next
                                 continue
 
                             max_procs = aux_cur
 
+
                             num_procs = max_procs - cur_procs
+                            
                             if num_procs > 0:
                                 if cur_free_slots - num_procs >= 0:
                                     v_print("         Free slots = "+str(cur_free_slots)+" requested procs = "+str(num_procs)+" ==> GRANTED", 4, self.verbosity_level)
                                     setop.set_processed()
                                     setop.additional_info.append({'key' : "mpi_num_procs_add", 'flags': 0, 'value' : str(num_procs), 'val_type' : PMIX_STRING})
                                     setop.additional_info.append({'key' : "mpi_num_procs_sub", 'flags': 0, 'value' : str(0), 'val_type' : PMIX_STRING})
                                     setops_to_execute.append(setop)
                                     setop.nodelist = [node for node in my_system.jobs[setop.jobid].node_names]
                                     num_to_add = num_procs
+                                    occupied_nodes = []
                                     for node in cur_free_nodes:
                                         if num_to_add > 0:
                                             setop.nodelist.append(node)
+                                            occupied_nodes.append(node)
                                             num_to_add -= my_system.node_pool[node].num_slots
                                         else:
                                             break
                                     
                                     my_system.apply_placeholder_setop(setop)
+                                    for node in occupied_nodes:
+                                        cur_free_nodes.remove(node)    
                                     cur_free_slots -= num_procs
                                 else:
                                     v_print("         Free slots = "+str(cur_free_slots)+" requested procs = "+str(num_procs)+" ==> DENIED", 4, self.verbosity_level)
                         elif setop.op == PMIX_PSETOP_NULL:
                             rm_setops.append(setop)
                             setop.additional_info.append({'key' : "PMIX_PSETOP_CANCELED", 'flags': 0, 'value' : True, 'val_type' : PMIX_BOOL})
                             setop.set_processed()
```

### Comparing `dyn_rm-1.0.1/dyn_rm/my_pmix.py` & `dyn_rm-1.0.2/dyn_rm/my_pmix.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.1/dyn_rm/my_pmix_constants.py` & `dyn_rm-1.0.2/dyn_rm/my_pmix_constants.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.1/dyn_rm/plotter.py` & `dyn_rm-1.0.2/dyn_rm/plotter.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.1/setup.py` & `dyn_rm-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='dyn_rm',
-    version='1.0.1',
+    version='1.0.2',
     description='A Dynamic Resource Manager for Dyn_PRRTE, Dyn_PMIx and Dyn_OMPI',
     author='Dominik Huber',
     author_email='domi.huber@tum.de',
     url='https://gitlab.inria.fr/dynres/dyn-procs/dyn_rm',
     packages=find_packages(),
     install_requires=[
         # List any dependencies your package requires
```

