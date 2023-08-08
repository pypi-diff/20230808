# Comparing `tmp/pierskarsenbarg_pulumi_sdm-1.4.0.tar.gz` & `tmp/pierskarsenbarg_pulumi_sdm-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.4.0.tar", last modified: Mon Jul 31 20:32:42 2023, max compression
+gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.4.1.tar", last modified: Tue Aug  8 09:48:45 2023, max compression
```

## Comparing `pierskarsenbarg_pulumi_sdm-1.4.0.tar` & `pierskarsenbarg_pulumi_sdm-1.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   755154 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (123)  1296574 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)   154776 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   756506 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1298694 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154776 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:48:45.000000 pierskarsenbarg_pulumi_sdm-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-08 09:48:44.000000 pierskarsenbarg_pulumi_sdm-1.4.1/setup.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg_pulumi_sdm
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/README.md` & `pierskarsenbarg_pulumi_sdm-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/__init__.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_inputs.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8275,27 +8275,29 @@
     def __init__(__self__, *,
                  endpoint: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  certificate_authority: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  service_account_key: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param pulumi.Input[str] certificate_authority: The CA to authenticate TLS connections with.
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param pulumi.Input[int] port_override: The local port used by clients to connect to this resource.
         :param pulumi.Input[str] remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
         :param pulumi.Input[str] remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] service_account_key: The service account key to authenticate with.
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
@@ -8305,14 +8307,16 @@
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
@@ -8391,14 +8395,26 @@
         return pulumi.get(self, "healthcheck_namespace")
 
     @healthcheck_namespace.setter
     def healthcheck_namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_namespace", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the remote identity group to use for remote identity connections.
         """
         return pulumi.get(self, "remote_identity_group_id")
 
@@ -8472,25 +8488,27 @@
     def __init__(__self__, *,
                  endpoint: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  certificate_authority: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  service_account_key: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param pulumi.Input[str] certificate_authority: The CA to authenticate TLS connections with.
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param pulumi.Input[int] port_override: The local port used by clients to connect to this resource.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] service_account_key: The service account key to authenticate with.
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -8498,14 +8516,16 @@
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
@@ -8580,14 +8600,26 @@
         return pulumi.get(self, "healthcheck_namespace")
 
     @healthcheck_namespace.setter
     def healthcheck_namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_namespace", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[pulumi.Input[str]]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_utilities.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/vars.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_node.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_role.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/node.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/outputs.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7528,14 +7528,16 @@
             suggest = "bind_interface"
         elif key == "certificateAuthority":
             suggest = "certificate_authority"
         elif key == "egressFilter":
             suggest = "egress_filter"
         elif key == "healthcheckNamespace":
             suggest = "healthcheck_namespace"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "remoteIdentityGroupId":
             suggest = "remote_identity_group_id"
         elif key == "remoteIdentityHealthcheckUsername":
             suggest = "remote_identity_healthcheck_username"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "serviceAccountKey":
@@ -7555,27 +7557,29 @@
     def __init__(__self__, *,
                  endpoint: str,
                  name: str,
                  bind_interface: Optional[str] = None,
                  certificate_authority: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
         :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
@@ -7585,14 +7589,16 @@
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
@@ -7647,14 +7653,22 @@
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
         """
         The ID of the remote identity group to use for remote identity connections.
         """
         return pulumi.get(self, "remote_identity_group_id")
 
@@ -7708,14 +7722,16 @@
             suggest = "bind_interface"
         elif key == "certificateAuthority":
             suggest = "certificate_authority"
         elif key == "egressFilter":
             suggest = "egress_filter"
         elif key == "healthcheckNamespace":
             suggest = "healthcheck_namespace"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "serviceAccountKey":
             suggest = "service_account_key"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ResourceGoogleGkeUserImpersonation. Access the value via the '{suggest}' property getter instead.")
@@ -7731,25 +7747,27 @@
     def __init__(__self__, *,
                  endpoint: str,
                  name: str,
                  bind_interface: Optional[str] = None,
                  certificate_authority: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -7757,14 +7775,16 @@
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
@@ -7815,14 +7835,22 @@
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
@@ -24160,28 +24188,30 @@
                  bind_interface: Optional[str] = None,
                  certificate_authority: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
         :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
@@ -24195,14 +24225,16 @@
             pulumi.set(__self__, "endpoint", endpoint)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
@@ -24265,14 +24297,22 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
         """
         The ID of the remote identity group to use for remote identity connections.
         """
         return pulumi.get(self, "remote_identity_group_id")
 
@@ -24323,26 +24363,28 @@
                  bind_interface: Optional[str] = None,
                  certificate_authority: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -24354,14 +24396,16 @@
             pulumi.set(__self__, "endpoint", endpoint)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
@@ -24420,14 +24464,22 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_peer.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/peering_group_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/provider.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/role.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm/secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg-pulumi-sdm
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_sdm-1.4.1/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.4.0/setup.py` & `pierskarsenbarg_pulumi_sdm-1.4.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.4.0"
-PLUGIN_VERSION = "1.4.0"
+VERSION = "1.4.1"
+PLUGIN_VERSION = "1.4.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-sdm'])
         except OSError as error:
```

