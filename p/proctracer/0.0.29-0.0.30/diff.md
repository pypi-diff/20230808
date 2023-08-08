# Comparing `tmp/proctracer-0.0.29.tar.gz` & `tmp/proctracer-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.29.tar", last modified: Mon Aug  7 17:42:06 2023, max compression
+gzip compressed data, was "proctracer-0.0.30.tar", last modified: Tue Aug  8 08:47:04 2023, max compression
```

## Comparing `proctracer-0.0.29.tar` & `proctracer-0.0.30.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.713570 proctracer-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-07 17:41:54.000000 proctracer-0.0.29/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 17:41:54.000000 proctracer-0.0.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 17:42:06.713570 proctracer-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-07 17:41:54.000000 proctracer-0.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.705570 proctracer-0.0.29/proctracer/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.713570 proctracer-0.0.29/proctracer/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_softnet_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5394 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/proctracer.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.709570 proctracer-0.0.29/proctracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 17:42:06.713570 proctracer-0.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-08-07 17:41:54.000000 proctracer-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:47:04.971057 proctracer-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 08:46:52.000000 proctracer-0.0.30/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 08:46:52.000000 proctracer-0.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-08 08:47:04.971057 proctracer-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-08 08:46:52.000000 proctracer-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:47:04.967057 proctracer-0.0.30/proctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:47:04.971057 proctracer-0.0.30/proctracer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/net_softnet_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5394 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/proctracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 08:46:52.000000 proctracer-0.0.30/proctracer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:47:04.967057 proctracer-0.0.30/proctracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 08:47:04.000000 proctracer-0.0.30/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 08:47:04.971057 proctracer-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-08-08 08:46:52.000000 proctracer-0.0.30/setup.py
```

### Comparing `proctracer-0.0.29/LICENSE.md` & `proctracer-0.0.30/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/PKG-INFO` & `proctracer-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.29
+Version: 0.0.30
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.29/README.md` & `proctracer-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/__init__.py` & `proctracer-0.0.30/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.30/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.30/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/net_softnet_stat.plugin.py` & `proctracer-0.0.30/proctracer/plugins/net_softnet_stat.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,31 @@
             values = 'processed dropped time_squeeze received_rps flow_limit_count softnet_backlog_len'.split()
             for value in values:
            
                 maxV=0
                 pivot_table = self.data_frame.pivot_table(index='time', columns=['index'], values=value)
                 if i == 0:
                     pivot_table -= pivot_table.iloc[0].values.squeeze() # relative count wrt. start time
-                                    
+                
+                pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
+                
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for j in pivot_table.columns:
                     axs[i].plot( pivot_table[[j]].dropna(), label="cpu%s" % j )
                 
                 axs[i].set_ylabel('%s' % value, fontsize='x-small', rotation=0)
                 axs[i].grid()
                 
                 if (i+1)<len(values):
                     axs[i].set_xticklabels([])
                 else:
-                    axs[i].legend(ncol=int(sqrt(len(pivot_table.columns))) , fontsize='xx-small', loc= 'upper right')
                     axs[i].set_xlabel("Time t [s]")
-                
+                    
+                axs[i].legend(ncol=int(sqrt(len(pivot_table.columns))) , fontsize='xx-small', loc= 'upper right')
+                axs[i].set_yscale('log')
                 axs[i].set_xlim(0,maxT)
-                axs[i].set_ylim(0,maxV*1.05+0.01)
+                axs[i].set_ylim(None,maxV*1.05+0.01)
                 
                 i+=1
 
         pdf.savefig(fig)
```

### Comparing `proctracer-0.0.29/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.30/proctracer/plugins/net_udpX.plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,16 @@
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[0].plot( pivot_table[[i]].dropna(), label="%s , %s" % (i, value ) )
                 
-            if not pivot_table.columns.empty:
-                axs[0].legend(fontsize='xx-small', loc= 'upper right')
-                 
+            
+            axs[0].legend(fontsize='xx-small', loc= 'upper right')   
             axs[0].set_ylabel('Size of tx/rx Queues')
             axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,maxV*1.05+0.01)
 
             ######### Drops
@@ -107,17 +106,16 @@
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[1].plot( pivot_table[[i]].dropna(), label=i )
             
-            if not pivot_table.columns.empty:
-                axs[1].legend(fontsize='xx-small', loc= 'upper right')
             
+            axs[1].legend(fontsize='xx-small', loc= 'upper right')
             axs[1].set_ylabel('Packet Drops [count]')
             axs[1].set_xticklabels([])
             axs[1].grid()
             axs[1].set_xlim(0,maxT)
             axs[1].set_ylim(0,maxV*1.05+0.01)
             
             ######### Drop-Rate
@@ -126,17 +124,15 @@
                 pivot_table = self.data_frame.pivot_table(index='time', columns=['socket'], values=value)
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[2].plot( pivot_table[[i]].dropna(), label=i )
 
-            if not pivot_table.columns.empty:
-                axs[2].legend(fontsize='xx-small', loc= 'upper right')
-
+            axs[2].legend(fontsize='xx-small', loc= 'upper right')
             axs[2].set_xlabel('Time t [s]')
             axs[2].set_ylabel('Packet Drop Rate [1/s]')
             axs[2].grid()
             axs[2].set_xlim(0,maxT)
             axs[2].set_ylim(0,maxV*1.05+0.01)
 
         pdf.savefig(fig)
```

### Comparing `proctracer-0.0.29/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.30/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/plugin_base.py` & `proctracer-0.0.30/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.30/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.30/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.30/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.30/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer/proctracer.py` & `proctracer-0.0.30/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.30/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.29
+Version: 0.0.30
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.29/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.30/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.29/setup.py` & `proctracer-0.0.30/setup.py`

 * *Files identical despite different names*

