# Comparing `tmp/hotsos-1.16.0.post7.tar.gz` & `tmp/hotsos-1.16.0.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.16.0.post7.tar", last modified: Tue Jul 25 19:46:31 2023, max compression
+gzip compressed data, was "hotsos-1.16.0.post8.tar", last modified: Wed Jul 26 20:27:16 2023, max compression
```

## Comparing `hotsos-1.16.0.post7.tar` & `hotsos-1.16.0.post8.tar`

### file list

```diff
@@ -1,411 +1,415 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.169097 hotsos-1.16.0.post7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-25 19:46:31.169097 hotsos-1.16.0.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.105096 hotsos-1.16.0.post7/hotsos/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:46:14.000000 hotsos-1.16.0.post7/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13787 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15371 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.109096 hotsos-1.16.0.post7/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.117096 hotsos-1.16.0.post7/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40487 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.117096 hotsos-1.16.0.post7/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.117096 hotsos-1.16.0.post7/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.117096 hotsos-1.16.0.post7/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.121096 hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/root_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/inputdef.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.125096 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/vardef.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.105096 hotsos-1.16.0.post7/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.129096 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/netlink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.133096 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.101096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.137096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.141096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.141096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.141096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.145096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.145096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.145096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.145096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.145096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.105096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.149096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.153096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.157096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.157096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.157096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.157096 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.157096 hotsos-1.16.0.post7/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.161096 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.165097 hotsos-1.16.0.post7/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:31.109096 hotsos-1.16.0.post7/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 19:46:31.000000 hotsos-1.16.0.post7/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:46:31.169097 hotsos-1.16.0.post7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-25 19:46:08.000000 hotsos-1.16.0.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.595013 hotsos-1.16.0.post8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-26 20:27:16.595013 hotsos-1.16.0.post8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.527012 hotsos-1.16.0.post8/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 20:27:01.000000 hotsos-1.16.0.post8/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13787 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15371 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.527012 hotsos-1.16.0.post8/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.531012 hotsos-1.16.0.post8/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40487 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.531012 hotsos-1.16.0.post8/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.535012 hotsos-1.16.0.post8/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.535012 hotsos-1.16.0.post8/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.535012 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.535012 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.535012 hotsos-1.16.0.post8/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.539012 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.539012 hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.539012 hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.539012 hotsos-1.16.0.post8/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.539012 hotsos-1.16.0.post8/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/root_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.543012 hotsos-1.16.0.post8/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.543012 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.543012 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/inputdef.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.543012 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/vardef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.547012 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.551012 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.551012 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.551012 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.519012 hotsos-1.16.0.post8/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.551012 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/netlink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.555012 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.515012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.519012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/cinder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/cinder/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.519012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.559013 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.563012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.563012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.563012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.563012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.563012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.567012 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.571012 hotsos-1.16.0.post8/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.571012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.571012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.519012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.571012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.579012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.579012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.583012 hotsos-1.16.0.post8/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.587012 hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.591013 hotsos-1.16.0.post8/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:27:16.527012 hotsos-1.16.0.post8/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 20:27:16.000000 hotsos-1.16.0.post8/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:27:16.595013 hotsos-1.16.0.post8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 20:26:54.000000 hotsos-1.16.0.post8/setup.py
```

### Comparing `hotsos-1.16.0.post7/LICENSE` & `hotsos-1.16.0.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/PKG-INFO` & `hotsos-1.16.0.post8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.16.0.post7
+Version: 1.16.0.post8
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.16.0.post7/README.md` & `hotsos-1.16.0.post8/README.md`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/cli.py` & `hotsos-1.16.0.post8/hotsos/cli.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/client.py` & `hotsos-1.16.0.post8/hotsos/client.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/analytics.py` & `hotsos-1.16.0.post8/hotsos/core/analytics.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/config.py` & `hotsos-1.16.0.post8/hotsos/core/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/factory.py` & `hotsos-1.16.0.post8/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/__init__.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/cli.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/cli.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/common.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/config.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/filestat.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/network.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/network.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/packaging.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/pebble.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/ssl.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/ssl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/systemd.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/host_helpers/uptime.py` & `hotsos-1.16.0.post8/hotsos/core/host_helpers/uptime.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/issues/issue_types.py` & `hotsos-1.16.0.post8/hotsos/core/issues/issue_types.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/issues/utils.py` & `hotsos-1.16.0.post8/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/log.py` & `hotsos-1.16.0.post8/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/juju/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/juju/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/juju/resources.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/juju/resources.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/config.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/net.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/net.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/kubernetes.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/lxd/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/maas.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/mysql.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/pacemaker.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/rabbitmq/report.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/sosreport.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/storage/bcache.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/storage/ceph.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/system/system.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/system/system.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugins/vault.py` & `hotsos-1.16.0.post8/hotsos/core/plugins/vault.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/plugintools.py` & `hotsos-1.16.0.post8/hotsos/core/plugintools.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/root_manager.py` & `hotsos-1.16.0.post8/hotsos/core/root_manager.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/search.py` & `hotsos-1.16.0.post8/hotsos/core/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/utils.py` & `hotsos-1.16.0.post8/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/common.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/inputdef.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/inputdef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         for p in self.installed:
             _versions.append(self.packaging_helper.get_version(p))
 
         return _versions
 
     def package_version_within_ranges(self, pkg, versions):
         result = False
-        versions = sorted(versions, key=lambda i: i['min'], reverse=True)
+        versions = sorted(versions, key=lambda i: str(i['min']), reverse=True)
         pkg_version = self.packaging_helper.get_version(pkg)
         for item in versions:
             v_min = str(item['min'])
             if 'max' in item:
                 v_max = str(item['max'])
                 lte_max = pkg_version <= DPKGVersionCompare(v_max)
             else:
```

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 
 
 class YAssertionAttrs(YPropertyOverrideBase):
 
     @classmethod
     def _override_keys(cls):
-        return ['key', 'section', 'ops', 'allow-unset']
+        return ['key', 'value', 'section', 'ops', 'allow-unset']
 
     @property
     def ops(self):
         """
         This is a list so needs its own property.
         """
         return self.content
@@ -69,40 +69,42 @@
         for n, cfg_obj in enumerate(handlers):
             if item.section:
                 actual = cfg_obj.get(item.key, section=item.section)
             else:
                 actual = cfg_obj.get(item.key)
 
             _result = item.allow_unset
-            if item.ops and actual is not None:
-                _result = self.apply_ops(item.ops, opinput=actual,
+
+            ops = item.ops or [['eq', item.value]]
+            if actual is not None:
+                _result = self.apply_ops(ops, opinput=actual,
                                          normalise_value_types=True)
             log.debug("assertion: %s (%s) %s result=%s",
-                      item.key, actual, self.ops_to_str(item.ops or []),
+                      item.key, actual, self.ops_to_str(ops or []),
                       _result)
             if not _result and n < len(handlers) - 1:
                 log.debug("assertion is false and there are more configs to "
                           "check so trying next")
                 continue
 
             cache = self.context.assertions_ctxt['cache']
             msg = "{} {}/actual=\"{}\"".format(item.key,
-                                               self.ops_to_str(item.ops or []),
+                                               self.ops_to_str(ops or []),
                                                actual)
             if cache.assertion_results is not None:
                 cache.set('assertion_results', "{}, {}".
                           format(cache.assertion_results, msg))
             else:
                 cache.set('assertion_results', msg)
 
             # NOTE: This can be useful for single assertion checks but should
             # be used with caution since it will only ever store the last
             # config checked.
             cache.set('key', item.key)
-            cache.set('ops', self.ops_to_str(item.ops or []))
+            cache.set('ops', self.ops_to_str(ops or []))
             cache.set('value_actual', actual)
 
         return _result
 
     @property
     def passes(self):
         log.debug("running assertion set")
```

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/engine/properties/vardef.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/engine/properties/vardef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/events.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/core/ycheck/scenarios.py` & `hotsos-1.16.0.post8/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openstack/octavia.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openstack/octavia.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.16.0.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/netlink.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/netlink.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/openvswitch/service_restarts.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.16.0.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/juju/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/sosreport/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/sosreport/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.16.0.post8/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos/templates/header.html` & `hotsos-1.16.0.post8/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.16.0.post7/hotsos.egg-info/PKG-INFO` & `hotsos-1.16.0.post8/hotsos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.16.0.post7
+Version: 1.16.0.post8
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.16.0.post7/hotsos.egg-info/SOURCES.txt` & `hotsos-1.16.0.post8/hotsos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 hotsos/defs/scenarios/openstack/openstack.yaml
 hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
 hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
 hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
 hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
 hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
 hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
 hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
 hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
 hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
 hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
@@ -185,14 +186,15 @@
 hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
 hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
 hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
 hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
 hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
 hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
 hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
 hotsos/defs/scenarios/openvswitch/openvswitch.yaml
 hotsos/defs/scenarios/openvswitch/service_restarts.yaml
```

### Comparing `hotsos-1.16.0.post7/pyproject.toml` & `hotsos-1.16.0.post8/pyproject.toml`

 * *Files identical despite different names*

