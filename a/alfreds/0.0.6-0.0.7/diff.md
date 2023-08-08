# Comparing `tmp/alfreds-0.0.6-py3-none-any.whl.zip` & `tmp/alfreds-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 8369 bytes, number of entries: 19
--rwxr-xr-x  2.0 unx     2616 b- defN 23-Aug-06 08:15 alfreds-0.0.6.data/scripts/alfreds
--rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.6.data/scripts/main.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_init/__init__.py
--rw-r--r--  2.0 unx     6598 b- defN 23-Aug-06 08:07 alfreds_init/init.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_seed/__init__.py
--rw-r--r--  2.0 unx      889 b- defN 23-Aug-04 11:07 alfreds_seed/seed.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_start/__init__.py
--rw-r--r--  2.0 unx      880 b- defN 23-Aug-05 07:22 alfreds_start/start.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_stop/__init__.py
--rw-r--r--  2.0 unx      139 b- defN 23-Aug-04 11:07 alfreds_stop/stop.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_update/__init__.py
--rw-r--r--  2.0 unx     1022 b- defN 23-Aug-04 11:07 alfreds_update/update_agent.py
--rw-r--r--  2.0 unx      990 b- defN 23-Aug-04 11:07 alfreds_update/update_working_directory.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-05 08:02 refresh/__init__.py
--rw-r--r--  2.0 unx      484 b- defN 23-Aug-05 08:04 refresh/refresh.py
--rw-r--r--  2.0 unx     2226 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1510 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/RECORD
-19 files, 17536 bytes uncompressed, 5883 bytes compressed:  66.5%
+Zip file size: 8562 bytes, number of entries: 19
+-rwxr-xr-x  2.0 unx     2760 b- defN 23-Aug-08 09:41 alfreds-0.0.7.data/scripts/alfreds
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.7.data/scripts/main.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 alfreds_init/__init__.py
+-rw-r--r--  2.0 unx     7424 b- defN 23-Aug-08 08:14 alfreds_init/init.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 alfreds_seed/__init__.py
+-rw-r--r--  2.0 unx      889 b- defN 23-Aug-08 07:32 alfreds_seed/seed.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 alfreds_start/__init__.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Aug-08 07:32 alfreds_start/start.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 alfreds_stop/__init__.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Aug-08 07:32 alfreds_stop/stop.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 alfreds_update/__init__.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Aug-08 07:32 alfreds_update/update_agent.py
+-rw-r--r--  2.0 unx      990 b- defN 23-Aug-08 07:32 alfreds_update/update_working_directory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:32 refresh/__init__.py
+-rw-r--r--  2.0 unx      484 b- defN 23-Aug-08 07:32 refresh/refresh.py
+-rw-r--r--  2.0 unx     2226 b- defN 23-Aug-08 09:41 alfreds-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 09:41 alfreds-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 23-Aug-08 09:41 alfreds-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-Aug-08 09:41 alfreds-0.0.7.dist-info/RECORD
+19 files, 18506 bytes uncompressed, 6076 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: alfreds-0.0.6.data/scripts/alfreds
+Filename: alfreds-0.0.7.data/scripts/alfreds
 Comment: 
 
-Filename: alfreds-0.0.6.data/scripts/main.py
+Filename: alfreds-0.0.7.data/scripts/main.py
 Comment: 
 
 Filename: alfreds_init/__init__.py
 Comment: 
 
 Filename: alfreds_init/init.py
 Comment: 
@@ -39,20 +39,20 @@
 
 Filename: refresh/__init__.py
 Comment: 
 
 Filename: refresh/refresh.py
 Comment: 
 
-Filename: alfreds-0.0.6.dist-info/METADATA
+Filename: alfreds-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: alfreds-0.0.6.dist-info/WHEEL
+Filename: alfreds-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: alfreds-0.0.6.dist-info/top_level.txt
+Filename: alfreds-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: alfreds-0.0.6.dist-info/RECORD
+Filename: alfreds-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alfreds_init/init.py

```diff
@@ -63,33 +63,50 @@
                         "-p", f"127.0.0.1:{port}:{port}"]
             if seed_path is not None:
                 print("Mounting seed directory...")
                 commands.append("-v")
                 commands.append(f"{seed_path}:{seed_path}")
 
             commands.append(image_name)
-            subprocess.check_call(commands, stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
+            subprocess.run(commands, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, text=True, check=True)
         else:
-            subprocess.check_call(
+            subprocess.run(
                 ["docker", "run", "--name", container_name, "-d", "-p", f"127.0.0.1:{port}:{port}", image_name],
-                stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
+                stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, text=True, check=True)
         return True
-    except subprocess.CalledProcessError:
+    except subprocess.CalledProcessError as e:
+        print_bold(e.stderr)
         return False
 
 
 def get_alfred_dir():
     home = str(Path.home())
     alfreds_dir = os.path.join(home, ".alfreds")
     return alfreds_dir
 
 
-def alfreds_init(agent_path, working_dir, seed_directory_path=None):
+def alfreds_init(agent_path: str, working_dir, seed_directory_path=None):
     print("Initializing Alfreds...")
 
+    # check if agent_path is a valid aboslute path and exists
+    if agent_path is not None and (not os.path.isabs(agent_path) or not os.path.exists(agent_path)):
+        print_bold("Agent path must be a valid absolute path.")
+        return
+
+    # check if working_dir is a valid aboslute path
+    if working_dir is not None and (not os.path.isabs(working_dir) or not os.path.exists(working_dir)):
+        print_bold("Working directory must be a valid absolute path.")
+        return
+
+    # check if seed_directory_path is a valid aboslute path
+    if seed_directory_path is not None and (not os.path.isabs(seed_directory_path) or not os.path.exists(seed_directory_path)):
+        print_bold("Seed directory path must a valid absolute path.")
+        return
+
+
     # Create a .alfred in user home directory
     alfreds_dir = get_alfred_dir()
     if not os.path.exists(alfreds_dir):
         os.mkdir(alfreds_dir)
 
     config = {
         "agent_path": agent_path,
```

## Comparing `alfreds-0.0.6.data/scripts/alfreds` & `alfreds-0.0.7.data/scripts/alfreds`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 from alfreds_start.start import alfred_start
 from alfreds_stop.stop import stop_containers
 from alfreds_update.update_agent import update_agent
 from alfreds_update.update_working_directory import update_working_directory
 
 # ignore all warnings
 import warnings
+
+from refresh.refresh import refresh
+
 warnings.filterwarnings("ignore")
 
 # Create the parser
 parser = argparse.ArgumentParser(prog='alfreds')
 
 # Create subparsers for different commands
 subparsers = parser.add_subparsers(dest='command')
 
 # Create a parser for 'init' command
 init_parser = subparsers.add_parser('init', help='Initialize Alfreds')
-init_parser.add_argument('--agent_path', help='Path to the agent')
-init_parser.add_argument('--working_dir', help='Working directory')
-init_parser.add_argument('--seed_directory_path', help='Directory path to seed', nargs='?')
+init_parser.add_argument('--agent_path', help='Path to the agent. It should be an absolute path')
+init_parser.add_argument('--working_dir', help='Working directory. It should be an absolute path')
+init_parser.add_argument('--seed_directory_path', help='Directory path to seed. It should be an absolute path', nargs='?')
 
 # Create a parser for 'start' command
 start_parser = subparsers.add_parser('start', help='Start Alfreds')
 
 # Create a parser for 'stop' command
 subparsers.add_parser('stop', help='Stop Alfreds')
 
@@ -66,9 +69,9 @@
     stop_containers()
     print("Alfreds stopped.")
 elif args.command == 'seed':
     seed_directory_path = args.seed_directory_path
     alfred_seed(seed_directory_path)
 elif args.command == 'refresh':
     print("Refreshing Alfreds...")
-
+    refresh()
     print("Alfreds refreshed.")
```

## Comparing `alfreds-0.0.6.dist-info/METADATA` & `alfreds-0.0.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfreds
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alfred Package
 Home-page: https://github.com/TBD
 Author: Data Facade
 Author-email: info@data-facade.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `alfreds-0.0.6.dist-info/RECORD` & `alfreds-0.0.7.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-alfreds-0.0.6.data/scripts/alfreds,sha256=rK_vo1SjqlUoR6UBhPSJ5X8sxE2f1YGJKyhn_BsffYQ,2616
-alfreds-0.0.6.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
+alfreds-0.0.7.data/scripts/alfreds,sha256=7IgunrihzehEAJSwIL8dP8WQX31IODOFJW6ONmnXDXc,2760
+alfreds-0.0.7.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
 alfreds_init/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-alfreds_init/init.py,sha256=tL-bT_cDy1CBTVoVZrwaoAR9CB0_3xpPJ7V1HwN_2yY,6598
+alfreds_init/init.py,sha256=BOaoRulP7dXr-GmwHFny9WFjO1S17KqNv5oADbaUjHA,7424
 alfreds_seed/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_seed/seed.py,sha256=FLqIgMCJWW8cb6KB7dtstioRW8wdzgKMq_wXiwbO5q4,889
 alfreds_start/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_start/start.py,sha256=YN4VjOKWkNdmUp-BuLChUnqsUOARPoWKoDZ-upEAqk4,880
 alfreds_stop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_stop/stop.py,sha256=T3klfHF8boqT4HpW_7ARtAg8Lql4GgZaK6O4Cm_8OAs,139
 alfreds_update/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_update/update_agent.py,sha256=D3-8uk_cKXmiCAFmd-2ib0n8YwmUSOvxgxqCUrWxXQA,1022
 alfreds_update/update_working_directory.py,sha256=IXQp4NYh-IGsgC2Hnl9mbOFPXhtnOJX1hqfO5Ta6iEo,990
 refresh/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 refresh/refresh.py,sha256=MtuP8GmB9Sf4ODYc7UnqeadFkbHTJmI4h12Qy_-T_eU,484
-alfreds-0.0.6.dist-info/METADATA,sha256=owsIRFTXn1eT6SALPGULkSrhLR8scx31b7JJnL_ZpC8,2226
-alfreds-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-alfreds-0.0.6.dist-info/top_level.txt,sha256=6Mb9L3LAWttfLTf738HUv9jpgLoTAOFPL7PgL-5cUY0,76
-alfreds-0.0.6.dist-info/RECORD,,
+alfreds-0.0.7.dist-info/METADATA,sha256=XSPdITAyYgYWdXjneSt1amLh4lghuVlmbS3y0EjfDv0,2226
+alfreds-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+alfreds-0.0.7.dist-info/top_level.txt,sha256=6Mb9L3LAWttfLTf738HUv9jpgLoTAOFPL7PgL-5cUY0,76
+alfreds-0.0.7.dist-info/RECORD,,
```

