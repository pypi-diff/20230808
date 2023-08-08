# Comparing `tmp/kubemarine-0.19.0.tar.gz` & `tmp/kubemarine-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.19.0.tar", last modified: Mon Jul 17 12:16:54 2023, max compression
+gzip compressed data, was "kubemarine-0.20.0.tar", last modified: Mon Aug  7 10:42:59 2023, max compression
```

## Comparing `kubemarine-0.19.0.tar` & `kubemarine-0.20.0.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.937780 kubemarine-0.19.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-17 12:16:40.000000 kubemarine-0.19.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-17 12:16:40.000000 kubemarine-0.19.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12511 2023-07-17 12:16:54.937780 kubemarine-0.19.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9063 2023-07-17 12:16:40.000000 kubemarine-0.19.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.913779 kubemarine-0.19.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-07-17 12:16:40.000000 kubemarine-0.19.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-17 12:16:40.000000 kubemarine-0.19.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.913779 kubemarine-0.19.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7885 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    45787 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     5069 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15384 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23767 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     5228 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    28488 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    19237 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    36274 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    14620 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8978 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15820 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    21435 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6620 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3892 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    22272 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4603 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    11022 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     3609 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11285 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    64809 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3496 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5850 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    31794 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    41882 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14948 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5769 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    17062 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    20607 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.921779 kubemarine-0.19.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20764 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2825 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50099 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    72373 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5247 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26685 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1830 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1728 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    13901 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    19949 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2476 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6032 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13897 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    11748 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3826 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5333 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     4067 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     6255 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3177 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    25036 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    10664 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.909779 kubemarine-0.19.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.925780 kubemarine-0.19.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2363 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.929780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4198 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1881 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2775 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1240 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     8533 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3927 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    27551 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.933780 kubemarine-0.19.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11474 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    17633 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     5696 2023-07-17 12:16:40.000000 kubemarine-0.19.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:16:54.917779 kubemarine-0.19.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12511 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9113 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-17 12:16:54.000000 kubemarine-0.19.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5480 2023-07-17 12:16:40.000000 kubemarine-0.19.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 12:16:54.937780 kubemarine-0.19.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 12:16:40.000000 kubemarine-0.19.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.827490 kubemarine-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-07 10:42:50.000000 kubemarine-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2023-08-07 10:42:50.000000 kubemarine-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12511 2023-08-07 10:42:59.827490 kubemarine-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9063 2023-08-07 10:42:50.000000 kubemarine-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.803489 kubemarine-0.20.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-08-07 10:42:50.000000 kubemarine-0.20.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-08-07 10:42:50.000000 kubemarine-0.20.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.807489 kubemarine-0.20.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8135 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    46861 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     5069 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.811489 kubemarine-0.20.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15569 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    24071 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    18901 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    36365 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    15061 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15290 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    22336 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.811489 kubemarine-0.20.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6620 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3892 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    22191 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    11022 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3609 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.811489 kubemarine-0.20.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    65423 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5850 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    31908 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.811489 kubemarine-0.20.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/patches/p1_kubeadm_flags.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.811489 kubemarine-0.20.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    42535 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14948 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5769 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    20607 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4980 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    21051 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2825 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50502 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    73406 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     4844 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26994 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1830 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1728 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    14057 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    19949 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2476 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6113 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    14054 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    11703 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.815490 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    25122 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    10664 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.803489 kubemarine-0.20.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.819490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      708 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.823490 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.827490 kubemarine-0.20.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    27551 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.827490 kubemarine-0.20.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.827490 kubemarine-0.20.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.827490 kubemarine-0.20.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    17741 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-08-07 10:42:50.000000 kubemarine-0.20.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:42:59.807489 kubemarine-0.20.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12511 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-07 10:42:59.000000 kubemarine-0.20.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-08-07 10:42:50.000000 kubemarine-0.20.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 10:42:59.827490 kubemarine-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-08-07 10:42:50.000000 kubemarine-0.20.0/setup.py
```

### Comparing `kubemarine-0.19.0/LICENSE` & `kubemarine-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/PKG-INFO` & `kubemarine-0.20.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.19.0
+Version: 0.20.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -34,36 +34,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -81,15 +81,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -100,15 +100,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.20.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -129,24 +129,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.19.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.20.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -175,42 +175,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.20.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.19.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.20.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.19.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.20.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.19.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.20.0/LICENSE)
```

### Comparing `kubemarine-0.19.0/README.md` & `kubemarine-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/bin/kubemarine` & `kubemarine-0.20.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/bin/kubemarine.cmd` & `kubemarine-0.20.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/__init__.py` & `kubemarine-0.20.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/__main__.py` & `kubemarine-0.20.0/kubemarine/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import sys
+import time
+import types
 from collections import OrderedDict
 from typing import Dict, List
 
 import ruamel.yaml.resolver
 import yaml
 
 # Don't remove this line. The idna encoding
@@ -40,16 +42,16 @@
 # https://stackoverflow.com/questions/30458977/yaml-loads-5e-6-as-string-and-not-a-number
 # https://github.com/yaml/pyyaml/issues/173
 for ir in ruamel.yaml.resolver.implicit_resolvers:
     # YAML 1.1 and float implicit resolver
     if (1, 1) in ir[0] and 'tag:yaml.org,2002:float' in ir[1]:
         float_patched_resolver = (ir[1], ir[2], ir[3])
         # Globally change behaviour of yaml.safe_load and yaml.dump
-        yaml.Dumper.add_implicit_resolver(*float_patched_resolver)
-        yaml.SafeLoader.add_implicit_resolver(*float_patched_resolver)
+        yaml.Dumper.add_implicit_resolver(*float_patched_resolver)  # type: ignore[no-untyped-call]
+        yaml.SafeLoader.add_implicit_resolver(*float_patched_resolver)  # type: ignore[no-untyped-call]
         break
 
 
 procedures = OrderedDict({
     'install': {
         'description': "Install a cluster from scratch",
         'group': 'installation'
@@ -117,15 +119,16 @@
     },
     'migrate_cri': {
         'description': "Migrate from Docker to Containerd",
         'group': 'maintenance'
     },
 })
 
-def main():
+
+def main() -> None:
     arguments = sys.argv[1:]
 
     if len(arguments) > 0:
         if arguments[0] == 'selftest':
             return selftest()
         elif arguments[0] == 'version':
             return version()
@@ -150,38 +153,36 @@
         print('''The following procedures available:
 %s
 
 Usage: kubemarine <procedure> <arguments>
 ''' % '\n'.join(descriptions_print_list))
         sys.exit(1)
 
-    import_procedure(arguments[0]).main(arguments[1:])
-
+    result = import_procedure(arguments[0]).main(arguments[1:])
+    if result is not None:
+        from kubemarine.testsuite import TestSuite
+        if isinstance(result, TestSuite) and result.is_any_test_failed():
+            sys.exit(1)
 
-def import_procedure(name):
+def import_procedure(name: str) -> types.ModuleType:
     module_name = 'kubemarine.procedures.%s' % name
     return __import__(module_name, fromlist=['object'])
 
 
-def version():
+def version() -> None:
     from kubemarine.core import utils
 
     print('Kubemarine %s' % utils.get_version())
 
 
-def selftest():
+def selftest() -> None:
     print("Running selftest")
 
-    import time
-
     time_start = int(round(time.time() * 1000))
 
-    from collections import OrderedDict
-    import types
-
     for procedure, procedure_details in procedures.items():
         print("\nImporting %s..." % procedure)
 
         if procedure in ['version', 'selftest']:
             continue
 
         module = import_procedure(procedure)
```

### Comparing `kubemarine-0.19.0/kubemarine/admission.py` & `kubemarine-0.20.0/kubemarine/admission.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 import uuid
 import re
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 
 from kubemarine import kubernetes
 from kubemarine.core import utils
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import NodeGroup
+from kubemarine.core.group import NodeGroup, RunnersGroupResult
 from kubemarine.core.yaml_merger import default_merger
 
 privileged_policy_filename = "privileged.yaml"
 policies_file_path = "./resources/psp/"
 tmp_filepath_pattern = "/tmp/%s"
 
 admission_template = "./templates/admission.yaml.j2"
@@ -49,15 +49,15 @@
 privileged_plugins = {"nginx-ingress-controller": "ingress-nginx", 
                       "local-path-provisioner": "local-path-storage"}
 
 loaded_oob_policies = {}
 
 # TODO: When KubeMarine is not support Kubernetes version lower than 1.25, the PSP implementation code should be deleted 
 
-def enrich_inventory_psp(inventory: dict, _):
+def enrich_inventory_psp(inventory: dict, _: KubernetesCluster) -> dict:
     global loaded_oob_policies
     loaded_oob_policies = load_oob_policies_files()
 
     # validate custom
     custom_policies = inventory["rbac"]["psp"]["custom-policies"]
     verify_custom(custom_policies)
 
@@ -70,15 +70,15 @@
     if 'PodSecurityPolicy' not in enabled_admissions:
         enabled_admissions = "%s,PodSecurityPolicy" % enabled_admissions
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["enable-admission-plugins"] = enabled_admissions
         
     return inventory
 
 
-def enrich_inventory_pss(inventory: dict, _):
+def enrich_inventory_pss(inventory: dict, _: KubernetesCluster) -> dict:
     if not is_security_enabled(inventory):
         return inventory
     # check flags, enforce and logs parameters
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if minor_version < 23:
         raise Exception("PSS is not supported properly in Kubernetes version before v1.23")
     for item in inventory["rbac"]["pss"]["defaults"]:
@@ -94,23 +94,25 @@
     else:     
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["feature-gates"] = "PodSecurity=true"
         inventory["services"]["kubeadm"]["apiServer"]["extraArgs"]["admission-control-config-file"] = admission_path
 
     return inventory
 
 
-def enrich_inventory(inventory: dict, _):
+def enrich_inventory(inventory: dict, _: KubernetesCluster) -> dict:
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return enrich_inventory_psp(inventory, _)
     elif admission_impl == "pss":
         return enrich_inventory_pss(inventory, _)
 
+    return inventory
+
 
-def manage_psp_enrichment(inventory: dict, cluster: KubernetesCluster):
+def manage_psp_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if minor_version >= 25:
         raise Exception("PSP is not supported in Kubernetes version higher than v1.24")
     if cluster.context.get('initial_procedure') != 'manage_psp':
         return inventory
 
     procedure_config = cluster.procedure_inventory["psp"]
@@ -129,47 +131,47 @@
     final_security_state = procedure_config.get("pod-security", current_security_state)
     if final_security_state == "disabled" and procedure_config.get("oob-policies"):
         raise Exception("OOB policies can not be configured when security is disabled")
 
     return inventory
 
 
-def verify_custom(custom_scope):
+def verify_custom(custom_scope: Dict[str, List[dict]]) -> None:
     psp_list = custom_scope.get(psp_list_option, None)
     if psp_list:
         verify_custom_list(psp_list, "PSP")
 
     roles_list = custom_scope.get(roles_list_option, None)
     if roles_list:
         verify_custom_list(roles_list, "role")
 
     bindings_list = custom_scope.get(bindings_list_option, None)
     if bindings_list:
         verify_custom_list(bindings_list, "binding")
 
 
-def verify_custom_list(custom_list, type):
+def verify_custom_list(custom_list: List[dict], type: str) -> None:
     for item in custom_list:
         # forbid using 'oob-' prefix in order to avoid conflicts of our policies and users policies
         if item["metadata"]["name"].startswith("oob-"):
             raise Exception("Name %s is not allowed for custom %s" % (item["metadata"]["name"], type))
 
 
-def verify_version(owner, version, minor_version_cfg):
+def verify_version(owner: str, version: str, minor_version_cfg: int) -> None:
     # check Kubernetes version and admission config matching
     if version != "latest":
         result = re.match(valid_versions_templ, version)
         if result is None:
             raise Exception("incorrect Kubernetes version %s, valid version(for example): v1.23" % owner)
         minor_version = int(version.split('.')[1])
         if minor_version > minor_version_cfg:
             raise Exception("%s version must not be higher than Kubernetes version" % owner)
 
 
-def finalize_inventory_psp(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def finalize_inventory_psp(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     if cluster.context.get('initial_procedure') != 'manage_psp':
         return inventory_to_finalize
     procedure_config = cluster.procedure_inventory["psp"]
 
     if "rbac" not in inventory_to_finalize:
         inventory_to_finalize["rbac"] = {}
     if "psp" not in inventory_to_finalize["rbac"]:
@@ -198,44 +200,46 @@
         else:
             for oob_policy in procedure_config["oob-policies"]:
                 current_config["oob-policies"][oob_policy] = procedure_config["oob-policies"][oob_policy]
 
     return inventory_to_finalize
 
 
-def merge_custom_policies(old_policies, added_policies, deleted_policies):
+def merge_custom_policies(old_policies: Dict[str, List[dict]],
+                          added_policies: Dict[str, List[dict]],
+                          deleted_policies: Dict[str, List[dict]]) -> Dict[str, List[dict]]:
     return {
         psp_list_option: merge_policy_lists(old_policies.get(psp_list_option, []),
                                             added_policies.get(psp_list_option, []),
                                             deleted_policies.get(psp_list_option, [])),
         roles_list_option: merge_policy_lists(old_policies.get(roles_list_option, []),
                                               added_policies.get(roles_list_option, []),
                                               deleted_policies.get(roles_list_option, [])),
         bindings_list_option: merge_policy_lists(old_policies.get(bindings_list_option, []),
                                                  added_policies.get(bindings_list_option, []),
                                                  deleted_policies.get(bindings_list_option, []))
     }
 
 
-def merge_policy_lists(old_list, added_list, deleted_list):
+def merge_policy_lists(old_list: List[dict], added_list: List[dict], deleted_list: List[dict]) -> List[dict]:
     resulting_list = added_list
     added_names_list = [item["metadata"]["name"] for item in added_list]
     deleted_names_list = [item["metadata"]["name"] for item in deleted_list]
     for old_item in old_list:
         old_item_name = old_item["metadata"]["name"]
         if old_item_name in added_names_list or old_item_name in deleted_names_list:
             # skip old item, since it was either deleted, replaced by new item, or deleted and then replaced
             continue
         # old item is nor deleted, nor updated, then we need to preserve it in resulting list
         resulting_list.append(old_item)
 
     return resulting_list
 
 
-def install_psp_task(cluster: KubernetesCluster):
+def install_psp_task(cluster: KubernetesCluster) -> None:
     if not is_security_enabled(cluster.inventory):
         cluster.log.debug("Pod security disabled, skipping policies installation...")
         return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Installing OOB policies...")
@@ -245,39 +249,39 @@
 
     cluster.log.debug("Installing custom policies...")
     first_control_plane.call(manage_policies,
                       manage_type="apply",
                       manage_scope=cluster.inventory["rbac"]["psp"]["custom-policies"])
 
 
-def delete_custom_task(cluster: KubernetesCluster):
+def delete_custom_task(cluster: KubernetesCluster) -> None:
     if "delete-policies" not in cluster.procedure_inventory["psp"]:
         cluster.log.debug("No 'delete-policies' specified, skipping...")
         return
 
     cluster.log.debug("Deleting custom 'delete-policies'")
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     first_control_plane.call(manage_policies,
                       manage_type="delete",
                       manage_scope=cluster.procedure_inventory["psp"]["delete-policies"])
 
 
-def add_custom_task(cluster: KubernetesCluster):
+def add_custom_task(cluster: KubernetesCluster) -> None:
     if "add-policies" not in cluster.procedure_inventory["psp"]:
         cluster.log.debug("No 'add-policies' specified, skipping...")
         return
 
     cluster.log.debug("Applying custom 'add-policies'")
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     first_control_plane.call(manage_policies,
                       manage_type="apply",
                       manage_scope=cluster.procedure_inventory["psp"]["add-policies"])
 
 
-def reconfigure_oob_task(cluster: KubernetesCluster):
+def reconfigure_oob_task(cluster: KubernetesCluster) -> None:
     target_security_state = cluster.procedure_inventory["psp"].get("pod-security")
     oob_policies = cluster.procedure_inventory["psp"].get("oob-policies")
 
     # reconfigure OOB only if state will be changed, or OOB configuration was changed
     if not target_security_state and not oob_policies:
         cluster.log.debug("No need to reconfigure OOB policies, skipping...")
         return
@@ -299,15 +303,15 @@
     for policy in provided_oob_policies:
         if procedure_config.get(policy, current_config[policy]) == "enabled":
             policies_to_recreate[policy] = True
     first_control_plane.call(apply_privileged_policy)
     first_control_plane.call(manage_policies, manage_type="apply", manage_scope=resolve_oob_scope(policies_to_recreate, "all"))
 
 
-def reconfigure_plugin_task(cluster: KubernetesCluster):
+def reconfigure_plugin_task(cluster: KubernetesCluster) -> None:
     target_state = cluster.procedure_inventory["psp"].get("pod-security")
 
     if not target_state:
         cluster.log.debug("Security plugin will not be reconfigured")
         return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
@@ -316,15 +320,15 @@
     final_admission_plugins_list = first_control_plane.call(update_kubeadm_configmap, target_state=target_state)
 
     # update api-server config on all control-planes
     cluster.log.debug("Updating kube-apiserver configs on control-planes")
     cluster.nodes["control-plane"].call(update_kubeapi_config, options_list=final_admission_plugins_list)
 
 
-def restart_pods_task(cluster: KubernetesCluster):
+def restart_pods_task(cluster: KubernetesCluster) -> None:
     if cluster.context.get('initial_procedure') == 'manage_pss':
         # check if pods restart is enabled
         is_restart = cluster.procedure_inventory.get("restart-pods", False)
         if not is_restart:
             cluster.log.debug("'restart-pods' is disabled, pods won't be restarted")
             return
 
@@ -380,15 +384,15 @@
     admission_impl = first_control_plane.cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
         return update_kubeadm_configmap_psp(first_control_plane, target_state)
     else:  # admission_impl == "pss":
         return update_kubeadm_configmap_pss(first_control_plane, target_state)
 
 
-def update_kubeapi_config_psp(control_planes: NodeGroup, plugins_list: str):
+def update_kubeapi_config_psp(control_planes: NodeGroup, plugins_list: str) -> None:
     yaml = ruamel.yaml.YAML()
 
     for control_plane in control_planes.get_ordered_members_list():
         result = control_plane.sudo("cat /etc/kubernetes/manifests/kube-apiserver.yaml")
 
         # update kube-apiserver config with updated plugins list
         conf = yaml.load(list(result.values())[0].stdout)
@@ -408,78 +412,82 @@
         else:
             control_plane.call(utils.wait_command_successful,
                                                    command="docker stop $(sudo docker ps -q -f 'name=k8s_kube-apiserver'"
                                                            " | awk '{print $1}')")
         control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
 
 
-def update_kubeapi_config(control_planes: NodeGroup, options_list: str):
+def update_kubeapi_config(control_planes: NodeGroup, options_list: str) -> None:
     admission_impl = control_planes.cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
-        return update_kubeapi_config_psp(control_planes, options_list)
+        update_kubeapi_config_psp(control_planes, options_list)
     elif admission_impl == "pss":
-        return update_kubeapi_config_pss(control_planes, options_list)
+        update_kubeapi_config_pss(control_planes, options_list)
 
-def is_security_enabled(inventory: dict):
+
+def is_security_enabled(inventory: dict) -> bool:
     admission_impl = inventory['rbac']['admission']
+    target_state = "disabled"
     if admission_impl == "psp":
-        return inventory["rbac"]["psp"]["pod-security"] == "enabled"
+        target_state = inventory["rbac"]["psp"]["pod-security"]
     elif admission_impl == "pss":
-        return inventory["rbac"]["pss"]["pod-security"] == "enabled"
+        target_state = inventory["rbac"]["pss"]["pod-security"]
+
+    return target_state == "enabled"
 
 
-def apply_privileged_policy(group: NodeGroup):
+def apply_privileged_policy(group: NodeGroup) -> RunnersGroupResult:
     return manage_privileged_from_file(group, privileged_policy_filename, "apply")
 
 
-def delete_privileged_policy(group: NodeGroup):
+def delete_privileged_policy(group: NodeGroup) -> RunnersGroupResult:
     return manage_privileged_from_file(group, privileged_policy_filename, "delete")
 
 
-def apply_admission(group: NodeGroup):
+def apply_admission(group: NodeGroup) -> None:
     admission_impl = group.cluster.inventory['rbac']['admission']
     if is_security_enabled(group.cluster.inventory):
         if admission_impl == "psp":
             group.cluster.log.debug("Setting up privileged psp...")
             apply_privileged_policy(group)
         elif admission_impl == "pss":
             group.cluster.log.debug("Setting up default pss...")
             apply_default_pss(group.cluster)
 
 
-def apply_default_pss(cluster: KubernetesCluster):
+def apply_default_pss(cluster: KubernetesCluster) -> None:
     if cluster.context.get('initial_procedure') == 'manage_pss':
         procedure_config = cluster.procedure_inventory["pss"]
         current_config = cluster.inventory["rbac"]["pss"]
         if procedure_config["pod-security"] == "enabled" and current_config["pod-security"] == "enabled":
-            return manage_pss(cluster, "apply")
+            manage_pss(cluster, "apply")
         elif procedure_config["pod-security"] == "enabled" and current_config["pod-security"] == "disabled":
-            return manage_pss(cluster, "install")
+            manage_pss(cluster, "install")
     else:
-            return manage_pss(cluster, "init")
+        manage_pss(cluster, "init")
 
 
-def delete_default_pss(cluster: KubernetesCluster):
+def delete_default_pss(cluster: KubernetesCluster) -> None:
     procedure_config = cluster.procedure_inventory["pss"]
     current_config = cluster.inventory["rbac"]["pss"]
     if procedure_config["pod-security"] == "disabled" and current_config["pod-security"] == "enabled":
         return manage_pss(cluster, "delete")
 
 
-def manage_privileged_from_file(group: NodeGroup, filename, manage_type):
+def manage_privileged_from_file(group: NodeGroup, filename: str, manage_type: str) -> RunnersGroupResult:
     if manage_type not in ["apply", "delete"]:
         raise Exception("unexpected manage type for privileged policy")
     privileged_policy = utils.read_internal(os.path.join(policies_file_path, filename))
     remote_path = tmp_filepath_pattern % filename
     group.put(io.StringIO(privileged_policy), remote_path, backup=True, sudo=True)
 
     return group.sudo("kubectl %s -f %s" % (manage_type, remote_path), warn=True)
 
 
-def resolve_oob_scope(oob_policies_conf: Dict[str, Any], selector: str):
+def resolve_oob_scope(oob_policies_conf: Dict[str, Any], selector: str) -> Dict[str, List[dict]]:
     result: Dict[str, List[dict]] = {
         psp_list_option: [],
         roles_list_option: [],
         bindings_list_option: []
     }
 
     for key, value in oob_policies_conf.items():
@@ -491,43 +499,46 @@
                 result[roles_list_option].append(policy["role"])
             if "binding" in policy:
                 result[bindings_list_option].append(policy["binding"])
 
     return result
 
 
-def load_oob_policies_files():
+def load_oob_policies_files() -> Dict[str, dict]:
     oob_policies = {}
     for oob_name in provided_oob_policies:
         local_path = os.path.join(policies_file_path, "%s.yaml" % oob_name)
         with utils.open_internal(local_path) as stream:
             oob_policies[oob_name] = yaml.safe_load(stream)
 
     return oob_policies
 
 
-def manage_policies(group: NodeGroup, manage_type, manage_scope):
+def manage_policies(group: NodeGroup, manage_type: str,
+                    manage_scope: Dict[str, List[dict]]) -> Optional[RunnersGroupResult]:
     psp_to_manage = manage_scope.get(psp_list_option, None)
     roles_to_manage = manage_scope.get(roles_list_option, None)
     bindings_to_manage = manage_scope.get(bindings_list_option, None)
 
     if not psp_to_manage and not roles_to_manage and not bindings_to_manage:
         group.cluster.log.verbose("No policies to %s" % manage_type)
-        return
+        return None
 
     template = collect_policies_template(psp_to_manage, roles_to_manage, bindings_to_manage)
     filename = uuid.uuid4().hex
     remote_path = tmp_filepath_pattern % filename
     group.put(io.StringIO(template), remote_path, backup=True, sudo=True)
     result = group.sudo("kubectl %s -f %s" % (manage_type, remote_path), warn=True)
     group.sudo("rm -f %s" % remote_path)
     return result
 
 
-def collect_policies_template(psp_list, roles_list, bindings_list):
+def collect_policies_template(psp_list: Optional[List[dict]],
+                              roles_list: Optional[List[dict]],
+                              bindings_list: Optional[List[dict]]) -> str:
     yaml = ruamel.yaml.YAML()
 
     buf = io.StringIO()
     if psp_list:
         for psp in psp_list:
             yaml.dump(psp, buf)
             buf.write("\n---\n")
@@ -538,20 +549,20 @@
     if bindings_list:
         for binding in bindings_list:
             yaml.dump(binding, buf)
             buf.write("\n---\n")
     return buf.getvalue()
 
 
-def resolve_final_plugins_list(cluster_config, target_state):
+def resolve_final_plugins_list(cluster_config: dict, target_state: str) -> str:
     if "enable-admission-plugins" not in cluster_config["apiServer"]["extraArgs"]:
         if target_state == "enabled":
             return "PodSecurityPolicy"
         else:
-            return None
+            return ""
     else:
         current_plugins = cluster_config["apiServer"]["extraArgs"]["enable-admission-plugins"]
         if "PodSecurityPolicy" not in current_plugins:
             if target_state == "enabled":
                 resulting_list = "%s,%s" % (current_plugins, "PodSecurityPolicy")
             else:
                 resulting_list = current_plugins
@@ -559,21 +570,21 @@
             resulting_list = current_plugins.replace("PodSecurityPolicy", "")
         else:
             resulting_list = current_plugins
 
         return resulting_list.replace(",,", ",").strip(",")
 
 
-def install(cluster: KubernetesCluster):
+def install(cluster: KubernetesCluster) -> None:
     admission_impl = cluster.inventory['rbac']['admission']
     if admission_impl == "psp":
-        return install_psp_task(cluster)
+        install_psp_task(cluster)
 
 
-def manage_pss_enrichment(inventory: dict, cluster: KubernetesCluster):
+def manage_pss_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get('initial_procedure') != 'manage_pss':
         return inventory
 
     procedure_config = cluster.procedure_inventory["pss"]
     minor_version = int(cluster.inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
         
     if not is_security_enabled(inventory) and procedure_config["pod-security"] == "disabled":
@@ -602,32 +613,32 @@
         for item in procedure_config["namespaces_defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["namespaces_defaults"][item], minor_version)
 
     return inventory
 
 
-def enrich_default_admission(inventory: dict, _):
+def enrich_default_admission(inventory: dict, _: KubernetesCluster) -> dict:
     minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
     if not inventory["rbac"].get("admission"):
         inventory["rbac"]["admission"] = "psp" if minor_version < 25 else "pss"
     return inventory
 
 
-def manage_enrichment(inventory: dict, cluster: KubernetesCluster):
+def manage_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return manage_psp_enrichment(inventory, cluster)
     elif admission_impl == "pss":
         return manage_pss_enrichment(inventory, cluster)
 
     return inventory
 
 
-def manage_pss(cluster: KubernetesCluster, manage_type: str):
+def manage_pss(cluster: KubernetesCluster, manage_type: str) -> None:
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     control_planes = cluster.nodes["control-plane"]
     # 'apply' - change options in admission.yaml, PSS is enabled
     if manage_type == "apply":
         # set labels for predifined plugins namespaces and namespaces defined in procedure config
         label_namespace_pss(cluster, manage_type)
         # copy admission config on control-planes
@@ -672,15 +683,15 @@
 
         # erase PSS admission config 
         cluster.log.debug("Erase admission configuration... %s" % admission_path)
         group = cluster.nodes["control-plane"]
         group.sudo("rm -f %s" % admission_path, warn=True)
 
 
-def update_kubeapi_config_pss(control_planes: NodeGroup, features_list: str):
+def update_kubeapi_config_pss(control_planes: NodeGroup, features_list: str) -> None:
     yaml = ruamel.yaml.YAML()
 
     for control_plane in control_planes.get_ordered_members_list():
         result = control_plane.sudo("cat /etc/kubernetes/manifests/kube-apiserver.yaml")
 
         # update kube-apiserver config with updated features list or delete '--feature-gates' and '--admission-control-config-file'
         conf = yaml.load(list(result.values())[0].stdout)
@@ -765,24 +776,26 @@
     first_control_plane.put(buf, "/tmp/%s.yaml" % filename)
     first_control_plane.sudo("kubectl apply -f /tmp/%s.yaml" % filename)
     first_control_plane.sudo("rm -f /tmp/%s.yaml" % filename)
 
     return final_feature_list
 
 
-def finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     admission_impl = cluster.inventory['rbac']['admission']
 
     if admission_impl == "psp":
         return finalize_inventory_psp(cluster, inventory_to_finalize)
     elif admission_impl == "pss":
         return finalize_inventory_pss(cluster, inventory_to_finalize)
 
+    return inventory_to_finalize
+
 
-def finalize_inventory_pss(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def finalize_inventory_pss(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     if cluster.context.get('initial_procedure') != 'manage_pss':
         return inventory_to_finalize
     procedure_config = cluster.procedure_inventory["pss"]
 
     current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("pss", {})
 
     # merge flags from procedure config and cluster config
@@ -790,42 +803,43 @@
     if "defaults" in procedure_config:
         default_merger.merge(current_config.setdefault("defaults", {}), procedure_config["defaults"])
     if "exemptions" in procedure_config:
         default_merger.merge(current_config.setdefault("exemptions", {}), procedure_config["exemptions"])
 
     return inventory_to_finalize
 
+
 # update PSP/PSS fields in the inventory dumped to cluster_finalized.yaml
-def update_finalized_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def update_finalized_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     if cluster.context.get('initial_procedure') == 'manage_pss':
         current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("pss", {})
         current_config["pod-security"] = cluster.procedure_inventory["pss"].get("pod-security", current_config.get("pod-security", "enabled"))
     elif cluster.context.get('initial_procedure') == 'manage_psp':
         current_config = inventory_to_finalize.setdefault("rbac", {}).setdefault("psp", {})
         current_config["pod-security"] = cluster.procedure_inventory["psp"].get("pod-security", current_config.get("pod-security", "enabled"))
     # remove PSP section from cluster_finalyzed.yaml  
     minor_version = int(inventory_to_finalize["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
-    if minor_version >= 24:
+    if minor_version > 24:
         del inventory_to_finalize["rbac"]["psp"]
 
-
     return inventory_to_finalize
 
-def copy_pss(group: NodeGroup):
-    if  group.cluster.inventory['rbac']['admission'] !=  "pss":
-        return
+
+def copy_pss(group: NodeGroup) -> Optional[RunnersGroupResult]:
+    if  group.cluster.inventory['rbac']['admission'] != "pss":
+        return None
     if group.cluster.context.get('initial_procedure') == 'manage_pss':
         if not is_security_enabled(group.cluster.inventory) and \
                 group.cluster.procedure_inventory["pss"]["pod-security"] != "enabled":
             group.cluster.log.debug("Pod security disabled, skipping pod admission installation...")
-            return
+            return None
     if group.cluster.context.get('initial_procedure') == 'install':
         if not is_security_enabled(group.cluster.inventory):
             group.cluster.log.debug("Pod security disabled, skipping pod admission installation...")
-            return
+            return None
 
     defaults = group.cluster.inventory["rbac"]["pss"]["defaults"]
     exemptions = group.cluster.inventory["rbac"]["pss"]["exemptions"]
     # create admission config from template and cluster.yaml
     admission_config = Template(utils.read_internal(admission_template))\
                        .render(defaults=defaults,exemptions=exemptions)
 
@@ -837,15 +851,15 @@
     group.sudo("mkdir -p %s" % admission_dir, warn=True)
     result = group.sudo("cp %s %s" % (remote_path, admission_path), warn=True)
     group.sudo("rm -f %s" % remote_path)
 
     return result
 
 
-def label_namespace_pss(cluster: KubernetesCluster, manage_type: str):
+def label_namespace_pss(cluster: KubernetesCluster, manage_type: str) -> None:
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     # set/delete labels on predifined plugins namsespaces
     for plugin in cluster.inventory["plugins"]:
         is_install = cluster.inventory["plugins"][plugin].get("install")
         if manage_type in ["apply", "install"]:
             if is_install and plugin in privileged_plugins.keys():
                 # set label 'pod-security.kubernetes.io/enforce: privileged' for local provisioner and ingress namespaces
@@ -920,12 +934,12 @@
                 cluster.log.debug(f"Delete PSS labels on {ns_name} namespace")
                 if isinstance(namespace, dict):
                     for item in list(namespace[ns_name]):
                         first_control_plane.sudo(f"kubectl label ns {ns_name} "
                                     f"pod-security.kubernetes.io/{item}-")
 
 
-def check_inventory(cluster: KubernetesCluster):
+def check_inventory(cluster: KubernetesCluster) -> None:
     # check if 'admission' option in cluster.yaml and procedure.yaml are inconsistent 
     if cluster.context.get('initial_procedure') == 'manage_pss' and cluster.inventory["rbac"]["admission"] != "pss" or \
         cluster.context.get('initial_procedure') == 'manage_psp' and cluster.inventory["rbac"]["admission"] != "psp":
         raise Exception("Procedure config and cluster config are inconsistent. Please check 'admission' option")
```

### Comparing `kubemarine-0.19.0/kubemarine/apparmor.py` & `kubemarine-0.20.0/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/apt.py` & `kubemarine-0.20.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/audit.py` & `kubemarine-0.20.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/controlplane.py` & `kubemarine-0.20.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/__init__.py` & `kubemarine-0.20.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/action.py` & `kubemarine-0.20.0/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/annotations.py` & `kubemarine-0.20.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/cluster.py` & `kubemarine-0.20.0/kubemarine/core/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,18 +78,20 @@
         return NodeGroup(ips, self)
 
     def get_access_address_from_node(self, node: dict) -> str:
         """
         Returns address which should be used to connect to the node via Fabric.
         The address also can be used as unique identifier of the node.
         """
-        address = node.get('connect_to')
-        if address is None:
-            address = node.get('address')
-        if address is None:
+        address: str
+        if node.get('connect_to') is not None:
+            address = node['connect_to']
+        elif node.get('address') is not None:
+            address = node['address']
+        else:
             address = node['internal_address']
 
         return address
 
     def get_nodes_by_names(self, node_names: List[str]) -> List[dict]:
         result = []
         for node in self.inventory["nodes"]:
@@ -200,18 +202,18 @@
         not_accessible = all.exclude_group(accessible)
         not_accessible_online = online.intersection_group(not_accessible)
         if not not_accessible_online.is_empty():
             raise Exception(f"{not_accessible_online.get_hosts()} are not accessible through ssh. "
                             f"Check ssh credentials.")
 
     def get_os_family_for_node(self, host: str) -> str:
-        node_context = self.context['nodes'].get(host)
-        if not node_context or not node_context.get('os', {}).get('family'):
+        os_family: Optional[str] = self.context['nodes'].get(host, {}).get('os', {}).get('family')
+        if os_family is None:
             raise Exception('Node %s do not contain necessary context data' % host)
-        return node_context['os']['family']
+        return os_family
 
     def get_os_family_for_nodes(self, hosts: Iterable[str]) -> str:
         """
         Returns the detected operating system family for hosts.
 
         :return: Detected OS family, possible values: "debian", "rhel", "rhel8", "multiple", "unknown", "unsupported".
         """
@@ -246,26 +248,30 @@
         os_ids = {}
         for host in nodes_check_os.get_hosts():
             os_details = self.context['nodes'][host]['os']
             os_ids[host] = (os_details['family'], os_details['version'])
 
         return os_ids
 
-    def get_associations(self) -> dict:
+    def _get_associations(self, os_family: str) -> Dict[str, dict]:
+        if os_family in ('unknown', 'unsupported', 'multiple'):
+            raise Exception("Failed to get associations for unsupported or multiple OS families")
+
+        associations: dict = self.inventory['services']['packages']['associations'][os_family]
+        return associations
+
+    def get_associations(self) -> Dict[str, dict]:
         """
         Returns association for all packages from inventory for the cluster.
         The method can be used only if cluster has nodes with the same and supported OS family.
         """
-        return self.inventory['services']['packages']['associations'][self.get_os_family()]
+        return self._get_associations(self.get_os_family())
 
     def _get_associations_for_os(self, os_family: str, package: str) -> dict:
-        if os_family in ('unknown', 'unsupported', 'multiple'):
-            raise Exception("Failed to get associations for unsupported or multiple OS families")
-
-        associations = self.inventory['services']['packages']['associations'][os_family].get(package)
+        associations = self._get_associations(os_family).get(package)
         if associations is None:
             raise Exception(f'Failed to get associations for package "{package}"')
 
         return associations
 
     def get_associations_for_node(self, host: str, package: str) -> dict:
         """
```

### Comparing `kubemarine-0.19.0/kubemarine/core/connections.py` & `kubemarine-0.20.0/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/defaults.py` & `kubemarine-0.20.0/kubemarine/core/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
 from importlib import import_module
 from copy import deepcopy
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, Tuple, List
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.errors import KME
 from kubemarine import jinja
 from kubemarine.core import utils, static, log, os
@@ -80,15 +80,15 @@
 }
 
 invalid_node_name_regex = re.compile("[^a-z-.\\d]", re.M)
 escaped_expression_regex = re.compile('({%[\\s*|]raw[\\s*|]%}.*?{%[\\s*|]endraw[\\s*|]%})', re.M)
 jinja_query_regex = re.compile("{{ .* }}", re.M)
 
 
-def apply_defaults(inventory, cluster: KubernetesCluster):
+def apply_defaults(inventory: dict, cluster: KubernetesCluster) -> dict:
     recursive_apply_defaults(supported_defaults, inventory)
 
     for i, node in enumerate(inventory["nodes"]):
         address = cluster.get_access_address_from_node(node)
 
         # we definitely know how to connect
         cluster.inventory["nodes"][i]["connect_to"] = address
@@ -105,15 +105,15 @@
                 cluster.ips[role] = []
             if address not in cluster.ips[role]:
                 cluster.ips[role].append(address)
 
     return inventory
 
 
-def apply_registry(inventory: dict, cluster: KubernetesCluster):
+def apply_registry(inventory: dict, cluster: KubernetesCluster) -> dict:
 
     if not inventory.get('registry'):
         cluster.log.verbose('Unified registry is not used')
         return inventory
 
     thirdparties_address = None
     containerd_endpoints = None
@@ -213,30 +213,30 @@
             config['source'] = source
             if 'sha1' not in config:
                 config['sha1'] = sha1
 
     return inventory
 
 
-def apply_registry_endpoints(inventory: dict):
+def apply_registry_endpoints(inventory: dict) -> Tuple[str, List[str], Optional[str]]:
 
     if not inventory['registry'].get('mirror_registry'):
         inventory['registry']['mirror_registry'] = 'registry.cluster.local'
 
     registry_mirror_address = inventory['registry']['mirror_registry']
 
     # todo Currently registry.endpoints is used only for containerd registry mirrors, but it can be provided explicitly.
     #  Probably we could make endpoints optional in this case.
     containerd_endpoints = inventory['registry']['endpoints']
     thirdparties_address = inventory['registry'].get('thirdparties')
 
     return registry_mirror_address, containerd_endpoints, thirdparties_address
 
 
-def append_controlplain(inventory, cluster: Optional[KubernetesCluster]):
+def append_controlplain(inventory: dict, cluster: Optional[KubernetesCluster]) -> dict:
 
     if inventory.get('control_plain', {}).get('internal') and inventory.get('control_plain', {}).get('external'):
         if cluster:
             cluster.log.verbose('Control plains are set manually, nothing to detect.')
         return inventory
 
     if cluster:
@@ -303,15 +303,15 @@
 
     if not inventory['control_plain'].get('external'):
         inventory['control_plain']['external'] = external_address
 
     return inventory
 
 
-def recursive_apply_defaults(defaults, section):
+def recursive_apply_defaults(defaults: dict, section: dict) -> None:
     for key, value in defaults.items():
         if isinstance(value, dict) and section.get(key) is not None and section[key]:
             recursive_apply_defaults(value, section[key])
         # check if target section exists and not empty
         elif section.get(value) is not None and section[value]:
 
             if isinstance(section[value], list):
@@ -331,15 +331,15 @@
                 section_copy = deepcopy(section[value])
                 for custom_key, custom_value in section_copy.items():
                     # here section['key'] refers to default, not custom value
                     default_value = deepcopy(section[key])
                     section[value][custom_key] = default_merger.merge(default_value, custom_value)
 
 
-def calculate_node_names(inventory: dict, _):
+def calculate_node_names(inventory: dict, _: KubernetesCluster) -> dict:
     roles_iterators: Dict[str, int] = {}
     for i, node in enumerate(inventory['nodes']):
         for role_name in ['control-plane', 'worker', 'balancer']:
             if role_name in node['roles']:
                 # The idea is this:
                 # If the name is already specified, we must skip this node,
                 # however, we must consider that we already have a node of this type
@@ -359,43 +359,44 @@
                 role_i = roles_iterators.get(role_name, 1)
                 roles_iterators[role_name] = role_i + 1
                 if node.get('name') is None:
                     inventory['nodes'][i]['name'] = '%s-%s' % (role_name, role_i)
     return inventory
 
 
-def verify_node_names(inventory: dict, _):
+def verify_node_names(inventory: dict, _: KubernetesCluster) -> dict:
     known_names = []
     for i, node in enumerate(inventory['nodes']):
         node_name = node['name']
         if node_name in known_names:
             raise Exception('Node name %s is duplicated in configfile' % node_name)
         if re.findall(invalid_node_name_regex, node_name):
             raise Exception('Node name \"%s\" contains invalid characters. A DNS-1123 subdomain must consist of lower '
                             'case alphanumeric characters, \'-\' or \'.\'' % node_name)
         known_names.append(node_name)
     return inventory
 
 
-def calculate_nodegroups(inventory: dict, cluster: KubernetesCluster):
+def calculate_nodegroups(inventory: dict, cluster: KubernetesCluster) -> dict:
     for role in cluster.ips.keys():
         cluster.nodes[role] = cluster.make_group(cluster.ips[role])
     return inventory
 
 
-def merge_defaults(inventory: dict, cluster: KubernetesCluster):
+def merge_defaults(inventory: dict, cluster: KubernetesCluster) -> dict:
     base_inventory = deepcopy(static.DEFAULTS)
 
     inventory = default_merger.merge(base_inventory, inventory)
     # it is necessary to temporary put half-compiled inventory to cluster inventory field
     cluster._inventory = inventory
     return inventory
 
 
-def enrich_inventory(cluster: KubernetesCluster, inventory: dict, make_dumps=True, enrichment_functions=None):
+def enrich_inventory(cluster: KubernetesCluster, inventory: dict,
+                     make_dumps: bool = True, enrichment_functions: List[str] = None) -> dict:
     if not enrichment_functions:
         enrichment_functions = DEFAULT_ENRICHMENT_FNS
 
     # run required fields calculation
     for enrichment_fn in enrichment_functions:
         fn_package_name, fn_method_name = enrichment_fn.rsplit('.', 1)
         mod = import_module(fn_package_name)
@@ -408,15 +409,15 @@
         from kubemarine import controlplane
         inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, prepare_for_dump(inventory))
         utils.dump_file(cluster, yaml.dump(inventory_for_dump, ), "cluster.yaml")
 
     return inventory
 
 
-def compile_inventory(inventory: dict, cluster: KubernetesCluster):
+def compile_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
 
     # convert references in yaml to normal values
     iterations = 100
     root = deepcopy(inventory)
     root['globals'] = static.GLOBALS
     root['env'] = os.Environ()
 
@@ -443,15 +444,15 @@
     inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, prepare_for_dump(inventory))
     merged_inventory = yaml.dump(inventory_for_dump)
     utils.dump_file(cluster, merged_inventory, "cluster_precompiled.yaml")
 
     return inventory
 
 
-def compile_object(logger: log.EnhancedLogger, struct: Any, root: dict, ignore_jinja_escapes=True) -> Any:
+def compile_object(logger: log.EnhancedLogger, struct: Any, root: dict, ignore_jinja_escapes: bool = True) -> Any:
     if isinstance(struct, list):
         new_struct = []
         for i, v in enumerate(struct):
             struct[i] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
             # delete empty list entries, which can appear after jinja compilation
             if struct[i] != '':
                 new_struct.append(struct[i])
@@ -462,15 +463,15 @@
     elif isinstance(struct, str) and ('{{' in struct or '{%' in struct):
         struct = compile_string(logger, struct, root, ignore_jinja_escapes=ignore_jinja_escapes)
 
     return struct
 
 
 def compile_string(logger: log.EnhancedLogger, struct: str, root: dict,
-                   ignore_jinja_escapes=True) -> str:
+                   ignore_jinja_escapes: bool = True) -> str:
     logger.verbose("Rendering \"%s\"" % struct)
 
     if ignore_jinja_escapes:
         iterator = escaped_expression_regex.finditer(struct)
         struct = re.sub(escaped_expression_regex, '', struct)
         struct = jinja.new(logger, True, root).from_string(struct).render(**root)
 
@@ -481,27 +482,27 @@
     else:
         struct = jinja.new(logger, True, root).from_string(struct).render(**root)
 
     logger.verbose("\tRendered as \"%s\"" % struct)
     return struct
 
 
-def escape_jinja_characters_for_inventory(cluster: KubernetesCluster, obj):
+def escape_jinja_characters_for_inventory(cluster: KubernetesCluster, obj: Any) -> Any:
     if isinstance(obj, dict):
         for key, value in obj.items():
             obj[key] = escape_jinja_characters_for_inventory(cluster, value)
     elif isinstance(obj, list):
         for key, value in enumerate(obj):
             obj[key] = escape_jinja_characters_for_inventory(cluster, value)
     elif isinstance(obj, str):
         obj = _escape_jinja_character(obj)
     return obj
 
 
-def _escape_jinja_character(value):
+def _escape_jinja_character(value: str) -> str:
     if '{{' in value and '}}' in value and re.search(jinja_query_regex, value):
         matches = re.findall(jinja_query_regex, value)
         for match in matches:
             # TODO: rewrite to correct way of match replacement: now it can cause "{raw}{raw}xxx.." circular bug
             value = value.replace(match, '{% raw %}'+match+'{% endraw %}')
     return value
 
@@ -513,15 +514,15 @@
         dump_inventory = deepcopy(inventory)
     else:
         dump_inventory = inventory
 
     return dump_inventory
 
 
-def manage_true_false_values(inventory: dict, _):
+def manage_true_false_values(inventory: dict, _: KubernetesCluster) -> dict:
     # Check undefined values for plugin.name.install and convert it to bool
     for plugin_name, plugin_item in inventory["plugins"].items():
         # Check install value
         if 'install' not in plugin_item:
             continue
         value = utils.true_or_false(plugin_item.get('install', False))
         if value == 'undefined':
```

### Comparing `kubemarine-0.19.0/kubemarine/core/environment.py` & `kubemarine-0.20.0/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/errors.py` & `kubemarine-0.20.0/kubemarine/core/errors.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/executor.py` & `kubemarine-0.20.0/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/flow.py` & `kubemarine-0.20.0/kubemarine/core/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import argparse
 import os
 import shlex
 import sys
 import time
 from abc import abstractmethod, ABC
 from copy import deepcopy
-from typing import Type, Optional, List, Union, Sequence
+from types import FunctionType
+from typing import Type, Optional, List, Union, Sequence, Tuple, cast, Callable, Dict, Any
 
 from kubemarine.core import utils, cluster as c, action, resources as res, errors, summary, log
 
 DEFAULT_CLUSTER_OBJ: Optional[Type[c.KubernetesCluster]] = None
 TASK_DESCRIPTION_TEMPLATE = """
 tasks list:
     %s
@@ -47,48 +48,48 @@
         else:
             resources = res.DynamicResources(context)
 
         context = resources.context
         args: dict = context['execution_arguments']
 
         try:
-            if not args.get('disable_dump', True):
-                utils.prepare_dump_directory(args.get('dump_location'),
-                                             reset_directory=not args.get('disable_dump_cleanup', False))
+            if not args['disable_dump']:
+                utils.prepare_dump_directory(args['dump_location'],
+                                             reset_directory=not args['disable_dump_cleanup'])
             resources.logger()
             self._run(resources)
         except Exception as exc:
             logger = resources.logger_if_initialized()
             if isinstance(exc, errors.FailException):
-                utils.do_fail(exc.message, exc.reason, exc.hint, log=logger)
+                utils.do_fail(exc.message, exc.reason, exc.hint, logger=logger)
             else:
                 utils.do_fail(f"'{context['initial_procedure'] or 'undefined'}' procedure failed.", exc,
-                              log=logger)
+                              logger=logger)
 
         time_end = time.time()
         logger = resources.logger()
 
         if print_summary:
             summary.schedule_report(resources.working_context, summary.SummaryItem.EXECUTION_TIME,
                                     utils.get_elapsed_string(time_start, time_end))
             summary.print_summary(resources.working_context, logger)
             logger.info("SUCCESSFULLY FINISHED")
 
         return FlowResult(resources.working_context, logger)
 
     @abstractmethod
-    def _run(self, resources: res.DynamicResources):
+    def _run(self, resources: res.DynamicResources) -> None:
         pass
 
 
 class ActionsFlow(Flow):
     def __init__(self, actions: List[action.Action]):
         self._actions = actions
 
-    def _run(self, resources: res.DynamicResources):
+    def _run(self, resources: res.DynamicResources) -> None:
         run_actions(resources, self._actions)
 
 
 def run_actions(resources: res.DynamicResources, actions: Sequence[action.Action]) -> None:
     """
     Runs actions one by one, recreates inventory when necessary,
     managing such resources as cluster object and raw inventory.
@@ -140,35 +141,28 @@
             last_cluster = None
 
     if successfully_performed:
         _post_process_actions_group(last_cluster, context, successfully_performed)
 
 
 def _post_process_actions_group(last_cluster: Optional[c.KubernetesCluster], context: dict,
-                                successfully_performed: list, failed=False):
+                                successfully_performed: list, failed: bool = False) -> None:
     if last_cluster is None:
         return
     try:
         last_cluster.dump_finalized_inventory()
     finally:
         if context['preserve_inventory']:
             last_cluster.context['successfully_performed'] = successfully_performed
             last_cluster.context['status'] = 'failed' if failed else 'successful'
             last_cluster.preserve_inventory()
 
-        # TODO remove in next release
-        if last_cluster.context.get('schema_errors_ignored'):
-            last_cluster.log.warning(
-                "Inventory file is failed to be validated against the schema, "
-                "that was suppressed with --ignore-schema-errors.\n"
-                "See the beginning of the logs for details.\n"
-                "The option will be removed in next release.")
 
-
-def run_tasks(resources: res.DynamicResources, tasks, cumulative_points=None, tasks_filter: list = None):
+def run_tasks(resources: res.DynamicResources, tasks: dict, cumulative_points: dict = None,
+              tasks_filter: list = None) -> None:
     """
     Filters and runs tasks.
     """
 
     if cumulative_points is None:
         cumulative_points = {}
 
@@ -192,27 +186,27 @@
 
     init_tasks_flow(cluster)
     run_tasks_recursive(tasks, final_list, cluster, cumulative_points, [])
     proceed_cumulative_point(cluster, cumulative_points, END_OF_TASKS,
                              force=args.get('force_cumulative_points', False))
 
 
-def create_empty_context(args: dict = None, procedure: str = None):
+def create_empty_context(args: dict = None, procedure: str = None) -> dict:
     if args is None:
         args = {}
     return {
         "execution_arguments": deepcopy(args),
         "nodes": {},
         'initial_procedure': procedure,
         'preserve_inventory': True,
         'runtime_vars': {}
     }
 
 
-def get_task_list(tasks, _task_path=''):
+def get_task_list(tasks: dict, _task_path: str = '') -> List[str]:
     result = []
     for task_name, task in tasks.items():
         __task_path = _task_path + "." + task_name if _task_path != '' else task_name
         result.extend(get_task_list(task, __task_path) if not callable(task) else [__task_path])
     return result
 
 
@@ -233,23 +227,24 @@
 
     context = create_empty_context(args=args, procedure=procedure)
     context["initial_cli_arguments"] = ' '.join(map(shlex.quote, args_list))
 
     return context
 
 
-def filter_flow(tasks, tasks_filter: List[str], excluded_tasks: List[str]):
+def filter_flow(tasks: dict, tasks_filter: List[str], excluded_tasks: List[str]) -> Tuple[dict, List[str]]:
     # Remove any whitespaces from filters, and split by '.'
     tasks_path_filter = [tasks.split(".") for tasks in list(map(str.strip, tasks_filter))]
     excluded_path_tasks = [tasks.split(".") for tasks in list(map(str.strip, excluded_tasks))]
 
     return _filter_flow_internal(tasks, tasks_path_filter, excluded_path_tasks, [])
 
 
-def _filter_flow_internal(tasks, tasks_filter: List[List[str]], excluded_tasks: List[List[str]], _task_path: List[str]):
+def _filter_flow_internal(tasks: dict, tasks_filter: List[List[str]], excluded_tasks: List[List[str]],
+                          _task_path: List[str]) -> Tuple[dict, List[str]]:
     filtered = {}
     final_list = []
 
     for task_name, task in tasks.items():
         __task_path = _task_path + [task_name]
         __task_name = ".".join(__task_path)
 
@@ -279,15 +274,15 @@
         else:
             print("\t%s" % __task_name)
 
     return filtered, final_list
 
 
 def run_tasks_recursive(tasks: dict, final_task_names: List[str], cluster: c.KubernetesCluster,
-                        cumulative_points: dict, _task_path: List[str]):
+                        cumulative_points: dict, _task_path: List[str]) -> None:
     for task_name, task in tasks.items():
         __task_path = _task_path + [task_name]
         __task_name = ".".join(__task_path)
         run = __task_name in final_task_names
 
         args = cluster.context['execution_arguments']
         # --force-cumulative-points forcibly run the point only if the related task is going to be executed
@@ -340,20 +335,14 @@
                         nargs='*',
                         help='Logging options, can be specified multiple times')
 
     parser.add_argument('-w', '--workdir',
                         default='',
                         help='Custom path of the workdir')
 
-    # TODO remove in next release
-    parser.add_argument('--ignore-schema-errors',
-                        action='store_true',
-                        help='Do not stop the run if validation by schema fails. '
-                             'The option will be removed in next release.')
-
     return parser
 
 
 def new_tasks_flow_parser(cli_help: str, tasks: dict = None) -> argparse.ArgumentParser:
     parser = new_common_parser(cli_help)
 
     parser.add_argument('--without-act',
@@ -396,27 +385,28 @@
         parser.add_argument('procedure_config', metavar='procedure_config', type=str, help=help_msg, nargs='?')
     else:
         parser.add_argument('procedure_config', metavar='procedure_config', type=str, help=help_msg)
 
     return parser
 
 
-def parse_args(parser: argparse.ArgumentParser, arguments: list):
+def parse_args(parser: argparse.ArgumentParser, arguments: list) -> argparse.Namespace:
     args = parser.parse_args(arguments)
 
     if args.workdir != '':
         os.chdir(args.workdir)
 
     return args
 
 
-def schedule_cumulative_point(cluster: c.KubernetesCluster, point_method) -> None:
+def schedule_cumulative_point(cluster: c.KubernetesCluster, point_method: Callable) -> None:
     _check_within_flow(cluster)
 
-    point_fullname = point_method.__module__ + '.' + point_method.__qualname__
+    func = cast(FunctionType, point_method)
+    point_fullname = func.__module__ + '.' + func.__qualname__
 
     if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
         cluster.log.verbose('Method %s not scheduled - cumulative points disabled' % point_fullname)
         return
 
     if point_fullname in cluster.context['execution_arguments']['exclude_cumulative_points_methods']:
         cluster.log.verbose('Method %s not scheduled - it set to be excluded' % point_fullname)
@@ -429,19 +419,19 @@
         cluster.context['scheduled_cumulative_points'] = scheduled_points
         cluster.log.verbose('Method %s scheduled' % point_fullname)
     else:
         cluster.log.verbose('Method %s already scheduled' % point_fullname)
 
 
 def proceed_cumulative_point(cluster: c.KubernetesCluster, points_list: dict,
-                             point_task_name: Union[str, object], force=False):
+                             point_task_name: Union[str, object], force: bool = False) -> Dict[str, Any]:
     _check_within_flow(cluster)
 
     if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
-        return
+        return {}
 
     scheduled_methods = cluster.context.get('scheduled_cumulative_points', [])
 
     results = {}
     for point_method, points_tasks_names in points_list.items():
         if point_task_name in points_tasks_names:
 
@@ -458,26 +448,26 @@
             if point_method in scheduled_methods:
                 scheduled_methods.remove(point_method)
             results[point_method_fullname] = call_result
 
     return results
 
 
-def init_tasks_flow(cluster: c.KubernetesCluster):
+def init_tasks_flow(cluster: c.KubernetesCluster) -> None:
     if 'proceeded_tasks' not in cluster.context:
         cluster.context['proceeded_tasks'] = []
 
 
-def add_task_to_proceeded_list(cluster: c.KubernetesCluster, task_path: str):
+def add_task_to_proceeded_list(cluster: c.KubernetesCluster, task_path: str) -> None:
     if not is_task_completed(cluster, task_path):
         cluster.context['proceeded_tasks'].append(task_path)
         utils.dump_file(cluster, "\n".join(cluster.context['proceeded_tasks'])+"\n", 'finished_tasks')
 
 
 def is_task_completed(cluster: c.KubernetesCluster, task_path: str) -> bool:
     _check_within_flow(cluster)
     return task_path in cluster.context['proceeded_tasks']
 
 
-def _check_within_flow(cluster: c.KubernetesCluster, check=True):
+def _check_within_flow(cluster: c.KubernetesCluster, check: bool = True) -> None:
     if check != ('proceeded_tasks' in cluster.context):
         raise NotImplementedError(f"The method is called {'not ' if check else ''}within tasks flow execution")
```

### Comparing `kubemarine-0.19.0/kubemarine/core/group.py` & `kubemarine-0.20.0/kubemarine/core/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,24 +48,27 @@
     def __len__(self) -> int:
         return len(self._result)
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._result)
 
     def get_simple_out(self) -> str:
+        return self.get_simple_result().stdout
+
+    def get_simple_result(self) -> RunnersResult:
         if len(self) != 1:
-            raise NotImplementedError("Simple output can be returned only for NodeGroupResult consisted of "
+            raise NotImplementedError("Simple result can be returned only for NodeGroupResult consisted of "
                                       "exactly one node, but %s were provided." % list(self.keys()))
 
         res = list(self.values())[0]
         if not isinstance(res, RunnersResult):
             raise NotImplementedError("It does not make sense to return simple output for result of type %s"
                                       % type(res))
 
-        return res.stdout
+        return res
 
     def __str__(self) -> str:
         host_outputs = []
         for host, result in self.items():
             output = f"{host}:"
 
             if isinstance(result, RunnersResult):
```

### Comparing `kubemarine-0.19.0/kubemarine/core/log.py` & `kubemarine-0.20.0/kubemarine/core/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 import sys
 from abc import ABC, abstractmethod
 
 from pygelf import gelf, GelfTcpHandler, GelfUdpHandler, GelfTlsHandler, GelfHttpHandler  # type: ignore[import]
 
 from copy import deepcopy
-from typing import Any, List, Optional, cast, Dict
+from typing import Any, List, Optional, cast, Dict, Union
 
 VERBOSE = 5
 gelf.LEVELS.update({VERBOSE: 8})
 
 DEFAULT_FORMAT = '%(asctime)s %(name)s %(levelname)s %(message)s'
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
@@ -83,23 +83,23 @@
 class VerboseLogger(ABC):
     @abstractmethod
     def verbose(self, msg: object, *args: object, **kwargs: Any) -> None:
         pass
 
 
 class EnhancedLogger(logging.Logger, VerboseLogger):
-    def __init__(self, name, level=logging.NOTSET):
+    def __init__(self, name: str, level: int = logging.NOTSET):
         super().__init__(name, level)
         logging.addLevelName(VERBOSE, 'VERBOSE')
 
     def verbose(self, msg: object, *args: object, **kwargs: Any) -> None:
         if self.isEnabledFor(VERBOSE):
             self._log(VERBOSE, msg, args, **kwargs)
 
-    def makeRecord(self, name: str, level: int, fn: str, lno: int, msg: object, args,
+    def makeRecord(self, name: str, level: int, fn: str, lno: int, msg: object, args,  # type: ignore[no-untyped-def]
                    exc_info, func=None, extra=None,
                    sinfo=None) -> logging.LogRecord:
         record = super().makeRecord(name, level, fn, lno, msg, args, exc_info, func, extra, sinfo)
         caller = record.__dict__.get('real_caller')
         if caller is not None:
             record.__dict__.update(record.__dict__.pop('real_caller'))
 
@@ -116,26 +116,27 @@
 
 
 logging.setLoggerClass(EnhancedLogger)
 logging.setLogRecordFactory(EnhancedLogRecord)
 
 
 class LogFormatter(logging.Formatter):
-    def __init__(self, fmt=None, datefmt=None, style='%', colorize=False, correct_newlines=False):
-        super().__init__(fmt, datefmt, style)
+    def __init__(self, fmt: str = None, datefmt: str = None,
+                 colorize: bool = False, correct_newlines: bool = False):
+        super().__init__(fmt, datefmt)
         self.colorize = colorize
         self.correct_newlines = correct_newlines
 
-    def _format(self, record):
+    def _format(self, record: logging.LogRecord) -> str:
         s = super().format(record)
         if self.colorize and record.levelname in COLORS_SCHEME:
             s = COLORS[COLORS_SCHEME[record.levelname]] + s + COLORS['RESET']
         return s
 
-    def format(self, record):
+    def format(self, record: logging.LogRecord) -> str:
         if self.correct_newlines:
             messages = str(record.msg).split('\n')
             if len(messages) == 1:
                 return self._format(record)
         else:
             return self._format(record)
 
@@ -153,37 +154,38 @@
 
 
 class StdoutHandler(logging.StreamHandler):
     def __init__(self, formatter: LogFormatter):
         super().__init__(sys.stdout)
         self.formatter: LogFormatter = formatter
 
-    def emit(self, record):
+    def emit(self, record: logging.LogRecord) -> None:
         if 'ignore_stdout' in record.__dict__:
             return
         super().emit(record)
         # TODO: if output stuck, then add here self.flush()
         # More about, see at https://stackoverflow.com/questions/16633911
 
 
 class FileHandlerWithHeader(logging.FileHandler):
-    def __init__(self, formatter: LogFormatter, filename, header=None, mode='a', encoding=None):
+    def __init__(self, formatter: LogFormatter, filename: str, header: str = None,
+                 mode: str = 'a', encoding: str = None):
         # Store the header information.
         self.header = header
 
         # Call the parent __init__
         logging.FileHandler.__init__(self, filename, mode, encoding)
 
         # Write the header if it was specified
         if header:
             self.stream.write('%s\n' % header)
 
         self.formatter: LogFormatter = formatter
 
-    def emit(self, record):
+    def emit(self, record: logging.LogRecord) -> None:
         # Call the parent class emit function.
         logging.FileHandler.emit(self, record)
 
 
 class LogHandler:
 
     def __init__(self,
@@ -191,15 +193,15 @@
                  level: str,
                  colorize: bool = False,
                  correct_newlines: bool = False,
                  filemode: str = 'a',
                  format: str = DEFAULT_FORMAT,
                  datefmt: str = None,
                  header: str = None,
-                 **kwargs):
+                 **kwargs: Union[str, bool, int]):
 
         self._colorize = colorize
         self._correct_newlines = correct_newlines
         self._format = format
         self._datefmt = datefmt
         self._header = header
 
@@ -215,15 +217,15 @@
             self._target = 'graylog'
             if not kwargs.get('host'):
                 raise Exception('Graylog host is not defined')
             if not kwargs.get('port'):
                 raise Exception(f'Graylog port is not defined for "{kwargs["host"]}"')
             if not kwargs.get('type'):
                 raise Exception(f'Graylog type is not defined for "{kwargs["host"]}:{kwargs["port"]}"')
-            handler_options = {
+            handler_options: Dict[str, Union[str, bool, int, None]] = {
                 'host': kwargs['host'],
                 'port': kwargs['port'],
                 '_app_name': kwargs.get('appname', 'kubemarine'),
                 'debug': kwargs.get('debug', False),
                 'version': kwargs.get('version', '1.1')
             }
             if kwargs['type'] == 'tcp':
@@ -254,27 +256,27 @@
             self.handler = FileHandlerWithHeader(self._formatter, self._target, mode=filemode, header=self._header, encoding='utf-8')
 
         if level not in LOGGING_LEVELS_BY_NAME:
             raise Exception(f'Failed to create logger - unknown logging level: "{level}"')
         self._level = LOGGING_LEVELS_BY_NAME[level]
         self.handler.setLevel(self._level)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'target: {self._target}, level: {LOGGING_NAMES_BY_LEVEL[self._level]}, colorize: {self._colorize}, datefmt: {self._datefmt}, format: {self._format}'
 
-    def append_to_logger(self, logger) -> None:
+    def append_to_logger(self, logger: EnhancedLogger) -> None:
         logger.addHandler(self.handler)
 
     def has_stdout_target(self) -> bool:
         return self._target == 'stdout'
 
 
 class Log:
 
-    def __init__(self, raw_inventory, handlers: List[LogHandler]):
+    def __init__(self, raw_inventory: dict, handlers: List[LogHandler]):
         logger = logging.getLogger(raw_inventory.get('cluster_name', 'cluster.local'))
         self._logger = cast(EnhancedLogger, logger)
         self._logger.setLevel(VERBOSE)
 
         if self._logger.hasHandlers():
             self._logger.handlers.clear()
 
@@ -323,39 +325,45 @@
     :param argument: Raw CLI argument string. For example: test.log;level=verbose;colorize=true
     :return: Initialized LogHandler
     """
     parameters: Dict[str, Any] = {}
     argument_parts = argument.split(';')
     if not argument_parts:
         raise Exception('Defined logger do not contain parameters')
-    parameters['target'] = argument_parts[0]
+    target = argument_parts[0]
+    level: Optional[str] = None
     for parameter in argument_parts[1:]:
         if parameter == '':
             continue
-        value: Any
+        value: Union[str, bool, int]
         key, value, *rest = parameter.split('=')
-        if key in ['colorize', 'correct_newlines', 'debug', 'compress', 'validate']:
-            value = value.lower() in ['true', '1']
-        elif key in ['chunk_size', 'timeout', 'port']:
-            value = int(value)
-        parameters[key] = value
-    if not parameters.get('level'):
-        raise Exception(f'Logging level is not set for logger "{parameters["target"]}"')
-    return LogHandler(**parameters)
+        if key == 'level':
+            level = value
+        else:
+            if key in ['colorize', 'correct_newlines', 'debug', 'compress', 'validate']:
+                value = value.lower() in ['true', '1']
+            elif key in ['chunk_size', 'timeout', 'port']:
+                value = int(value)
+
+            parameters[key] = value
+
+    if level is None:
+        raise Exception(f'Logging level is not set for logger "{target}"')
+    return LogHandler(target, level, **parameters)
 
 
 def get_dump_debug_filepath(context: dict) -> Optional[str]:
     args = context['execution_arguments']
-    if args.get('disable_dump', True):
+    if args['disable_dump']:
         return None
 
     return os.path.join(args['dump_location'], 'dump', 'debug.log')
 
 
-def init_log_from_context_args(globals, context, raw_inventory) -> Log:
+def init_log_from_context_args(globals: dict, context: dict, raw_inventory: dict) -> Log:
     """
     Create Log from raw CLI arguments in Cluster context
     :param globals: parsed globals collection
     :param context: context holding execution arguments.
     :param raw_inventory: parsed but not yet enriched inventory
     :return: Initialized Log, based on all parsed logging arguments
     """
```

### Comparing `kubemarine-0.19.0/kubemarine/core/os.py` & `kubemarine-0.20.0/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/patch.py` & `kubemarine-0.20.0/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/resources.py` & `kubemarine-0.20.0/kubemarine/core/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 logger.info(msg)
         try:
             data = utils.read_external(self.inventory_filepath)
             self._raw_inventory = yaml.safe_load(data)
             # load inventory as ruamel.yaml to save original structure
             self._formatted_inventory = utils.yaml_structure_preserver().load(data)
         except (yaml.YAMLError, ruamel.yaml.YAMLError) as exc:
-            utils.do_fail("Failed to load inventory file", exc, log=logger)
+            utils.do_fail("Failed to load inventory file", exc, logger=logger)
 
     def make_final_inventory(self) -> None:
         self._formatted_inventory = utils.get_final_inventory(self.cluster(), initial_inventory=self.formatted_inventory())
 
     def recreate_inventory(self) -> None:
         """
         Recreates initial inventory file using DynamicResources.formatted_inventory and resets all dynamic resources.
```

### Comparing `kubemarine-0.19.0/kubemarine/core/schema.py` & `kubemarine-0.20.0/kubemarine/core/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,19 +55,15 @@
 
     errs = list(validator.iter_errors(inventory))
     if not errs:
         return
 
     context = cluster.context
     logger = cluster.log
-    # TODO remove in next release
-    ignore_schema_errors = context['execution_arguments']['ignore_schema_errors']
-
-    log_method = logger.warning if ignore_schema_errors else logger.error
-    log_method(f"Inventory file{for_procedure} is failed to be validated against the schema.")
+    logger.error(f"Inventory file{for_procedure} is failed to be validated against the schema.")
 
     errs = _resolve_errors(errs)
     for err in errs:
         logger.verbose("------------------------------------------")
         logger.verbose(_verbose_msg(validator, err))
 
     debug_filepath = log.get_dump_debug_filepath(context)
@@ -79,22 +75,14 @@
     version = utils.get_version()
     public_schema = f"https://raw.githubusercontent.com/Netcracker/KubeMarine/{version}/kubemarine/{root_schema_resource}"
     hint = f"Inventory file{for_procedure} has incorrect format. {detailed_msg}\n" \
            f"To validate the file manually, you can use JSON schema {root_schema_uri}\n" \
            f"or its public alternative {public_schema}\n"
 
     msg = _error_msg(validator, errs[0])
-    if ignore_schema_errors:
-        context['schema_errors_ignored'] = True
-        logger.warning(msg + "\n\n" + hint)
-        return
-    else:
-        hint += f"If you are sure that the file is correct, please contact support,\n" \
-                f"and use --ignore-schema-errors to proceed (option will be removed in next release).\n"
-
     raise errors.FailException(msg, hint=hint)
 
 
 def _resolve_errors(errs: List[jsonschema.ValidationError]) -> List[jsonschema.ValidationError]:
     key = _extended_relevance()
     for error in errs:
         _unnest_errors(error)
```

### Comparing `kubemarine-0.19.0/kubemarine/core/static.py` & `kubemarine-0.20.0/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/summary.py` & `kubemarine-0.20.0/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/core/utils.py` & `kubemarine-0.20.0/kubemarine/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,63 +16,72 @@
 import json
 import os
 import shutil
 import sys
 import time
 import tarfile
 
-from typing import Tuple, Callable, List, IO
+from typing import Tuple, Callable, List, TextIO, cast, Union, TypeVar
 
 import yaml
 import ruamel.yaml
 from copy import deepcopy
 from datetime import datetime
 from collections import OrderedDict
 
 from ruamel.yaml import CommentedMap
+from typing_extensions import Protocol
 
+from kubemarine.core import log
 from kubemarine.core.errors import pretty_print_error
 
 
-def do_fail(message='', reason: Exception = None, hint='', log=None):
+_T_contra = TypeVar("_T_contra", contravariant=True)
 
-    if not log:
+
+class SupportsDunderLT(Protocol[_T_contra]):
+    def __lt__(self, __other: _T_contra) -> bool: ...
+
+
+def do_fail(message: str = '', reason: Exception = None, hint: str = '', logger: log.EnhancedLogger = None) -> None:
+
+    if not logger:
         sys.stderr.write("\033[91m")
 
-    pretty_print_error(message, reason, log)
+    pretty_print_error(message, reason, logger)
 
     # Please do not rewrite this to logging approach:
     # hint should be visible only in stdout and without special formatting
     if hint != "":
         sys.stderr.write("\n")
         sys.stderr.write(hint + "\n")
 
-    if not log:
+    if not logger:
         sys.stderr.write("\033[0m")
 
     sys.exit(1)
 
 
-def get_elapsed_string(start, end):
+def get_elapsed_string(start: float, end: float) -> str:
     elapsed = end - start
     hours, remainder = divmod(elapsed, 3600)
     minutes, seconds = divmod(remainder, 60)
     return '{:02}h {:02}m {:02}s'.format(int(hours), int(minutes), int(seconds))
 
 
-def prepare_dump_directory(location, reset_directory=True):
+def prepare_dump_directory(location: str, reset_directory: bool = True) -> None:
     dumpdir = os.path.join(location, 'dump')
     if reset_directory and os.path.exists(dumpdir) and os.path.isdir(dumpdir):
         shutil.rmtree(dumpdir)
     os.makedirs(dumpdir, exist_ok=True)
 
 
-def make_ansible_inventory(location, c):
+def make_ansible_inventory(location: str, c: object) -> None:
     from kubemarine.core.cluster import KubernetesCluster
-    cluster: KubernetesCluster = c
+    cluster = cast(KubernetesCluster, c)
 
     inventory = get_final_inventory(cluster)
     roles = []
     for node in inventory['nodes']:
         for role in node['roles']:
             if role not in roles:
                 roles.append(role)
@@ -146,21 +155,21 @@
         for string in strings:
             config_compiled += '\n' + string
         config_compiled += '\n\n'
 
     dump_file({}, config_compiled, location, dump_location=False)
 
 
-def get_current_timestamp_formatted():
+def get_current_timestamp_formatted() -> str:
     return datetime.now().strftime("%Y%m%d-%H%M%S")
 
 
-def get_final_inventory(c, initial_inventory=None):
+def get_final_inventory(c: object, initial_inventory: dict = None) -> dict:
     from kubemarine.core.cluster import KubernetesCluster
-    cluster: KubernetesCluster = c
+    cluster = cast(KubernetesCluster, c)
 
     if initial_inventory is None:
         inventory = deepcopy(cluster.inventory)
     else:
         inventory = deepcopy(initial_inventory)
 
     from kubemarine import admission, kubernetes, packages, plugins, thirdparties
@@ -181,61 +190,66 @@
 
     for finalize_fn in inventory_finalize_functions:
         inventory = finalize_fn(cluster, inventory)
 
     return inventory
 
 
-def merge_vrrp_ips(procedure_inventory, inventory):
+def merge_vrrp_ips(procedure_inventory: dict, inventory: dict) -> None:
     if "vrrp_ips" in inventory and len(inventory["vrrp_ips"]) > 0:
         raise Exception("vrrp_ips section already defined, merging not supported yet")
     else:
         inventory["vrrp_ips"] = procedure_inventory["vrrp_ips"]
 
     if isinstance(inventory, OrderedDict):
         inventory.move_to_end("vrrp_ips", last=False)
 
 
-def dump_file(context, data: object, filename: str,
-              *, dump_location=True):
+def dump_file(context: Union[dict, object], data: Union[TextIO, str], filename: str,
+              *, dump_location: bool = True) -> None:
     if dump_location:
         if not isinstance(context, dict):
             # cluster is passed instead of the context directly
-            cluster = context
+            from kubemarine.core.cluster import KubernetesCluster
+            cluster = cast(KubernetesCluster, context)
             context = cluster.context
 
         args = context['execution_arguments']
-        if args.get('disable_dump', True) \
+        if args['disable_dump'] \
                 and not (filename in ClusterStorage.PRESERVED_DUMP_FILES and context['preserve_inventory']):
             return
 
-        prepare_dump_directory(args.get('dump_location'), reset_directory=False)
+        prepare_dump_directory(args['dump_location'], reset_directory=False)
         target_path = get_dump_filepath(context, filename)
     else:
         target_path = get_external_resource_path(filename)
 
     if isinstance(data, io.StringIO):
-        data = data.getvalue()
-    if isinstance(data, io.TextIOWrapper):
-        data = data.read()
+        text = data.getvalue()
+    elif isinstance(data, str):
+        text = data
+    else:
+        text = data.read()
 
     with open_utf8(target_path, 'w') as file:
-        file.write(data)
+        file.write(text)
 
 
-def get_dump_filepath(context, filename):
+def get_dump_filepath(context: dict, filename: str) -> str:
     if context.get("dump_filename_prefix"):
         filename = f"{context['dump_filename_prefix']}_{filename}"
 
     return get_external_resource_path(os.path.join(context['execution_arguments']['dump_location'], 'dump', filename))
 
 
-def wait_command_successful(g, command, retries=15, timeout=5, warn=True, hide=False):
+def wait_command_successful(g: object, command: str,
+                            retries: int = 15, timeout: int = 5,
+                            warn: bool = True, hide: bool = False) -> None:
     from kubemarine.core.group import NodeGroup
-    group: NodeGroup = g
+    group = cast(NodeGroup, g)
 
     log = group.cluster.log
 
     while retries > 0:
         log.debug("Waiting for command to succeed, %s retries left" % retries)
         result = group.sudo(command, warn=warn, hide=hide)
         exit_code = list(result.values())[0].exited
@@ -243,23 +257,23 @@
             log.debug("Command succeeded")
             return
         retries = retries - 1
         time.sleep(timeout)
     raise Exception("Command failed")
 
 
-def open_utf8(path: str, mode='r') -> IO:
-    return open(path, mode + 't', encoding='utf-8')
+def open_utf8(path: str, mode: str = 'r') -> TextIO:
+    return cast(TextIO, open(path, mode + 't', encoding='utf-8'))
 
 
-def open_internal(path: str, mode: str = 'r') -> IO:
+def open_internal(path: str, mode: str = 'r') -> TextIO:
     return open_utf8(get_internal_resource_path(path), mode)
 
 
-def open_external(path: str, mode: str = 'r') -> IO:
+def open_external(path: str, mode: str = 'r') -> TextIO:
     return open_utf8(get_external_resource_path(path), mode)
 
 
 def read_internal(path: str) -> str:
     with open_internal(path) as f:
         return f.read()
 
@@ -349,33 +363,34 @@
     :return: boolean flag if the list is sorted
     """
     if key is None:
         key = lambda x: x
     return all(key(l[i]) <= key(l[i + 1]) for i in range(len(l) - 1))
 
 
-def map_sorted(map_: CommentedMap, key: Callable = None) -> CommentedMap:
+def map_sorted(map_: CommentedMap, key: Callable[[str], SupportsDunderLT] = None) -> CommentedMap:
     """
     Check that the specified CommentedMap is sorted, or create new sorted map from it otherwise.
 
     :param map_: CommentedMap instance to check
     :param key: custom key function to customize the sort order of the map keys
     :return: the same or new sorted instance of the map
     """
-    if key is None:
-        _key = lambda x: x
-    else:
+    if key is not None:
         _key = key
+    else:
+        _key = lambda x: x
     map_keys = list(map_)
     if not is_sorted(map_keys, key=_key):
         map_ = CommentedMap(sorted(map_.items(), key=lambda item: _key(item[0])))
 
     return map_
 
-def insert_map_sorted(map_: CommentedMap, k, v, key: Callable = None) -> None:
+
+def insert_map_sorted(map_: CommentedMap, k: str, v: object, key: Callable = None) -> None:
     """
     Insert new item to the CommentedMap or update the value for the existing key.
     The map should be already sorted.
 
     :param map_: sorted CommentedMap instance
     :param k: new key
     :param v: new value
@@ -391,39 +406,40 @@
     pos = max((mi + 1 for mi, mv in enumerate(map_)
                if key(mv) < key(k)),
               default=0)
 
     map_.insert(pos, k, v)
 
 
-def load_yaml(filepath) -> dict:
+def load_yaml(filepath: str) -> dict:
     try:
         with open_utf8(filepath, 'r') as stream:
-            return yaml.safe_load(stream)
+            data: dict = yaml.safe_load(stream)
+            return data
     except yaml.YAMLError as exc:
         do_fail(f"Failed to load {filepath}", exc)
         return {}  # unreachable
 
 
-def true_or_false(value) -> str:
+def true_or_false(value: Union[str, bool]) -> str:
     """
     The method check string and boolean value
     :param value: Value that should be checked
     """
     input_string = str(value)
     if input_string in ['true', 'True', 'TRUE']:
         result = "true"
     elif input_string in ['false', 'False', 'FALSE']:
         result = "false"
     else:
         result = "undefined"
     return result
 
 
-def get_version_filepath():
+def get_version_filepath() -> str:
     return get_internal_resource_path("version")
 
 
 def get_version() -> str:
     return read_internal(get_version_filepath()).strip()
 
 
@@ -478,33 +494,33 @@
     3- Uploading dumps to nodes
     4- Copying dumps to new nodes
     """
 
     PRESERVED_DUMP_FILES = ['procedure.yaml', 'procedure_parameters', 'cluster_precompiled.yaml',
                             'cluster.yaml','cluster_initial.yaml', 'cluster_finalized.yaml']
 
-    def __init__(self, cluster):
+    def __init__(self, cluster: object):
         from kubemarine.core.cluster import KubernetesCluster
-        self.cluster: KubernetesCluster = cluster
+        self.cluster = cast(KubernetesCluster, cluster)
         self.dir_path = "/etc/kubemarine/procedures/"
         self.dir_name = ''
         self.dir_location = ''
 
-    def make_dir(self):
+    def make_dir(self) -> None:
         """
         This method creates a directory in which logs about operations on the cluster will be stored.
         """
         readable_timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         initial_procedure = self.cluster.context["initial_procedure"]
         self.dir_name = readable_timestamp + "_" + initial_procedure + "/"
         self.dir_location = self.dir_path + self.dir_name
         self.cluster.nodes['control-plane'].get_final_nodes().sudo(f"mkdir -p {self.dir_location} ; sudo rm {self.dir_path + 'latest_dump'} ;"
                                                  f" sudo ln -s {self.dir_location} {self.dir_path + 'latest_dump'}")
 
-    def rotation_file(self):
+    def rotation_file(self) -> None:
         """
         This method packs files with logs and maintains a structured storage of logs on the cluster.
         """
         not_pack_file = self.cluster.inventory['procedure_history']['archive_threshold']
         delete_old = self.cluster.inventory['procedure_history']['delete_threshold']
 
         command = f'ls {self.dir_path} | grep -v latest_dump'
@@ -519,15 +535,15 @@
                         if 'tar.gz' not in file:
                             control_plane.sudo(
                                 f'tar -czvf {self.dir_path + file + ".tar.gz"} {self.dir_path + file} &&'
                                 f'sudo rm -r {self.dir_path + file}')
                     elif i >= delete_old:
                         control_plane.sudo(f'rm -rf {self.dir_path + file}')
 
-    def compress_and_upload_archive(self):
+    def compress_and_upload_archive(self) -> None:
         """
         This method compose dump files and sends the collected files to the nodes.
         """
         context = self.cluster.context
         archive = get_dump_filepath(context, "local.tar.gz")
         with tarfile.open(archive, "w:gz") as tar:
             for name in ClusterStorage.PRESERVED_DUMP_FILES:
@@ -538,30 +554,30 @@
             tar.add(get_version_filepath(), 'version')
 
         self.cluster.log.debug('Uploading archive with preserved information about the procedure.')
         self.cluster.nodes['control-plane'].get_final_nodes().put(archive, self.dir_location + 'local.tar.gz', sudo=True)
         self.cluster.nodes['control-plane'].get_final_nodes().sudo(f'tar -C {self.dir_location} -xzv --no-same-owner -f {self.dir_location + "local.tar.gz"}  && '
                                                  f'sudo rm -f {self.dir_location + "local.tar.gz"} ')
 
-    def collect_procedure_info(self):
+    def collect_procedure_info(self) -> None:
         """
         This method collects information about the type of procedure and the version of the tool we are working with.
         """
         context = self.cluster.context
         out = dict()
         out['arguments'] = context['initial_cli_arguments']
         if 'proceeded_tasks' in context:
             out['finished_tasks'] = context['proceeded_tasks']
         out["initial_procedure"] = context["initial_procedure"]
         out["successfully_performed"] = context["successfully_performed"]
         out['status'] = context['status']
         output = yaml.dump(out)
         dump_file(context, output, "procedure_parameters")
 
-    def upload_info_new_control_planes(self):
+    def upload_info_new_control_planes(self) -> None:
         """
         This method is used to transfer backup logs from the initial control-plane to the new control-planes.
         """
         new_control_planes = self.cluster.nodes['control-plane'].get_new_nodes()
         if new_control_planes.is_empty():
             return
```

### Comparing `kubemarine-0.19.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.20.0/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/coredns.py` & `kubemarine-0.20.0/kubemarine/coredns.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Any, Dict, Tuple
 
 import yaml
 
 from kubemarine import system
 from kubemarine.core import utils
 
 import io
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import RunnersGroupResult
 
 
-def proceed_section_keyvalue(data, tabsize):
+def proceed_section_keyvalue(data: Dict[str, Any], tabsize: int) -> str:
     tab = " "*tabsize
     config = ''
 
     for key, value in data.items():
         if isinstance(value, bool):
             if value:
                 config += '\n' + tab + '%s' % key
@@ -48,74 +48,72 @@
             config += generate_nested_sections(key, value, tabsize)
             continue
         raise Exception('Unknown type of field in coredns services')
 
     return config
 
 
-def generate_nested_sections(type, data, tabsize):
+def generate_nested_sections(type: str, data: Dict[str, Dict[str, Any]], tabsize: int) -> str:
     tab = " "*tabsize
     config = ''
 
     max_priority = 0
     for section_name, section_value in data.items():
         if section_value.get('priority') is not None and section_value['priority'] > max_priority:
             max_priority = section_value['priority']
 
     iterated = 0
-    sections = []
+    sections: List[Tuple[str, int]] = []
     for section_name, section_value in data.items():
         if section_value.get('priority') is None:
             iterated += 1
             section_priority = max_priority + iterated
         else:
             section_priority = section_value['priority']
 
         if section_value.get('enabled', True) in ['1', 1, True, 'True']:
-            sections.append({
-                'name': section_name,
-                'priority': section_priority
-            })
+            sections.append((section_name, section_priority))
 
-    sections = sorted(sections, key=lambda i: i['priority'])
+    sections = sorted(sections, key=lambda i: i[1])
 
     for section in sections:
-
+        section_name, _ = section
+        section_value = data[section_name]
         if type == 'kubernetes':
             config += '\n' + tab + type
-            if data[section['name']].get('zone'):
-                if isinstance(data[section['name']]['zone'], list):
-                    data[section['name']]['zone'] = ' '.join(data[section['name']]['zone'])
-                config += ' ' + data[section['name']]['zone']
-            config += ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2) + '\n' + tab + '}'
+            if section_value.get('zone'):
+                if isinstance(section_value['zone'], list):
+                    section_value['zone'] = ' '.join(section_value['zone'])
+                config += ' ' + section_value['zone']
+            config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
         elif type == 'hosts':
             config += '\n' + tab + type
-            if data[section['name']].get('file') and isinstance(data[section['name']]['file'], str):
-                config += ' ' + data[section['name']]['file']
-            config += ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2) + '\n' + tab + '}'
+            if section_value.get('file') and isinstance(section_value['file'], str):
+                config += ' ' + section_value['file']
+            config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
         elif type == 'template':
             zones: Union[str, List[Optional[str]]] = [None]
-            if data[section['name']].get('zone'):
-                zones = data[section['name']]['zone']
+            if section_value.get('zone'):
+                zones = section_value['zone']
                 if isinstance(zones, str):
                     zones = [zones]
             for zone in zones:
                 config += '\n' + tab + type
-                if data[section['name']].get('class'):
-                    config += ' ' + data[section['name']]['class']
-                if data[section['name']].get('type'):
-                    config += ' ' + data[section['name']]['type']
+                if section_value.get('class'):
+                    config += ' ' + section_value['class']
+                if section_value.get('type'):
+                    config += ' ' + section_value['type']
                 if zone:
                     config += ' ' + zone
-                config += ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2) + '\n' + tab + '}'
+                config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
         else:
-            config += '\n' + tab + type + ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2)\
+            config += '\n' + tab + type + ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2)\
                       + '\n' + tab + '}'
 
     return config
 
 
 def generate_configmap(inventory: dict) -> str:
     # coredns.configmap.Hosts must exist even if it's empty
```

### Comparing `kubemarine-0.19.0/kubemarine/cri/__init__.py` & `kubemarine-0.20.0/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/cri/containerd.py` & `kubemarine-0.20.0/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/cri/docker.py` & `kubemarine-0.20.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/demo.py` & `kubemarine-0.20.0/kubemarine/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import argparse
 import io
 import re
 import threading
 import time
 from abc import ABC
 from copy import deepcopy
-from typing import List, Dict, Union, Any, Optional, Mapping, Iterable, IO
+from typing import List, Dict, Union, Any, Optional, Mapping, Iterable, IO, Tuple
 
 import fabric  # type: ignore[import]
 import invoke
 
 from kubemarine import system
 from kubemarine.core.cluster import KubernetesCluster, _AnyConnectionTypes
 from kubemarine.core import flow, connections, static
@@ -38,24 +38,24 @@
 from kubemarine.core.resources import DynamicResources
 
 _ShellResult = Dict[str, Any]
 _ROLE_SPEC = Union[int, List[str]]
 
 
 class FakeShell:
-    def __init__(self):
+    def __init__(self) -> None:
         self.results: Dict[str, List[_ShellResult]] = {}
         self.history: Dict[str, List[_ShellResult]] = {}
         self._lock = threading.Lock()
 
-    def reset(self):
+    def reset(self) -> None:
         self.results = {}
         self.history = {}
 
-    def add(self, results: Mapping[str, GenericResult], do_type, args, usage_limit=0):
+    def add(self, results: Mapping[str, GenericResult], do_type: str, args: List[str], usage_limit: int = 0) -> None:
         args.sort()
 
         for host, result in results.items():
             result = {
                 'result': result,
                 'do_type': do_type,
                 'args': args,
@@ -63,19 +63,17 @@
             }
 
             if usage_limit > 0:
                 result['usage_limit'] = usage_limit
 
             self.results.setdefault(host, []).append(result)
 
-    def find(self, host: str, do_type, args, kwargs) -> GenericResult:
+    def find(self, host: str, do_type: str, args: List[str]) -> Optional[GenericResult]:
         # TODO: Support kwargs
         with self._lock:
-            if isinstance(args, tuple):
-                args = list(args)
             results = self.results.get(host, [])
             for i, item in enumerate(results):
                 if item['do_type'] == do_type and item['args'] == args:
                     history_found = any(history_item is item for history_item in self.history.get(host, []))
                     if not history_found:
                         self.history.setdefault(host, []).append(item)
 
@@ -84,70 +82,67 @@
                         item['usage_limit'] -= 1
                         if item['usage_limit'] < 1:
                             del results[i]
                     return item['result']
             return None
 
     # covered by test.test_demo.TestFakeShell.test_calculate_calls
-    def history_find(self, host: str, do_type, args):
+    def history_find(self, host: str, do_type: str, args: List[str]) -> List[_ShellResult]:
         # TODO: Support kwargs
         result = []
-        if isinstance(args, tuple):
-            args = list(args)
         for item in self.history.get(host, []):
             if item['do_type'] == do_type and item['args'] == args:
                 result.append(item)
         return result
 
-    def is_called_each(self, hosts: List[str], do_type: str, args: list) -> bool:
+    def is_called_each(self, hosts: List[str], do_type: str, args: List[str]) -> bool:
         return all((self.is_called(host, do_type, args) for host in hosts))
 
-    def is_called(self, host: str, do_type: str, args: list) -> bool:
+    def is_called(self, host: str, do_type: str, args: List[str]) -> bool:
         """
         Returns true if the specified command has already been executed in FakeShell for the specified connection.
         :param host: host to check, for which the desirable command should have been executed.
         :param do_type: The type of required command
         :param args: Required command arguments
         :return: Boolean
         """
         found_entries = self.history_find(host, do_type, args)
-        return sum(found_entry['used_times'] for found_entry in found_entries) > 0
+        total_used_times: int = sum(found_entry['used_times'] for found_entry in found_entries)
+        return total_used_times > 0
 
 
 class FakeFS:
-    def __init__(self):
+    def __init__(self) -> None:
         self.storage: Dict[str, Dict[str, str]] = {}
         self.emulate_latency = False
         self._lock = threading.Lock()
 
-    def reset(self):
+    def reset(self) -> None:
         self.storage = {}
         self.emulate_latency = False
 
-    def reset_host(self, host):
+    def reset_host(self, host: str) -> None:
         self.storage[host] = {}
 
     # covered by test.test_demo.TestFakeFS.test_put_file
     # covered by test.test_demo.TestFakeFS.test_put_bytesio
     # covered by test.test_group.TestGroupCall.test_write_stream
-    def write(self, host, filename, data):
+    def write(self, host: str, filename: str, data: Union[io.BytesIO, str]) -> None:
         if isinstance(data, io.BytesIO):
             # Emulate how fabric handles file-like objects.
             # See fabric.transfer.Transfer.put
             pointer = data.tell()
             try:
                 data.seek(0)
                 text = self._transfer(data)
             finally:
                 data.seek(pointer)
-        elif isinstance(data, str):
+        else:
             with open(data, "rb") as fl:
                 text = self._transfer(fl)
-        else:
-            raise ValueError("Unsupported data type " + str(type(data)))
 
         with self._lock:
             self.storage.setdefault(host, {})[filename] = text
 
     def _transfer(self, fl: IO) -> str:
         # Emulate how paramiko transfers files.
         # See paramiko.sftp_client.SFTPClient._transfer_with_callback
@@ -159,61 +154,51 @@
                 time.sleep(0.1)
             if len(data) == 0:
                 break
         return target.getvalue().decode('utf-8')
 
     # covered by test.test_demo.TestFakeFS.test_put_string
     # covered by test.test_demo.TestFakeFS.test_get_nonexistent
-    def read(self, host, filename):
+    def read(self, host: str, filename: str) -> Optional[str]:
         return self.storage.get(host, {}).get(filename)
 
     # covered by test.test_demo.TestFakeFS.test_write_file_to_cluster
-    def read_all(self, hosts: List[str], filename):
+    def read_all(self, hosts: List[str], filename: str) -> Dict[str, Optional[str]]:
         result = {}
         for host in hosts:
             result[host] = self.read(host, filename)
         return result
 
-    def ls(self, host, path):
-        for _path in list(self.storage.get(host, {}).keys()):
-            # TODO
-            pass
-
-    def rm(self, host, path):
-        for _path in list(self.storage.get(host, {}).keys()):
-            if path in _path:
-                del self.storage[host][_path]
-
 
 class FakeKubernetesCluster(KubernetesCluster):
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any):
         self.fake_shell = kwargs.pop("fake_shell", FakeShell())
         self.fake_fs = kwargs.pop("fake_fs", FakeFS())
         super().__init__(*args, **kwargs)
 
     @property
     def connection_pool(self) -> ConnectionPool:
         if self._connection_pool is None:
             self._connection_pool = FakeConnectionPool(self.inventory, self.fake_shell, self.fake_fs)
 
         return self._connection_pool
 
     def make_group(self, ips: Iterable[_AnyConnectionTypes]) -> FakeNodeGroup:
         return FakeNodeGroup(ips, self)
 
-    def dump_finalized_inventory(self):
+    def dump_finalized_inventory(self) -> None:
         return
 
-    def preserve_inventory(self):
+    def preserve_inventory(self) -> None:
         return
 
 
 class FakeResources(DynamicResources):
-    def __init__(self, context, raw_inventory: dict, procedure_inventory: dict = None,
+    def __init__(self, context: dict, raw_inventory: dict, procedure_inventory: dict = None,
                  nodes_context: dict = None,
                  fake_shell: FakeShell = None, fake_fs: FakeFS = None):
         super().__init__(context, True)
         self.inventory_filepath = None
         self.procedure_inventory_filepath = None
         self.stored_inventory = raw_inventory
         self.last_cluster: Optional[FakeKubernetesCluster] = None
@@ -236,101 +221,94 @@
             fake_shell=self.fake_shell, fake_fs=self.fake_fs
         )
         return self.last_cluster
 
 
 class FakeConnection(fabric.connection.Connection):  # type: ignore[misc]
 
-    def __init__(self, ip, fake_shell: FakeShell, fake_fs: FakeFS, **kw):
+    def __init__(self, ip: str, fake_shell: FakeShell, fake_fs: FakeFS, **kw: Any):
         super().__init__(ip, **kw)
         self.fake_shell = fake_shell
         self.fake_fs = fake_fs
 
         command_sep = r'[=\-_]{32}'
         sep_symbol = r'\&\&|;'
         final_sep = rf" ({sep_symbol}) " \
                     rf"printf \"%s\\n\$\?\\n%s\\n\" \"({command_sep})\" \"\2\" \1 " \
                     rf"echo \"\2\" 1>\&2 \1 (sudo )?"
 
         self.separator_ptrn = re.compile(final_sep)
 
-    def __setattr__(self, key, value):
+    def __setattr__(self, key: str, value: Any) -> None:
         # fabric Connection has special handling of this method. Call default behaviour for custom attributes.
         if key in ('fake_shell', 'fake_fs', 'separator_ptrn'):
             return object.__setattr__(self, key, value)
         super().__setattr__(key, value)
 
-    def run(self, command, **kwargs) -> fabric.runners.Result:
+    def run(self, command: str, **kwargs: Any) -> fabric.runners.Result:
         return self._do("run", command, **kwargs)
 
-    def sudo(self, command, **kwargs) -> fabric.runners.Result:
+    def sudo(self, command: str, **kwargs: Any) -> fabric.runners.Result:
         return self._do("sudo", command, **kwargs)
 
     # not implemented
-    def get(self, *args, **kwargs):
-        return self._do("get", *args, **kwargs)
+    def get(self, remote_file: str, local_file: str, **kwargs: Any) -> None:
+        raise NotImplementedError("Stub for fabric Connection.get() is not implemented")
 
-    def put(self, *args, **kwargs):
-        return self._do("put", *args, **kwargs)
+    def put(self, data: Union[io.BytesIO, str], filename: str, **kwargs: Any) -> None:
+        # It should return fabric.transfer.Result, but currently returns None.
+        # Transfer Result is currently never handled.
+        self.fake_fs.write(self.host, filename, data)
+
+    def _do(self, do_type: str, original_command: str, **kwargs: Any) -> fabric.runners.Result:
+        # start fake execution of commands
+        commands, sep_symbol, command_sep = self._split_command(do_type, original_command)
+
+        final_res = fabric.runners.Result(stdout="", stderr="", exited=None,
+                                          connection=self, command=original_command)
+        prev_exited = None
+        i = 0
+        for command in commands:
+            found_result = self.fake_shell.find(self.host, do_type, [command])
 
-    def _do(self, do_type, *args, **kwargs) -> fabric.runners.Result:
-        if do_type in ['sudo', 'run']:
-            # start fake execution of commands
-            original_command = list(args)[0]
-            commands, sep_symbol, command_sep = self._split_command(do_type, original_command)
-
-            final_res = fabric.runners.Result(stdout="", stderr="", exited=None,
-                                              connection=self, command=original_command)
-            prev_exited = None
-            i = 0
-            for command in commands:
-                found_result = self.fake_shell.find(self.host, do_type, [command], kwargs)
-
-                if found_result is None:
-                    raise Exception('Fake result not found for requested action type \'%s\' and command %s' % (do_type, [command]))
-
-                timeout_exception = None
-                if isinstance(found_result, Exception):
-                    if i > 0:
-                        raise ValueError("Exception can be thrown only for the whole command")
-                    elif isinstance(found_result, CommandTimedOut):
-                        timeout_exception = found_result
-                        found_result = found_result.result
-                    else:
-                        raise found_result
+            if found_result is None:
+                raise Exception('Fake result not found for requested action type \'%s\' and command %s' % (do_type, [command]))
 
+            timeout_exception = None
+            if isinstance(found_result, Exception):
                 if i > 0:
-                    final_res.stdout += command_sep + '\n' + str(prev_exited) + '\n' + command_sep + '\n'
-                    final_res.stderr += command_sep + '\n'
-                i += 1
-
-                final_res.stdout += found_result.stdout
-                final_res.stderr += found_result.stderr
-                final_res.exited = prev_exited = found_result.exited
-
-                if timeout_exception is not None:
-                    raise invoke.CommandTimedOut(final_res, timeout_exception.timeout)
+                    raise ValueError("Exception can be thrown only for the whole command")
+                elif isinstance(found_result, CommandTimedOut):
+                    timeout_exception = found_result
+                    found_result = found_result.result
+                else:
+                    raise found_result
+
+            if i > 0:
+                final_res.stdout += command_sep + '\n' + str(prev_exited) + '\n' + command_sep + '\n'
+                final_res.stderr += command_sep + '\n'
+            i += 1
 
-                if prev_exited != 0 and sep_symbol != ';':
-                    # stop fake execution
-                    break
+            final_res.stdout += found_result.stdout
+            final_res.stderr += found_result.stderr
+            final_res.exited = prev_exited = found_result.exited
 
-            if prev_exited == 0 or kwargs.get('warn', False):
-                return final_res
+            if timeout_exception is not None:
+                raise invoke.CommandTimedOut(final_res, timeout_exception.timeout)
 
-            raise invoke.UnexpectedExit(final_res)
+            if prev_exited != 0 and sep_symbol != ';':
+                # stop fake execution
+                break
 
-        elif do_type == 'put':
-            # It should return fabric.transfer.Result, but currently returns None.
-            # Transfer Result is currently never handled.
-            return self.fake_fs.write(self.host, args[1], args[0])
+        if prev_exited == 0 or kwargs.get('warn', False):
+            return final_res
 
-        raise Exception('Unsupported do type')
+        raise invoke.UnexpectedExit(final_res)
 
-    def _split_command(self, do_type, command: str):
+    def _split_command(self, do_type: str, command: str) -> Tuple[List[str], str, str]:
         """
         This is a reverse operation to the RemoteExecutor#_merge_actions
         """
         tokens = self.separator_ptrn.split(command)
         commands = []
         i = 0
         sep_symbol = None
@@ -341,29 +319,29 @@
             if i < len(tokens):
                 sep_symbol = self._compare_and_return(sep_symbol, tokens[i], "Separator symbols are not equal")
                 command_sep = self._compare_and_return(command_sep, tokens[i + 1], "Command separators are not equal")
                 resolved_do_type = "sudo" if tokens[i + 2] == 'sudo ' else "run"
                 self._compare_and_return(do_type, resolved_do_type, "Do types are not equal")
                 i += 3
 
-        return commands, sep_symbol, command_sep
+        return commands, sep_symbol or '', command_sep or ''
 
-    def _compare_and_return(self, one, another, msg):
+    def _compare_and_return(self, one: Optional[str], another: str, msg: str) -> str:
         if one is None or one == another:
             return another
         else:
             raise ValueError(msg)
 
-    def close(self):
+    def close(self) -> None:
         pass
 
 
 class FakeAbstractGroup(AbstractGroup[GROUP_RUN_TYPE], ABC):
     def _put_with_mv(self, local_stream: Union[io.BytesIO, str], remote_file: str,
-                     backup=False, sudo=False, mkdir=False, immutable=False):
+                     backup: bool, sudo: bool, mkdir: bool, immutable: bool) -> None:
         super()._put_with_mv(local_stream, remote_file, backup=False, sudo=False, mkdir=False, immutable=False)
 
 
 class FakeNodeGroup(NodeGroup, FakeAbstractGroup[RunnersGroupResult]):
     def _make_group(self, ips: Iterable[Union[str, NodeGroup]]) -> FakeNodeGroup:
         return FakeNodeGroup(ips, self.cluster)
 
@@ -384,39 +362,42 @@
 
 class FakeConnectionPool(connections.ConnectionPool):
     def __init__(self, inventory: dict, fake_shell: FakeShell, fake_fs: FakeFS):
         super().__init__(inventory)
         self.fake_shell = fake_shell
         self.fake_fs = fake_fs
 
-    def _create_connection_from_details(self, ip: str, conn_details: dict, gateway=None, inline_ssh_env=True):
+    def _create_connection_from_details(self, ip: str, conn_details: dict,
+                                        gateway: fabric.connection.Connection = None,
+                                        inline_ssh_env: bool = True) -> fabric.connection.Connection:
         return FakeConnection(
             ip, self.fake_shell, self.fake_fs,
             user=conn_details.get('username', static.GLOBALS['connection']['defaults']['username']),
             port=conn_details.get('connection_port', static.GLOBALS['connection']['defaults']['port'])
         )
 
 
-def create_silent_context(args: list = None, parser: argparse.ArgumentParser = None, procedure='install'):
+def create_silent_context(args: list = None, parser: argparse.ArgumentParser = None,
+                          procedure: str = 'install') -> dict:
     args = list(args) if args else []
     # todo probably increase logging level to get rid of spam in logs.
     if '--disable-dump' not in args:
         args.append('--disable-dump')
 
     if parser is None:
         parser = flow.new_common_parser("Help text")
     context = flow.create_context(parser, args, procedure=procedure)
     del context['execution_arguments']['ansible_inventory_location']
     context['preserve_inventory'] = False
 
     return context
 
 
-def new_cluster(inventory, procedure_inventory=None, context: dict = None,
-                fake=True) -> Union[KubernetesCluster, FakeKubernetesCluster]:
+def new_cluster(inventory: dict, procedure_inventory: dict = None, context: dict = None,
+                fake: bool = True) -> Union[KubernetesCluster, FakeKubernetesCluster]:
     if context is None:
         context = create_silent_context()
 
     nodes_context = generate_nodes_context(inventory)
     nodes_context.update(context['nodes'])
     context['nodes'] = nodes_context
 
@@ -427,15 +408,16 @@
     else:
         cluster = KubernetesCluster(inventory, context, procedure_inventory=procedure_inventory)
 
     cluster.enrich()
     return cluster
 
 
-def generate_nodes_context(inventory: dict, os_name='centos', os_version='7.9', net_interface='eth0') -> dict:
+def generate_nodes_context(inventory: dict, os_name: str = 'centos', os_version: str = '7.9',
+                           net_interface: str = 'eth0') -> dict:
     os_family = system.detect_of_family_by_name_version(os_name, os_version)
 
     context = {}
     for node in inventory['nodes']:
         node_context = {
             'access': {
                 'online': True,
@@ -550,44 +532,36 @@
     return create_nodegroup_result_by_hosts(group_.cluster, hosts_to_result)
 
 
 def create_hosts_exception_result(hosts: List[str], exception: Exception) -> Dict[str, GenericResult]:
     return {host: exception for host in hosts}
 
 
-def create_nodegroup_result(group_: AbstractGroup[RunResult], stdout='', stderr='',
-                            code=0, timeout: int = None) -> NodeGroupResult:
+def create_nodegroup_result(group_: AbstractGroup[RunResult], stdout: str = '', stderr: str = '',
+                            code: int = 0, timeout: int = None) -> NodeGroupResult:
     hosts_to_result = create_hosts_result(group_.get_hosts(), stdout, stderr, code, timeout)
     return create_nodegroup_result_by_hosts(group_.cluster, hosts_to_result)
 
 
-def create_hosts_result(hosts: List[str], stdout='', stderr='',
-                        code=0, timeout: int = None) -> Dict[str, GenericResult]:
+def create_hosts_result(hosts: List[str], stdout: str = '', stderr: str = '',
+                        code: int = 0, timeout: int = None) -> Dict[str, GenericResult]:
     # each host should have its own result instance.
     return {host: create_result(stdout, stderr, code, timeout) for host in hosts}
 
 
-def create_result(stdout='', stderr='', code=0, timeout: int = None) -> GenericResult:
+def create_result(stdout: str = '', stderr: str = '', code: int = 0, timeout: int = None) -> GenericResult:
     # command and 'hide' option will be later replaced with actual
     result = RunnersResult(["fake command"], [code], stdout=stdout, stderr=stderr)
     if timeout is None:
         return result
 
     return CommandTimedOut(result, timeout)
 
 
-def empty_action(*args, **kwargs) -> None:
-    """
-    A dummy method that does nothing
-    :return: None
-    """
-    pass
-
-
-def new_scheme(scheme: dict, role: str, number: int):
+def new_scheme(scheme: dict, role: str, number: int) -> dict:
     scheme = deepcopy(scheme)
     scheme[role] = number
     return scheme
 
 
 FULLHA: Dict[str, _ROLE_SPEC] = {'balancer': 1, 'master': 3, 'worker': 3}
 FULLHA_KEEPALIVED: Dict[str, _ROLE_SPEC] = {'balancer': 2, 'master': 3, 'worker': 3, 'keepalived': 1}
```

### Comparing `kubemarine-0.19.0/kubemarine/etcd.py` & `kubemarine-0.20.0/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/haproxy.py` & `kubemarine-0.20.0/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/jinja.py` & `kubemarine-0.20.0/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/k8s_certs.py` & `kubemarine-0.20.0/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/keepalived.py` & `kubemarine-0.20.0/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.20.0/kubemarine/kubernetes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,36 +15,38 @@
 import io
 import math
 import os
 import time
 import uuid
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import List, Dict, Tuple, Iterator
+from typing import List, Dict, Tuple, Iterator, Any, Optional
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 import ipaddress
 
 from kubemarine import system, plugins, admission, etcd, packages
 from kubemarine.core import utils, static, summary, log, errors
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import Token
-from kubemarine.core.group import NodeGroup, NodeConfig, RunnersGroupResult, RunResult, AbstractGroup, DeferredGroup, \
-    CollectorCallback
+from kubemarine.core.group import (
+    NodeGroup, AbstractGroup, DeferredGroup,
+    NodeConfig, RunnersGroupResult, RunResult, CollectorCallback
+)
 from kubemarine.core.errors import KME
 
 ERROR_DOWNGRADE='Kubernetes old version \"%s\" is greater than new one \"%s\"'
 ERROR_SAME='Kubernetes old version \"%s\" is the same as new one \"%s\"'
 ERROR_MAJOR_RANGE_EXCEEDED='Major version \"%s\" rises to new \"%s\" more than one'
 ERROR_MINOR_RANGE_EXCEEDED='Minor version \"%s\" rises to new \"%s\" more than one'
 
 
-def add_node_enrichment(inventory: dict, cluster: KubernetesCluster):
+def add_node_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get('initial_procedure') != 'add_node':
         return inventory
 
     # adding role "new_node" for all specified new nodes and putting these nodes to all "nodes" list
     for new_node in cluster.procedure_inventory.get("nodes", []):
         # deepcopy is necessary, otherwise role append will happen in procedure_inventory too
         node = deepcopy(new_node)
@@ -53,15 +55,15 @@
 
     if "vrrp_ips" in cluster.procedure_inventory:
         utils.merge_vrrp_ips(cluster.procedure_inventory, inventory)
 
     return inventory
 
 
-def remove_node_enrichment(inventory: dict, cluster: KubernetesCluster):
+def remove_node_enrichment(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get('initial_procedure') != 'remove_node':
         return inventory
 
     # adding role "remove_node" for all specified nodes
     node_names_to_remove = [node['name'] for node in cluster.procedure_inventory.get("nodes", [])]
     for i, node in enumerate(inventory['nodes']):
         if node['name'] in node_names_to_remove:
@@ -90,15 +92,15 @@
         return inventory
 
     upgrade_version = cluster.context.get("upgrade_version")
     inventory.setdefault("services", {}).setdefault("kubeadm", {})['kubernetesVersion'] = upgrade_version
     return inventory
 
 
-def enrich_inventory(inventory: dict, _):
+def enrich_inventory(inventory: dict, _: KubernetesCluster) -> dict:
     repository = inventory['services']['kubeadm'].get('imageRepository', "")
     if repository:
         inventory['services']['kubeadm']['dns'] = {}
         inventory['services']['kubeadm']['dns']['imageRepository'] = ("%s/coredns" % repository)
     # if user redefined apiServer as, string, for example?
     if not isinstance(inventory["services"]["kubeadm"].get('apiServer'), dict):
         inventory["services"]["kubeadm"]['apiServer'] = {}
@@ -196,15 +198,15 @@
 
     preflight_errors.extend(default_preflight_errors)
     inventory["services"]["kubeadm_flags"]["ignorePreflightErrors"] = ",".join(set(preflight_errors))
 
     return inventory
 
 
-def reset_installation_env(group: NodeGroup):
+def reset_installation_env(group: NodeGroup) -> Optional[RunnersGroupResult]:
     log = group.cluster.log
 
     log.debug("Cleaning up previous installation...")
 
     cluster: KubernetesCluster = group.cluster
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
@@ -271,16 +273,19 @@
         # result.update(cri.prune(active_nodes, all_implementations=True))
 
         log.debug(f"Nodes {active_nodes.get_hosts()} cleaned up successfully:\n" + "%s" % result)
 
     if is_add_or_remove_procedure:
         return delete_nodes(group)
 
+    return None
 
-def drain_nodes(group: NodeGroup, disable_eviction=False, drain_timeout=None, grace_period=None):
+
+def drain_nodes(group: NodeGroup, disable_eviction: bool = False,
+                drain_timeout: int = None, grace_period: int = None) -> RunnersGroupResult:
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     control_plane = cluster.nodes['control-plane'].get_final_nodes().get_first_member()
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
@@ -296,15 +301,15 @@
             control_plane.sudo(drain_cmd, hide=False)
         else:
             log.warning("Node %s is not found in cluster and can't be drained" % node_name)
 
     return control_plane.sudo("kubectl get nodes")
 
 
-def delete_nodes(group: NodeGroup):
+def delete_nodes(group: NodeGroup) -> RunnersGroupResult:
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     control_plane = cluster.nodes['control-plane'].get_final_nodes().get_first_member()
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
@@ -351,21 +356,21 @@
         join_control_plane(group.cluster, node, join_dict)
 
     group.cluster.log.debug("Verifying installation...")
     first_control_plane = group.get_first_member()
     return first_control_plane.sudo("kubectl get pods --all-namespaces -o=wide")
 
 
-def join_new_control_plane(group: NodeGroup):
+def join_new_control_plane(group: NodeGroup) -> None:
     join_dict = get_join_dict(group)
     for node in group.get_ordered_members_list():
         join_control_plane(group.cluster, node, join_dict)
 
 
-def join_control_plane(cluster: KubernetesCluster, node: NodeGroup, join_dict: dict):
+def join_control_plane(cluster: KubernetesCluster, node: NodeGroup, join_dict: dict) -> None:
     log = cluster.log
     node_config = node.get_config()
     node_name = node.get_node_name()
     defer = node.new_defer()
 
     join_config: dict = {
         'apiVersion': cluster.inventory["services"]["kubeadm"]['apiVersion'],
@@ -600,38 +605,38 @@
     cluster.context["join_dict"] = join_dict
 
     wait_for_any_pods(cluster, first_control_plane, apply_filter=node_name)
     # refresh cluster installation status in cluster context
     is_cluster_installed(cluster)
 
 
-def wait_for_any_pods(cluster: KubernetesCluster, connection: NodeGroup, apply_filter: str = None) :
+def wait_for_any_pods(cluster: KubernetesCluster, connection: NodeGroup, apply_filter: str = None) -> None:
     plugins.expect_pods(cluster, [
         'kube-apiserver',
         'kube-controller-manager',
         'kube-proxy',
         'kube-scheduler',
         'etcd'
     ], node=connection, apply_filter=apply_filter,
                         timeout=cluster.inventory['globals']['expect']['pods']['kubernetes']['timeout'],
                         retries=cluster.inventory['globals']['expect']['pods']['kubernetes']['retries'])
 
 
-def wait_uncordon(node: NodeGroup):
+def wait_uncordon(node: NodeGroup) -> None:
     cluster = node.cluster
     timeout_config = cluster.inventory['globals']['expect']['pods']['kubernetes']
     # This forces to use local API server and waits till it is up.
     with local_admin_config(node) as kubeconfig:
         utils.wait_command_successful(node, f"kubectl --kubeconfig {kubeconfig} uncordon {node.get_node_name()}",
                                       hide=False,
                                       timeout=timeout_config['timeout'],
                                       retries=timeout_config['retries'])
 
 
-def wait_for_nodes(group: NodeGroup):
+def wait_for_nodes(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
     node_names = group.get_nodes_names()
 
     wait_conditions = {
@@ -768,15 +773,15 @@
     log.debug("Successfully applied additional taints")
 
     return control_plane.sudo(
         "kubectl get nodes -o=jsonpath="
         "'{range .items[*]}{\"node: \"}{.metadata.name}{\"\\ntaints: \"}{.spec.taints}{\"\\n\"}'")
 
 
-def is_cluster_installed(cluster: KubernetesCluster):
+def is_cluster_installed(cluster: KubernetesCluster) -> bool:
     cluster.log.verbose('Searching for already installed cluster...')
     try:
         results = cluster.nodes['control-plane'].sudo('kubectl cluster-info', warn=True, timeout=15)
         for host, result in results.items():
             if 'is running at' in result.stdout:
                 cluster.log.verbose('Detected running Kubernetes cluster on %s' % host)
                 for line in result.stdout.split("\n"):
@@ -786,21 +791,21 @@
     except Exception as e:
         cluster.log.verbose(e)
     cluster.context['controlplain_uri'] = None
     cluster.log.verbose('Failed to detect any Kubernetes cluster')
     return False
 
 
-def get_kubeadm_config(inventory: dict):
+def get_kubeadm_config(inventory: dict) -> str:
     kubeadm_kubelet = yaml.dump(inventory["services"]["kubeadm_kubelet"], default_flow_style=False)
     kubeadm = yaml.dump(inventory["services"]["kubeadm"], default_flow_style=False)
     return f'{kubeadm_kubelet}---\n{kubeadm}'
 
 
-def upgrade_first_control_plane(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+def upgrade_first_control_plane(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs: Any) -> None:
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     node_name = first_control_plane.get_node_name()
 
     if not upgrade_group.has_node(node_name):
         cluster.log.debug("First control-plane \"%s\" upgrade is not required" % node_name)
         return
@@ -813,16 +818,16 @@
     # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
     # and only "else" branch remains
     if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s'" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
     else:
         flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s' --patches=/etc/kubernetes/patches" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
 
-    if patch_kubeadm_configmap(first_control_plane, cluster):
-        flags += " --config /tmp/kubeadm_config.yaml"
+    patch_kubeadm_configmap(first_control_plane, cluster)
+    flags += " --config /tmp/kubeadm_config.yaml"
 
     drain_cmd = prepare_drain_command(cluster, node_name, **drain_kwargs)
     first_control_plane.sudo(drain_cmd, hide=False)
 
     upgrade_cri_if_required(first_control_plane)
 
     # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
@@ -836,15 +841,15 @@
     copy_admin_config(cluster.log, first_control_plane)
 
     expect_kubernetes_version(cluster, version, apply_filter=node_name)
     wait_for_any_pods(cluster, first_control_plane, apply_filter=node_name)
     exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
-def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs: Any) -> None:
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
     for node in cluster.nodes['control-plane'].get_ordered_members_list():
         node_name = node.get_node_name()
         if node_name != first_control_plane.get_node_name():
 
@@ -884,15 +889,15 @@
 
             expect_kubernetes_version(cluster, version, apply_filter=node_name)
             copy_admin_config(cluster.log, node)
             wait_for_any_pods(cluster, node, apply_filter=node_name)
             exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
-def patch_kubeadm_configmap(first_control_plane: NodeGroup, cluster: KubernetesCluster):
+def patch_kubeadm_configmap(first_control_plane: NodeGroup, cluster: KubernetesCluster) -> None:
     '''
     Checks and patches the Kubeadm configuration for compliance with the current imageRepository, audit log path
     and the corresponding version of the CoreDNS path to the image.
     '''
     # TODO: get rid of this method after k8s 1.21 support stop
     current_kubernetes_version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
     kubeadm_config_map = first_control_plane.sudo("kubectl get cm -o yaml -n kube-system kubeadm-config") \
@@ -923,18 +928,16 @@
     cluster_config['dns']['imageRepository'] = "%s/coredns" % cluster_config["imageRepository"]
 
     kubelet_config = first_control_plane.sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
     ryaml.dump(cluster_config, updated_config)
     result_config = kubelet_config + "---\n" + updated_config.getvalue()
     first_control_plane.put(io.StringIO(result_config), "/tmp/kubeadm_config.yaml", sudo=True)
 
-    return True
-
 
-def upgrade_workers(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs):
+def upgrade_workers(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs: Any) -> None:
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
     for node in cluster.nodes['worker'].exclude_group(cluster.nodes['control-plane'])\
             .get_ordered_members_list():
         node_name = node.get_node_name()
 
@@ -971,31 +974,31 @@
         expect_kubernetes_version(cluster, version, apply_filter=node_name)
         # workers do not have system pods to wait for their start
         exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
 def prepare_drain_command(cluster: KubernetesCluster, node_name: str,
                           *,
-                          disable_eviction=False,
-                          drain_timeout: int = None, grace_period: int = None):
+                          disable_eviction: bool = False,
+                          drain_timeout: int = None, grace_period: int = None) -> str:
     drain_globals = static.GLOBALS['nodes']['drain']
     if drain_timeout is None:
         drain_timeout = recalculate_proper_timeout(cluster, drain_globals['timeout'])
 
     if grace_period is None:
         grace_period = drain_globals['grace_period']
 
     drain_cmd = f"kubectl drain {node_name} --force --ignore-daemonsets --delete-emptydir-data " \
                 f"--timeout={drain_timeout}s --grace-period={grace_period}"
     if disable_eviction:
         drain_cmd += " --disable-eviction=true"
     return drain_cmd
 
 
-def upgrade_cri_if_required(group: NodeGroup):
+def upgrade_cri_if_required(group: NodeGroup) -> None:
     # currently it is invoked only for single node
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
 
     if cri_impl in cluster.context["packages"]["upgrade_required"]:
         cri_packages = cluster.get_package_association_for_node(group.get_host(), cri_impl, 'package_name')
@@ -1007,15 +1010,15 @@
             group.sudo("docker container rm -f $(sudo docker container ls -q)", warn=True)
         else:
             group.sudo("crictl rm -fa", warn=True)
     else:
         log.debug(f"{cri_impl} upgrade is not required")
 
 
-def verify_upgrade_versions(cluster: KubernetesCluster):
+def verify_upgrade_versions(cluster: KubernetesCluster) -> None:
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     upgrade_version = cluster.context["upgrade_version"]
 
     k8s_nodes_group = cluster.nodes["worker"].include_group(cluster.nodes['control-plane'])
     for node in k8s_nodes_group.get_ordered_members_list():
         cluster.log.debug(f"Verifying current k8s version for node {node.get_node_name()}")
         result = first_control_plane.sudo("kubectl get nodes "
@@ -1023,22 +1026,24 @@
                                           " -o custom-columns='VERSION:.status.nodeInfo.kubeletVersion' "
                                           "| grep -vw ^VERSION ")
         curr_version = list(result.values())[0].stdout
         test_version_upgrade_possible(curr_version, upgrade_version, skip_equal=True)
 
 
 def get_initial_kubernetes_version(inventory: dict) -> str:
-    kubernetes_version = inventory.get("services", {}).get("kubeadm", {}).get("kubernetesVersion")
-    if kubernetes_version is None:
+    kubernetes_version: str
+    if inventory.get("services", {}).get("kubeadm", {}).get("kubernetesVersion") is not None:
+        kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
+    else:
         kubernetes_version = static.DEFAULTS['services']['kubeadm']['kubernetesVersion']
 
     return kubernetes_version
 
 
-def verify_initial_version(inventory: dict, _) -> dict:
+def verify_initial_version(inventory: dict, _: KubernetesCluster) -> dict:
     version = get_initial_kubernetes_version(inventory)
     verify_allowed_version(version)
     return inventory
 
 
 def verify_allowed_version(version: str) -> None:
     allowed_versions = static.KUBERNETES_VERSIONS['compatibility_map'].keys()
@@ -1053,15 +1058,16 @@
     minor_version = utils.minor_version(target_version)
     supported_versions = static.KUBERNETES_VERSIONS['kubernetes_versions']
     if not supported_versions.get(minor_version, {}).get("supported", False):
         logger.warning(f"Specified target Kubernetes version {target_version!r} - is not supported!")
 
 
 def expect_kubernetes_version(cluster: KubernetesCluster, version: str,
-                              timeout=None, retries=None, node: NodeGroup = None, apply_filter: str = None):
+                              timeout: int = None, retries: int = None,
+                              node: NodeGroup = None, apply_filter: str = None) -> None:
     if timeout is None:
         timeout = cluster.globals['nodes']['expect']['kubernetes_version']['timeout']
     if retries is None:
         retries = cluster.globals['nodes']['expect']['kubernetes_version']['retries']
 
     cluster.log.debug("Expecting Kubernetes version %s" % version)
     cluster.log.debug("Max expectation time: %ss" % (timeout * retries))
@@ -1093,15 +1099,15 @@
             retries -= 1
             cluster.log.debug("Some nodes have invalid Kubernetes version... (%ss left)" % (retries * timeout), result)
             time.sleep(timeout)
 
     raise Exception('In the expected time, the nodes did not receive correct Kubernetes version')
 
 
-def test_version_upgrade_possible(old: str, new: str, skip_equal=False):
+def test_version_upgrade_possible(old: str, new: str, skip_equal: bool = False) -> None:
     versions_unchanged = {
         'old': old.strip(),
         'new': new.strip()
     }
     versions: Dict[str, Tuple[int, int, int]] = {}
 
     for v_type, version in versions_unchanged.items():
@@ -1120,23 +1126,23 @@
         raise Exception(ERROR_MAJOR_RANGE_EXCEEDED % (versions_unchanged['old'], versions_unchanged['new']))
 
     # test minor step is not greater than 1
     if versions['new'][1] - versions['old'][1] > 1:
         raise Exception(ERROR_MINOR_RANGE_EXCEEDED % (versions_unchanged['old'], versions_unchanged['new']))
 
 
-def recalculate_proper_timeout(cluster: KubernetesCluster, timeout: int):
+def recalculate_proper_timeout(cluster: KubernetesCluster, timeout: int) -> int:
     try:
         amount_str = cluster.nodes['control-plane'].get_first_member().sudo('kubectl get pods -A | wc -l').get_simple_out()
         return timeout * int(amount_str)
     except Exception:
         return timeout * 10 * cluster.nodes['all'].nodes_amount()
 
 
-def configure_container_runtime(cluster: KubernetesCluster, kubeadm_config: dict):
+def configure_container_runtime(cluster: KubernetesCluster, kubeadm_config: dict) -> None:
     if cluster.inventory['services']['cri']['containerRuntime'] == "containerd":
         if 'nodeRegistration' not in kubeadm_config:
             kubeadm_config['nodeRegistration'] = {}
         if 'kubeletExtraArgs' not in kubeadm_config['nodeRegistration']:
             kubeadm_config['nodeRegistration']['kubeletExtraArgs'] = {}
 
         kubeadm_config['nodeRegistration']['criSocket'] = '/var/run/containerd/containerd.sock'
@@ -1145,16 +1151,16 @@
         if minor_version < 27:
             kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime'] = 'remote'
 
         kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime-endpoint'] = \
             'unix:///run/containerd/containerd.sock'
 
 
-def exclude_node_from_upgrade_list(first_control_plane: NodeGroup, node_name: str):
-    return first_control_plane.sudo('sed -i \'/%s/d\' /etc/kubernetes/nodes-k8s-versions.txt' % node_name, warn=True)
+def exclude_node_from_upgrade_list(first_control_plane: NodeGroup, node_name: str) -> None:
+    first_control_plane.sudo('sed -i \'/%s/d\' /etc/kubernetes/nodes-k8s-versions.txt' % node_name, warn=True)
 
 
 def autodetect_non_upgraded_nodes(cluster: KubernetesCluster, future_version: str) -> List[str]:
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     try:
         nodes_list_result = first_control_plane.sudo('[ ! -f /etc/kubernetes/nodes-k8s-versions.txt ] && '
                                               'sudo kubectl get nodes -o custom-columns=\''
@@ -1196,18 +1202,18 @@
             upgrade_list.append(node_name)
         else:
             cluster.log.verbose("Node \"%s\" already upgraded." % node_name)
 
     return upgrade_list
 
 
-def get_group_for_upgrade(cluster: KubernetesCluster, ignore_cache=False) -> NodeGroup:
-
-    if cluster.context.get('upgrade_group') and not ignore_cache:
-        return cluster.context['upgrade_group']
+def get_group_for_upgrade(cluster: KubernetesCluster) -> NodeGroup:
+    upgrade_group: Optional[NodeGroup] = cluster.context.get('upgrade_group')
+    if upgrade_group is not None:
+        return upgrade_group
 
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
     if cluster.procedure_inventory.get('upgrade_nodes'):
         nodes_for_upgrade = []
         for node in cluster.procedure_inventory['upgrade_nodes']:
             if isinstance(node, str):
                 node_name = node
@@ -1218,18 +1224,18 @@
             cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt', warn=True)
     else:
         nodes_for_upgrade = autodetect_non_upgraded_nodes(cluster, version)
 
     upgrade_group = cluster.make_group_from_nodes(nodes_for_upgrade)
     cluster.context['upgrade_group'] = upgrade_group
 
-    return cluster.context['upgrade_group']
+    return upgrade_group
 
 
-def images_grouped_prepull(group: NodeGroup, group_size: int = None):
+def images_grouped_prepull(group: NodeGroup, group_size: int = None) -> RunnersGroupResult:
     """
     Prepull kubeadm images on group, separated on sub-groups with certain group size. Separation required to avoid high
     load on images repository server, when using large clusters.
     :param group: NodeGroup where prepull should be performed.
     :param group_size: integer number of nodes per group. Will be automatically used from procedure_yaml or globals, if not set.
     :return: String results from all nodes in presented group.
     """
@@ -1265,15 +1271,17 @@
 
     return collector.result
 
 
 def images_prepull(group: DeferredGroup, collector: CollectorCallback) -> Token:
     """
     Prepull kubeadm images on group.
+
     :param group: NodeGroup where prepull should be performed.
+    :param collector: CollectorCallback instance
     :return: NodeGroupResult from all nodes in presented group.
     """
 
     config = get_kubeadm_config(group.cluster.inventory)
     kubeadm_init: dict = {
         'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
         'kind': 'InitConfiguration',
@@ -1284,19 +1292,19 @@
 
     group.put(io.StringIO(config), '/etc/kubernetes/prepull-config.yaml', sudo=True)
 
     return group.sudo("kubeadm config images pull --config=/etc/kubernetes/prepull-config.yaml",
                       callback=collector)
 
 
-def schedule_running_nodes_report(cluster: KubernetesCluster):
+def schedule_running_nodes_report(cluster: KubernetesCluster) -> None:
     summary.schedule_delayed_report(cluster, exec_running_nodes_report)
 
 
-def exec_running_nodes_report(cluster: KubernetesCluster):
+def exec_running_nodes_report(cluster: KubernetesCluster) -> None:
     nodes_description = get_nodes_description(cluster)
     actual_roles = get_actual_roles(nodes_description)
     nodes_conditions = get_nodes_conditions(nodes_description)
     nodes_names = actual_roles.keys()
     for role in ('control-plane', 'worker'):
         members = 0
         ready = 0
@@ -1317,15 +1325,16 @@
     return 'kubectl get node -o yaml'
 
 
 def get_nodes_description(cluster: KubernetesCluster) -> dict:
     cmd = get_nodes_description_cmd()
     result = cluster.nodes['control-plane'].get_final_nodes().get_any_member().sudo(cmd)
     cluster.log.verbose(result)
-    return yaml.safe_load(list(result.values())[0].stdout)
+    data: dict = yaml.safe_load(list(result.values())[0].stdout)
+    return data
 
 
 def get_actual_roles(nodes_description: dict) -> Dict[str, List[str]]:
     result: Dict[str, List[str]] = {}
     for node_description in nodes_description['items']:
         node_name = node_description['metadata']['name']
         labels = node_description['metadata']['labels']
@@ -1346,16 +1355,17 @@
         conditions_by_type: Dict[str, dict] = {}
         result[node_name] = conditions_by_type
         for condition in node_description['status']['conditions']:
             conditions_by_type[condition['type']] = condition
 
     return result
 
+
 # function to get dictionary of flags to be patched for a given control plane item and a given node
-def get_patched_flags_for_control_plane_item(inventory: dict, control_plane_item: str, node: NodeConfig):
+def get_patched_flags_for_control_plane_item(inventory: dict, control_plane_item: str, node: NodeConfig) -> Dict[str, str]:
     flags = {}
 
     for n in inventory['services']['kubeadm_patches'][control_plane_item]:
         if n.get('groups') is not None and list(set(node['roles']) & set(n['groups'])):
             if n.get('patch') is not None:
                 for arg, value in n['patch'].items():
                     flags[arg] = value
@@ -1368,15 +1378,15 @@
     if control_plane_item == 'apiServer' and 'control-plane' in node['roles']:
         flags['bind-address'] = node['internal_address']
 
     return flags
 
 
 # function to create kubeadm patches and put them to a node
-def create_kubeadm_patches_for_node(cluster: KubernetesCluster, node: NodeGroup):
+def create_kubeadm_patches_for_node(cluster: KubernetesCluster, node: NodeGroup) -> None:
     cluster.log.verbose(f"Create and upload kubeadm patches to %s..." % node.get_node_name())
     node.sudo('sudo rm -rf /etc/kubernetes/patches ; sudo mkdir -p /etc/kubernetes/patches', warn=True)
 
     # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
     if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
         # do nothing, patches are supported since v1.22
         return
@@ -1400,33 +1410,31 @@
                 template_filename = 'templates/patches/control-plane-pod.json.j2'
 
             control_plane_patch = Template(utils.read_internal(template_filename)).render(flags=patched_flags)
             patch_file = '/etc/kubernetes/patches/' + control_plane_patch_files[control_plane_item]
             node.put(io.StringIO(control_plane_patch + "\n"), patch_file, sudo=True)
             node.sudo(f'chmod 644 {patch_file}')
 
-    return
-
 
-def fix_flag_kubelet(cluster: KubernetesCluster, node: NodeGroup):
-    #Deprecated flag removal function for kubelet
+def fix_flag_kubelet(cluster: KubernetesCluster, node: NodeGroup) -> None:
+    # Deprecated flag removal function for kubelet
     kubeadm_file = "/var/lib/kubelet/kubeadm-flags.env"
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
 
     if utils.version_key(version) < utils.version_key("v1.27.0"):
         # Target version is lower than v1.27.0. Flag is actual and should not be removed.
         return
 
     kubeadm_flags = node.sudo(f"cat {kubeadm_file}").get_simple_out()
     if kubeadm_flags.find('--container-runtime=remote') != -1:
         kubeadm_flags = kubeadm_flags.replace('--container-runtime=remote', '')
         node.put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
  
 
-def _config_changer(config: str, word: str):
+def _config_changer(config: str, word: str) -> str:
     equal_pos = word.find("=") + 1
     param_begin_pos = config.find(word[:equal_pos])
     if param_begin_pos != -1:
         param_end_pos = config[param_begin_pos:].find(" ")
         if param_end_pos == -1:
             return config[:param_begin_pos] + word + "\""
         return config[:param_begin_pos] + word + config[param_end_pos + param_begin_pos:]
```

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.20.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.20.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/object.py` & `kubemarine-0.20.0/kubemarine/kubernetes/object.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 import io
 import json
 import uuid
 import time
-from typing import TypeVar
+from typing import TypeVar, Optional
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 
 _T = TypeVar('_T', bound='KubernetesObject')
@@ -52,37 +52,41 @@
             }
 
     def __str__(self) -> str:
         return self.to_yaml()
 
     @property
     def uid(self) -> str:
-        uid = self._obj['metadata'].get('uid')
+        uid: Optional[str] = self._obj['metadata'].get('uid')
         if uid:
             return uid
 
         return str(uuid.uuid4())
 
     @property
     def kind(self) -> str:
-        return self._obj['kind'].lower()
+        kind: str = self._obj['kind'].lower()
+        return kind
 
     @property
     def namespace(self) -> str:
-        return self._obj['metadata']['namespace'].lower()
+        namespace: str = self._obj['metadata']['namespace'].lower()
+        return namespace
 
     @property
     def name(self) -> str:
-        return self._obj['metadata']['name'].lower()
+        name: str = self._obj['metadata']['name'].lower()
+        return name
 
     def to_json(self) -> str:
         return json.dumps(self._obj)
 
     def to_yaml(self) -> str:
-        return yaml.dump(self._obj)
+        data: str = yaml.dump(self._obj)
+        return data
 
     def is_reloaded(self) -> bool:
         return self._reload_t > -1
 
     def reload(self: _T, control_plane: NodeGroup = None, suppress_exceptions: bool = False) -> _T:
         if not control_plane:
             control_plane = self._cluster.nodes['control-plane'].get_any_member()
```

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.20.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.20.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.20.0/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/packages.py` & `kubemarine-0.20.0/kubemarine/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,14 +515,16 @@
 
     def create_repo_file(self, group: AbstractGroup[RunResult],
                          repo_data: Union[List[str], Dict[str, dict], str],
                          repo_file: str) -> None: ...
 
     def clean(self, group: NodeGroup) -> RunnersGroupResult: ...
 
+    def get_install_cmd(self, include: Union[str, List[str]], exclude: Union[str, List[str]] = None) -> str: ...
+
     def install(self, group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
                 exclude: Union[str, List[str]] = None,
                 callback: Callback = None) -> GROUP_RUN_TYPE: ...
 
     def remove(self, group: AbstractGroup[GROUP_RUN_TYPE], include: Union[str, List[str]] = None,
                exclude: Union[str, List[str]] = None,
                warn: bool = False, hide: bool = True) -> GROUP_RUN_TYPE: ...
```

### Comparing `kubemarine-0.19.0/kubemarine/patches/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.20.0/kubemarine/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/__init__.py` & `kubemarine-0.20.0/kubemarine/plugins/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,46 +27,46 @@
 import urllib.request
 import zipfile
 from copy import deepcopy
 from distutils.dir_util import copy_tree
 from distutils.dir_util import remove_tree
 from distutils.dir_util import mkpath
 from itertools import chain
-from types import ModuleType
-from typing import Dict, List, Tuple, Callable, Union, no_type_check, Set
+from types import ModuleType, FunctionType
+from typing import Dict, List, Tuple, Callable, Union, no_type_check, Set, Any, cast
 
 import yaml
 import inspect
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine import jinja, thirdparties
-from kubemarine.core import utils, static, errors, os as kos
+from kubemarine.core import utils, static, errors, os as kos, log
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.group import NodeGroup
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.kubernetes.replicaset import ReplicaSet
 from kubemarine.kubernetes.statefulset import StatefulSet
 
 # list of plugins owned and managed by kubemarine
 oob_plugins = list(static.DEFAULTS["plugins"].keys())
 LOADED_MODULES: Dict[str, ModuleType] = {}
 
 
-def verify_inventory(inventory: dict, cluster: KubernetesCluster):
+def verify_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     for plugin_name, plugin_item in inventory["plugins"].items():
         for step in plugin_item.get('installation', {}).get('procedures', []):
             for procedure_type, configs in step.items():
                 if procedure_types()[procedure_type].get('verify') is not None:
                     procedure_types()[procedure_type]['verify'](cluster, configs)
 
     return inventory
 
 
-def enrich_inventory(inventory: dict, cluster: KubernetesCluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     for plugin_name, plugin_item in inventory["plugins"].items():
         for i, step in enumerate(plugin_item.get('installation', {}).get('procedures', [])):
             for procedure_type, configs in step.items():
                 if procedure_types()[procedure_type].get('convert') is not None:
                     step[procedure_type] = procedure_types()[procedure_type]['convert'](cluster, configs)
     return inventory
 
@@ -108,30 +108,31 @@
 
     _verify_upgrade_plan(cluster.raw_inventory, previous_version, plugins_verify, upgrade_plan)
 
     return generic_upgrade_inventory(cluster, inventory)
 
 
 def _verify_upgrade_plan(raw_inventory: dict, previous_version: str,
-                         plugins_verify: List[str], upgrade_plan: List[Tuple[str, dict]]):
+                         plugins_verify: List[str], upgrade_plan: List[Tuple[str, dict]]) -> None:
     raw_plugins = deepcopy(raw_inventory.get('plugins', {}))
 
     # validate all plugin sections in procedure inventory
     for version, upgrade_plugins in upgrade_plan:
         for plugin_name in plugins_verify:
             verify_image_redefined(plugin_name,
                                    previous_version,
                                    version,
                                    raw_plugins.get(plugin_name, {}),
                                    upgrade_plugins.get(plugin_name, {}))
         default_merger.merge(raw_plugins, upgrade_plugins)
         previous_version = version
 
 
-def verify_image_redefined(plugin_name, previous_version, next_version, raw_plugins, upgrade_plugin):
+def verify_image_redefined(plugin_name: str, previous_version: str, next_version: str,
+                           raw_plugins: Dict[str, Any], upgrade_plugin: Dict[str, Any]) -> None:
     """
     If some image in "cluster_plugin" is different from image in "base_plugin",
     i.e. redefined, then "upgrade_plugin" should have this image explicitly
     redefined too.
     """
     sensitive_keys = ['image', 'helper-pod-image', 'version']
     for key, value in raw_plugins.items():
@@ -163,49 +164,54 @@
     _, upgrade_plugins = upgrade_plan[0]
     if upgrade_plugins:
         default_merger.merge(inventory.setdefault("plugins", {}), upgrade_plugins)
 
     return inventory
 
 
-def install(cluster: KubernetesCluster, plugins_: Dict[str, dict] = None):
+def _get_plugin_priority(plugin_item: dict, default: int) -> int:
+    priority: int = plugin_item.get("installation", {}).get('priority', default)
+    return priority
+
+
+def install(cluster: KubernetesCluster, plugins_: Dict[str, dict] = None) -> None:
     if plugins_ is None:
         plugins = cluster.inventory["plugins"]
     else:
         plugins = plugins_
     plugins_queue: List[str] = []
     max_priority = 0
     for plugin_name, plugin_item in plugins.items():
         if plugin_item.get("install", False) and plugin_item.get("installation", {}).get('procedures') is not None:
             plugins_queue.append(plugin_name)
             if plugin_item.get("installation", {}).get('priority') is not None \
                     and plugin_item['installation']['priority'] > max_priority:
                 max_priority = plugin_item['installation']['priority']
 
-    plugins_queue.sort(key=lambda name: plugins[name].get("installation", {}).get('priority', max_priority + 1))
+    plugins_queue.sort(key=lambda name: _get_plugin_priority(plugins[name], max_priority + 1))
 
     cluster.log.debug('The following plugins will be installed:')
     for plugin_name in plugins_queue:
         cluster.log.debug('%i. %s' % (
             plugins[plugin_name].get("installation", {}).get('priority', max_priority + 1),
             plugin_name
         ))
 
     cluster.log.debug('Starting plugins installation:')
 
     for plugin_name in plugins_queue:
         install_plugin(cluster, plugin_name, plugins[plugin_name]["installation"]['procedures'])
 
 
-def install_plugin(cluster: KubernetesCluster, plugin_name: str, installation_procedure: List[dict]):
+def install_plugin(cluster: KubernetesCluster, plugin_name: str, installation_procedure: List[dict]) -> None:
     cluster.log.debug("**** INSTALLING PLUGIN %s ****" % plugin_name)
 
     for current_step_i, step in enumerate(installation_procedure):
         for apply_type, configs in step.items():
-            procedure_types()[apply_type]['apply'](cluster, configs, plugin_name)
+            procedure_types()[apply_type]['apply'](cluster, configs)
 
 
 def expect_daemonset(cluster: KubernetesCluster,
                      daemonsets_names: List[Union[str, Dict[str, str]]],
                      timeout: int = None,
                      retries: int = None,
                      node: NodeGroup = None) -> None:
@@ -360,15 +366,15 @@
     raise Exception('In the expected time, the StatefulSets did not become ready. Try to increase number of retries in expect.statefulsets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_deployment(cluster: KubernetesCluster,
                       deployments_names: List[Union[str, Dict[str, str]]],
                       timeout: int = None,
                       retries: int = None,
-                      node: NodeGroup = None):
+                      node: NodeGroup = None) -> None:
     """
     The method waits for the configuration parameters of the given Deployments to be applied.
     :param cluster: KubernetesCluster object where method should be performed
     :param deployments_names: List of Deployments names (or dicts with name and namespace) to be
     expected
     :param timeout: Retry attempt time (seconds)
     :param retries: Number of retry attempts
@@ -408,16 +414,17 @@
             retries -= 1
             cluster.log.debug(f"Deployments are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
     raise Exception('In the expected time, the Deployments did not become ready. Try to increase number of retries in expect.deployments: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
-def expect_pods(cluster: KubernetesCluster, pods: List[str], namespace=None, timeout=None, retries=None,
-                node: NodeGroup = None, apply_filter: str = None):
+def expect_pods(cluster: KubernetesCluster, pods: List[str], namespace: str = None,
+                timeout: int = None, retries: int = None,
+                node: NodeGroup = None, apply_filter: str = None) -> None:
 
     if timeout is None:
         timeout = cluster.inventory['globals']['expect']['pods']['plugins']['timeout']
     if retries is None:
         retries = cluster.inventory['globals']['expect']['pods']['plugins']['retries']
 
     cluster.log.debug("Expecting the following pods to be ready: %s" % pods)
@@ -490,38 +497,38 @@
             cluster.log.debug("Pods are not ready yet... (%ss left)" % (retries * timeout))
             cluster.log.debug(running_pods_stdout)
             time.sleep(timeout)
 
     raise Exception('In the expected time, the pods did not become ready')
 
 
-def is_critical_state_in_stdout(cluster: KubernetesCluster, stdout: str):
+def is_critical_state_in_stdout(cluster: KubernetesCluster, stdout: str) -> bool:
     for state in cluster.globals['pods']['critical_states']:
         if state in stdout:
             return True
     return False
 
 
 # **** TEMPLATES ****
 
-def convert_template(_, config):
+def convert_template(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     return _convert_file(config)
 
 
-def verify_template(_, config: dict):
-    return _verify_file(config, "Template")
+def verify_template(_: KubernetesCluster, config: dict) -> None:
+    _verify_file(config, "Template")
 
 
-def apply_template(cluster: KubernetesCluster, config: dict, plugin_name=None):
-    return _apply_file(cluster, config, "Template")
+def apply_template(cluster: KubernetesCluster, config: dict) -> None:
+    _apply_file(cluster, config, "Template")
 
 
 # **** EXPECT ****
 
-def convert_expect(_, config: dict):
+def convert_expect(_: KubernetesCluster, config: dict) -> dict:
     if config.get('daemonsets') is not None and isinstance(config['daemonsets'], list):
         config['daemonsets'] = {
             'list': config['daemonsets']
         }
     if config.get('replicasets') is not None and isinstance(config['replicasets'], list):
         config['replicasets'] = {
             'list': config['replicasets']
@@ -537,15 +544,15 @@
     if config.get('pods') is not None and isinstance(config['pods'], list):
         config['pods'] = {
             'list': config['pods']
         }
     return config
 
 
-def apply_expect(cluster: KubernetesCluster, config: dict, plugin_name=None):
+def apply_expect(cluster: KubernetesCluster, config: dict) -> None:
     # TODO: Add support for expect services and expect nodes
 
     for expect_type, expect_conf in config.items():
         if expect_type == 'daemonsets':
             expect_daemonset(cluster, config['daemonsets']['list'],
                              timeout=config['daemonsets'].get('timeout'),
                              retries=config['daemonsets'].get('retries'))
@@ -570,29 +577,29 @@
                         timeout=config['pods'].get('timeout'),
                         retries=config['pods'].get('retries'))
 
 # **** PYTHON ****
 
 
 @no_type_check
-def get_python_module(module_path: str):
+def get_python_module(module_path: str) -> ModuleType:
     if module_path in LOADED_MODULES:
         return LOADED_MODULES[module_path]
 
     spec = importlib.util.spec_from_file_location('module', module_path)
     try:
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         LOADED_MODULES[module_path] = module
     except Exception as e:
         raise ValueError(f"Could not import module {module_path}: {e}")
     return module 
 
 
-def get_python_method_args(cluster: KubernetesCluster, step: dict):
+def get_python_method_args(cluster: KubernetesCluster, step: dict) -> Tuple[Callable[..., None], Dict[str, Any]]:
     module_path, _ = utils.determine_resource_absolute_file(step['module'])
     method_name = step['method']
     method_arguments = step.get('arguments', {})
 
     module = get_python_module(module_path)
 
     # Check if the method exists
@@ -610,50 +617,51 @@
         signature.bind(cluster=cluster, **method_arguments)
     except TypeError as e:
         raise ValueError(f"Invalid arguments for method {method_name}: {e}")
 
     return method, method_arguments
 
 
-def verify_python(cluster: KubernetesCluster, step: dict):
+def verify_python(cluster: KubernetesCluster, step: dict) -> None:
     method, method_arguments = get_python_method_args(cluster, step)
     # Additional verification logic can be added here
 
 
-def apply_python(cluster: KubernetesCluster, step: dict, plugin_name=None):
+def apply_python(cluster: KubernetesCluster, step: dict) -> None:
     method, method_arguments = get_python_method_args(cluster, step)
 
-    cluster.log.debug("Running method %s from %s module..." % (method.__name__, method.__module__))
+    func = cast(FunctionType, method)
+    cluster.log.debug("Running method %s from %s module..." % (func.__name__, func.__module__))
     method(cluster, **method_arguments)
 
 
 # **** THIRDPARTIES ****
 
-def verify_thirdparty(cluster: KubernetesCluster, thirdparty: str):
+def verify_thirdparty(cluster: KubernetesCluster, thirdparty: str) -> None:
     defined_thirdparties = list(cluster.inventory['services'].get('thirdparties', {}).keys())
     if thirdparty not in defined_thirdparties:
         raise Exception('Specified thirdparty %s not found in thirdpartirs definition. Expected any of %s.'
                         % (thirdparty, defined_thirdparties))
 
 
-def apply_thirdparty(cluster: KubernetesCluster, thirdparty: str, plugin_name=None):
-    return thirdparties.install_thirdparty(cluster.nodes['all'], thirdparty)
+def apply_thirdparty(cluster: KubernetesCluster, thirdparty: str) -> None:
+    thirdparties.install_thirdparty(cluster.nodes['all'], thirdparty)
 
 
 # **** SHELL ****
 
-def convert_shell(_, config):
+def convert_shell(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     if isinstance(config, str):
         config = {
             'command': config
         }
     return config
 
 
-def verify_shell(cluster: KubernetesCluster, config: dict):
+def verify_shell(cluster: KubernetesCluster, config: dict) -> None:
     out_vars = config.get('out_vars', [])
     groups = config.get('groups', [])
     nodes = config.get('nodes', [])
     explicit_group = cluster.create_group_from_groups_nodes_names(groups, nodes)
     if out_vars and (groups or nodes) and explicit_group.nodes_amount() != 1:
         raise Exception('Shell output variables could be used for single-node groups, but multi-node group was found')
 
@@ -663,15 +671,15 @@
         var_name = var['name']
         if len(words_splitter.split(var_name)) > 1:
             raise Exception(f"'{var_name}' is not a valid shell variable name")
 
     # TODO: verify fields types and contents
 
 
-def apply_shell(cluster: KubernetesCluster, step: dict, plugin_name=None):
+def apply_shell(cluster: KubernetesCluster, step: dict) -> None:
     commands = step['command']
     sudo = step.get('sudo', False)
     groups = step.get('groups', [])
     nodes = step.get('nodes', [])
     in_vars = step.get('in_vars', [])
     out_vars = step.get('out_vars', [])
     vars_separator = "~~~~EXPORTED_VARIABLE~~~~"
@@ -725,39 +733,37 @@
             var = yaml.safe_load(part)
             aliases = out_vars_aliases[var['name']]
             for alias in aliases:
                 cluster.context['runtime_vars'][alias] = var['value']
     else:
         cluster.log.debug(result)
 
-    return result
-
 
 # **** ANSIBLE ****
 
-def convert_ansible(_, config):
+def convert_ansible(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     if isinstance(config, str):
         config = {
             'playbook': config
         }
     return config
 
 
 def _get_absolute_playbook(config: dict) -> str:
     return utils.determine_resource_absolute_file(config['playbook'])[0]
 
 
-def verify_ansible(cluster: KubernetesCluster, config: dict):
+def verify_ansible(cluster: KubernetesCluster, config: dict) -> None:
     _get_absolute_playbook(config)
     if cluster.is_deploying_from_windows():
         raise Exception("Executing of playbooks on Windows deployer is currently not supported")
     # TODO: verify fields types and contents
 
 
-def apply_ansible(cluster: KubernetesCluster, step: dict, plugin_name=None):
+def apply_ansible(cluster: KubernetesCluster, step: dict) -> None:
     playbook_path = _get_absolute_playbook(step)
     external_vars = step.get('vars', {})
     become = step.get('become', False)
     groups = step.get('groups', [])
     nodes = step.get('nodes', [])
 
     command = 'ansible-playbook -i ansible-inventory.ini %s' % playbook_path
@@ -777,18 +783,16 @@
 
     cluster.log.verbose("Running shell \"%s\"" % command)
 
     result = subprocess.run(command, stdout=sys.stdout, stderr=sys.stderr, shell=True)
     if result.returncode != 0:
         raise Exception("Failed to apply ansible plugin, see error above")
 
-    return result
-
 
-def apply_helm(cluster: KubernetesCluster, config: dict, plugin_name=None):
+def apply_helm(cluster: KubernetesCluster, config: dict) -> None:
     chart_path = get_local_chart_path(cluster.log, config)
     process_chart_values(config, chart_path)
 
     from kubemarine import kubernetes
     local_config_path = kubernetes.fetch_admin_config(cluster)
 
     with utils.open_external(os.path.join(chart_path, 'Chart.yaml'), 'r') as stream:
@@ -819,18 +823,16 @@
         cluster.log.debug("Deployed release %s is not found. Installing it..." % release)
         deployment_mode = "install"
 
     command = prepare_for_helm_command + f'{deployment_mode} {release} {chart_path} --create-namespace --debug'
     output = subprocess.check_output(command, shell=True)
     cluster.log.debug(output.decode('utf-8'))
 
-    return output
-
 
-def process_chart_values(config: dict, local_chart_path: str):
+def process_chart_values(config: dict, local_chart_path: str) -> None:
     config_values = config.get("values")
     file_values = None
     config_values_file = config.get("values_file")
     if config_values_file is not None:
         with utils.open_external(config_values_file) as stream:
             file_values = yaml.safe_load(stream)
 
@@ -846,95 +848,95 @@
     # Values from 'values' section have priority over values in 'values_file' section
     if config_values is not None:
         merged_values = default_merger.merge(merged_values, config_values)
 
     utils.dump_file({}, yaml.dump(merged_values), chart_values, dump_location=False)
 
 
-def get_local_chart_path(log, config: dict):
+def get_local_chart_path(logger: log.EnhancedLogger, config: dict) -> str:
     chart_path = config['chart_path']
 
     is_curl = chart_path[:4] == 'http' and '://' in chart_path[4:8]
 
     local_chart_folder = "local_chart_folder"
     if os.path.isdir(local_chart_folder):
         remove_tree(local_chart_folder)
     mkpath(local_chart_folder)
     if is_curl:
-        log.verbose('Chart download via curl detected')
+        logger.verbose('Chart download via curl detected')
         destination = os.path.basename(chart_path)
 
         ctx = ssl.create_default_context()
         ctx.check_hostname = False
         # todo probably add option which will manage if certificate should be verified?
         ctx.verify_mode = ssl.CERT_NONE
         with urllib.request.urlopen(chart_path, context=ctx) as u, \
                 open(destination, 'wb') as f:
             shutil.copyfileobj(u, f)
 
         extension = destination.split('.')[-1]
         if extension == 'zip':
-            log.verbose('Unzip will be used for unpacking')
+            logger.verbose('Unzip will be used for unpacking')
             with zipfile.ZipFile(destination, 'r') as zf:
                 zf.extractall(local_chart_folder)
         else:
-            log.verbose('Tar will be used for unpacking')
+            logger.verbose('Tar will be used for unpacking')
             with tarfile.open(destination, "r:gz") as tf:
                 tf.extractall(local_chart_folder)
     else:
-        log.debug("Create copy of chart to work with")
+        logger.debug("Create copy of chart to work with")
         copy_tree(chart_path, local_chart_folder)
 
     # Find all Chart.yaml files in the chart.
     glob_search = os.path.join(local_chart_folder, '**', 'Chart.yaml')
     chart_metadata = glob.glob(glob_search, recursive=True)
     if not chart_metadata:
         raise Exception("Incorrect format of helm chart: Chart.yaml not found")
 
     # Sort by number of parts in path to find outermost Chart.yaml
     chart_metadata.sort(key=lambda path: len(path.split(os.sep)))
     local_chart_folder = os.path.dirname(chart_metadata[0])
-    log.debug("Detected chart path = %s" % local_chart_folder)
+    logger.debug("Detected chart path = %s" % local_chart_folder)
 
     # Check all nested Chart.yaml are inside chart path
     for i in range(1, len(chart_metadata)):
         if not os.path.commonpath([chart_metadata[i], local_chart_folder]) == local_chart_folder:
             raise Exception(
                 f"Incorrect format of helm chart: inner {chart_metadata[i]} is not inside {local_chart_folder} directory.")
 
     return local_chart_folder
 
 
-def convert_config(_, config):
+def convert_config(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     return _convert_file(config)
 
 
-def verify_config(_, config: dict):
-    return _verify_file(config, "Config")
+def verify_config(_: KubernetesCluster, config: dict) -> None:
+    _verify_file(config, "Config")
 
 
-def apply_config(cluster: KubernetesCluster, config: dict, plugin_name=None):
-    return _apply_file(cluster, config, "Config")
+def apply_config(cluster: KubernetesCluster, config: dict) -> None:
+    _apply_file(cluster, config, "Config")
 
 
-def _convert_file(config):
+def _convert_file(config: Union[str, dict]) -> dict:
     if isinstance(config, str):
         config = {
             'source': config
         }
     return config
 
 
 def get_source_absolute_pattern(config: dict) -> Tuple[str, bool]:
     abs_dir, is_external = utils.determine_resource_absolute_dir(config['source'])
     basename = os.path.basename(config['source'])
     return os.path.join(abs_dir, basename), is_external
 
 
-def _verify_file(config: dict, file_type: str):
+def _verify_file(config: dict, file_type: str) -> None:
     """
         Verifies if the path matching the config 'source' key exists and points to
         existing files.
     """
 
     # Determite absolute path to templates
     source, _ = get_source_absolute_pattern(config)
```

### Comparing `kubemarine-0.19.0/kubemarine/plugins/builtin.py` & `kubemarine-0.20.0/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/calico.py` & `kubemarine-0.20.0/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.20.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.20.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/manifest.py` & `kubemarine-0.20.0/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.20.0/kubemarine/plugins/nginx_ingress.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.20.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/__init__.py` & `kubemarine-0.20.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/add_node.py` & `kubemarine-0.20.0/kubemarine/procedures/add_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
+import collections
 import copy
-import typing
 
-from collections import OrderedDict
-from typing import Any
+from typing import Any, OrderedDict, List
 
 from kubemarine import kubernetes, packages
 from kubemarine.core import flow, utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 
 
-def deploy_kubernetes_join(cluster: KubernetesCluster):
+def deploy_kubernetes_join(cluster: KubernetesCluster) -> None:
 
     group = cluster.make_group_from_roles(['control-plane', 'worker']).get_new_nodes()
 
     if group.is_empty():
         cluster.log.debug("No kubernetes nodes to perform")
         return
 
@@ -48,15 +45,15 @@
     ])
 
     cluster.log.debug("Waiting for new kubernetes nodes...")
     kubernetes.wait_for_nodes(group)
     kubernetes.schedule_running_nodes_report(cluster)
 
 
-def add_node_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def add_node_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     if cluster.context.get('initial_procedure') != 'add_node':
         return inventory_to_finalize
 
     new_nodes = cluster.nodes['all'].get_new_nodes()
 
     # add nodes to inventory if they in new nodes
     for new_node in new_nodes.get_ordered_members_list():
@@ -89,41 +86,41 @@
     # maybe merge vrrp ips only when adding?
     if "vrrp_ips" in cluster.procedure_inventory:
         utils.merge_vrrp_ips(cluster.procedure_inventory, inventory_to_finalize)
 
     return inventory_to_finalize
 
 
-def cache_installed_packages(cluster: KubernetesCluster):
+def cache_installed_packages(cluster: KubernetesCluster) -> None:
     """
     Task which is used to collect already installed packages versions on already existing nodes.
     It is called first during "add_node" procedure,
     so that new nodes install exactly the same packages as on other already existing nodes.
     """
     packages.cache_package_versions(cluster, cluster.inventory, by_initial_nodes=True)
 
 
-tasks: typing.OrderedDict[str, Any] = OrderedDict(copy.deepcopy(install.tasks))
+tasks: OrderedDict[str, Any] = collections.OrderedDict(copy.deepcopy(install.tasks))
 del tasks["deploy"]["plugins"]
 del tasks["deploy"]["accounts"]
 tasks["deploy"]["kubernetes"]["init"] = deploy_kubernetes_join
 tasks["cache_packages"] = cache_installed_packages
 tasks.move_to_end("cache_packages", last=False)
 
 
 class AddNodeAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('add node', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks, cumulative_points=install.cumulative_points)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     cli_help = '''
     Script for adding node to Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/backup.py` & `kubemarine-0.20.0/kubemarine/procedures/backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 import json
 import os
 import random
 import shutil
 import tarfile
 import time
 from collections import OrderedDict
-from typing import List
+from typing import List, Tuple
 
 import yaml
 
-from kubemarine.core import utils, flow
+from kubemarine.core import utils, flow, log
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 
 
-def get_default_backup_files_list(cluster: KubernetesCluster):
+def get_default_backup_files_list(cluster: KubernetesCluster) -> List[str]:
     haproxy_service = cluster.get_package_association('haproxy', 'service_name')
     keepalived_service = cluster.get_package_association('keepalived', 'service_name')
 
     backup_files_list = [
         "/etc/resolv.conf",
         "/etc/hosts",
         "/etc/chrony.conf",
@@ -63,67 +63,67 @@
     elif cri_impl == "containerd":
         backup_files_list.append("/etc/containerd/config.toml")
         backup_files_list.append("/etc/crictl.yaml")
 
     return backup_files_list
 
 
-def prepare_backup_tmpdir(cluster: KubernetesCluster):
+def prepare_backup_tmpdir(cluster: KubernetesCluster) -> str:
     backup_directory = cluster.context.get('backup_tmpdir')
     if not backup_directory:
         cluster.log.verbose('Backup directory is not ready yet, preparing..')
         backup_directory = cluster.context['backup_tmpdir'] = utils.get_dump_filepath(cluster.context, 'backup')
         shutil.rmtree(backup_directory, ignore_errors=True)
         os.mkdir(backup_directory)
         cluster.log.verbose('Backup directory prepared')
     return backup_directory
 
 
-def verify_backup_location(cluster: KubernetesCluster):
+def verify_backup_location(cluster: KubernetesCluster) -> None:
     target = utils.get_external_resource_path(cluster.procedure_inventory.get('backup_location', 'backup.tar.gz'))
     if not os.path.isdir(target) and not os.path.isdir(os.path.abspath(os.path.join(target, os.pardir))):
         raise FileNotFoundError('Backup location directory not exists')
 
 
-def export_ansible_inventory(cluster: KubernetesCluster):
+def export_ansible_inventory(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
     shutil.copyfile(cluster.context['execution_arguments']['ansible_inventory_location'],
                     os.path.join(backup_directory, 'ansible-inventory.ini'))
     cluster.log.verbose('ansible-inventory.ini exported to backup')
 
 
-def export_packages_list(cluster: KubernetesCluster):
+def export_packages_list(cluster: KubernetesCluster) -> None:
     cluster.context['backup_descriptor']['nodes']['packages'] = {}
     if cluster.get_os_family() in ['rhel', 'rhel8']:
         cmd = r"rpm -qa"
     else:
         cmd = r"dpkg-query -f '${Package}=${Version}\n' -W"
     results = cluster.nodes['all'].sudo(cmd)
     for host, result in results.items():
         cluster.context['backup_descriptor']['nodes']['packages'][host] = result.stdout.strip().split('\n')
 
 
-def export_hostname(cluster: KubernetesCluster):
+def export_hostname(cluster: KubernetesCluster) -> None:
     cluster.context['backup_descriptor']['nodes']['hostnames'] = {}
     results = cluster.nodes['all'].sudo('hostnamectl status | head -n 1 | sed -e \'s/[a-zA-Z ]*://g\'')
     cluster.log.verbose(results)
     for host, result in results.items():
         cluster.context['backup_descriptor']['nodes']['hostnames'][host] = result.stdout.strip()
 
 
-def export_cluster_yaml(cluster: KubernetesCluster):
+def export_cluster_yaml(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
     shutil.copyfile(utils.get_dump_filepath(cluster.context, 'cluster.yaml'),
                     os.path.join(backup_directory, 'cluster.yaml'))
     shutil.copyfile(utils.get_external_resource_path(cluster.context['execution_arguments']['config']),
                     os.path.join(backup_directory, 'original_cluster.yaml'))
     cluster.log.verbose('cluster.yaml exported to backup')
 
 
-def export_nodes(cluster: KubernetesCluster):
+def export_nodes(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
     backup_nodes_data_dir = os.path.join(backup_directory, 'nodes_data')
     os.mkdir(backup_nodes_data_dir)
 
     backup_list = get_default_backup_files_list(cluster)
     for filepath, enabled in cluster.procedure_inventory.get('backup_plan', {}).get('nodes', {}).items():
         if not enabled and filepath in backup_list:
@@ -148,26 +148,26 @@
                  os.path.join(backup_nodes_data_dir, '%s.tar.gz' % node.get_node_name()))
         cluster.log.debug('Backup \'%s\' downloaded' % node.get_node_name())
 
     cluster.log.verbose('Deleting backup file from nodes...')
     cluster.nodes['all'].sudo('rm -f /tmp/kubemarine-backup.tar.gz')
 
 
-def export_etcd(cluster: KubernetesCluster):
+def export_etcd(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
     etcd_node, is_custom_etcd_node = select_etcd_node(cluster)
     cluster.context['backup_descriptor']['etcd']['image'] = retrieve_etcd_image(cluster, etcd_node)
 
     # Try to detect cluster health and other metadata like db size, leader
     etcd_status = None
     try:
-        result = etcd_node.sudo('etcdctl endpoint status --cluster -w json').get_simple_out()
-        cluster.log.verbose(result)
+        status_json = etcd_node.sudo('etcdctl endpoint status --cluster -w json').get_simple_out()
+        cluster.log.verbose(status_json)
 
-        etcd_status = json.load(io.StringIO(result.lower()))
+        etcd_status = json.load(io.StringIO(status_json.lower()))
         parsed_etcd_status = {}
         for item in etcd_status:
             # get rid of https:// and :2379
             address = item['endpoint'].split('//')[1].split(':')[0]
             node_name = cluster.nodes['all'].get_first_member(apply_filter={"internal_address": address}).get_node_name()
             parsed_etcd_status[node_name] = item
         cluster.context['backup_descriptor']['etcd']['status'] = parsed_etcd_status
@@ -202,27 +202,27 @@
                             f'&& sudo chmod 666 /tmp/{snap_name}', timeout=600)
     cluster.log.debug(result)
     etcd_node.get('/tmp/' + snap_name, backup_directory + '/etcd.db')
     cluster.log.verbose('Deleting ETCD snapshot file from "%s"...')
     etcd_node.sudo('rm -f /tmp/%s' % snap_name)
 
 
-def select_etcd_node(cluster: KubernetesCluster):
+def select_etcd_node(cluster: KubernetesCluster) -> Tuple[NodeGroup, bool]:
     custom_etcd_node = cluster.procedure_inventory.get('backup_plan', {}).get('etcd', {}).get('source_node')
 
     if custom_etcd_node:
         if not cluster.nodes['all'].has_node(custom_etcd_node):
             raise Exception('Unknown ETCD node selected as source')
         etcd_node = cluster.nodes['all'].get_member_by_name(custom_etcd_node)
         return etcd_node, True
     else:
         return cluster.nodes['control-plane'].get_any_member(), False
 
 
-def retrieve_etcd_image(cluster: KubernetesCluster, etcd_node: NodeGroup):
+def retrieve_etcd_image(cluster: KubernetesCluster, etcd_node: NodeGroup) -> str:
     # TODO: Detect ETCD version via /etc/kubernetes/manifests/etcd.yaml config if presented, otherwise use containers
     node_name = etcd_node.get_node_name()
     if "docker" == cluster.inventory['services']['cri']['containerRuntime']:
         cont_inspect = "docker inspect $(sudo docker ps -a | grep etcd-%s | awk '{print $1; exit}')" % node_name
         etcd_container_json = json.loads(list(etcd_node.sudo(cont_inspect).values())[0].stdout)[0]
         etcd_image_sha = etcd_container_json['Image'][7:]  # remove "sha256:" prefix
 
@@ -237,36 +237,37 @@
         cont_inspect = f"crictl inspect $({cont_search})"
         etcd_container_json = json.loads(list(etcd_node.sudo(cont_inspect).values())[0].stdout)
         etcd_image_sha = etcd_container_json['info']['config']['image']['image']
 
         images_json = json.loads(list(etcd_node.sudo("crictl images -v -o json").values())[0].stdout)['images']
         for image in images_json:
             if image['id'] == etcd_image_sha:
-                return image['repoTags'][0]
+                return f"{image['repoTags'][0]}"
 
     raise Exception("Unable to find etcd image on node %s" % node_name)
 
 
-def export_kubernetes_version(cluster: KubernetesCluster):
+def export_kubernetes_version(cluster: KubernetesCluster) -> None:
     control_plane = cluster.nodes['control-plane'].get_any_member()
     version = control_plane.sudo('kubectl get nodes --no-headers | head -n 1 | awk \'{print $5; exit}\'').get_simple_out()
     cluster.context['backup_descriptor']['kubernetes']['version'] = version.strip()
 
 
 # There is no way to parallel resources connection via Queue or Pool:
 # the ssh connection is not possible to parallelize due to thread lock
-def download_resources(log, resources: List[str], location, control_plane: NodeGroup, namespace=None):
+def download_resources(logger: log.EnhancedLogger, resources: List[str], location: str, control_plane: NodeGroup,
+                       namespace: str = None) -> List[str]:
 
     if namespace:
-        log.debug('Downloading resources from namespace "%s"...' % namespace)
+        logger.debug('Downloading resources from namespace "%s"...' % namespace)
 
     actual_resources: List[str] = []
 
     if not resources:
-        log.debug('No resources found to download')
+        logger.debug('No resources found to download')
         return actual_resources
 
     cmd = ''
     resource_separator = ''.join(random.choice('=-_') for _ in range(32))
 
     for resource in resources:
         if cmd != '':
@@ -287,15 +288,15 @@
         if result and result != '':
             actual_resources.append(resource)
             utils.dump_file({}, result, resource_file_path, dump_location=False)
 
     return actual_resources
 
 
-def export_kubernetes(cluster: KubernetesCluster):
+def export_kubernetes(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
     control_plane = cluster.nodes['control-plane'].get_any_member()
 
     cluster.log.debug('Loading namespaces:')
     namespaces_result = control_plane.sudo('kubectl get ns -o yaml')
     cluster.log.verbose(namespaces_result)
     namespaces_string = list(namespaces_result.values())[0].stdout.strip()
@@ -379,25 +380,25 @@
     if namespaced_resources_map:
         cluster.context['backup_descriptor']['kubernetes']['resources']['namespaced'] = namespaced_resources_map
 
     if nonnamespaced_resources_list:
         cluster.context['backup_descriptor']['kubernetes']['resources']['nonnamespaced'] = nonnamespaced_resources_list
 
 
-def make_descriptor(cluster: KubernetesCluster):
+def make_descriptor(cluster: KubernetesCluster) -> None:
     backup_directory = prepare_backup_tmpdir(cluster)
 
     cluster.context['backup_descriptor']['kubernetes']['thirdparties'] = cluster.inventory['services']['thirdparties']
     cluster.context['backup_descriptor']['meta']['time']['finished'] = datetime.datetime.now()
 
     with utils.open_external(os.path.join(backup_directory, 'descriptor.yaml'), 'w') as output:
         output.write(yaml.dump(cluster.context['backup_descriptor']))
 
 
-def pack_data(cluster: KubernetesCluster):
+def pack_data(cluster: KubernetesCluster) -> None:
     cluster_name = cluster.inventory['cluster_name']
     backup_directory = prepare_backup_tmpdir(cluster)
 
     backup_filename = 'backup-%s-%s.tar.gz' % (cluster_name, utils.get_current_timestamp_formatted())
 
     target = utils.get_external_resource_path(cluster.procedure_inventory.get('backup_location', backup_filename))
     if os.path.isdir(target):
@@ -433,22 +434,22 @@
     },
     "make_descriptor": make_descriptor,
     "pack": pack_data,
 })
 
 
 class BackupAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('backup')
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
     Script for making backup of Kubernetes resources and nodes contents.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.20.0/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.20.0/kubemarine/procedures/check_iaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.core.group import NodeConfig, GroupException, GroupResultException, CollectorCallback
 
 
-def connection_ssh_connectivity(cluster: KubernetesCluster):
+def connection_ssh_connectivity(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '001', 'SSH', 'Connectivity', default_results='Connected'):
         failed_nodes = []
         for node in cluster.nodes['all'].get_ordered_members_list():
             try:
                 cluster.log.verbose(node.run("echo 1"))
             except GroupException as e:
                 failed_nodes.append(node.get_node_name())
@@ -49,15 +49,15 @@
         if failed_nodes:
             raise TestFailure("Failed to connect to %s nodes" % len(failed_nodes),
                               hint="Failed to connect from the deploy node to the remote node of the cluster. Check that "
                                    "the inventory details (key, username, and nodes addresses) are entered correctly, and verify "
                                    "the access to remote nodes.")
 
 
-def connection_ssh_latency_single(cluster: KubernetesCluster):
+def connection_ssh_latency_single(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '002',  'SSH', 'Latency - Single Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 5:
             i += 1
@@ -77,15 +77,15 @@
         if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
-def connection_ssh_latency_multiple(cluster: KubernetesCluster):
+def connection_ssh_latency_multiple(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '003',  'SSH', 'Latency - Multi Thread',
                   minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical'],
                   recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']) as tc:
         i = 0
         measurements = []
         while i < 10:
             i += 1
@@ -104,30 +104,30 @@
         if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
                                 "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
-def connection_sudoer_access(cluster: KubernetesCluster):
+def connection_sudoer_access(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '004', 'SSH', 'Sudoer Access', default_results='Access provided'):
         non_root = []
         for host, node_context in cluster.context['nodes'].items():
             access_info = node_context['access']
             if access_info['online'] and access_info['sudo'] == 'Root':
                 cluster.log.debug("%s online and has root" % host)
             else:
                 non_root.append(host)
         if non_root:
             raise TestFailure("Non-sudoer access found at: %s" % ", ".join(non_root),
                               hint="Certain nodes do not have the appropriate sudoer access. At these nodes, add "
                                    "a connection user to the sudoers group.")
 
 
-def hardware_members_amount(cluster: KubernetesCluster, group_name: str):
+def hardware_members_amount(cluster: KubernetesCluster, group_name: str) -> None:
     beauty_name = group_name.capitalize()
     if group_name == 'vip':
         beauty_name = 'VIP'
     if group_name == 'all':
         beauty_name = 'Total Node'
 
     with TestCase(cluster, '005',  'Hardware', '%ss Amount' % beauty_name,
@@ -160,15 +160,15 @@
             raise TestWarn("Less than recommended. Detected %s item%s" % (amount, s),
                            hint="Increase the number of resources, so that the number of %ss in the cluster should not "
                                 "be less than %s." % (beauty_name, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount']))
 
         tc.success("%s item%s" % (amount, s))
 
 
-def hardware_cpu(cluster: KubernetesCluster, group_name: str):
+def hardware_cpu(cluster: KubernetesCluster, group_name: str) -> None:
     minimal_cpu = cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'] \
         if group_name == 'balancer' or cluster.nodes['all'].nodes_amount() > 1 \
         else cluster.globals['compatibility_map']['hardware']['minimal']['control-plane']['vcpu']
     with TestCase(cluster, '006',  'Hardware', 'VCPUs Amount - %ss' % group_name.capitalize(),
                   minimal=minimal_cpu,
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
@@ -200,15 +200,15 @@
         if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']:
             raise TestWarn("Less than recommended. Detected %s VCPU%s" % (minimal_amount, s),
                            hint="Increase the number of VCPUs in the node configuration up to %s VCPUs."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'])
         tc.success(results='%s VCPU%s' % (minimal_amount, s))
 
 
-def hardware_ram(cluster: KubernetesCluster, group_name: str):
+def hardware_ram(cluster: KubernetesCluster, group_name: str) -> None:
     with TestCase(cluster, '007',  'Hardware', 'RAM Amount - %ss' % group_name.capitalize(),
                   minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'],
                   recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']) as tc:
         if cluster.nodes.get(group_name) is None or cluster.nodes[group_name].is_empty():
             return tc.success(results='Skipped')
         results = cluster.nodes[group_name].sudo("cat /proc/meminfo | awk '/DirectMap/ { print $2 }'")
         cluster.log.verbose(results)
@@ -232,15 +232,15 @@
         if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']:
             raise TestWarn("Less than recommended. Detected %sGB" % minimal_amount,
                            hint="Increase the number of RAM in the node configuration up to %s GB."
                                 % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'])
         tc.success(results='%sGB' % minimal_amount)
 
 
-def system_distributive(cluster: KubernetesCluster):
+def system_distributive(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '008', 'System', 'Distibutive') as tc:
         supported_distributives = cluster.globals['compatibility_map']['distributives'].keys()
 
         cluster.log.debug(system.fetch_os_versions(cluster))
 
         detected_unsupported_os = []
         detected_supported_os = []
@@ -284,15 +284,15 @@
                 f"Nodes have different OS families or versions. "
                 f"List of (OS family, version): {list(different_os)}")
             raise TestWarn(f"Nodes have different OS families or versions")
         
         tc.success(results=", ".join(detected_supported_os))
 
 
-def check_kernel_version(cluster: KubernetesCluster):
+def check_kernel_version(cluster: KubernetesCluster) -> None:
     """
     This method compares the linux kernel version with the bad version
     """
     with TestCase(cluster, '015', "Software", "Kernel version") as tc:
         bad_results = {}
         unstable_kernel_ubuntu: List[str] = cluster.globals['compatibility_map']['distributives']['ubuntu'][0].get('unstable_kernel')
         unstable_kernel_centos: List[str] = []
@@ -313,15 +313,15 @@
                 cluster.log.debug(f"Unstable kernel %s on: %s" % (kernel_version, host))
             cluster.log.debug(f"Update the linux kernel version to 5.4.0-135-generic")
             raise TestWarn("Kernel version unstable")
         else:
             tc.success("All kernel have stable versions")
 
 
-def check_access_to_thirdparties(cluster: KubernetesCluster):
+def check_access_to_thirdparties(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '012', 'Software', 'Thirdparties Availability') as tc:
         detect_preinstalled_python(cluster)
         broken = []
         nodes_without_python = set()
 
         # Load script for checking sources
         all_group = cluster.nodes['all']
@@ -350,19 +350,19 @@
         rm_command = "rm %s" % random_temp_path
         all_group.run(rm_command)
 
         if broken:
             raise TestFailure('Required thirdparties are unavailable', hint=yaml.safe_dump(broken))
         if nodes_without_python:
             raise TestWarn("Can't detect python version for some nodes, procedure can't be performed for them",
-                           hint=list(nodes_without_python))
+                           hint=yaml.safe_dump(list(nodes_without_python)))
         tc.success('All thirdparties are available')
 
 
-def check_resolv_conf(cluster: KubernetesCluster):
+def check_resolv_conf(cluster: KubernetesCluster) -> None:
     nodes_context = cluster.context['nodes']
     hosts = [host for host, node_context in nodes_context.items() if 'resolv_conf_is_actual' not in node_context]
     group = cluster.make_group(hosts)
 
     if cluster.inventory["services"].get("resolv.conf") is None:
         for host in hosts:
             nodes_context[host]["resolv_conf_is_actual"] = True
@@ -380,15 +380,15 @@
 
         for host, res in results.items():
             nodes_context[host]["resolv_conf_is_actual"] = not res.failed
         # Remove temp resolv.conf file
         group.run("rm %s" % random_resolv_conf_path)
 
 
-def check_package_repositories(cluster: KubernetesCluster):
+def check_package_repositories(cluster: KubernetesCluster) -> None:
     nodes_context = cluster.context['nodes']
     hosts = [host for host, node_context in nodes_context.items() if 'package_repos_are_actual' not in node_context]
 
     repositories = cluster.inventory['services']['packages']['package_manager'].get("repositories")
     if repositories is None:
         for host in hosts:
             nodes_context[host]["package_repos_are_actual"] = True
@@ -411,15 +411,15 @@
         for host, result in collector.result.items():
             nodes_context[host]["package_repos_are_actual"] = not result.failed
 
         # Remove temp .repo file
         group.sudo("rm %s" % random_repos_conf_path)
 
 
-def check_access_to_package_repositories(cluster: KubernetesCluster):
+def check_access_to_package_repositories(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '013', 'Software', 'Package Repositories') as tc:
         detect_preinstalled_python(cluster)
         check_resolv_conf(cluster)
         broken = []
         warnings = []
 
         # Collect repository urls
@@ -504,15 +504,15 @@
         if broken:
             raise TestFailure('Found problems for package repositories', hint=yaml.safe_dump(broken))
         elif warnings:
             raise TestWarn('Found potential problems for package repositories or nodes', hint=yaml.safe_dump(warnings))
         tc.success('All package repositories are correct and available')
 
 
-def check_access_to_packages(cluster: KubernetesCluster):
+def check_access_to_packages(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '014', 'Software', 'Package Availability') as tc:
         check_package_repositories(cluster)
         broken: List[str] = []
         warnings: List[str] = []
         group = cluster.nodes['all']
         hosts_to_packages = packages.get_all_managed_packages_for_group(group, cluster.inventory)
         collector = CollectorCallback(cluster)
@@ -544,15 +544,15 @@
         if broken:
             raise TestFailure('Required packages are unavailable', hint=yaml.safe_dump(broken))
         elif warnings:
             raise TestWarn('Found potential problems for packages', hint=yaml.safe_dump(warnings))
         tc.success('All packages are available')
 
 
-def detect_preinstalled_python(cluster: KubernetesCluster):
+def detect_preinstalled_python(cluster: KubernetesCluster) -> None:
     version_pattern = r'^Python{space}([2-3])(\.[0-9]+){{0,2}}$'
     bash_version_pattern = version_pattern.format(space='[[:space:]]')
     python_version_pattern = version_pattern.format(space=' ')
     nodes_context = cluster.context['nodes']
     hosts_unknown_python = [host for host, node_context in nodes_context.items() if 'python' not in node_context]
     group_unknown_python = cluster.make_group(hosts_unknown_python)
     detected_python = group_unknown_python.run(
@@ -571,15 +571,15 @@
             nodes_context[host]["python"] = {
                 "executable": executable,
                 "major_version": version
             }
 
 
 @contextmanager
-def suspend_firewalld(cluster: KubernetesCluster):
+def suspend_firewalld(cluster: KubernetesCluster) -> Iterator[None]:
     firewalld_statuses = system.fetch_firewalld_status(cluster.nodes["all"])
     stop_firewalld_group = firewalld_statuses.get_nodes_group_where_value_in_stdout("active (running)")
 
     nodes_to_rollback = cluster.make_group([])
     try:
         try:
             nodes_to_rollback = system.stop_service(stop_firewalld_group, "firewalld").get_group()
@@ -601,15 +601,15 @@
             continue
         nodes[node["connect_to"]] = node
 
     return nodes
 
 
 @contextmanager
-def assign_random_ips(cluster: KubernetesCluster, nodes: Dict[str, NodeConfig], subnet) -> Iterator[Dict[str, Any]]:
+def assign_random_ips(cluster: KubernetesCluster, nodes: Dict[str, NodeConfig], subnet: str) -> Iterator[Dict[str, Any]]:
     inet = ipaddress.ip_network(subnet)
     net_mask = str(inet.netmask)
     prefix = str(inet.prefixlen)
     subnet_hosts = []
     ip_numbers = 0
     for addr in inet.hosts():
         subnet_hosts.append(addr)
@@ -672,15 +672,15 @@
                           warn=True)
 
     if skipped_nodes:
         raise TestWarn(f"Cannot perform check on {skipped_nodes}: subnet is already in use. "
                        f"Use check_paas procedure if you already have installed cluster.")
 
 
-def pod_subnet_connectivity(cluster: KubernetesCluster):
+def pod_subnet_connectivity(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '009', 'Network', 'PodSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         pod_subnet = cluster.inventory['services']['kubeadm']['networking']['podSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, pod_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
@@ -688,15 +688,15 @@
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Traffic is not allowed for the pod subnet({pod_subnet}) "
                                        f"on nodes: {failed_nodes}.")
 
 
-def service_subnet_connectivity(cluster: KubernetesCluster):
+def service_subnet_connectivity(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '010', 'Network', 'ServiceSubnet', default_results='Connected'),\
             suspend_firewalld(cluster):
         service_subnet = cluster.inventory['services']['kubeadm']['networking']['serviceSubnet']
         nodes = _get_not_balancers(cluster)
         tcp_ports = ["30050"]
         with assign_random_ips(cluster, nodes, service_subnet) as host_to_ip, \
                 install_tcp_listener(cluster, nodes, tcp_ports):
@@ -704,32 +704,32 @@
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Traffic is not allowed for the service subnet({service_subnet}) "
                                        f"on nodes: {failed_nodes}.")
 
 
-def cmd_for_ports(ports, query):
+def cmd_for_ports(ports: List[str], query: str) -> str:
     result = ""
     for port in ports:
         result += f" && echo 'port: {port}' && ( {query % port} ) "
     return result[3:]
 
 
 def tcp_connect(cluster: KubernetesCluster, node_from: NodeConfig, node_to: NodeConfig,
-                tcp_ports: List[str], host_to_ip: Dict[str, Any], mtu):
+                tcp_ports: List[str], host_to_ip: Dict[str, Any], mtu: int) -> None:
     # 40 bites for headers
     mtu -= 40
     cluster.log.verbose(f"Trying connection from '{node_from['name']}' to '{node_to['name']}")
     cmd = cmd_for_ports(tcp_ports, f"echo $(dd if=/dev/urandom bs={mtu}  count=1) >/dev/tcp/{host_to_ip[node_to['connect_to']]}/%s")
     group = cluster.make_group([node_from['connect_to']])
     group.sudo(cmd, timeout=cluster.globals['connection']['defaults']['timeout'])
 
 
-def get_start_tcp_listener_cmd(python_executable, tcp_listener, ip_version):
+def get_start_tcp_listener_cmd(python_executable: str, tcp_listener: str, ip_version: int) -> str:
     # 1. Create anonymous pipe
     # 2. Create python tcp listener process in background and redirect output to pipe
     # 3. Wait till the listener successfully binds the port, or till it fails and exits.
     #    Read one line from pipe to check that.
     # 4. Exit with success or fail correspondingly.
     return "PORT=%s; PIPE=$(mktemp -u); mkfifo $PIPE; exec 3<>$PIPE; rm $PIPE; " \
            f"sudo nohup {python_executable} {tcp_listener} $PORT {ip_version} >&3 2>&1 & " \
@@ -745,22 +745,22 @@
                "exit 0; " \
            "fi; " \
            "DATA=$(echo $DATA && dd iflag=nonblock status=none <&3 2>/dev/null); " \
            "echo \"$DATA\" >&2 ; " \
            "exit 1"
 
 
-def get_stop_tcp_listener_cmd(tcp_listener):
+def get_stop_tcp_listener_cmd(tcp_listener: str) -> str:
     identify_pid = "ps aux | grep \" %s ${port} \" | grep -v grep | grep -v nohup | awk '{print $2}'" % tcp_listener
     return f"port=%s;pid=$({identify_pid}) " \
            "&& if [ ! -z $pid ]; then sudo kill -9 $pid; echo \"killed pid $pid for port $port\"; fi"
 
 
 def check_tcp_connect_between_all_nodes(cluster: KubernetesCluster, node_list: List[NodeConfig],
-                                        tcp_ports: List[str], host_to_ip: Dict[str, Any]):
+                                        tcp_ports: List[str], host_to_ip: Dict[str, Any]) -> List[str]:
     if len(node_list) <= 1:
         return []
 
     mtu = cluster.inventory['plugins']['calico']['mtu']
 
     cluster.log.verbose("Searching for success node...")
     success_node = None
@@ -798,15 +798,16 @@
                 cluster.log.error(f"Subnet connectivity test failed from '{success_node['name']}' to '{node['name']}'")
                 cluster.log.verbose(f"Exception details: {e}")
 
     return failed_nodes
 
 
 @contextmanager
-def install_tcp_listener(cluster: KubernetesCluster, nodes: Dict[str, NodeConfig], tcp_ports):
+def install_tcp_listener(cluster: KubernetesCluster,
+                         nodes: Dict[str, NodeConfig], tcp_ports: List[str]) -> Iterator[None]:
     detect_preinstalled_python(cluster)
     nodes_without_python = {node_config['name']: node_config for host, node_config in nodes.items()
                             if cluster.context['nodes'][host]['python'] == "Not installed"}
     for node_nonfig in nodes_without_python.values():
         del nodes[node_nonfig['connect_to']]
 
     # currently tcp listener can be run on both python 2 and 3
@@ -859,15 +860,15 @@
                        f"Use check_paas procedure if you already have installed cluster.")
 
     if nodes_without_python:
         cluster.log.warning(f"Nodes without python: {nodes_without_python.keys()}")
         raise TestWarn(f"Cannot perform check on {list(nodes_without_python.keys())}: python doesn't exist.")
 
 
-def check_tcp_ports(cluster: KubernetesCluster):
+def check_tcp_ports(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '011', 'Network', 'TCPPorts', default_results='Connected'),\
             suspend_firewalld(cluster):
         tcp_ports = ["80", "443", "179", "5473", "6443", "8443", "2379", "2380", "9091", "9094", "10250", "10254",
                      "10257", "10259", "30001", "30002"]
         nodes = {node["connect_to"]: node
                  for node in cluster.inventory['nodes']}
         host_to_ip = {host: node['internal_address'] for host, node in nodes.items()}
@@ -876,15 +877,15 @@
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Not all needed tcp ports are opened on nodes: {failed_nodes}. "
                                        f"Ports that should be opened: {tcp_ports}")
 
 
-def make_reports(context: dict):
+def make_reports(context: dict) -> None:
     if not context['execution_arguments'].get('disable_csv_report', False):
         context['testsuite'].save_csv(context['execution_arguments']['csv_report'], context['execution_arguments']['csv_report_delimiter'])
     if not context['execution_arguments'].get('disable_html_report', False):
         context['testsuite'].save_html(context['execution_arguments']['html_report'], context['initial_procedure'].upper())
 
 
 tasks = OrderedDict({
@@ -936,22 +937,22 @@
             'availability': check_access_to_packages
         }
     }
 })
 
 
 class IaasAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('check iaas')
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> TestSuite:
     cli_help = '''
     Script for checking Kubernetes cluster IAAS layer.
     
     Hot to use:
 
     '''
 
@@ -988,13 +989,14 @@
     testsuite: TestSuite = context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If test results are required for parsing, they can be found in the test results files
     print(testsuite.get_final_summary())
     testsuite.print_final_status(result.logger)
     make_reports(context)
-    if testsuite.is_any_test_failed():
-        sys.exit(1)
+    return testsuite
 
 
 if __name__ == '__main__':
-    main()
+    testsuite = main()
+    if testsuite.is_any_test_failed():
+        sys.exit(1)
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.20.0/kubemarine/procedures/check_paas.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.coredns import generate_configmap
 from deepdiff import DeepDiff  # type: ignore[import]
 
 
-def services_status(cluster: KubernetesCluster, service_type: str):
+def services_status(cluster: KubernetesCluster, service_type: str) -> None:
     with TestCase(cluster, '201', "Services", "%s Status" % service_type.capitalize(),
                   default_results='active (running)'):
         service_name = service_type
 
         if cluster.get_os_family() != 'multiple' and service_type != 'kubelet':
             service_name = cluster.get_package_association(service_type, 'service_name')
 
@@ -90,25 +90,25 @@
         statuses = list(set(statuses))
 
         if failed:
             raise TestFailure("Bad status detected: %s" % ', '.join(statuses),
                               hint="Fix the service to be enabled and has running status.")
 
 
-def _check_same_os(cluster: KubernetesCluster):
+def _check_same_os(cluster: KubernetesCluster) -> None:
     os_ids = cluster.get_os_identifiers()
     different_os = set(os_ids.values())
     if len(different_os) > 1:
         cluster.log.warning(
             f"Nodes have different OS families or versions, packages versions cannot be checked. "
             f"List of (OS family, version): {list(different_os)}")
         raise TestFailure(f"Nodes have different OS families or versions")
 
 
-def recommended_system_package_versions(cluster: KubernetesCluster, pckg_alias: str):
+def recommended_system_package_versions(cluster: KubernetesCluster, pckg_alias: str) -> None:
     """
     Function that checks if defined package are compatible with the configured k8s version and OS.
     Raise Warn if unable to detect the OS family, configured not recommended k8s version or
     if configured not recommended system packages versions.
     """
     os_family = cluster.get_os_family()
     if os_family not in pckgs.get_associations_os_family_keys():
@@ -143,15 +143,15 @@
             bad_results.append(expected_pckg_name)
 
     if bad_results:
         raise TestWarn(f"Detected not recommended packages versions: {bad_results}")
     cluster.log.debug(f"Detected packages with recommended versions: {good_results}")
 
 
-def system_packages_versions(cluster: KubernetesCluster, pckg_alias: str):
+def system_packages_versions(cluster: KubernetesCluster, pckg_alias: str) -> None:
     """
     Verifies that system packages are installed on required nodes and have equal versions.
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     :param pckg_alias: system package alias to retrieve "package_name" association.
     """
     with TestCase(cluster, '205', "Services", f"{pckg_alias} version") as tc:
@@ -162,15 +162,15 @@
         check_packages_versions(cluster, tc, hosts_to_packages, raise_successful=False)
 
         if pckg_alias in ["haproxy", "keepalived", "containerd", "docker"]:
             recommended_system_package_versions(cluster, pckg_alias)
         tc.success("all packages have correct versions")
 
 
-def mandatory_packages_versions(cluster: KubernetesCluster):
+def mandatory_packages_versions(cluster: KubernetesCluster) -> None:
     """
     Verifies that mandatory packages are installed on required nodes and have equal versions.
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     """
     with TestCase(cluster, '205', "Services", "Mandatory package versions") as tc:
         _check_same_os(cluster)
@@ -184,28 +184,28 @@
 
         if not hosts_to_packages:
             raise TestWarn(f"No mandatory packages to check")
 
         return check_packages_versions(cluster, tc, hosts_to_packages)
 
 
-def generic_packages_versions(cluster: KubernetesCluster):
+def generic_packages_versions(cluster: KubernetesCluster) -> None:
     """
     Verifies that user-provided packages are installed on required nodes and have equal versions.
     Warning is shown if check is not successful.
     """
     with TestCase(cluster, '206', "Services", f"Generic packages version") as tc:
         _check_same_os(cluster)
         packages = cluster.inventory['services']['packages'].get('install', {}).get('include', [])
         hosts_to_packages = {host: packages for host in cluster.nodes['all'].get_hosts()}
         return check_packages_versions(cluster, tc, hosts_to_packages, warn_on_bad_result=True)
 
 
 def check_packages_versions(cluster: KubernetesCluster, tc: TestCase, hosts_to_packages: Dict[str, List[str]],
-                            warn_on_bad_result=False, raise_successful=True):
+                            warn_on_bad_result: bool = False, raise_successful: bool = True) -> None:
     """
     Verifies that all packages are installed on required nodes and have equal versions
     :param cluster: main cluster object
     :param tc: current test case object
     :param hosts_to_packages: hosts where to check packages
     :param warn_on_bad_result: if true then uses Warning instead of Failure. Default False.
     """
@@ -238,19 +238,19 @@
             raise TestWarn("detected incorrect packages versions", hint=hint_message)
         raise TestFailure("detected incorrect packages versions", hint=hint_message)
     cluster.log.debug(f"installed packages: {good_results}")
     if raise_successful:
         tc.success("all packages have correct versions")
 
 
-def get_nodes_description(cluster: KubernetesCluster):
+def get_nodes_description(cluster: KubernetesCluster) -> dict:
     return kubernetes.get_nodes_description(cluster)
 
 
-def kubelet_version(cluster: KubernetesCluster):
+def kubelet_version(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '203', "Services", "Kubelet Version",
                   default_results=cluster.inventory['services']['kubeadm']['kubernetesVersion']):
         nodes_description = get_nodes_description(cluster)
         bad_versions = []
         for node_description in nodes_description['items']:
             node_name = node_description['metadata']['name']
             kubelet_version = node_description['status']['nodeInfo']['kubeletVersion']
@@ -261,15 +261,15 @@
         if bad_versions:
             raise TestFailure("Invalid version detected: %s" % ', '.join(bad_versions),
                               hint="All nodes must have the same correct Kubelet version \"%s\". Remove nodes with the "
                                    "incorrect version from the cluster and reinstall them to the corresponding "
                                    "versions." % cluster.inventory['services']['kubeadm']['kubernetesVersion'])
 
 
-def thirdparties_hashes(cluster: KubernetesCluster):
+def thirdparties_hashes(cluster: KubernetesCluster) -> None:
     """
     Task which is used to verify configured thirdparties hashes agains actual hashes on nodes.
     If thirdparty is an archive, then archive files hashes are also verified.
     If hash is not specified, then thirdparty is skipped.
     If there is no thirdparties with hashes, then warning is shown.
     """
     with TestCase(cluster, '212', "Thirdparties", "Hashes") as tc:
@@ -419,15 +419,15 @@
     missing = []
     for host, result in results.items():
         if result.failed:
             missing.append(host)
     return missing
 
 
-def kubernetes_nodes_existence(cluster: KubernetesCluster):
+def kubernetes_nodes_existence(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '209', "Kubernetes", "Nodes Existence",
                   default_results="All nodes presented"):
         nodes_description = get_nodes_description(cluster)
         nodes_names = kubernetes.get_actual_roles(nodes_description).keys()
         not_found = []
         for node in cluster.inventory['nodes']:
             if 'control-plane' in node['roles'] or 'worker' in node['roles']:
@@ -439,15 +439,15 @@
         not_found = list(set(not_found))
         if not_found:
             raise TestFailure("Nodes not found: %s" % ', '.join(not_found),
                               hint="The cluster must contain all the nodes that are described in the inventory. Add "
                                    "the missing nodes to the cluster.")
 
 
-def kubernetes_nodes_roles(cluster: KubernetesCluster):
+def kubernetes_nodes_roles(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '210', "Kubernetes", "Nodes Roles",
                   default_results="All nodes have the correct roles"):
         nodes_description = get_nodes_description(cluster)
         nodes_roles = kubernetes.get_actual_roles(nodes_description)
         nodes_with_bad_roles = []
         for node_name, actual_roles in nodes_roles.items():
             node = cluster.get_node_by_name(node_name)
@@ -466,15 +466,15 @@
         nodes_with_bad_roles = list(set(nodes_with_bad_roles))
         if nodes_with_bad_roles:
             raise TestFailure("Incorrect role detected at: %s" % ', '.join(nodes_with_bad_roles),
                               hint="Some nodes whose role differs from that specified in the "
                                    "inventory were detected. The configuration of these nodes should be fixed.")
 
 
-def kubernetes_nodes_condition(cluster: KubernetesCluster, condition_type: str):
+def kubernetes_nodes_condition(cluster: KubernetesCluster, condition_type: str) -> None:
     with TestCase(cluster, '211', "Kubernetes", "Nodes Condition - %s" % condition_type) as tc:
         nodes_description = get_nodes_description(cluster)
         expected_status = 'False'
         if condition_type == 'Ready':
             expected_status = 'True'
         positive_conditions = []
         negative_conditions = []
@@ -498,23 +498,23 @@
             raise TestFailure("%s" % ', '.join(negative_conditions),
                               hint="A condition in negative status means that there are problems with the health of "
                                    "the node.")
 
         tc.success(results="%s" % ', '.join(positive_conditions))
 
 
-def get_not_running_pods(cluster: KubernetesCluster):
+def get_not_running_pods(cluster: KubernetesCluster) -> str:
     # Completed pods should be excluded from the list as well
     get_pods_cmd = 'kubectl get pods -A --field-selector status.phase!=Running | awk \'{ print $1" "$2" "$4 }\' | grep -vw Completed || true'
     result = cluster.nodes['control-plane'].get_any_member().sudo(get_pods_cmd)
     cluster.log.verbose(result)
     return list(result.values())[0].stdout.strip()
 
 
-def kubernetes_pods_condition(cluster: KubernetesCluster):
+def kubernetes_pods_condition(cluster: KubernetesCluster) -> None:
     system_namespaces = ["kube-system", "ingress-nginx", "kube-public", "kubernetes-dashboard", "default"]
     critical_states = cluster.globals['pods']['critical_states']
     with TestCase(cluster, '207', "Kubernetes", "Pods Condition") as tc:
         pods_description = get_not_running_pods(cluster)
         total_failed_amount = len(pods_description.split('\n')[1:])
         critical_system_failed_amount = 0
 
@@ -538,15 +538,15 @@
                            hint="Try to determine the reason the pods are not operational, "
                                 "try to wait, redeploy, reapply, or restart them. "
                                 "If this is not fixed, some deployed applications may not work or may work incorrectly.")
         else:
             tc.success(results="All pods are running")
 
 
-def kubernetes_dashboard_status(cluster: KubernetesCluster):
+def kubernetes_dashboard_status(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '208', "Plugins", "Dashboard Availability") as tc:
         retries = 10
         test_succeeded = False
         i = 0
         while not test_succeeded and i < retries:
             i += 1
             if cluster.inventory['plugins']['kubernetes-dashboard']['install']:
@@ -572,15 +572,15 @@
                 test_succeeded = True
                 tc.success(results="skipped")
         if not test_succeeded:
             raise TestFailure("not available",
                               hint=f"Please verify the following Kubernetes Dashboard status and fix this issue:\n{status}")
 
 
-def nodes_pid_max(cluster: KubernetesCluster):
+def nodes_pid_max(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '202', "Nodes", "Nodes pid_max correctly installed") as tc:
         control_plane = cluster.nodes['control-plane'].get_any_member()
         yaml = ruamel.yaml.YAML()
         nodes_failed_pid_max_check = {}
         for node in cluster.make_group_from_roles(['control-plane', 'worker']).get_ordered_members_list():
             node_name = node.get_node_name()
 
@@ -784,15 +784,15 @@
             tc.success(results='valid')
         else:
             raise TestFailure('invalid',
                               hint=f"Modprobe rules do not match those loaded in modprobe on cluster nodes. Check "
                                    f"manually what the differences are and make changes on the appropriate nodes.")
 
 
-def etcd_health_status(cluster: KubernetesCluster):
+def etcd_health_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, check ETCD health
     :param cluster: KubernetesCluster object
     :return: None
     """
     with TestCase(cluster, '219', "ETCD", "Health status ETCD") as tc:
         try:
@@ -802,15 +802,15 @@
             raise TestFailure('invalid',
                               hint=f"ETCD not ready, please check"
                                    f" because of {e} ")
         cluster.log.debug(etcd_health_status)
         tc.success(results='healthy')
 
 
-def control_plane_configuration_status(cluster: KubernetesCluster):
+def control_plane_configuration_status(cluster: KubernetesCluster) -> None:
     '''
     This test verifies the consistency of the configuration (image version, `extra_args`, `extra_volumes`) of static pods of Control Plain like `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '220', "Control plane", "configuration status") as tc:
         results: List[dict] = []
@@ -859,15 +859,15 @@
 
         if not message:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=message)
 
 
-def check_extra_args(cluster: KubernetesCluster, static_pod: dict, node: NodeConfig):
+def check_extra_args(cluster: KubernetesCluster, static_pod: dict, node: NodeConfig) -> bool:
     static_pod_name = static_pod[static_pod['metadata']['name']]
     for arg, value in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraArgs", {}).items():
         if arg == "bind-address":
             # for "bind-address" we do not take default value into account, because its patched to node internal-address
             value = node["internal_address"]
         correct_property = False
         original_property = arg + "=" + value
@@ -877,15 +877,15 @@
                 correct_property = True
                 break
         if not correct_property:
             return False
     return True
 
 
-def check_extra_volumes(cluster: KubernetesCluster, static_pod: dict):
+def check_extra_volumes(cluster: KubernetesCluster, static_pod: dict) -> bool:
     static_pod_name = static_pod[static_pod['metadata']['name']]
     #for original_volume in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraVolumes", {}).items():
     for original_volume in cluster.inventory["services"]["kubeadm"][static_pod_name].get("extraVolumes", {}):
         correct_volume = False
         volume_mounts = static_pod["spec"]["containers"][0].get("volumeMounts", {})
         for volumeMount in volume_mounts:
             if volumeMount['mountPath'] == original_volume['mountPath'] and \
@@ -906,15 +906,15 @@
                 correct_volume = True
                 break
         if not correct_volume:
             return False
     return True
 
 
-def control_plane_health_status(cluster: KubernetesCluster):
+def control_plane_health_status(cluster: KubernetesCluster) -> None:
     '''
     This test verifies the health of static pods `kube-apiserver`, `kube-controller-manager` and `kube-scheduler`
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '221', "Control plane", "health status") as tc:
         static_pods = ['kube-apiserver', 'kube-controller-manager', 'kube-scheduler']
@@ -937,15 +937,15 @@
 
         if len(not_found_pod) == 0:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=f"{not_found_pod} pods doesn't running")
 
 
-def default_services_configuration_status(cluster: KubernetesCluster):
+def default_services_configuration_status(cluster: KubernetesCluster) -> None:
     '''
     In this test, the versions of the images of the default services, such as `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`, are checked, and the `coredns` configmap is also checked.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '222', "Default services", "configuration status") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
@@ -988,15 +988,15 @@
 
         if message:
             raise TestFailure('invalid', hint=f"{message}")
         else:
             tc.success(results='valid')
 
 
-def default_services_health_status(cluster: KubernetesCluster):
+def default_services_health_status(cluster: KubernetesCluster) -> None:
     '''
     This test verifies the health of pods `kube-proxy`, `coredns`, `calico-node`, `calico-kube-controllers` and `ingress-nginx-controller`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '223', "Default services", "health status") as tc:
         entities_to_check = {"kube-system": [{"DaemonSet": ["calico-node", "kube-proxy"]},
@@ -1025,15 +1025,15 @@
                                 not_ready_entities.append(service)
         if len(not_ready_entities) == 0:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=f"{not_ready_entities} pods doesn't ready")
 
 
-def calico_config_check(cluster: KubernetesCluster):
+def calico_config_check(cluster: KubernetesCluster) -> None:
     '''
     This test checks the configuration of the `calico-node` envs, Calico's ConfigMap in case of `ipam`, and also performed `calicoctl ipam check`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '224', "Calico", "configuration check") as tc:
         message = ""
@@ -1059,24 +1059,38 @@
         else:
             ipam_config = cluster.inventory["plugins"]["calico"]["cni"]["ipam"]["ipv6"]
         ddiff = DeepDiff(ipam_config, cni_network_config["plugins"][0]["ipam"], ignore_order=True)
         if ddiff:
             message += f"calico cm is outdated: {ddiff.to_dict()}\n"
 
         result = first_control_plane.sudo("calicoctl ipam check | grep 'found .* problems' |  tr -dc '0-9'")
-        if int(result.get_simple_out()) > 0:
+        found_problems = result.get_simple_result()
+        if 'Version mismatch' in found_problems.stderr:
+            version_mismatch_lines = found_problems.stderr.split('\n')
+
+            def calico_version(criteria: str) -> str:
+                return next(map(lambda l: l.split()[-1],
+                                filter(lambda l: criteria in l,
+                                       version_mismatch_lines),
+                                ),
+                            'unknown')
+
+            client_version = calico_version('Client Version')
+            cluster_version = calico_version('Cluster Version')
+            message += f"client version {client_version} mismatches the cluster version {cluster_version}"
+        elif int(found_problems.stdout) > 0:
             message += "ipam check indicates some problems," \
                        " for more info you can use `calicoctl ipam check --show-problem-ips`"
         if message:
             raise TestFailure('invalid', hint=message)
         else:
             tc.success(results='valid')
 
 
-def kubernetes_admission_status(cluster: KubernetesCluster):
+def kubernetes_admission_status(cluster: KubernetesCluster) -> None:
     """
     The method checks status of Pod Security Admissions, default Pod Security Profile,
     and 'kube-apiserver.yaml' and 'kubeadm-config' consistancy
     """
     with TestCase(cluster, '225', "Kubernetes", "Pod Security Admissions") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         profile_inv = ""
@@ -1126,15 +1140,15 @@
                          f"that is applied on cluster in 'kube-apiserver.yaml' and 'admission.yaml'")
         if not profile:
             kube_admission_status = 'PSS is "disabled"'
             cluster.log.debug(kube_admission_status)
             tc.success(results='disabled')
 
 
-def geo_check(cluster: KubernetesCluster):
+def geo_check(cluster: KubernetesCluster) -> None:
     """
     This test checks connectivity between clusters in geo schemas using paas-geo-monitor service.
     This test only work if "procedure.yaml" has "geo-monitor" section filled.
     """
     if not cluster.procedure_inventory or not cluster.procedure_inventory.get("geo-monitor"):
         cluster.log.debug("Geo connectivity check is skipped, no configuration provided")
         return
@@ -1359,22 +1373,22 @@
         "config_check": calico_config_check
     },
     'geo_check': geo_check,
 })
 
 
 class PaasAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('check paas')
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> TestSuite:
     cli_help = '''
     Script for checking Kubernetes cluster PAAS layer.
     
     Hot to use:
 
     '''
 
@@ -1411,13 +1425,14 @@
     testsuite: TestSuite = context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If tests results required for parsing, they can be found in test results files
     print(testsuite.get_final_summary(show_minimal=False, show_recommended=False))
     testsuite.print_final_status(result.logger)
     check_iaas.make_reports(context)
-    if testsuite.is_any_test_failed():
-        sys.exit(1)
+    return testsuite
 
 
 if __name__ == '__main__':
-    main()
+    testsuite = main()
+    if testsuite.is_any_test_failed():
+        sys.exit(1)
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/do.py` & `kubemarine-0.20.0/kubemarine/procedures/do.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         sys.exit(0)
 
 
 def main(cli_arguments: List[str] = None) -> None:
 
     if not cli_arguments:
-        cli_arguments = sys.argv
+        cli_arguments = sys.argv[1:]
 
     if '--' in cli_arguments:
         kubemarine_args = cli_arguments[:cli_arguments.index('--')]
         remote_args = cli_arguments[cli_arguments.index('--') + 1:]
     else:
         kubemarine_args = cli_arguments
         remote_args = []
@@ -73,41 +73,33 @@
                                      description=HELP_DESCRIPTION,
                                      usage='%(prog)s [-h] [-c CONFIG] [-n NODE] [-g GROUP] [--no_stream] -- shell_command')
 
     parser.add_argument('-c', '--config',
                             default='cluster.yaml',
                             help='define main cluster configuration file')
 
-    # TODO remove in next release
-    parser.add_argument('--ignore-schema-errors',
-                        action='store_true',
-                        help='Do not stop the run if validation by schema fails. '
-                             'The option will be removed in next release.')
-
     parser.add_argument('-n', '--node',
                             help='node(s) name to execute on, can be combined with groups')
 
     parser.add_argument('-g', '--group',
                             help='group(s) name to execute on, can be combined with nodes')
 
     parser.add_argument('--no_stream',
                             action='store_true',
                             help='do not stream all remote results in real-time, show node names')
 
     arguments = vars(parser.parse_args(kubemarine_args))
     configfile_path = arguments.get('config')
-    ignore_schema_errors = arguments.get('ignore_schema_errors')
 
     context = flow.create_empty_context({
         'disable_dump': True,
         'log': [
             ['stdout;level=error;colorize=true;correct_newlines=true']
         ],
         'config': configfile_path,
-        'ignore_schema_errors': ignore_schema_errors
     })
     context['preserve_inventory'] = False
 
     def node_group_provider(cluster: KubernetesCluster) -> NodeGroup:
         if arguments.get('node', None) is not None or arguments.get('group', None) is not None:
             executor_lists: Dict[str, List[str]] = {
                     'node': [],
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/install.py` & `kubemarine-0.20.0/kubemarine/procedures/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,29 +64,29 @@
                 cluster.log.debug(f"Skip running {fn_name} as no new node with roles {roles} has been found.")
 
         return cluster_wrapper
 
     return roles_wrapper
 
 
-def system_prepare_check_sudoer(cluster: KubernetesCluster):
+def system_prepare_check_sudoer(cluster: KubernetesCluster) -> None:
     not_sudoers = []
     for host, node_context in cluster.context['nodes'].items():
         access_info = node_context['access']
         if access_info['online'] and access_info['sudo'] == 'Root':
             cluster.log.debug("%s online and has root" % host)
         else:
             not_sudoers.append(host)
 
     if not_sudoers:
         raise KME("KME0005", hostnames=not_sudoers)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_check_system(group: NodeGroup):
+def system_prepare_check_system(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     cluster.log.debug(system.fetch_os_versions(cluster))
     for address, context in cluster.context["nodes"].items():
         if address not in group.nodes:
             continue
         if context["os"]["family"] == "unsupported":
             raise Exception('%s host operating system is unsupported' % address)
@@ -98,89 +98,89 @@
             raise Exception("%s running on unknown %s version. "
                             "Expected %s, got '%s'" % (address,
                                                        context["os"]["name"],
                                                        supported_os_versions,
                                                        context["os"]["version"]))
 
 
-def system_prepare_check_cluster_installation(cluster: KubernetesCluster):
+def system_prepare_check_cluster_installation(cluster: KubernetesCluster) -> None:
     if kubernetes.is_cluster_installed(cluster):
         cluster.log.debug('Cluster already installed and available at %s' % cluster.context['controlplain_uri'])
     else:
         cluster.log.debug('There is no any installed cluster')
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_chrony(group: NodeGroup):
+def system_prepare_system_chrony(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     if cluster.inventory['services']['ntp'].get('chrony', {}).get('servers') is None:
         cluster.log.debug("Skipped - NTP servers from chrony is not defined in config file")
         return
     group.call(system.configure_chronyd)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_timesyncd(group: NodeGroup):
+def system_prepare_system_timesyncd(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     if not cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('NTP') and \
             not cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('FallbackNTP'):
         cluster.log.debug("Skipped - NTP servers from timesyncd is not defined in config file")
         return
     group.call(system.configure_timesyncd)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_sysctl(group: NodeGroup):
+def system_prepare_system_sysctl(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     if cluster.inventory['services'].get('sysctl') is None or not cluster.inventory['services']['sysctl']:
         cluster.log.debug("Skipped - sysctl is not defined or empty in config file")
         return
     group.call_batch([
         sysctl.configure,
         sysctl.reload,
     ])
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_setup_selinux(group: NodeGroup):
+def system_prepare_system_setup_selinux(group: NodeGroup) -> None:
     group.call(selinux.setup_selinux)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_setup_apparmor(group: NodeGroup):
+def system_prepare_system_setup_apparmor(group: NodeGroup) -> None:
     group.call(apparmor.setup_apparmor)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_disable_firewalld(group: NodeGroup):
+def system_prepare_system_disable_firewalld(group: NodeGroup) -> None:
     group.call(system.disable_firewalld)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_disable_swap(group: NodeGroup):
+def system_prepare_system_disable_swap(group: NodeGroup) -> None:
     group.call(system.disable_swap)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_system_modprobe(group: NodeGroup):
+def system_prepare_system_modprobe(group: NodeGroup) -> None:
     group.call(system.setup_modprobe)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def system_install_audit(group: NodeGroup):
+def system_install_audit(group: NodeGroup) -> None:
     group.call(audit.install)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def system_prepare_audit_daemon(group: NodeGroup):
+def system_prepare_audit_daemon(group: NodeGroup) -> None:
     group.call(audit.apply_audit_rules)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane')
-def system_prepare_policy(group: NodeGroup):
+def system_prepare_policy(group: NodeGroup) -> None:
     """
     Task generates rules for logging kubernetes and on audit
     """
     cluster: KubernetesCluster = group.cluster
     api_server_extra_args = cluster.inventory['services']['kubeadm']['apiServer']['extraArgs']
     audit_log_dir = os.path.dirname(api_server_extra_args['audit-log-path'])
     audit_file_name = api_server_extra_args['audit-policy-file']
@@ -248,63 +248,63 @@
                                            " | awk '{print $1}')")
             control_plane.call(utils.wait_command_successful, command="kubectl get pod -n kube-system")
             control_plane.sudo("kubeadm init phase upload-config kubeadm "
                                "--config=/etc/kubernetes/audit-on-config.yaml")
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_dns_hostname(group: NodeGroup):
+def system_prepare_dns_hostname(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     with group.new_executor() as exe:
         for node in exe.group.get_ordered_members_list():
             cluster.log.debug("Changing hostname '%s' = '%s'" % (node.get_host(), node.get_node_name()))
             node.sudo("hostnamectl set-hostname %s" % node.get_node_name())
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_dns_resolv_conf(group: NodeGroup):
+def system_prepare_dns_resolv_conf(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     if cluster.inventory["services"].get("resolv.conf") is None:
         cluster.log.debug("Skipped - resolv.conf section not defined in config file")
         return
 
     system.update_resolv_conf(group, config=cluster.inventory["services"].get("resolv.conf"))
     cluster.log.debug(group.sudo("ls -la /etc/resolv.conf; sudo lsattr /etc/resolv.conf"))
 
 
-def system_prepare_dns_etc_hosts(cluster: KubernetesCluster):
+def system_prepare_dns_etc_hosts(cluster: KubernetesCluster) -> None:
     config = system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts')
     config += system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts_generated')
 
     utils.dump_file(cluster, config, 'etc_hosts')
     cluster.log.debug("\nUploading...")
 
     group = cluster.nodes['all'].get_final_nodes()
 
     system.update_etc_hosts(group, config=config)
     cluster.log.debug(group.sudo("ls -la /etc/hosts"))
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_package_manager_configure(group: NodeGroup):
+def system_prepare_package_manager_configure(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     repositories = cluster.inventory['services']['packages']['package_manager'].get("repositories")
     if not repositories:
         cluster.log.debug("Skipped - no repositories defined for configuration")
         return
 
     group.call(packages.backup_repo)
     group.call(packages.add_repo, repo_data=repositories)
 
     cluster.log.debug("Nodes contain the following repositories:")
     cluster.log.debug(packages.ls_repofiles(group))
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_package_manager_manage_packages(group: NodeGroup):
+def system_prepare_package_manager_manage_packages(group: NodeGroup) -> None:
     group.call_batch([
         manage_mandatory_packages,
         manage_custom_packages
     ])
 
 
 def manage_mandatory_packages(group: NodeGroup) -> RunnersGroupResult:
@@ -370,45 +370,45 @@
     else:
         cluster.log.verbose('No packages changed, nodes restart will not be scheduled')
 
     return None
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def system_cri_install(group: NodeGroup):
+def system_cri_install(group: NodeGroup) -> None:
     """
     Task which is used to install CRI. Could be skipped, if CRI already installed.
     """
     group.call(cri.install)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def system_cri_configure(group: NodeGroup):
+def system_cri_configure(group: NodeGroup) -> None:
     """
     Task which is used to configure CRI. Could be skipped, if CRI already configured.
     """
     group.call(cri.configure)
 
 
 @_applicable_for_new_nodes_with_roles('all')
-def system_prepare_thirdparties(group: NodeGroup):
+def system_prepare_thirdparties(group: NodeGroup) -> None:
     cluster: KubernetesCluster = group.cluster
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
 
     group.call(thirdparties.install_all_thirparties)
 
 
 @_applicable_for_new_nodes_with_roles('balancer')
-def deploy_loadbalancer_haproxy_install(group: NodeGroup):
+def deploy_loadbalancer_haproxy_install(group: NodeGroup) -> None:
     group.call(haproxy.install)
 
 
-def deploy_loadbalancer_haproxy_configure(cluster: KubernetesCluster):
+def deploy_loadbalancer_haproxy_configure(cluster: KubernetesCluster) -> None:
 
     if not cluster.inventory['services'].get('loadbalancer', {}) \
             .get('haproxy', {}).get('keep_configs_updated', True):
         cluster.log.debug('Skipped - haproxy balancers configs update manually disabled')
         return
 
     group = None
@@ -430,15 +430,15 @@
             haproxy.configure,
             haproxy.override_haproxy18,
         ])
 
     haproxy.restart(group)
 
 
-def deploy_loadbalancer_keepalived_install(cluster: KubernetesCluster):
+def deploy_loadbalancer_keepalived_install(cluster: KubernetesCluster) -> None:
     group = None
     if 'vrrp_ips' in cluster.inventory and cluster.inventory['vrrp_ips']:
 
         group = cluster.nodes['keepalived']
 
         # if remove/add node, then reconfigure only new keepalives
         if cluster.context['initial_procedure'] != 'install':
@@ -454,15 +454,15 @@
         cluster.log.debug('Skipped - no VRRP IPs to perform')
         return
 
     # add_node will impact all keepalived
     group.call(keepalived.install)
 
 
-def deploy_loadbalancer_keepalived_configure(cluster: KubernetesCluster):
+def deploy_loadbalancer_keepalived_configure(cluster: KubernetesCluster) -> None:
     group = None
     if 'vrrp_ips' in cluster.inventory and cluster.inventory['vrrp_ips']:
 
         group = cluster.nodes['keepalived'].get_final_nodes()
 
         # if remove/add node, then reconfigure only new keepalives
         if cluster.context['initial_procedure'] != 'install':
@@ -477,31 +477,31 @@
         return
 
     # add_node will impact all keepalived
     group.call(keepalived.configure)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def deploy_kubernetes_reset(group: NodeGroup):
+def deploy_kubernetes_reset(group: NodeGroup) -> None:
     group.call(kubernetes.reset_installation_env)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def deploy_kubernetes_install(group: NodeGroup):
+def deploy_kubernetes_install(group: NodeGroup) -> None:
     group.cluster.log.debug("Setting up Kubernetes...")
     group.call(kubernetes.install)
 
 
 @_applicable_for_new_nodes_with_roles('control-plane', 'worker')
-def deploy_kubernetes_prepull_images(group: NodeGroup):
+def deploy_kubernetes_prepull_images(group: NodeGroup) -> None:
     group.cluster.log.debug("Prepulling Kubernetes images...")
     group.call(kubernetes.images_grouped_prepull)
 
 
-def deploy_kubernetes_init(cluster: KubernetesCluster):
+def deploy_kubernetes_init(cluster: KubernetesCluster) -> None:
     cluster.nodes['control-plane'].call_batch([
         kubernetes.init_first_control_plane,
         kubernetes.join_other_control_planes
     ])
 
     if 'worker' in cluster.nodes:
         cluster.nodes['worker'].exclude_group(cluster.nodes['control-plane']) \
@@ -511,33 +511,33 @@
         kubernetes.apply_labels,
         kubernetes.apply_taints
     ])
 
     kubernetes.schedule_running_nodes_report(cluster)
 
 
-def deploy_coredns(cluster: KubernetesCluster):
+def deploy_coredns(cluster: KubernetesCluster) -> None:
     config = coredns.generate_configmap(cluster.inventory)
 
     cluster.log.debug('Applying patch...')
     cluster.log.debug(coredns.apply_patch(cluster))
 
     cluster.log.debug('Applying configmap...')
     cluster.log.debug(coredns.apply_configmap(cluster, config))
 
 
-def deploy_plugins(cluster: KubernetesCluster):
+def deploy_plugins(cluster: KubernetesCluster) -> None:
     plugins.install(cluster)
 
 
-def deploy_accounts(cluster: KubernetesCluster):
+def deploy_accounts(cluster: KubernetesCluster) -> None:
     kubernetes_accounts.install(cluster)
 
 
-def overview(cluster: KubernetesCluster):
+def overview(cluster: KubernetesCluster) -> None:
     cluster.log.debug("Retrieving cluster status...")
     control_plane = cluster.nodes["control-plane"].get_final_nodes().get_first_member()
     cluster.log.debug("\nNAMESPACES:")
     control_plane.sudo("kubectl get namespaces", hide=False)
     cluster.log.debug("\nNODES:")
     control_plane.sudo("kubectl get nodes -o wide", hide=False)
     cluster.log.debug("\nPODS:")
@@ -640,26 +640,26 @@
     summary.exec_delayed: [
         flow.END_OF_TASKS
     ]
 }
 
 
 class InstallAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('install')
         self.target_version = "not supported"
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         self.target_version = kubernetes.get_initial_kubernetes_version(res.raw_inventory())
         kubernetes.verify_supported_version(self.target_version, res.logger())
 
         flow.run_tasks(res, tasks, cumulative_points=cumulative_points)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
     Script for installing Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.20.0/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.20.0/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.20.0/kubemarine/procedures/migrate_cri.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from kubemarine.core.resources import DynamicResources
 from kubemarine.cri import docker
 from kubemarine.procedures import install
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine import packages
 
 
-def enrich_inventory(inventory: dict, cluster: KubernetesCluster):
+def enrich_inventory(inventory: dict, cluster: KubernetesCluster) -> dict:
     if cluster.context.get("initial_procedure") != "migrate_cri":
         return inventory
 
     os_family = cluster.get_os_family()
     if os_family in ('unknown', 'unsupported', 'multiple'):
         raise Exception("Migration of CRI is possible only for cluster "
                         "with all nodes having the same and supported OS family")
@@ -49,15 +49,15 @@
     ]
     for enrichment_fn in enrichment_functions:
         cluster.log.verbose('Calling fn "%s"' % enrichment_fn.__qualname__)
         inventory = enrichment_fn(cluster, inventory)
     return inventory
 
 
-def _prepare_yum_repos(cluster: KubernetesCluster, inventory: dict, finalization=False):
+def _prepare_yum_repos(cluster: KubernetesCluster, inventory: dict, finalization: bool = False) -> dict:
     if not cluster.procedure_inventory.get("yum", {}):
         cluster.log.debug("Skipped - no yum section defined in procedure config file")
         return inventory
 
     if not cluster.procedure_inventory["yum"].get("repositories", {}):
         cluster.log.debug("No repositories will be added on nodes")
         return inventory
@@ -70,15 +70,15 @@
                              cluster.procedure_inventory["yum"]["repositories"])
     else:
         default_merger.merge(inventory["services"]["yum"],
                              cluster.procedure_inventory["yum"])
     return inventory
 
 
-def _prepare_packages(cluster: KubernetesCluster, inventory: dict, finalization=False):
+def _prepare_packages(cluster: KubernetesCluster, inventory: dict, finalization: bool = False) -> dict:
     if not cluster.procedure_inventory.get("packages", {}):
         cluster.log.debug("Skipped - no packages defined in procedure config file")
         return inventory
 
     if not cluster.procedure_inventory["packages"].get("associations", {}):
         cluster.log.debug("Skipped - no associations defined in procedure config file")
         return inventory
@@ -96,55 +96,55 @@
         # but in future the restriction can be eliminated.
         default_merger.merge(inventory["services"]["packages"]["associations"][cluster.get_os_family()],
                              cluster.procedure_inventory["packages"]["associations"])
 
     return inventory
 
 
-def _prepare_crictl(cluster: KubernetesCluster, inventory: dict, finalization=False):
+def _prepare_crictl(cluster: KubernetesCluster, inventory: dict, finalization: bool = False) -> dict:
     if cluster.procedure_inventory.get("thirdparties", {}) \
             and cluster.procedure_inventory["thirdparties"].get("/usr/bin/crictl.tar.gz", {}):
 
         if not inventory["services"].get("thirdparties", {}):
             inventory["services"]["thirdparties"] = {}
 
         default_merger.merge(inventory["services"]["thirdparties"],
                              cluster.procedure_inventory["thirdparties"])
         cluster.log.debug("Third-party crictl added")
         return inventory
     else:
         return inventory
 
 
-def _configure_containerd_on_nodes(cluster: KubernetesCluster, inventory: dict):
+def _configure_containerd_on_nodes(cluster: KubernetesCluster, inventory: dict) -> dict:
     if inventory["services"]["cri"]["containerRuntime"] == cluster.procedure_inventory["cri"]["containerRuntime"]:
         raise Exception("You already have such cri or you should explicitly specify 'cri.containerRuntime: docker' in cluster.yaml")
 
     inventory = _merge_containerd(cluster, inventory)
     return inventory
 
 
-def _merge_containerd(cluster: KubernetesCluster, inventory: dict, finalization=False):
+def _merge_containerd(cluster: KubernetesCluster, inventory: dict, finalization: bool = False) -> dict:
     if not inventory["services"].get("cri", {}):
         inventory["services"]["cri"] = {}
 
     if inventory["services"]["cri"].get("dockerConfig", {}):
         del inventory["services"]["cri"]["dockerConfig"]
 
     default_merger.merge(inventory["services"]["cri"], cluster.procedure_inventory["cri"])
     return inventory
 
 
-def migrate_cri(cluster: KubernetesCluster):
+def migrate_cri(cluster: KubernetesCluster) -> None:
     _migrate_cri(cluster, cluster.nodes["worker"].exclude_group(cluster.nodes["control-plane"])
                  .get_ordered_members_list())
     _migrate_cri(cluster, cluster.nodes["control-plane"].get_ordered_members_list())
 
 
-def _migrate_cri(cluster: KubernetesCluster, node_group: List[NodeGroup]):
+def _migrate_cri(cluster: KubernetesCluster, node_group: List[NodeGroup]) -> None:
     """
     Migrate CRI from docker to already installed containerd.
     This method works node-by-node, configuring kubelet to use containerd.
     :param cluster: main object describing a cluster
     :param node_group: group of nodes to migrate
     """
 
@@ -242,15 +242,15 @@
         control_plane.sudo(f"sudo kubectl annotate node {node_name} "
                            f"--overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock")
 
         # delete docker socket
         node.sudo("rm -rf /var/run/docker.sock", hide=False)
 
 
-def release_calico_leaked_ips(cluster: KubernetesCluster):
+def release_calico_leaked_ips(cluster: KubernetesCluster) -> None:
     """
     During drain command we ignore daemon sets, as result this such pods as ingress-nginx-controller arent't deleted before migration.
     For this reason their ips can stay in calico ipam despite they aren't used. You can check this, if you run "calicoctl ipam check --show-problem-ips" right after apply_new_cri task.
     Those ips are cleaned by calico garbage collector, but it can take about 20 minutes.
     This task releases problem ips with force.
     """
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
@@ -262,21 +262,21 @@
     cluster.log.debug(f"Found {leaked_ips_count} leaked ips")
     if leaked_ips_count != 0:
         first_control_plane.sudo(f"calicoctl ipam release --from-report={random_report_name} --force", hide=False)
         cluster.log.debug("Leaked ips was released")
     first_control_plane.sudo(f"rm {random_report_name}", hide=False)
 
 
-def edit_config(kubeadm_flags: str):
+def edit_config(kubeadm_flags: str) -> str:
     kubeadm_flags = kubernetes._config_changer(kubeadm_flags, "--container-runtime=remote")
     return kubernetes._config_changer(kubeadm_flags,
                            "--container-runtime-endpoint=unix:///run/containerd/containerd.sock")
 
 
-def migrate_cri_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict):
+def migrate_cri_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
 
     if cluster.context.get("initial_procedure") != "migrate_cri":
         return inventory_to_finalize
     finalize_functions: List[Callable[[KubernetesCluster, dict, bool], dict]] = [
         _prepare_yum_repos,
         _prepare_packages,
         _prepare_crictl,
@@ -293,23 +293,23 @@
     "add_repos": install.system_prepare_package_manager_configure,
     "apply_new_cri": migrate_cri,
     "release_calico_ipam_leacked_ips": release_calico_leaked_ips
 })
 
 
 class MigrateCRIAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('migrate cri', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
         Script for automated migration from docker to containerd.
 
         How to use:
 
         '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.20.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,25 +379,25 @@
     for package_name in ['haproxy', 'keepalived']:
         if any(upgrade_config['packages'][package_name].get(v_key)
                for v_key in ('version_rhel', 'version_rhel8', 'version_debian')):
             upgrade_patches.append(BalancerUpgradePatch(upgrade_config, package_name))
 
     default_plugins = static.DEFAULTS['plugins']
     plugins = list(default_plugins)
-    plugins.sort(key=get_default_plugin_prioriry)
+    plugins.sort(key=get_default_plugin_priority)
     for plugin_name in plugins:
         k8s_versions = upgrade_config['plugins'][plugin_name]
         if k8s_versions:
             verify_allowed_kubernetes_versions(k8s_versions)
             upgrade_patches.append(PluginUpgradePatch(plugin_name, k8s_versions))
 
     return upgrade_patches
 
 
-def get_default_plugin_prioriry(plugin: str) -> int:
+def get_default_plugin_priority(plugin: str) -> int:
     priority: int = static.DEFAULTS['plugins'][plugin]['installation']['priority']
     return priority
 
 
 def verify_allowed_kubernetes_versions(kubernetes_versions: List[str]) -> None:
     not_allowed_versions = set(kubernetes_versions) - set(static.KUBERNETES_VERSIONS['compatibility_map'])
     if not_allowed_versions:
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/reboot.py` & `kubemarine-0.20.0/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.20.0/kubemarine/procedures/remove_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
-from typing import Optional
+from typing import Optional, List
 
 from kubemarine import kubernetes, haproxy, keepalived
 from kubemarine.core import flow, summary
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
@@ -40,40 +40,40 @@
         return None
     if not disabled_nodes.is_empty():
         cluster.log.debug("Partly Skipped - several %s nodes are inactive: %s"
                           % (node_type, ", ".join(disabled_nodes.nodes)))
     return active_nodes
 
 
-def loadbalancer_remove_haproxy(cluster: KubernetesCluster):
+def loadbalancer_remove_haproxy(cluster: KubernetesCluster) -> None:
     nodes = _get_active_nodes("balancer", cluster)
     if nodes is None:
         return
     nodes.call(haproxy.disable)
 
 
-def loadbalancer_remove_keepalived(cluster: KubernetesCluster):
+def loadbalancer_remove_keepalived(cluster: KubernetesCluster) -> None:
     nodes = _get_active_nodes("keepalived", cluster)
     if nodes is None:
         return
     nodes.call(keepalived.disable)
 
 
-def remove_kubernetes_nodes(cluster: KubernetesCluster):
+def remove_kubernetes_nodes(cluster: KubernetesCluster) -> None:
     group = cluster.make_group_from_roles(['control-plane', 'worker']).get_nodes_for_removal()
 
     if group.is_empty():
         cluster.log.debug("No kubernetes nodes to perform")
         return
 
     group.call(kubernetes.reset_installation_env)
     kubernetes.schedule_running_nodes_report(cluster)
 
 
-def remove_node_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize):
+def remove_node_finalize_inventory(cluster: KubernetesCluster, inventory_to_finalize: dict) -> dict:
     if cluster.context.get('initial_procedure') != 'remove_node':
         return inventory_to_finalize
 
     nodes_for_removal = cluster.nodes['all'].get_nodes_for_removal()
     final_nodes = cluster.nodes['all'].get_final_nodes()
 
     # check if there are no more hosts where keepalived installed - remove according vrrp_ips
@@ -140,23 +140,23 @@
     summary.exec_delayed: [
         flow.END_OF_TASKS
     ]
 }
 
 
 class RemoveNodeAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('remove node', recreate_inventory=True)
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks, cumulative_points=cumulative_points)
         res.make_final_inventory()
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
 
     cli_help = '''
     Script for removing node from Kubernetes cluster.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/restore.py` & `kubemarine-0.20.0/kubemarine/procedures/restore.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 
 
 import os
 import re
 import tarfile
 import time
 from collections import OrderedDict
+from typing import List
+
 import yaml
 
 from kubemarine.core import utils, flow, defaults
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install, backup
 from kubemarine import system, kubernetes, etcd
 
 
-def missing_or_empty(file):
+def missing_or_empty(file: str) -> bool:
     if not os.path.exists(file):
         return True
     content = utils.read_external(file)
     if re.search(r'^\s*$', content):
         return True
 
+    return False
+
 
-def replace_config_from_backup_if_needed(procedure_inventory_filepath: str, config: str):
+def replace_config_from_backup_if_needed(procedure_inventory_filepath: str, config: str) -> None:
     if missing_or_empty(config):
         print('Config is missing or empty - retrieving config from backup archive...')
         with utils.open_external(procedure_inventory_filepath, 'r') as stream:
             procedure = yaml.safe_load(stream)
         backup_location = procedure.get("backup_location")
         if not backup_location:
             raise Exception('Backup location is not specified in procedure')
@@ -49,15 +53,15 @@
         print('Unpacking cluster.yaml...')
         with tarfile.open(backup_location, 'r:gz') as tar:
             member = tar.getmember('original_cluster.yaml')
             tar.makefile(member, config)
             tar.close()
 
 
-def unpack_data(cluster: KubernetesCluster):
+def unpack_data(cluster: KubernetesCluster) -> None:
     backup_tmp_directory = backup.prepare_backup_tmpdir(cluster)
     backup_file_source = cluster.procedure_inventory.get('backup_location')
 
     if not backup_file_source:
         raise Exception('Backup source not specified in procedure')
 
     backup_file_source = utils.get_external_resource_path(backup_file_source)
@@ -83,15 +87,15 @@
     if not os.path.isfile(descriptor_filepath):
         raise FileNotFoundError('Descriptor not found in backup file')
 
     with utils.open_external(descriptor_filepath, 'r') as stream:
         cluster.context['backup_descriptor'] = yaml.safe_load(stream)
 
 
-def verify_backup_data(cluster: KubernetesCluster):
+def verify_backup_data(cluster: KubernetesCluster) -> None:
     if not cluster.context['backup_descriptor'].get('kubernetes', {}).get('version'):
         cluster.log.debug('Not possible to verify Kubernetes version, because descriptor do not contain such information')
         return
 
     if cluster.context['backup_descriptor']['kubernetes']['version'] != cluster.inventory['services']['kubeadm']['kubernetesVersion']:
         cluster.log.warning('Installed kubernetes versions do not match version from backup')
         cluster.log.verbose('Cluster re-parse required')
@@ -101,15 +105,15 @@
             cluster.raw_inventory['services']['kubeadm'] = {}
         cluster.raw_inventory['services']['kubeadm']['kubernetesVersion'] = cluster.context['backup_descriptor']['kubernetes']['version']
         cluster._inventory = defaults.enrich_inventory(cluster, cluster.raw_inventory)
     else:
         cluster.log.debug('Kubernetes version from backup is correct')
 
 
-def stop_cluster(cluster: KubernetesCluster):
+def stop_cluster(cluster: KubernetesCluster) -> None:
     cluster.log.debug('Stopping the existing cluster...')
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
     if cri_impl == "docker":
         result = cluster.nodes['control-plane'].sudo('systemctl stop kubelet; '
                                               'sudo docker kill $(sudo docker ps -q); '
                                               'sudo docker rm -f $(sudo docker ps -a -q); '
                                               'sudo docker ps -a; '
@@ -120,26 +124,26 @@
                                               'sudo crictl rm -fa; '
                                               'sudo crictl ps -a; '
                                               'sudo rm -rf /var/lib/etcd; '
                                               'sudo mkdir -p /var/lib/etcd', warn=True)
     cluster.log.verbose(result)
 
 
-def restore_thirdparties(cluster: KubernetesCluster):
+def restore_thirdparties(cluster: KubernetesCluster) -> None:
     custom_thirdparties = cluster.procedure_inventory.get('restore_plan', {}).get('thirdparties', {})
     if custom_thirdparties:
         for name, value in custom_thirdparties.items():
             cluster.inventory['services']['thirdparties'][name]['source'] = value['source']
             if value.get('sha1'):
                 cluster.inventory['services']['thirdparties'][name]['sha1'] = value['sha1']
 
     install.system_prepare_thirdparties(cluster)
 
 
-def import_nodes(cluster: KubernetesCluster):
+def import_nodes(cluster: KubernetesCluster) -> None:
     with cluster.nodes['all'].new_executor() as exe:
         for node in exe.group.get_ordered_members_list():
             node_name = node.get_node_name()
             cluster.log.debug('Uploading backup for \'%s\'' % node_name)
             node.put(os.path.join(cluster.context['backup_tmpdir'], 'nodes_data', '%s.tar.gz' % node_name),
                      '/tmp/kubemarine-backup.tar.gz')
 
@@ -150,15 +154,15 @@
         f"readlink /etc/resolv.conf ; "
         f"if [ $? -ne 0 ]; then sudo chattr -i /etc/resolv.conf; {unpack_cmd} && sudo chattr +i /etc/resolv.conf; "
         f"else {unpack_cmd}; fi ")
 
     cluster.log.debug(result)
 
 
-def import_etcd(cluster: KubernetesCluster):
+def import_etcd(cluster: KubernetesCluster) -> None:
     etcd_all_certificates = cluster.procedure_inventory.get('restore_plan', {}).get('etcd', {}).get('certificates', {})
     etcd_cert = etcd_all_certificates.get('cert', cluster.globals['etcd']['default_arguments']['cert'])
     etcd_key = etcd_all_certificates.get('key', cluster.globals['etcd']['default_arguments']['key'])
     etcd_cacert = etcd_all_certificates.get('cacert', cluster.globals['etcd']['default_arguments']['cacert'])
     etcd_peer_cert = etcd_all_certificates.get('peer_cert', cluster.globals['etcd']['default_arguments']['peer_cert'])
     etcd_peer_key = etcd_all_certificates.get('peer_key', cluster.globals['etcd']['default_arguments']['peer_key'])
     etcd_peer_cacert = etcd_all_certificates.get('peer_cacert',
@@ -247,15 +251,15 @@
             if expected_dbsize > real_dbsize:
                 raise Exception('ETCD member "%s" has invalid DB size' % item.get('endpoint'))
         cluster.log.debug('DB size "%s" is correct' % expected_dbsize)
     else:
         cluster.log.verbose('It is not possible to verify db size - descriptor do not contain such information')
 
 
-def reboot(cluster: KubernetesCluster):
+def reboot(cluster: KubernetesCluster) -> None:
     system.reboot_group(cluster.nodes['all'], try_graceful=False)
     kubernetes.wait_for_nodes(cluster.nodes['control-plane'])
 
 
 tasks = OrderedDict({
     "prepare": {
         "unpack": unpack_data,
@@ -270,22 +274,22 @@
         "etcd": import_etcd
     },
     "reboot": reboot
 })
 
 
 class RestoreAction(Action):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__('restore')
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
     Script for restoring Kubernetes resources and nodes contents from backup file.
 
     How to use:
 
     '''
```

### Comparing `kubemarine-0.19.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.20.0/kubemarine/procedures/upgrade.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,36 +23,35 @@
 import toml
 
 from kubemarine import kubernetes, plugins
 from kubemarine.core import flow
 from kubemarine.core import utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import CollectorCallback
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install
 
 
 
-def system_prepare_thirdparties(cluster: KubernetesCluster):
+def system_prepare_thirdparties(cluster: KubernetesCluster) -> None:
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
 
     install.system_prepare_thirdparties(cluster)
 
 
-def prepull_images(cluster: KubernetesCluster):
+def prepull_images(cluster: KubernetesCluster) -> None:
     cluster.log.debug("Prepulling Kubernetes images...")
     fix_cri_socket(cluster)
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
     upgrade_group.call(kubernetes.images_grouped_prepull)
 
 
-def kubernetes_upgrade(cluster: KubernetesCluster):
+def kubernetes_upgrade(cluster: KubernetesCluster) -> None:
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
     grace_period = cluster.procedure_inventory.get('grace_period')
     disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
     drain_kwargs = {
         'disable_eviction': disable_eviction, 'drain_timeout': drain_timeout, 'grace_period': grace_period
@@ -69,46 +68,46 @@
     if cluster.nodes.get('worker', []):
         kubernetes.upgrade_workers(upgrade_group, cluster, **drain_kwargs)
 
     cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     cluster.context['cached_nodes_versions_cleaned'] = True
 
 
-def kubernetes_cleanup_nodes_versions(cluster: KubernetesCluster):
+def kubernetes_cleanup_nodes_versions(cluster: KubernetesCluster) -> None:
     if not cluster.context.get('cached_nodes_versions_cleaned', False):
         cluster.log.verbose('Cached nodes versions required')
         cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     else:
         cluster.log.verbose('Cached nodes versions already cleaned')
     kubernetes_apply_taints(cluster)
 
 
-def upgrade_packages(cluster: KubernetesCluster):
+def upgrade_packages(cluster: KubernetesCluster) -> None:
     upgrade_version = cluster.context["upgrade_version"]
 
     packages = cluster.procedure_inventory.get(upgrade_version, {}).get("packages", {})
     if packages.get("install") is not None or packages.get("upgrade") is not None or packages.get("remove") is not None:
         install.manage_custom_packages(cluster.nodes['all'])
 
 
-def upgrade_plugins(cluster: KubernetesCluster):
+def upgrade_plugins(cluster: KubernetesCluster) -> None:
     upgrade_version = cluster.context["upgrade_version"]
 
     # upgrade_candidates is a source of upgradeable plugins, not list of plugins to upgrade.
     # Some plugins from upgrade_candidates will not be upgraded, because they have "install: false"
     upgrade_candidates = {}
     defined_plugins = cluster.procedure_inventory.get(upgrade_version, {}).get("plugins", {}).keys()
     for plugin in chain(defined_plugins, plugins.oob_plugins):
         # TODO: use only OOB plugins that have changed version so that we do not perform redundant installations
         upgrade_candidates[plugin] = cluster.inventory["plugins"][plugin]
 
     plugins.install(cluster, upgrade_candidates)
 
 
-def upgrade_containerd(cluster: KubernetesCluster):
+def upgrade_containerd(cluster: KubernetesCluster) -> None:
     """
         This function fixes the incorrect version of pause during the cluster update procedure
     """
 
     cri = cluster.inventory["services"]["cri"]['containerRuntime']
     if cri == 'containerd':
         path = 'plugins."io.containerd.grpc.v1.cri"'
@@ -136,32 +135,29 @@
             for key, value in containerd_config.items():
                 # next we process all "complex" `key: dict_value` pairs, representing named sections
                 if isinstance(value, dict):
                     config_string += f"\n[{key}]\n{toml.dumps(value)}"
             utils.dump_file(cluster, config_string, 'containerd-config.toml')
 
             kubernetes_nodes = cluster.make_group_from_roles(['control-plane', 'worker'])
-            collector = CollectorCallback(cluster)
             for member_node in kubernetes_nodes.get_ordered_members_list():
                 kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
                 kubeadm_flags = member_node.sudo(f"cat {kubeadm_flags_file}").get_simple_out()
                 updated_kubeadm_flags = kubernetes._config_changer(kubeadm_flags, f"--pod-infra-container-image={sandbox}")
                 member_node.put(StringIO(updated_kubeadm_flags), kubeadm_flags_file, backup=True, sudo=True)
 
             with kubernetes_nodes.new_executor() as exe:
                 for node in exe.group.get_ordered_members_list():
                     os_specific_associations = cluster.get_associations_for_node(node.get_host(), 'containerd')
                     node.put(StringIO(config_string), os_specific_associations['config_location'],
                              backup=True, sudo=True, mkdir=True)
                     node.sudo(
                         f"sudo systemctl restart {os_specific_associations['service_name']} && "
                         f"systemctl status {os_specific_associations['service_name']} && " 
-                        f"sudo systemctl restart kubelet",
-                        callback=collector)
-            return collector.result
+                        f"sudo systemctl restart kubelet")
 
 
 tasks = OrderedDict({
     "verify_upgrade_versions": kubernetes.verify_upgrade_versions,
     "thirdparties": system_prepare_thirdparties,
     "prepull_images": prepull_images,
     "configure_policy": install.system_prepare_policy,
@@ -172,18 +168,18 @@
     "plugins": upgrade_plugins,
     "overview": install.overview
 
 })
 
 
 class UpgradeFlow(flow.Flow):
-    def __init__(self):
+    def __init__(self) -> None:
         self.target_version = "not supported"
 
-    def _run(self, resources: DynamicResources):
+    def _run(self, resources: DynamicResources) -> None:
         logger = resources.logger()
 
         previous_version = kubernetes.get_initial_kubernetes_version(resources.raw_inventory())
         upgrade_plan = resources.procedure_inventory()['upgrade_plan']
         upgrade_plan = verify_upgrade_plan(previous_version, upgrade_plan)
         logger.debug(f"Loaded upgrade plan: current ({previous_version}) ⭢ {' ⭢ '.join(upgrade_plan)}")
 
@@ -196,28 +192,28 @@
 
         # todo inventory is preserved few times, probably need to preserve it once instead.
         actions = [UpgradeAction(version) for version in upgrade_plan]
         flow.run_actions(resources, actions)
 
 
 class UpgradeAction(Action):
-    def __init__(self, upgrade_version: str):
+    def __init__(self, upgrade_version: str) -> None:
         super().__init__('upgrade to ' + upgrade_version, recreate_inventory=True)
         self.upgrade_version = upgrade_version
 
-    def run(self, res: DynamicResources):
+    def run(self, res: DynamicResources) -> None:
         flow.run_tasks(res, tasks)
         res.make_final_inventory()
 
     def prepare_context(self, context: dict) -> None:
         context['upgrade_version'] = self.upgrade_version
         context['dump_filename_prefix'] = self.upgrade_version
 
 
-def main(cli_arguments=None):
+def main(cli_arguments: List[str] = None) -> None:
     cli_help = '''
     Script for automated upgrade of the entire Kubernetes cluster to a new version.
 
     How to use:
 
     '''
 
@@ -226,43 +222,43 @@
     context = flow.create_context(parser, cli_arguments, procedure='upgrade')
     flow_ = UpgradeFlow()
     result = flow_.run_flow(context)
 
     kubernetes.verify_supported_version(flow_.target_version, result.logger)
 
 
-def verify_upgrade_plan(previous_version: str, upgrade_plan: List[str]):
+def verify_upgrade_plan(previous_version: str, upgrade_plan: List[str]) -> List[str]:
     kubernetes.verify_allowed_version(previous_version)
     for version in upgrade_plan:
         kubernetes.verify_allowed_version(version)
 
     upgrade_plan.sort(key=utils.version_key)
 
     for version in upgrade_plan:
         kubernetes.test_version_upgrade_possible(previous_version, version)
         previous_version = version
 
     return upgrade_plan
 
 
-def fix_cri_socket(cluster: KubernetesCluster):
+def fix_cri_socket(cluster: KubernetesCluster) -> None:
     """
     This method fixs the issue with 'kubeadm.alpha.kubernetes.io/cri-socket' node annotation
     and delete the docker socket if it exists
     """
 
     if cluster.inventory["services"]["cri"]["containerRuntime"] == "containerd":
         control_plane = cluster.nodes["control-plane"].get_first_member()
         control_plane.sudo(f"sudo kubectl annotate nodes --all "
                            f"--overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock")
         upgrade_group = kubernetes.get_group_for_upgrade(cluster)
         upgrade_group.sudo("rm -rf /var/run/docker.sock")
 
 
-def kubernetes_apply_taints(cluster: KubernetesCluster):
+def kubernetes_apply_taints(cluster: KubernetesCluster) -> None:
     # Apply taints after upgrade
     group = cluster.nodes['control-plane']
     kubernetes.apply_taints(group)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.19.0/kubemarine/resources/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,16 @@
             - /etc/resolv.conf
       Hosts: |
         127.0.0.1 localhost localhost.localdomain
         {% if not nodes[0]["internal_address"]|isipv4 %}::1 localhost localhost.localdomain{% endif %}
 
   loadbalancer:
     haproxy:
+      global:
+        maxconn: 10000
       defaults:
         timeout_connect: '10s'
         timeout_client: '1m'
         timeout_server: '1m'
         timeout_tunnel: '60m'
         timeout_client_fin: '1m'
         maxconn: 10000
@@ -553,14 +555,16 @@
               plugin_name: nginx-ingress-controller
         - expect:
             daemonsets:
               - name: ingress-nginx-controller
                 namespace: ingress-nginx
             pods:
               - ingress-nginx-controller
+    config_map:
+      use-proxy-protocol: "true"
     webhook:
       image: 'ingress-nginx/kube-webhook-certgen:{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion]["webhook-version"] }}'
     controller:
       image: 'ingress-nginx/controller:{{ plugins["nginx-ingress-controller"].version }}'
       ssl:
         enableSslPassthrough: false
       nodeSelector:
```

### Comparing `kubemarine-0.19.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.20.0/kubemarine/resources/configurations/globals.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.20.0/kubemarine/patches/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
+from kubemarine.patches.p1_kubeadm_flags import KubeadmFlags
 
 patches: List[Patch] = [
+  KubeadmFlags(),
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.19.0/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.20.0/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.20.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.20.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.20.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.20.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.20.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988095238095237%*

 * *Differences: {"'properties'": "{'haproxy': {'properties': {'global': OrderedDict([('type', 'object'), "*

 * *                 '(\'description\', "Parameters that are passed directly to the \'global\' section '*

 * *                 'of haproxy.cfg file."), (\'properties\', OrderedDict([(\'maxconn\', '*

 * *                 "OrderedDict([('type', 'integer'), ('default', 10000), ('description', 'Set the "*

 * *                 "total number of connections allowed, process-wide.')]))]))])}}}"}*

```diff
@@ -46,14 +46,25 @@
                             "default": "60m",
                             "description": "Set the maximum inactivity time on the client and server sides for tunnels",
                             "type": "string"
                         }
                     },
                     "type": "object"
                 },
+                "global": {
+                    "description": "Parameters that are passed directly to the 'global' section of haproxy.cfg file.",
+                    "properties": {
+                        "maxconn": {
+                            "default": 10000,
+                            "description": "Set the total number of connections allowed, process-wide.",
+                            "type": "integer"
+                        }
+                    },
+                    "type": "object"
+                },
                 "keep_configs_updated": {
                     "default": true,
                     "description": "Allows Kubemarine update haproxy configs every time, when cluster (re)installed or it's schema updated (added/removed nodes)",
                     "type": "boolean"
                 },
                 "maintenance_mode": {
                     "default": false,
```

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.20.0/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.20.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.20.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.20.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.20.0/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/selinux.py` & `kubemarine-0.20.0/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/sysctl.py` & `kubemarine-0.20.0/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/system.py` & `kubemarine-0.20.0/kubemarine/system.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/__init__.py` & `kubemarine-0.20.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.20.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 global
     log                 127.0.0.1 local2 debug
     user haproxy
     group haproxy
+    maxconn             {{ config_options['global']['maxconn'] }}
 
 defaults
     log                 global
     option              dontlognull
     timeout connect     {{ config_options['defaults']['timeout_connect'] }}
     timeout client      {{ config_options['defaults']['timeout_client'] }}
     timeout server      {{ config_options['defaults']['timeout_server'] }}
@@ -24,15 +25,15 @@
 backend http_backend
     mode                tcp
     balance             source
     option              tcp-check
     default-server      inter 2s fall 2 rise 3
 {%- for node in nodes -%}
 {% if 'worker' in node['roles'] %}
-    server {{ node['name'] }} {{ node['internal_address'] }}:80 check port 80
+    server {{ node['name'] }} {{ node['internal_address'] }}:80 check port 80 send-proxy
 {%- endif %}
 {%- endfor %}
 
 frontend https
 {%- for binding in bindings %}
     bind                {{ binding }}:443
 {%- endfor %}
@@ -43,15 +44,15 @@
 backend https_backend
     mode                tcp
     balance             source
     option              tcp-check
     default-server      inter 2s fall 2 rise 3
 {%- for node in nodes -%}
 {% if 'worker' in node['roles'] %}
-    server {{ node['name'] }} {{ node['internal_address'] }}:443 check port 443
+    server {{ node['name'] }} {{ node['internal_address'] }}:443 check port 443 send-proxy
 {%- endif %}
 {%- endfor %}
 
 frontend kubernetes_api
 {%- for binding in bindings %}
     bind                {{ binding }}:6443
 {%- endfor %}
```

### Comparing `kubemarine-0.19.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.20.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.20.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.20.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.20.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine/testsuite.py` & `kubemarine-0.20.0/kubemarine/testsuite.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import textwrap
 from traceback import *
 import csv
 from datetime import datetime
-from typing import Dict
+from types import TracebackType
+from typing import Dict, Optional, Type, Union, List
 
 from kubemarine.core import utils, log
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import GroupException
 
 TC_UNKNOWN = -1
@@ -36,72 +37,69 @@
     'excepted': 3,
     'unknown': 4,
 }
 
 
 class TestCase:
 
-    def __enter__(self):
+    def __enter__(self) -> 'TestCase':
         return self
 
-    def __exit__(self, type, value, traceback):
-        if type is None:
+    def __exit__(self, type: Optional[Type[Exception]], value: Optional[Exception],
+                 traceback: Optional[TracebackType]) -> bool:
+        if value is None:
             if self.status is TC_UNKNOWN:
                 self.success()
-        elif type is TestFailure:
+        elif isinstance(value, TestFailure):
             self.fail(value)
-        elif type is TestWarn:
+        elif isinstance(value, TestWarn):
             self.warn(value)
         else:
             self.exception(value)
         print(self.get_summary(show_hint=True))
         return True
 
-    def __init__(self, cluster: KubernetesCluster, id, category, name, default_results=None, minimal=None, recommended=None):
+    def __init__(self, cluster: KubernetesCluster, id: str, category: str, name: str,
+                 default_results: str = None, minimal: int = None, recommended: int = None):
         self.include_in_ts(cluster.context['testsuite'])
         self.category = category
         self.id = str(id)
         self.name = name
         self.status = TC_UNKNOWN
-        self.results = default_results
+        self.results: Union[str, BaseException, None] = default_results
         self.minimal = minimal
         self.recommended = recommended
         self.cluster = cluster
 
-    def include_in_ts(self, ts):
+    def include_in_ts(self, ts: 'TestSuite') -> None:
         ts.register_tc(self)
-        return self
 
-    def success(self, results=None):
+    def success(self, results: str = None) -> None:
         if self.results is None:
             self.results = results
         self.status = TC_PASSED
-        return self
 
-    def fail(self, results):
+    def fail(self, results: BaseException) -> None:
         self.status = TC_FAILED
         self.results = results
-        return self
 
-    def warn(self, results):
+    def warn(self, results: BaseException) -> None:
         self.status = TC_WARNED
         self.results = results
-        return self
 
-    def exception(self, results):
+    def exception(self, results: BaseException) -> None:
         self.status = TC_EXCEPTED
         if isinstance(results, GroupException):
             self.cluster.log.debug(results)
             self.results = "Remote group exception"
         else:
             print_exc()
             self.results = results
-        return self
 
-    def get_summary(self, show_description=False, show_hint=False, show_minimal=False, show_recommended=False):
+    def get_summary(self, show_hint: bool = False, show_minimal: bool = False, show_recommended: bool = False) -> str:
         output = ""
 
         output += " " * (15 - len(self.category))
         output += self.category + "  "
 
         color = ""
         if self.is_succeeded():
@@ -155,85 +153,82 @@
                 output += ' ' * (14-len(recommended)) + recommended
 
         if show_hint and (isinstance(self.results, TestFailure) or isinstance(self.results, TestWarn)) and self.results.hint is not None:
             output += "\n                  HINT:\n" + textwrap.indent(str(self.results.hint), "                       ")
 
         return output
 
-    def check_color(self):
+    def check_color(self) -> bool:
         for handler in self.cluster.log.handlers:
             if isinstance(handler, log.StdoutHandler) and handler.formatter.colorize:
                 return True
         return False
 
-    def get_readable_status(self):
+    def get_readable_status(self) -> str:
         if self.is_succeeded():
             return 'ok'
         if self.is_failed():
             return 'fail'
         if self.is_warned():
             return 'warning'
         if self.is_excepted():
             return 'exception'
 
-    def is_succeeded(self):
+        return "unknown"
+
+    def is_succeeded(self) -> bool:
         return self.status is TC_PASSED
 
-    def is_failed(self):
+    def is_failed(self) -> bool:
         return self.status is TC_FAILED
 
-    def is_warned(self):
+    def is_warned(self) -> bool:
         return self.status is TC_WARNED
 
-    def is_excepted(self):
+    def is_excepted(self) -> bool:
         return self.status is TC_EXCEPTED
 
 
 class TestCaseNegativeResult(BaseException):
 
-    def __init__(self, message, hint=None, group_result=None):
+    def __init__(self, message: str, hint: str = None):
         super().__init__(message)
         self.message = message
         self.hint = hint
-        self.group_result = group_result
 
 
 class TestFailure(TestCaseNegativeResult):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    pass
 
 
 class TestWarn(TestCaseNegativeResult):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    pass
 
 
 class TestSuite:
 
-    def __init__(self):
-        self.tcs = []
+    def __init__(self) -> None:
+        self.tcs: List[TestCase] = []
 
-    def register_tc(self, tc):
+    def register_tc(self, tc: TestCase) -> None:
         self.tcs.append(tc)
 
-    def is_any_test_failed(self):
+    def is_any_test_failed(self) -> bool:
         for tc in self.tcs:
             if tc.is_failed() or tc.is_excepted():
                 return True
         return False
 
-    def is_any_test_warned(self):
+    def is_any_test_warned(self) -> bool:
         for tc in self.tcs:
             if tc.is_warned():
                 return True
         return False
 
-    def get_final_summary(self, show_minimal=True, show_recommended=True):
+    def get_final_summary(self, show_minimal: bool = True, show_recommended: bool = True) -> str:
         result = "          Group    Status   ID    Test                                                               Actual result"
         if show_minimal:
             result += "        Minimal"
         if show_recommended:
             result += "   Recommended"
         result += "\n"
 
@@ -257,26 +252,26 @@
             else:
                 result += "%s %s  " % (value ,key.upper())
 
         result += "\n"
 
         return result
 
-    def print_final_status(self, log):
+    def print_final_status(self, logger: log.EnhancedLogger) -> None:
         if self.is_any_test_failed():
-            log.error("\nTEST FAILED"
+            logger.error("\nTEST FAILED"
                       "\nThe environment does not meet the minimal requirements. Check the test report and resolve the issues.")
             return
         if self.is_any_test_warned():
-            log.warning("\nTEST PASSED WITH WARNINGS"
+            logger.warning("\nTEST PASSED WITH WARNINGS"
                         "\nThe environment meets the minimal requirements, but is not as recommended. Try to check the test report and resolve the issues.")
             return
-        log.info("\nTEST PASSED")
+        logger.info("\nTEST PASSED")
 
-    def get_stats_data(self):
+    def get_stats_data(self) -> Dict[str, int]:
         results: Dict[str, int] = {}
         for tc in self.tcs:
             key = 'unknown'
             if tc.is_succeeded():
                 key = 'succeeded'
             elif tc.is_failed():
                 key = 'failed'
@@ -284,15 +279,15 @@
                 key = 'warned'
             elif tc.is_excepted():
                 key = 'excepted'
             value = results.get(key, 0) + 1
             results[key] = value
         return results
 
-    def save_csv(self, destination_file_path, delimiter=';'):
+    def save_csv(self, destination_file_path: str, delimiter: str = ';') -> None:
         stream = io.StringIO()
 
         csv_writer = csv.writer(stream, delimiter=delimiter, quotechar='"', quoting=csv.QUOTE_MINIMAL)
         csv_writer.writerow(['group', 'status', 'test_id', 'test_name', 'current_result', 'minimal_result', 'recommended_result'])
         for tc in self.tcs:
             csv_writer.writerow([
                 tc.category.lower(),
@@ -302,29 +297,29 @@
                 tc.results,
                 tc.minimal,
                 tc.recommended
             ])
 
         utils.dump_file({}, stream, destination_file_path, dump_location=False)
 
-    def save_html(self, destination_file_path, check_type, append_styles=True):
+    def save_html(self, destination_file_path: str, check_type: str, append_styles: bool = True) -> None:
         stream = io.StringIO()
 
         stream.write('<!DOCTYPE html><html><head><meta charset="utf-8"><title>%s Check Report</title></head><body><div id="date">%s</div><div id="stats">' % (check_type, datetime.utcnow()))
         for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
             stream.write('<div class="%s">%s %s</div>' % (key, value, key))
         stream.write('</div><h1>%s Check Report</h1><table>' % check_type)
         stream.write('<thead><tr><td>Group</td><td>Status</td><td>ID</td><td>Test</td><td>Actual Result</td><td>Minimal</td><td>Recommended</td></tr></thead><tbody>')
         for tc in self.tcs:
-            minimal = tc.minimal
-            if minimal is None:
-                minimal = ''
-            recommended = tc.recommended
-            if recommended is None:
-                recommended = ''
+            minimal = ''
+            if tc.minimal is not None:
+                minimal = str(tc.minimal)
+            recommended = ''
+            if tc.recommended is not None:
+                recommended = str(tc.recommended)
             stream.write('<tr class="%s"><td>%s</td><td><div>%s</div></td><td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>' %
                          (tc.get_readable_status(),
                           tc.category.lower(),
                           tc.get_readable_status(),
                           tc.id,
                           tc.name,
                           tc.results,
```

### Comparing `kubemarine-0.19.0/kubemarine/thirdparties.py` & `kubemarine-0.20.0/kubemarine/thirdparties.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,24 +377,24 @@
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     if not cluster.inventory['services'].get('thirdparties', {}):
         return
 
     for destination in cluster.inventory['services']['thirdparties'].keys():
-        skip_thirdparty = False
+        managing_plugin: Optional[str] = None
 
-        if cluster.context.get("initial_procedure") != "add_node":
-            # TODO: speed up algorithm via else/continue/break
-            for plugin_name, plugin_configs in cluster.inventory['plugins'].items():
-                for plugin_procedure in plugin_configs['installation']['procedures']:
-                    if plugin_procedure.get('thirdparty') == destination:
-                        log.verbose('Thirdparty \'%s\' should be installed with \'%s\' plugin'
-                                    % (destination, plugin_name))
-                        skip_thirdparty = True
+        # install and upgrade procedures have separate tasks for thirdparties managed by plugins
+        if cluster.context.get("initial_procedure") in ("install", "upgrade"):
+            managing_plugin = next((plugin_name
+                                    for plugin_name, plugin_configs in cluster.inventory['plugins'].items()
+                                    for plugin_procedure in plugin_configs['installation']['procedures']
+                                    if plugin_procedure.get('thirdparty') == destination),
+                                   None)
 
-        if skip_thirdparty:
-            log.verbose('Thirdparty %s installation delayed' % destination)
+        if managing_plugin is not None:
+            log.verbose('Thirdparty \'%s\' installation is delayed as it should be installed with \'%s\' plugin.'
+                        % (destination, managing_plugin))
         else:
             res = install_thirdparty(group, destination)
             if res is not None:
                 log.debug(res)
```

### Comparing `kubemarine-0.19.0/kubemarine/yum.py` & `kubemarine-0.20.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.19.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.20.0/kubemarine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.19.0
+Version: 0.20.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -34,36 +34,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -81,15 +81,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -100,15 +100,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.20.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -129,24 +129,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.19.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.20.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -175,42 +175,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.19.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.20.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.19.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.20.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.19.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.20.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.19.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.20.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.19.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.20.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.19.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.20.0/LICENSE)
```

### Comparing `kubemarine-0.19.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.20.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 kubemarine/kubernetes/__init__.py
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
+kubemarine/patches/p1_kubeadm_flags.py
 kubemarine/patches/software_upgrade.yaml
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
```

### Comparing `kubemarine-0.19.0/setup.py` & `kubemarine-0.20.0/setup.py`

 * *Files identical despite different names*

