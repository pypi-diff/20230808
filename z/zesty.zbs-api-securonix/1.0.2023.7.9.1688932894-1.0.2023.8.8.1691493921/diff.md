# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.8.8.1691493921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar", last modified: Sun Jul  9 20:01:35 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.8.8.1691493921.tar", last modified: Tue Aug  8 11:25:22 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16536 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    14309 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3794 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16587 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    14309 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-08-08 11:24:52.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-08 11:25:22.000000 zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.9.1688932894
+Version: 1.0.2023.8.8.1691493921
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/README.md` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/BlockDevice.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,18 +77,21 @@
 
         if not unlock_ts:
             self.unlock_ts = 0
         else:
             self.unlock_ts = unlock_ts
 
         self.volume_type = volume_type
-        self.btrfs_size = btrfs_size
+
         self.extendable = extendable
         self.removable = removable
-    
+
+        # if btrfs_size is None (e.g- windows/old collector, set btrfs_size to size)
+        self.btrfs_size = btrfs_size if btrfs_size is not None else size
+
     def as_dict(self) -> dict:
         return_dict = json.loads(json.dumps(self, default=self.object_dumper))
         return {k: v for k, v in return_dict.items() if v is not None}
 
     @staticmethod
     def object_dumper(obj) -> dict:
         try:
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/ManagedFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 
 class ManagedFs(ManagedFsMixin, BaseMixin, Base):
     __tablename__ = "managed_filesystems"
 
 
 class MigrationStatus(Enum):
     Active = auto()
+    Aborting = auto()
     Aborted = auto()
     Completed = auto()
     Failed = auto()
 
 
 class RunningMigrations(BaseMixin, Base):
     __tablename__ = "active_migration"
@@ -360,14 +361,15 @@
 
 
 class MigrationHistory(BaseMixin, Base):
     __tablename__ = "migration_history"
 
     time_start = Column(TIMESTAMP)
     time_end = Column(TIMESTAMP)
+    status = Column(VARCHAR)
     phase = Column(VARCHAR, primary_key=True)
     progress = Column(FLOAT)
     completed = Column(BOOLEAN)
     failed = Column(BOOLEAN)
     failure_reason = Column(VARCHAR)
     fs_id = Column(VARCHAR)
     migration_uuid = Column(UUID(as_uuid=True), ForeignKey("active_migration.migration_uuid",  ondelete="CASCADE"),
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.9.1688932894
+Version: 1.0.2023.8.8.1691493921
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.8.8.1691493921/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

