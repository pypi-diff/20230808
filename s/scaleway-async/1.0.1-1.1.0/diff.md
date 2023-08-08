# Comparing `tmp/scaleway_async-1.0.1.tar.gz` & `tmp/scaleway_async-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_async-1.0.1.tar", max compression
+gzip compressed data, was "scaleway_async-1.1.0.tar", max compression
```

## Comparing `scaleway_async-1.0.1.tar` & `scaleway_async-1.1.0.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0       30 2023-08-07 09:35:28.530149 scaleway_async-1.0.1/README.md
--rw-r--r--   0        0        0     1123 2023-08-07 09:35:54.278707 scaleway_async-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      913 2023-08-07 09:35:28.530149 scaleway_async-1.0.1/scaleway_async/__init__.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.530149 scaleway_async-1.0.1/scaleway_async/account/__init__.py
--rw-r--r--   0        0        0      382 2023-08-07 09:35:28.530149 scaleway_async-1.0.1/scaleway_async/account/v2/__init__.py
--rw-r--r--   0        0        0     8672 2023-08-07 09:35:28.530149 scaleway_async-1.0.1/scaleway_async/account/v2/api.py
--rw-r--r--   0        0        0     2500 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v2/marshalling.py
--rw-r--r--   0        0        0     2636 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v2/types.py
--rw-r--r--   0        0        0      396 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v3/__init__.py
--rw-r--r--   0        0        0     8342 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v3/api.py
--rw-r--r--   0        0        0     2560 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v3/marshalling.py
--rw-r--r--   0        0        0     2676 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/account/v3/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/__init__.py
--rw-r--r--   0        0        0      968 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18230 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      497 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     6527 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7305 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/__init__.py
--rw-r--r--   0        0        0     3212 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    53458 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/v1/api.py
--rw-r--r--   0        0        0     1066 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/v1/content.py
--rw-r--r--   0        0        0    26856 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    28859 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/billing/__init__.py
--rw-r--r--   0        0        0      698 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/__init__.py
--rw-r--r--   0        0        0     4436 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/api.py
--rw-r--r--   0        0        0     3385 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/marshalling.py
--rw-r--r--   0        0        0     4206 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/cockpit/__init__.py
--rw-r--r--   0        0        0     1468 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    26849 2023-08-07 09:35:28.534149 scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      419 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    15740 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0    10634 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/__init__.py
--rw-r--r--   0        0        0     3386 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    65864 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/v1beta1/api.py
--rw-r--r--   0        0        0     1587 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/v1beta1/content.py
--rw-r--r--   0        0        0    26245 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    28456 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/__init__.py
--rw-r--r--   0        0        0     8426 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    87528 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1955 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/v2beta1/content.py
--rw-r--r--   0        0        0    88058 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    40494 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/__init__.py
--rw-r--r--   0        0        0      978 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20847 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      651 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     7038 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     9176 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/__init__.py
--rw-r--r--   0        0        0     3642 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    64980 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/v1beta1/api.py
--rw-r--r--   0        0        0     1579 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/v1beta1/content.py
--rw-r--r--   0        0        0    28021 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    30155 2023-08-07 09:35:28.538149 scaleway_async-1.0.1/scaleway_async/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iam/__init__.py
--rw-r--r--   0        0        0     2300 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    74957 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    26114 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    30264 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/__init__.py
--rw-r--r--   0        0        0     8194 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/__init__.py
--rw-r--r--   0        0        0   131162 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/api.py
--rw-r--r--   0        0        0     2210 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/content.py
--rw-r--r--   0        0        0    97574 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/marshalling.py
--rw-r--r--   0        0        0    57214 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/types.py
--rw-r--r--   0        0        0    11049 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/__init__.py
--rw-r--r--   0        0        0     3456 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/v1/__init__.py
--rw-r--r--   0        0        0    62302 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/v1/api.py
--rw-r--r--   0        0        0      364 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/v1/content.py
--rw-r--r--   0        0        0    31989 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/v1/marshalling.py
--rw-r--r--   0        0        0    33256 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/iot/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/__init__.py
--rw-r--r--   0        0        0     3430 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/__init__.py
--rw-r--r--   0        0        0    58254 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/api.py
--rw-r--r--   0        0        0      937 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/content.py
--rw-r--r--   0        0        0    34447 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    45370 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/types.py
--rw-r--r--   0        0        0      540 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/k8s/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/lb/__init__.py
--rw-r--r--   0        0        0     5060 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/lb/v1/__init__.py
--rw-r--r--   0        0        0   226461 2023-08-07 09:35:28.542149 scaleway_async-1.0.1/scaleway_async/lb/v1/api.py
--rw-r--r--   0        0        0     1111 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/lb/v1/content.py
--rw-r--r--   0        0        0    83655 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/lb/v1/marshalling.py
--rw-r--r--   0        0        0   102503 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/lb/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/__init__.py
--rw-r--r--   0        0        0      636 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v1/__init__.py
--rw-r--r--   0        0        0     4172 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v1/api.py
--rw-r--r--   0        0        0     5360 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v1/marshalling.py
--rw-r--r--   0        0        0     3161 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v1/types.py
--rw-r--r--   0        0        0      948 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    14905 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v2/api.py
--rw-r--r--   0        0        0     5380 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     5365 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/mnq/__init__.py
--rw-r--r--   0        0        0     1008 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18549 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/api.py
--rw-r--r--   0        0        0     8332 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     9028 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/types.py
--rw-r--r--   0        0        0        0 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/py.typed
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/__init__.py
--rw-r--r--   0        0        0     5874 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/v1/__init__.py
--rw-r--r--   0        0        0   118057 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/v1/api.py
--rw-r--r--   0        0        0     1956 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/v1/content.py
--rw-r--r--   0        0        0    50774 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    53443 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/__init__.py
--rw-r--r--   0        0        0     2130 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/v1/__init__.py
--rw-r--r--   0        0        0    44493 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/v1/api.py
--rw-r--r--   0        0        0      489 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/v1/content.py
--rw-r--r--   0        0        0    20527 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/v1/marshalling.py
--rw-r--r--   0        0        0    19830 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/redis/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/__init__.py
--rw-r--r--   0        0        0     1190 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/v1/__init__.py
--rw-r--r--   0        0        0    29053 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/v1/api.py
--rw-r--r--   0        0        0      713 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/v1/content.py
--rw-r--r--   0        0        0     7013 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/v1/marshalling.py
--rw-r--r--   0        0        0    11691 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/registry/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/secret/__init__.py
--rw-r--r--   0        0        0      946 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    42808 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/api.py
--rw-r--r--   0        0        0     9169 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    16883 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/tem/__init__.py
--rw-r--r--   0        0        0     1522 2023-08-07 09:35:28.546149 scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    24987 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      551 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/content.py
--rw-r--r--   0        0        0    11457 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    14380 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/__init__.py
--rw-r--r--   0        0        0      598 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/v1/__init__.py
--rw-r--r--   0        0        0    12099 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/v1/api.py
--rw-r--r--   0        0        0      350 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/v1/content.py
--rw-r--r--   0        0        0     5840 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/v1/marshalling.py
--rw-r--r--   0        0        0     3303 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/test/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/__init__.py
--rw-r--r--   0        0        0      416 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v1/__init__.py
--rw-r--r--   0        0        0    11833 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v1/api.py
--rw-r--r--   0        0        0     2898 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     4346 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v1/types.py
--rw-r--r--   0        0        0      820 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v2/__init__.py
--rw-r--r--   0        0        0    29529 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v2/api.py
--rw-r--r--   0        0        0     9247 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v2/marshalling.py
--rw-r--r--   0        0        0    10566 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpc/v2/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/__init__.py
--rw-r--r--   0        0        0     2168 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    79348 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/v1/api.py
--rw-r--r--   0        0        0      757 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/v1/content.py
--rw-r--r--   0        0        0    25219 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    35284 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/vpcgw/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/__init__.py
--rw-r--r--   0        0        0     1378 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/__init__.py
--rw-r--r--   0        0        0    17184 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/api.py
--rw-r--r--   0        0        0      422 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/content.py
--rw-r--r--   0        0        0     8924 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    10942 2023-08-07 09:35:28.550149 scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/types.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 scaleway_async-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/README.md
+-rw-r--r--   0        0        0     1123 2023-08-08 08:29:55.286882 scaleway_async-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      913 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/__init__.py
+-rw-r--r--   0        0        0      382 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v2/__init__.py
+-rw-r--r--   0        0        0     8672 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v2/api.py
+-rw-r--r--   0        0        0     2500 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2713 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v2/types.py
+-rw-r--r--   0        0        0      396 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v3/__init__.py
+-rw-r--r--   0        0        0     8342 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v3/api.py
+-rw-r--r--   0        0        0     2560 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v3/marshalling.py
+-rw-r--r--   0        0        0     2753 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/account/v3/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/__init__.py
+-rw-r--r--   0        0        0      968 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18230 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      497 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0     6527 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7427 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/baremetal/__init__.py
+-rw-r--r--   0        0        0     3212 2023-08-08 08:29:36.378365 scaleway_async-1.1.0/scaleway_async/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    53458 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1066 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/baremetal/v1/content.py
+-rw-r--r--   0        0        0    26856 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    29257 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/billing/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/__init__.py
+-rw-r--r--   0        0        0     4436 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/api.py
+-rw-r--r--   0        0        0     3385 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/marshalling.py
+-rw-r--r--   0        0        0     4328 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/__init__.py
+-rw-r--r--   0        0        0     1468 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    26849 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      419 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    15740 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    10825 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/__init__.py
+-rw-r--r--   0        0        0     3386 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    65864 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1587 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/v1beta1/content.py
+-rw-r--r--   0        0        0    26245 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    28946 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/__init__.py
+-rw-r--r--   0        0        0     8426 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    87528 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1955 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    88058 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    41122 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.382365 scaleway_async-1.1.0/scaleway_async/flexibleip/__init__.py
+-rw-r--r--   0        0        0      978 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20847 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      651 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     7038 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9321 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/__init__.py
+-rw-r--r--   0        0        0     3642 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    64980 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1579 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/v1beta1/content.py
+-rw-r--r--   0        0        0    28021 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    30668 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iam/__init__.py
+-rw-r--r--   0        0        0     2300 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    74957 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    26114 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    30617 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/__init__.py
+-rw-r--r--   0        0        0     8194 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/__init__.py
+-rw-r--r--   0        0        0   131162 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/api.py
+-rw-r--r--   0        0        0     2210 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/content.py
+-rw-r--r--   0        0        0    97574 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/marshalling.py
+-rw-r--r--   0        0        0    57885 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/types.py
+-rw-r--r--   0        0        0    11049 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/__init__.py
+-rw-r--r--   0        0        0     3456 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/v1/__init__.py
+-rw-r--r--   0        0        0    62302 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/v1/api.py
+-rw-r--r--   0        0        0      364 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/v1/content.py
+-rw-r--r--   0        0        0    31989 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    33631 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/k8s/__init__.py
+-rw-r--r--   0        0        0     3430 2023-08-08 08:29:36.386365 scaleway_async-1.1.0/scaleway_async/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    58254 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/k8s/v1/api.py
+-rw-r--r--   0        0        0      937 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/k8s/v1/content.py
+-rw-r--r--   0        0        0    34447 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    45768 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/k8s/v1/types.py
+-rw-r--r--   0        0        0      540 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/k8s/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/__init__.py
+-rw-r--r--   0        0        0     5060 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/v1/__init__.py
+-rw-r--r--   0        0        0   226461 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/v1/api.py
+-rw-r--r--   0        0        0     1111 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/v1/content.py
+-rw-r--r--   0        0        0    83655 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/v1/marshalling.py
+-rw-r--r--   0        0        0   103131 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/__init__.py
+-rw-r--r--   0        0        0      636 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v1/__init__.py
+-rw-r--r--   0        0        0     4172 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v1/api.py
+-rw-r--r--   0        0        0     5360 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v1/marshalling.py
+-rw-r--r--   0        0        0     3161 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v1/types.py
+-rw-r--r--   0        0        0      948 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    14905 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v2/api.py
+-rw-r--r--   0        0        0     5380 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     5510 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/mnq/__init__.py
+-rw-r--r--   0        0        0     1008 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18549 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/api.py
+-rw-r--r--   0        0        0     8332 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9150 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/py.typed
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/__init__.py
+-rw-r--r--   0        0        0     5874 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   118057 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/v1/api.py
+-rw-r--r--   0        0        0     1956 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/v1/content.py
+-rw-r--r--   0        0        0    50774 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    53979 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/__init__.py
+-rw-r--r--   0        0        0     2130 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/v1/__init__.py
+-rw-r--r--   0        0        0    44493 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/v1/api.py
+-rw-r--r--   0        0        0      489 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/v1/content.py
+-rw-r--r--   0        0        0    20527 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    19998 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/__init__.py
+-rw-r--r--   0        0        0     1190 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/v1/__init__.py
+-rw-r--r--   0        0        0    29053 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/v1/api.py
+-rw-r--r--   0        0        0      713 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/v1/content.py
+-rw-r--r--   0        0        0     7013 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    11905 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/secret/__init__.py
+-rw-r--r--   0        0        0      946 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    42808 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0     9169 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    17051 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/__init__.py
+-rw-r--r--   0        0        0     1522 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    24987 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      551 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0    11457 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    14571 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/test/__init__.py
+-rw-r--r--   0        0        0      598 2023-08-08 08:29:36.390365 scaleway_async-1.1.0/scaleway_async/test/v1/__init__.py
+-rw-r--r--   0        0        0    12099 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/test/v1/api.py
+-rw-r--r--   0        0        0      350 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/test/v1/content.py
+-rw-r--r--   0        0        0     5840 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3426 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/test/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/__init__.py
+-rw-r--r--   0        0        0      416 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    11833 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v1/api.py
+-rw-r--r--   0        0        0     2898 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4422 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v1/types.py
+-rw-r--r--   0        0        0      820 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v2/__init__.py
+-rw-r--r--   0        0        0    29529 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v2/api.py
+-rw-r--r--   0        0        0     9247 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v2/marshalling.py
+-rw-r--r--   0        0        0    10665 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpc/v2/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/__init__.py
+-rw-r--r--   0        0        0     2168 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    79348 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      757 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    25219 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    35567 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/__init__.py
+-rw-r--r--   0        0        0     1378 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    17184 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      422 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0     8924 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    11202 2023-08-08 08:29:36.394365 scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 scaleway_async-1.1.0/PKG-INFO
```

### Comparing `scaleway_async-1.0.1/pyproject.toml` & `scaleway_async-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-async"
-version = "1.0.1"
+version = "1.1.0"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway_async-1.0.1/scaleway_async/__init__.py` & `scaleway_async-1.1.0/scaleway_async/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v2/api.py` & `scaleway_async-1.1.0/scaleway_async/account/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v2/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/account/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v2/types.py` & `scaleway_async-1.1.0/scaleway_async/account/v3/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
-class ListProjectsRequestOrderBy(str, Enum):
+
+class ListProjectsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
@@ -69,33 +73,33 @@
     description: str
     """
     Description of the Project.
     """
 
 
 @dataclass
-class CreateProjectRequest:
+class ProjectApiCreateProjectRequest:
     name: Optional[str]
     """
     Name of the Project.
     """
 
     organization_id: Optional[str]
     """
     Organization ID of the Project.
     """
 
-    description: Optional[str]
+    description: str
     """
     Description of the Project.
     """
 
 
 @dataclass
-class ListProjectsRequest:
+class ProjectApiListProjectsRequest:
     organization_id: Optional[str]
     """
     Organization ID of the Project.
     """
 
     name: Optional[str]
     """
@@ -120,31 +124,31 @@
     project_ids: Optional[List[str]]
     """
     Project IDs to filter for. The results will be limited to any Projects with an ID in this array.
     """
 
 
 @dataclass
-class GetProjectRequest:
+class ProjectApiGetProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
 
 @dataclass
-class DeleteProjectRequest:
+class ProjectApiDeleteProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
 
 @dataclass
-class UpdateProjectRequest:
+class ProjectApiUpdateProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
     name: Optional[str]
     """
```

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v3/api.py` & `scaleway_async-1.1.0/scaleway_async/account/v3/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v3/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/account/v3/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/account/v3/types.py` & `scaleway_async-1.1.0/scaleway_async/account/v2/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
-class ListProjectsRequestOrderBy(str, Enum):
+
+class ListProjectsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
@@ -69,33 +73,33 @@
     description: str
     """
     Description of the Project.
     """
 
 
 @dataclass
-class ProjectApiCreateProjectRequest:
+class CreateProjectRequest:
     name: Optional[str]
     """
     Name of the Project.
     """
 
     organization_id: Optional[str]
     """
     Organization ID of the Project.
     """
 
-    description: str
+    description: Optional[str]
     """
     Description of the Project.
     """
 
 
 @dataclass
-class ProjectApiListProjectsRequest:
+class ListProjectsRequest:
     organization_id: Optional[str]
     """
     Organization ID of the Project.
     """
 
     name: Optional[str]
     """
@@ -120,31 +124,31 @@
     project_ids: Optional[List[str]]
     """
     Project IDs to filter for. The results will be limited to any Projects with an ID in this array.
     """
 
 
 @dataclass
-class ProjectApiGetProjectRequest:
+class GetProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
 
 @dataclass
-class ProjectApiDeleteProjectRequest:
+class DeleteProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
 
 @dataclass
-class ProjectApiUpdateProjectRequest:
+class UpdateProjectRequest:
     project_id: Optional[str]
     """
     Project ID of the Project.
     """
 
     name: Optional[str]
     """
```

### Comparing `scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/applesilicon/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/applesilicon/v1alpha1/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListServersRequestOrderBy(str, Enum):
+class ListServersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerStatus(str, Enum):
+class ServerStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     STARTING = "starting"
     READY = "ready"
     ERROR = "error"
     REBOOTING = "rebooting"
     UPDATING = "updating"
     LOCKING = "locking"
@@ -32,15 +35,15 @@
     UNLOCKING = "unlocking"
     REINSTALLING = "reinstalling"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerTypeStock(str, Enum):
+class ServerTypeStock(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STOCK = "unknown_stock"
     NO_STOCK = "no_stock"
     LOW_STOCK = "low_stock"
     HIGH_STOCK = "high_stock"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/baremetal/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/baremetal/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/baremetal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/baremetal/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/baremetal/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/baremetal/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/baremetal/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/baremetal/v1/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,139 +8,142 @@
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Money,
     TimeSeries,
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class IPReverseStatus(str, Enum):
+class IPReverseStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     PENDING = "pending"
     ACTIVE = "active"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class IPVersion(str, Enum):
+class IPVersion(str, Enum, metaclass=StrEnumMeta):
     IPV4 = "IPv4"
     IPV6 = "IPv6"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListServerEventsRequestOrderBy(str, Enum):
+class ListServerEventsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListServerPrivateNetworksRequestOrderBy(str, Enum):
+class ListServerPrivateNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListServersRequestOrderBy(str, Enum):
+class ListServersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListSettingsRequestOrderBy(str, Enum):
+class ListSettingsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class OfferStock(str, Enum):
+class OfferStock(str, Enum, metaclass=StrEnumMeta):
     EMPTY = "empty"
     LOW = "low"
     AVAILABLE = "available"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class OfferSubscriptionPeriod(str, Enum):
+class OfferSubscriptionPeriod(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_SUBSCRIPTION_PERIOD = "unknown_subscription_period"
     HOURLY = "hourly"
     MONTHLY = "monthly"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerBootType(str, Enum):
+class ServerBootType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_BOOT_TYPE = "unknown_boot_type"
     NORMAL = "normal"
     RESCUE = "rescue"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerInstallStatus(str, Enum):
+class ServerInstallStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     TO_INSTALL = "to_install"
     INSTALLING = "installing"
     COMPLETED = "completed"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerOptionOptionStatus(str, Enum):
+class ServerOptionOptionStatus(str, Enum, metaclass=StrEnumMeta):
     OPTION_STATUS_UNKNOWN = "option_status_unknown"
     OPTION_STATUS_ENABLE = "option_status_enable"
     OPTION_STATUS_ENABLING = "option_status_enabling"
     OPTION_STATUS_DISABLING = "option_status_disabling"
     OPTION_STATUS_ERROR = "option_status_error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerPingStatus(str, Enum):
+class ServerPingStatus(str, Enum, metaclass=StrEnumMeta):
     PING_STATUS_UNKNOWN = "ping_status_unknown"
     PING_STATUS_UP = "ping_status_up"
     PING_STATUS_DOWN = "ping_status_down"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerPrivateNetworkStatus(str, Enum):
+class ServerPrivateNetworkStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ATTACHING = "attaching"
     ATTACHED = "attached"
     ERROR = "error"
     DETACHING = "detaching"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerStatus(str, Enum):
+class ServerStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     DELIVERING = "delivering"
     READY = "ready"
     STOPPING = "stopping"
     STOPPED = "stopped"
     STARTING = "starting"
     ERROR = "error"
@@ -150,15 +153,15 @@
     ORDERED = "ordered"
     RESETTING = "resetting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SettingType(str, Enum):
+class SettingType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     SMTP = "smtp"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/billing/v2alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/billing/v2alpha1/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Money,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class DownloadInvoiceRequestFileType(str, Enum):
+class DownloadInvoiceRequestFileType(str, Enum, metaclass=StrEnumMeta):
     PDF = "pdf"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class InvoiceType(str, Enum):
+class InvoiceType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_TYPE = "unknown_type"
     PERIODIC = "periodic"
     PURCHASE = "purchase"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListInvoicesRequestOrderBy(str, Enum):
+class ListInvoicesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     INVOICE_NUMBER_DESC = "invoice_number_desc"
     INVOICE_NUMBER_ASC = "invoice_number_asc"
     START_DATE_DESC = "start_date_desc"
     START_DATE_ASC = "start_date_asc"
     ISSUED_DATE_DESC = "issued_date_desc"
     ISSUED_DATE_ASC = "issued_date_asc"
     DUE_DATE_DESC = "due_date_desc"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/api.py` & `scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/cockpit/v1beta1/types.py` & `scaleway_async-1.1.0/scaleway_async/cockpit/v1beta1/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,64 +6,67 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     TimeSeries,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class CockpitStatus(str, Enum):
+class CockpitStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     CREATING = "creating"
     READY = "ready"
     DELETING = "deleting"
     UPDATING = "updating"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class GrafanaUserRole(str, Enum):
+class GrafanaUserRole(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_ROLE = "unknown_role"
     EDITOR = "editor"
     VIEWER = "viewer"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListGrafanaUsersRequestOrderBy(str, Enum):
+class ListGrafanaUsersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     LOGIN_ASC = "login_asc"
     LOGIN_DESC = "login_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPlansRequestOrderBy(str, Enum):
+class ListPlansRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTokensRequestOrderBy(str, Enum):
+class ListTokensRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PlanName(str, Enum):
+class PlanName(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_NAME = "unknown_name"
     FREE = "free"
     PREMIUM = "premium"
     CUSTOM = "custom"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/container/v1beta1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/container/v1beta1/api.py` & `scaleway_async-1.1.0/scaleway_async/container/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/container/v1beta1/content.py` & `scaleway_async-1.1.0/scaleway_async/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/container/v1beta1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/container/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/container/v1beta1/types.py` & `scaleway_async-1.1.0/scaleway_async/container/v1beta1/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,196 +6,199 @@
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ContainerHttpOption(str, Enum):
+class ContainerHttpOption(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_HTTP_OPTION = "unknown_http_option"
     ENABLED = "enabled"
     REDIRECTED = "redirected"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContainerPrivacy(str, Enum):
+class ContainerPrivacy(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_PRIVACY = "unknown_privacy"
     PUBLIC = "public"
     PRIVATE = "private"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContainerProtocol(str, Enum):
+class ContainerProtocol(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_PROTOCOL = "unknown_protocol"
     HTTP1 = "http1"
     H2C = "h2c"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContainerStatus(str, Enum):
+class ContainerStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
     CREATED = "created"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class CronStatus(str, Enum):
+class CronStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainStatus(str, Enum):
+class DomainStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListContainersRequestOrderBy(str, Enum):
+class ListContainersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListCronsRequestOrderBy(str, Enum):
+class ListCronsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDomainsRequestOrderBy(str, Enum):
+class ListDomainsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     HOSTNAME_ASC = "hostname_asc"
     HOSTNAME_DESC = "hostname_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListLogsRequestOrderBy(str, Enum):
+class ListLogsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     TIMESTAMP_DESC = "timestamp_desc"
     TIMESTAMP_ASC = "timestamp_asc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNamespacesRequestOrderBy(str, Enum):
+class ListNamespacesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTokensRequestOrderBy(str, Enum):
+class ListTokensRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTriggersRequestOrderBy(str, Enum):
+class ListTriggersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LogStream(str, Enum):
+class LogStream(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     STDOUT = "stdout"
     STDERR = "stderr"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NamespaceStatus(str, Enum):
+class NamespaceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NullValue(str, Enum):
+class NullValue(str, Enum, metaclass=StrEnumMeta):
     NULL_VALUE = "NULL_VALUE"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TokenStatus(str, Enum):
+class TokenStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TriggerInputType(str, Enum):
+class TriggerInputType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_INPUT_TYPE = "unknown_input_type"
     SQS = "sqs"
     SCW_SQS = "scw_sqs"
     NATS = "nats"
     SCW_NATS = "scw_nats"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TriggerStatus(str, Enum):
+class TriggerStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
     PENDING = "pending"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/domain/v2beta1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/domain/v2beta1/api.py` & `scaleway_async-1.1.0/scaleway_async/domain/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/domain/v2beta1/content.py` & `scaleway_async-1.1.0/scaleway_async/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/domain/v2beta1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/domain/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/domain/v2beta1/types.py` & `scaleway_async-1.1.0/scaleway_async/domain/v2beta1/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,41 +6,44 @@
 from datetime import datetime
 from enum import Enum
 from typing import Dict, List, Optional
 
 from scaleway_core.bridge import (
     Money,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ContactEmailStatus(str, Enum):
+class ContactEmailStatus(str, Enum, metaclass=StrEnumMeta):
     EMAIL_STATUS_UNKNOWN = "email_status_unknown"
     VALIDATED = "validated"
     NOT_VALIDATED = "not_validated"
     INVALID_EMAIL = "invalid_email"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContactExtensionFRMode(str, Enum):
+class ContactExtensionFRMode(str, Enum, metaclass=StrEnumMeta):
     MODE_UNKNOWN = "mode_unknown"
     INDIVIDUAL = "individual"
     COMPANY_IDENTIFICATION_CODE = "company_identification_code"
     DUNS = "duns"
     LOCAL = "local"
     ASSOCIATION = "association"
     TRADEMARK = "trademark"
     CODE_AUTH_AFNIC = "code_auth_afnic"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContactExtensionNLLegalForm(str, Enum):
+class ContactExtensionNLLegalForm(str, Enum, metaclass=StrEnumMeta):
     LEGAL_FORM_UNKNOWN = "legal_form_unknown"
     OTHER = "other"
     NON_DUTCH_EU_COMPANY = "non_dutch_eu_company"
     NON_DUTCH_LEGAL_FORM_ENTERPRISE_SUBSIDIARY = (
         "non_dutch_legal_form_enterprise_subsidiary"
     )
     LIMITED_COMPANY = "limited_company"
@@ -60,37 +63,37 @@
     TRADING_PARTNERSHIP = "trading_partnership"
     NATURAL_PERSON = "natural_person"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ContactLegalForm(str, Enum):
+class ContactLegalForm(str, Enum, metaclass=StrEnumMeta):
     LEGAL_FORM_UNKNOWN = "legal_form_unknown"
     INDIVIDUAL = "individual"
     CORPORATE = "corporate"
     ASSOCIATION = "association"
     OTHER = "other"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DNSZoneStatus(str, Enum):
+class DNSZoneStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ACTIVE = "active"
     PENDING = "pending"
     ERROR = "error"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DSRecordAlgorithm(str, Enum):
+class DSRecordAlgorithm(str, Enum, metaclass=StrEnumMeta):
     RSAMD5 = "rsamd5"
     DH = "dh"
     DSA = "dsa"
     RSASHA1 = "rsasha1"
     DSA_NSEC3_SHA1 = "dsa_nsec3_sha1"
     RSASHA1_NSEC3_SHA1 = "rsasha1_nsec3_sha1"
     RSASHA256 = "rsasha256"
@@ -101,45 +104,45 @@
     ED25519 = "ed25519"
     ED448 = "ed448"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DSRecordDigestType(str, Enum):
+class DSRecordDigestType(str, Enum, metaclass=StrEnumMeta):
     SHA_1 = "sha_1"
     SHA_256 = "sha_256"
     GOST_R_34_11_94 = "gost_r_34_11_94"
     SHA_384 = "sha_384"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainFeatureStatus(str, Enum):
+class DomainFeatureStatus(str, Enum, metaclass=StrEnumMeta):
     FEATURE_STATUS_UNKNOWN = "feature_status_unknown"
     ENABLING = "enabling"
     ENABLED = "enabled"
     DISABLING = "disabling"
     DISABLED = "disabled"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainRecordHTTPServiceConfigStrategy(str, Enum):
+class DomainRecordHTTPServiceConfigStrategy(str, Enum, metaclass=StrEnumMeta):
     RANDOM = "random"
     HASHED = "hashed"
     ALL = "all"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainRecordType(str, Enum):
+class DomainRecordType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     A = "A"
     AAAA = "AAAA"
     CNAME = "CNAME"
     TXT = "TXT"
     SRV = "SRV"
     TLSA = "TLSA"
@@ -157,27 +160,27 @@
     NAPTR = "NAPTR"
     DNAME = "DNAME"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainRegistrationStatusTransferStatus(str, Enum):
+class DomainRegistrationStatusTransferStatus(str, Enum, metaclass=StrEnumMeta):
     STATUS_UNKNOWN = "status_unknown"
     PENDING = "pending"
     WAITING_VOTE = "waiting_vote"
     REJECTED = "rejected"
     PROCESSING = "processing"
     DONE = "done"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainStatus(str, Enum):
+class DomainStatus(str, Enum, metaclass=StrEnumMeta):
     STATUS_UNKNOWN = "status_unknown"
     ACTIVE = "active"
     CREATING = "creating"
     CREATE_ERROR = "create_error"
     RENEWING = "renewing"
     RENEW_ERROR = "renew_error"
     XFERING = "xfering"
@@ -189,134 +192,134 @@
     LOCKED = "locked"
     DELETING = "deleting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HostStatus(str, Enum):
+class HostStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     ACTIVE = "active"
     UPDATING = "updating"
     DELETING = "deleting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LanguageCode(str, Enum):
+class LanguageCode(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_LANGUAGE_CODE = "unknown_language_code"
     EN_US = "en_US"
     FR_FR = "fr_FR"
     DE_DE = "de_DE"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListContactsRequestRole(str, Enum):
+class ListContactsRequestRole(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_ROLE = "unknown_role"
     OWNER = "owner"
     ADMINISTRATIVE = "administrative"
     TECHNICAL = "technical"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDNSZoneRecordsRequestOrderBy(str, Enum):
+class ListDNSZoneRecordsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDNSZonesRequestOrderBy(str, Enum):
+class ListDNSZonesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     DOMAIN_ASC = "domain_asc"
     DOMAIN_DESC = "domain_desc"
     SUBDOMAIN_ASC = "subdomain_asc"
     SUBDOMAIN_DESC = "subdomain_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDomainsRequestOrderBy(str, Enum):
+class ListDomainsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     DOMAIN_ASC = "domain_asc"
     DOMAIN_DESC = "domain_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListRenewableDomainsRequestOrderBy(str, Enum):
+class ListRenewableDomainsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     DOMAIN_ASC = "domain_asc"
     DOMAIN_DESC = "domain_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTasksRequestOrderBy(str, Enum):
+class ListTasksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     DOMAIN_DESC = "domain_desc"
     DOMAIN_ASC = "domain_asc"
     TYPE_ASC = "type_asc"
     TYPE_DESC = "type_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RawFormat(str, Enum):
+class RawFormat(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RAW_FORMAT = "unknown_raw_format"
     BIND = "bind"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RenewableDomainStatus(str, Enum):
+class RenewableDomainStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     RENEWABLE = "renewable"
     LATE_RENEWEABLE = "late_reneweable"
     NOT_RENEWABLE = "not_renewable"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SSLCertificateStatus(str, Enum):
+class SSLCertificateStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     NEW = "new"
     PENDING = "pending"
     SUCCESS = "success"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TaskStatus(str, Enum):
+class TaskStatus(str, Enum, metaclass=StrEnumMeta):
     UNAVAILABLE = "unavailable"
     NEW = "new"
     WAITING_PAYMENT = "waiting_payment"
     PENDING = "pending"
     SUCCESS = "success"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TaskType(str, Enum):
+class TaskType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATE_DOMAIN = "create_domain"
     CREATE_EXTERNAL_DOMAIN = "create_external_domain"
     RENEW_DOMAIN = "renew_domain"
     TRANSFER_DOMAIN = "transfer_domain"
     TRADE_DOMAIN = "trade_domain"
     LOCK_DOMAIN_TRANSFER = "lock_domain_transfer"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/content.py` & `scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/flexibleip/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/flexibleip/v1alpha1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,50 +6,53 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class FlexibleIPStatus(str, Enum):
+class FlexibleIPStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     UPDATING = "updating"
     ATTACHED = "attached"
     ERROR = "error"
     DETACHING = "detaching"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListFlexibleIPsRequestOrderBy(str, Enum):
+class ListFlexibleIPsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class MACAddressStatus(str, Enum):
+class MACAddressStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     UPDATING = "updating"
     USED = "used"
     ERROR = "error"
     DELETING = "deleting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class MACAddressType(str, Enum):
+class MACAddressType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_TYPE = "unknown_type"
     VMWARE = "vmware"
     XEN = "xen"
     KVM = "kvm"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/function/v1beta1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/function/v1beta1/api.py` & `scaleway_async-1.1.0/scaleway_async/function/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/function/v1beta1/content.py` & `scaleway_async-1.1.0/scaleway_async/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/function/v1beta1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/function/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/function/v1beta1/types.py` & `scaleway_async-1.1.0/scaleway_async/function/v1beta1/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,60 +6,63 @@
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class CronStatus(str, Enum):
+class CronStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainStatus(str, Enum):
+class DomainStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class FunctionHttpOption(str, Enum):
+class FunctionHttpOption(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_HTTP_OPTION = "unknown_http_option"
     ENABLED = "enabled"
     REDIRECTED = "redirected"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class FunctionPrivacy(str, Enum):
+class FunctionPrivacy(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_PRIVACY = "unknown_privacy"
     PUBLIC = "public"
     PRIVATE = "private"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class FunctionRuntime(str, Enum):
+class FunctionRuntime(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RUNTIME = "unknown_runtime"
     GOLANG = "golang"
     PYTHON = "python"
     PYTHON3 = "python3"
     NODE8 = "node8"
     NODE10 = "node10"
     NODE14 = "node14"
@@ -81,154 +84,154 @@
     GO120 = "go120"
     NODE20 = "node20"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class FunctionStatus(str, Enum):
+class FunctionStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
     CREATED = "created"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListCronsRequestOrderBy(str, Enum):
+class ListCronsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDomainsRequestOrderBy(str, Enum):
+class ListDomainsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     HOSTNAME_ASC = "hostname_asc"
     HOSTNAME_DESC = "hostname_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListFunctionsRequestOrderBy(str, Enum):
+class ListFunctionsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListLogsRequestOrderBy(str, Enum):
+class ListLogsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     TIMESTAMP_DESC = "timestamp_desc"
     TIMESTAMP_ASC = "timestamp_asc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNamespacesRequestOrderBy(str, Enum):
+class ListNamespacesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTokensRequestOrderBy(str, Enum):
+class ListTokensRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTriggersRequestOrderBy(str, Enum):
+class ListTriggersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LogStream(str, Enum):
+class LogStream(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     STDOUT = "stdout"
     STDERR = "stderr"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NamespaceStatus(str, Enum):
+class NamespaceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     CREATING = "creating"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NullValue(str, Enum):
+class NullValue(str, Enum, metaclass=StrEnumMeta):
     NULL_VALUE = "NULL_VALUE"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RuntimeStatus(str, Enum):
+class RuntimeStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     BETA = "beta"
     AVAILABLE = "available"
     DEPRECATED = "deprecated"
     END_OF_SUPPORT = "end_of_support"
     END_OF_LIFE = "end_of_life"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TokenStatus(str, Enum):
+class TokenStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TriggerInputType(str, Enum):
+class TriggerInputType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_INPUT_TYPE = "unknown_input_type"
     SQS = "sqs"
     SCW_SQS = "scw_sqs"
     NATS = "nats"
     SCW_NATS = "scw_nats"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TriggerStatus(str, Enum):
+class TriggerStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     CREATING = "creating"
     PENDING = "pending"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iam/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/iam/v1alpha1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,146 +3,150 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
-class BearerType(str, Enum):
+
+class BearerType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_BEARER_TYPE = "unknown_bearer_type"
     USER = "user"
     APPLICATION = "application"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListAPIKeysRequestOrderBy(str, Enum):
+class ListAPIKeysRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     EXPIRES_AT_ASC = "expires_at_asc"
     EXPIRES_AT_DESC = "expires_at_desc"
     ACCESS_KEY_ASC = "access_key_asc"
     ACCESS_KEY_DESC = "access_key_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListApplicationsRequestOrderBy(str, Enum):
+class ListApplicationsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListGroupsRequestOrderBy(str, Enum):
+class ListGroupsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListJWTsRequestOrderBy(str, Enum):
+class ListJWTsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPermissionSetsRequestOrderBy(str, Enum):
+class ListPermissionSetsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPoliciesRequestOrderBy(str, Enum):
+class ListPoliciesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     POLICY_NAME_ASC = "policy_name_asc"
     POLICY_NAME_DESC = "policy_name_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListQuotaRequestOrderBy(str, Enum):
+class ListQuotaRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListSSHKeysRequestOrderBy(str, Enum):
+class ListSSHKeysRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListUsersRequestOrderBy(str, Enum):
+class ListUsersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     EMAIL_ASC = "email_asc"
     EMAIL_DESC = "email_desc"
     LAST_LOGIN_ASC = "last_login_asc"
     LAST_LOGIN_DESC = "last_login_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PermissionSetScopeType(str, Enum):
+class PermissionSetScopeType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_SCOPE_TYPE = "unknown_scope_type"
     PROJECTS = "projects"
     ORGANIZATION = "organization"
     ACCOUNT_ROOT_USER = "account_root_user"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class UserStatus(str, Enum):
+class UserStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     INVITATION_PENDING = "invitation_pending"
     ACTIVATED = "activated"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class UserType(str, Enum):
+class UserType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_TYPE = "unknown_type"
     GUEST = "guest"
     OWNER = "owner"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,259 +6,263 @@
 from datetime import datetime
 from enum import Enum
 from typing import Dict, List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class Arch(str, Enum):
+class Arch(str, Enum, metaclass=StrEnumMeta):
     X86_64 = "x86_64"
     ARM = "arm"
+    ARM64 = "arm64"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class BootType(str, Enum):
+class BootType(str, Enum, metaclass=StrEnumMeta):
     LOCAL = "local"
     BOOTSCRIPT = "bootscript"
     RESCUE = "rescue"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ImageState(str, Enum):
+class ImageState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     CREATING = "creating"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class IpState(str, Enum):
+class IpState(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATE = "unknown_state"
     DETACHED = "detached"
     ATTACHED = "attached"
     PENDING = "pending"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class IpType(str, Enum):
+class IpType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_IPTYPE = "unknown_iptype"
     NAT = "nat"
     ROUTED_IPV4 = "routed_ipv4"
     ROUTED_IPV6 = "routed_ipv6"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListServersRequestOrder(str, Enum):
+class ListServersRequestOrder(str, Enum, metaclass=StrEnumMeta):
     CREATION_DATE_DESC = "creation_date_desc"
     CREATION_DATE_ASC = "creation_date_asc"
     MODIFICATION_DATE_DESC = "modification_date_desc"
     MODIFICATION_DATE_ASC = "modification_date_asc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PlacementGroupPolicyMode(str, Enum):
+class PlacementGroupPolicyMode(str, Enum, metaclass=StrEnumMeta):
     OPTIONAL = "optional"
     ENFORCED = "enforced"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PlacementGroupPolicyType(str, Enum):
+class PlacementGroupPolicyType(str, Enum, metaclass=StrEnumMeta):
     MAX_AVAILABILITY = "max_availability"
     LOW_LATENCY = "low_latency"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PrivateNICState(str, Enum):
+class PrivateNICState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SYNCING = "syncing"
     SYNCING_ERROR = "syncing_error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecurityGroupPolicy(str, Enum):
+class SecurityGroupPolicy(str, Enum, metaclass=StrEnumMeta):
     ACCEPT = "accept"
     DROP = "drop"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecurityGroupRuleAction(str, Enum):
+class SecurityGroupRuleAction(str, Enum, metaclass=StrEnumMeta):
     ACCEPT = "accept"
     DROP = "drop"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecurityGroupRuleDirection(str, Enum):
+class SecurityGroupRuleDirection(str, Enum, metaclass=StrEnumMeta):
     INBOUND = "inbound"
     OUTBOUND = "outbound"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecurityGroupRuleProtocol(str, Enum):
+class SecurityGroupRuleProtocol(str, Enum, metaclass=StrEnumMeta):
     TCP = "TCP"
     UDP = "UDP"
     ICMP = "ICMP"
     ANY = "ANY"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecurityGroupState(str, Enum):
+class SecurityGroupState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SYNCING = "syncing"
     SYNCING_ERROR = "syncing_error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerAction(str, Enum):
+class ServerAction(str, Enum, metaclass=StrEnumMeta):
     POWERON = "poweron"
     BACKUP = "backup"
     STOP_IN_PLACE = "stop_in_place"
     POWEROFF = "poweroff"
     TERMINATE = "terminate"
     REBOOT = "reboot"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerIpIpFamily(str, Enum):
+class ServerIpIpFamily(str, Enum, metaclass=StrEnumMeta):
     INET = "inet"
     INET6 = "inet6"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerIpProvisioningMode(str, Enum):
+class ServerIpProvisioningMode(str, Enum, metaclass=StrEnumMeta):
     MANUAL = "manual"
     DHCP = "dhcp"
     SLAAC = "slaac"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerState(str, Enum):
+class ServerState(str, Enum, metaclass=StrEnumMeta):
     RUNNING = "running"
     STOPPED = "stopped"
     STOPPED_IN_PLACE = "stopped in place"
     STARTING = "starting"
     STOPPING = "stopping"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ServerTypesAvailability(str, Enum):
+class ServerTypesAvailability(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SCARCE = "scarce"
     SHORTAGE = "shortage"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SnapshotState(str, Enum):
+class SnapshotState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SNAPSHOTTING = "snapshotting"
     ERROR = "error"
     INVALID_DATA = "invalid_data"
     IMPORTING = "importing"
     EXPORTING = "exporting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SnapshotVolumeType(str, Enum):
+class SnapshotVolumeType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_VOLUME_TYPE = "unknown_volume_type"
     L_SSD = "l_ssd"
     B_SSD = "b_ssd"
     UNIFIED = "unified"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TaskStatus(str, Enum):
+class TaskStatus(str, Enum, metaclass=StrEnumMeta):
     PENDING = "pending"
     STARTED = "started"
     SUCCESS = "success"
     FAILURE = "failure"
     RETRY = "retry"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class VolumeServerState(str, Enum):
+class VolumeServerState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SNAPSHOTTING = "snapshotting"
     ERROR = "error"
     FETCHING = "fetching"
     RESIZING = "resizing"
     SAVING = "saving"
     HOTSYNCING = "hotsyncing"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class VolumeServerVolumeType(str, Enum):
+class VolumeServerVolumeType(str, Enum, metaclass=StrEnumMeta):
     L_SSD = "l_ssd"
     B_SSD = "b_ssd"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class VolumeState(str, Enum):
+class VolumeState(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SNAPSHOTTING = "snapshotting"
     ERROR = "error"
     FETCHING = "fetching"
     RESIZING = "resizing"
     SAVING = "saving"
     HOTSYNCING = "hotsyncing"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class VolumeVolumeType(str, Enum):
+class VolumeVolumeType(str, Enum, metaclass=StrEnumMeta):
     L_SSD = "l_ssd"
     B_SSD = "b_ssd"
     UNIFIED = "unified"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/instance/v1/types_private.py` & `scaleway_async-1.1.0/scaleway_async/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iot/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iot/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/iot/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iot/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/iot/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/iot/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/iot/v1/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,58 +7,61 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from scaleway_core.bridge import (
     Region,
     TimeSeries,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class DeviceMessageFiltersRulePolicy(str, Enum):
+class DeviceMessageFiltersRulePolicy(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ACCEPT = "accept"
     REJECT = "reject"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DeviceStatus(str, Enum):
+class DeviceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ERROR = "error"
     ENABLED = "enabled"
     DISABLED = "disabled"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HubProductPlan(str, Enum):
+class HubProductPlan(str, Enum, metaclass=StrEnumMeta):
     PLAN_UNKNOWN = "plan_unknown"
     PLAN_SHARED = "plan_shared"
     PLAN_DEDICATED = "plan_dedicated"
     PLAN_HA = "plan_ha"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HubStatus(str, Enum):
+class HubStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ERROR = "error"
     ENABLING = "enabling"
     READY = "ready"
     DISABLING = "disabling"
     DISABLED = "disabled"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDevicesRequestOrderBy(str, Enum):
+class ListDevicesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
     HUB_ID_ASC = "hub_id_asc"
     HUB_ID_DESC = "hub_id_desc"
     CREATED_AT_ASC = "created_at_asc"
@@ -68,15 +71,15 @@
     ALLOW_INSECURE_ASC = "allow_insecure_asc"
     ALLOW_INSECURE_DESC = "allow_insecure_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListHubsRequestOrderBy(str, Enum):
+class ListHubsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
     PRODUCT_PLAN_ASC = "product_plan_asc"
     PRODUCT_PLAN_DESC = "product_plan_desc"
     CREATED_AT_ASC = "created_at_asc"
@@ -84,88 +87,88 @@
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNetworksRequestOrderBy(str, Enum):
+class ListNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     TYPE_ASC = "type_asc"
     TYPE_DESC = "type_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListRoutesRequestOrderBy(str, Enum):
+class ListRoutesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     HUB_ID_ASC = "hub_id_asc"
     HUB_ID_DESC = "hub_id_desc"
     TYPE_ASC = "type_asc"
     TYPE_DESC = "type_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NetworkNetworkType(str, Enum):
+class NetworkNetworkType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     SIGFOX = "sigfox"
     REST = "rest"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NullValue(str, Enum):
+class NullValue(str, Enum, metaclass=StrEnumMeta):
     NULL_VALUE = "NULL_VALUE"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RouteDatabaseConfigEngine(str, Enum):
+class RouteDatabaseConfigEngine(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     POSTGRESQL = "postgresql"
     MYSQL = "mysql"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RouteRestConfigHttpVerb(str, Enum):
+class RouteRestConfigHttpVerb(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     GET = "get"
     POST = "post"
     PUT = "put"
     PATCH = "patch"
     DELETE = "delete"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RouteRouteType(str, Enum):
+class RouteRouteType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     S3 = "s3"
     DATABASE = "database"
     REST = "rest"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class RouteS3ConfigS3Strategy(str, Enum):
+class RouteS3ConfigS3Strategy(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     PER_TOPIC = "per_topic"
     PER_MESSAGE = "per_message"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,92 +7,95 @@
 from enum import Enum
 from typing import Dict, List, Optional
 
 from scaleway_core.bridge import (
     Region,
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class AutoscalerEstimator(str, Enum):
+class AutoscalerEstimator(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_ESTIMATOR = "unknown_estimator"
     BINPACKING = "binpacking"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class AutoscalerExpander(str, Enum):
+class AutoscalerExpander(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_EXPANDER = "unknown_expander"
     RANDOM = "random"
     MOST_PODS = "most_pods"
     LEAST_WASTE = "least_waste"
     PRIORITY = "priority"
     PRICE = "price"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class CNI(str, Enum):
+class CNI(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_CNI = "unknown_cni"
     CILIUM = "cilium"
     CALICO = "calico"
     WEAVE = "weave"
     FLANNEL = "flannel"
     KILO = "kilo"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ClusterStatus(str, Enum):
+class ClusterStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATING = "creating"
     READY = "ready"
     DELETING = "deleting"
     DELETED = "deleted"
     UPDATING = "updating"
     LOCKED = "locked"
     POOL_REQUIRED = "pool_required"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ClusterTypeAvailability(str, Enum):
+class ClusterTypeAvailability(str, Enum, metaclass=StrEnumMeta):
     AVAILABLE = "available"
     SCARCE = "scarce"
     SHORTAGE = "shortage"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ClusterTypeResiliency(str, Enum):
+class ClusterTypeResiliency(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RESILIENCY = "unknown_resiliency"
     STANDARD = "standard"
     HIGH_AVAILABILITY = "high_availability"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class Ingress(str, Enum):
+class Ingress(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_INGRESS = "unknown_ingress"
     NONE = "none"
     NGINX = "nginx"
     TRAEFIK = "traefik"
     TRAEFIK2 = "traefik2"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListClustersRequestOrderBy(str, Enum):
+class ListClustersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     STATUS_ASC = "status_asc"
@@ -100,23 +103,23 @@
     VERSION_ASC = "version_asc"
     VERSION_DESC = "version_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNodesRequestOrderBy(str, Enum):
+class ListNodesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPoolsRequestOrderBy(str, Enum):
+class ListPoolsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     STATUS_ASC = "status_asc"
@@ -124,29 +127,29 @@
     VERSION_ASC = "version_asc"
     VERSION_DESC = "version_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class MaintenanceWindowDayOfTheWeek(str, Enum):
+class MaintenanceWindowDayOfTheWeek(str, Enum, metaclass=StrEnumMeta):
     ANY = "any"
     MONDAY = "monday"
     TUESDAY = "tuesday"
     WEDNESDAY = "wednesday"
     THURSDAY = "thursday"
     FRIDAY = "friday"
     SATURDAY = "saturday"
     SUNDAY = "sunday"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NodeStatus(str, Enum):
+class NodeStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATING = "creating"
     NOT_READY = "not_ready"
     READY = "ready"
     DELETING = "deleting"
     DELETED = "deleted"
     LOCKED = "locked"
@@ -156,38 +159,38 @@
     STARTING = "starting"
     REGISTERING = "registering"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PoolStatus(str, Enum):
+class PoolStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     DELETED = "deleted"
     SCALING = "scaling"
     WARNING = "warning"
     LOCKED = "locked"
     UPGRADING = "upgrading"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PoolVolumeType(str, Enum):
+class PoolVolumeType(str, Enum, metaclass=StrEnumMeta):
     DEFAULT_VOLUME_TYPE = "default_volume_type"
     L_SSD = "l_ssd"
     B_SSD = "b_ssd"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class Runtime(str, Enum):
+class Runtime(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RUNTIME = "unknown_runtime"
     DOCKER = "docker"
     CONTAINERD = "containerd"
     CRIO = "crio"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/k8s/v1/types_private.py` & `scaleway_async-1.1.0/scaleway_async/k8s/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/lb/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/lb/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/lb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/lb/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/lb/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/lb/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/lb/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/lb/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,105 +7,108 @@
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class AclActionRedirectRedirectType(str, Enum):
+class AclActionRedirectRedirectType(str, Enum, metaclass=StrEnumMeta):
     LOCATION = "location"
     SCHEME = "scheme"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class AclActionType(str, Enum):
+class AclActionType(str, Enum, metaclass=StrEnumMeta):
     ALLOW = "allow"
     DENY = "deny"
     REDIRECT = "redirect"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class AclHttpFilter(str, Enum):
+class AclHttpFilter(str, Enum, metaclass=StrEnumMeta):
     ACL_HTTP_FILTER_NONE = "acl_http_filter_none"
     PATH_BEGIN = "path_begin"
     PATH_END = "path_end"
     REGEX = "regex"
     HTTP_HEADER_MATCH = "http_header_match"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class BackendServerStatsHealthCheckStatus(str, Enum):
+class BackendServerStatsHealthCheckStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     NEUTRAL = "neutral"
     FAILED = "failed"
     PASSED = "passed"
     CONDPASS = "condpass"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class BackendServerStatsServerState(str, Enum):
+class BackendServerStatsServerState(str, Enum, metaclass=StrEnumMeta):
     STOPPED = "stopped"
     STARTING = "starting"
     RUNNING = "running"
     STOPPING = "stopping"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class CertificateStatus(str, Enum):
+class CertificateStatus(str, Enum, metaclass=StrEnumMeta):
     PENDING = "pending"
     READY = "ready"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class CertificateType(str, Enum):
+class CertificateType(str, Enum, metaclass=StrEnumMeta):
     LETSENCRYT = "letsencryt"
     CUSTOM = "custom"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ForwardPortAlgorithm(str, Enum):
+class ForwardPortAlgorithm(str, Enum, metaclass=StrEnumMeta):
     ROUNDROBIN = "roundrobin"
     LEASTCONN = "leastconn"
     FIRST = "first"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class InstanceStatus(str, Enum):
+class InstanceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     PENDING = "pending"
     STOPPED = "stopped"
     ERROR = "error"
     LOCKED = "locked"
     MIGRATING = "migrating"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LbStatus(str, Enum):
+class LbStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     PENDING = "pending"
     STOPPED = "stopped"
     ERROR = "error"
     LOCKED = "locked"
     MIGRATING = "migrating"
@@ -114,127 +117,127 @@
     TO_DELETE = "to_delete"
     DELETING = "deleting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LbTypeStock(str, Enum):
+class LbTypeStock(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     LOW_STOCK = "low_stock"
     OUT_OF_STOCK = "out_of_stock"
     AVAILABLE = "available"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListAclRequestOrderBy(str, Enum):
+class ListAclRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListBackendsRequestOrderBy(str, Enum):
+class ListBackendsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListCertificatesRequestOrderBy(str, Enum):
+class ListCertificatesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListFrontendsRequestOrderBy(str, Enum):
+class ListFrontendsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListLbsRequestOrderBy(str, Enum):
+class ListLbsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPrivateNetworksRequestOrderBy(str, Enum):
+class ListPrivateNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListRoutesRequestOrderBy(str, Enum):
+class ListRoutesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListSubscriberRequestOrderBy(str, Enum):
+class ListSubscriberRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class OnMarkedDownAction(str, Enum):
+class OnMarkedDownAction(str, Enum, metaclass=StrEnumMeta):
     ON_MARKED_DOWN_ACTION_NONE = "on_marked_down_action_none"
     SHUTDOWN_SESSIONS = "shutdown_sessions"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PrivateNetworkStatus(str, Enum):
+class PrivateNetworkStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     PENDING = "pending"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class Protocol(str, Enum):
+class Protocol(str, Enum, metaclass=StrEnumMeta):
     TCP = "tcp"
     HTTP = "http"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ProxyProtocol(str, Enum):
+class ProxyProtocol(str, Enum, metaclass=StrEnumMeta):
     """
     PROXY protocol to use between the Load Balancer and backend servers. Allows the backend servers to be informed of the client's real IP address. PROXY protocol must be supported by the backend servers' software. For more information on the different protocols available, see the [dedicated documentation](https://www.scaleway.com/en/docs/network/load-balancer/reference-content/configuring-load-balancer/#choosing-a-proxy-protocol).
     Proxy protocol.
     """
 
     PROXY_PROTOCOL_UNKNOWN = "proxy_protocol_unknown"
     PROXY_PROTOCOL_NONE = "proxy_protocol_none"
@@ -243,25 +246,25 @@
     PROXY_PROTOCOL_V2_SSL = "proxy_protocol_v2_ssl"
     PROXY_PROTOCOL_V2_SSL_CN = "proxy_protocol_v2_ssl_cn"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SSLCompatibilityLevel(str, Enum):
+class SSLCompatibilityLevel(str, Enum, metaclass=StrEnumMeta):
     SSL_COMPATIBILITY_LEVEL_UNKNOWN = "ssl_compatibility_level_unknown"
     SSL_COMPATIBILITY_LEVEL_INTERMEDIATE = "ssl_compatibility_level_intermediate"
     SSL_COMPATIBILITY_LEVEL_MODERN = "ssl_compatibility_level_modern"
     SSL_COMPATIBILITY_LEVEL_OLD = "ssl_compatibility_level_old"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class StickySessionsType(str, Enum):
+class StickySessionsType(str, Enum, metaclass=StrEnumMeta):
     NONE = "none"
     COOKIE = "cookie"
     TABLE = "table"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v2/__init__.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v2/api.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v2/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/marketplace/v2/types.py` & `scaleway_async-1.1.0/scaleway_async/marketplace/v2/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,48 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListImagesRequestOrderBy(str, Enum):
+class ListImagesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListLocalImagesRequestOrderBy(str, Enum):
+class ListLocalImagesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListVersionsRequestOrderBy(str, Enum):
+class ListVersionsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class LocalImageType(str, Enum):
+class LocalImageType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_TYPE = "unknown_type"
     INSTANCE_LOCAL = "instance_local"
     INSTANCE_SBS = "instance_sbs"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/mnq/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/mnq/v1alpha1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListCredentialsRequestOrderBy(str, Enum):
+class ListCredentialsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     ID_ASC = "id_asc"
     ID_DESC = "id_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNamespacesRequestOrderBy(str, Enum):
+class ListNamespacesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     ID_ASC = "id_asc"
     ID_DESC = "id_desc"
     NAME_ASC = "name_asc"
@@ -34,15 +37,15 @@
     PROJECT_ID_ASC = "project_id_asc"
     PROJECT_ID_DESC = "project_id_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NamespaceProtocol(str, Enum):
+class NamespaceProtocol(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     NATS = "nats"
     SQS_SNS = "sqs_sns"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/rdb/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/rdb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/rdb/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/rdb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/rdb/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/rdb/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/rdb/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/rdb/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/rdb/v1/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,76 +8,79 @@
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
     TimeSeries,
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ACLRuleAction(str, Enum):
+class ACLRuleAction(str, Enum, metaclass=StrEnumMeta):
     ALLOW = "allow"
     DENY = "deny"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ACLRuleDirection(str, Enum):
+class ACLRuleDirection(str, Enum, metaclass=StrEnumMeta):
     INBOUND = "inbound"
     OUTBOUND = "outbound"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ACLRuleProtocol(str, Enum):
+class ACLRuleProtocol(str, Enum, metaclass=StrEnumMeta):
     TCP = "tcp"
     UDP = "udp"
     ICMP = "icmp"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DatabaseBackupStatus(str, Enum):
+class DatabaseBackupStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATING = "creating"
     READY = "ready"
     RESTORING = "restoring"
     DELETING = "deleting"
     ERROR = "error"
     EXPORTING = "exporting"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class EngineSettingPropertyType(str, Enum):
+class EngineSettingPropertyType(str, Enum, metaclass=StrEnumMeta):
     BOOLEAN = "BOOLEAN"
     INT = "INT"
     STRING = "STRING"
     FLOAT = "FLOAT"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class InstanceLogStatus(str, Enum):
+class InstanceLogStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     CREATING = "creating"
     ERROR = "error"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class InstanceStatus(str, Enum):
+class InstanceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     PROVISIONING = "provisioning"
     CONFIGURING = "configuring"
     DELETING = "deleting"
     ERROR = "error"
     AUTOHEALING = "autohealing"
@@ -88,130 +91,130 @@
     SNAPSHOTTING = "snapshotting"
     RESTARTING = "restarting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDatabaseBackupsRequestOrderBy(str, Enum):
+class ListDatabaseBackupsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDatabasesRequestOrderBy(str, Enum):
+class ListDatabasesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     SIZE_ASC = "size_asc"
     SIZE_DESC = "size_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListInstanceLogsRequestOrderBy(str, Enum):
+class ListInstanceLogsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListInstancesRequestOrderBy(str, Enum):
+class ListInstancesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     REGION = "region"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPrivilegesRequestOrderBy(str, Enum):
+class ListPrivilegesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     USER_NAME_ASC = "user_name_asc"
     USER_NAME_DESC = "user_name_desc"
     DATABASE_NAME_ASC = "database_name_asc"
     DATABASE_NAME_DESC = "database_name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListSnapshotsRequestOrderBy(str, Enum):
+class ListSnapshotsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     EXPIRES_AT_ASC = "expires_at_asc"
     EXPIRES_AT_DESC = "expires_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListUsersRequestOrderBy(str, Enum):
+class ListUsersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     IS_ADMIN_ASC = "is_admin_asc"
     IS_ADMIN_DESC = "is_admin_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class MaintenanceStatus(str, Enum):
+class MaintenanceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     PENDING = "pending"
     DONE = "done"
     CANCELED = "canceled"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NodeTypeGeneration(str, Enum):
+class NodeTypeGeneration(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_GENERATION = "unknown_generation"
     GENERATION_V1 = "generation_v1"
     GENERATION_V2 = "generation_v2"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NodeTypeStock(str, Enum):
+class NodeTypeStock(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     LOW_STOCK = "low_stock"
     OUT_OF_STOCK = "out_of_stock"
     AVAILABLE = "available"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class Permission(str, Enum):
+class Permission(str, Enum, metaclass=StrEnumMeta):
     READONLY = "readonly"
     READWRITE = "readwrite"
     ALL = "all"
     CUSTOM = "custom"
     NONE = "none"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ReadReplicaStatus(str, Enum):
+class ReadReplicaStatus(str, Enum, metaclass=StrEnumMeta):
     """
     Read replica. status.
     """
 
     UNKNOWN = "unknown"
     PROVISIONING = "provisioning"
     INITIALIZING = "initializing"
@@ -222,28 +225,28 @@
     CONFIGURING = "configuring"
     PROMOTING = "promoting"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SnapshotStatus(str, Enum):
+class SnapshotStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATING = "creating"
     READY = "ready"
     RESTORING = "restoring"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class VolumeType(str, Enum):
+class VolumeType(str, Enum, metaclass=StrEnumMeta):
     LSSD = "lssd"
     BSSD = "bssd"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/redis/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/redis/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/redis/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/redis/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/redis/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/redis/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/redis/v1/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     TimeSeries,
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class AvailableClusterSettingPropertyType(str, Enum):
+class AvailableClusterSettingPropertyType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "UNKNOWN"
     BOOLEAN = "BOOLEAN"
     INT = "INT"
     STRING = "STRING"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ClusterStatus(str, Enum):
+class ClusterStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     PROVISIONING = "provisioning"
     CONFIGURING = "configuring"
     DELETING = "deleting"
     ERROR = "error"
     AUTOHEALING = "autohealing"
@@ -35,35 +38,35 @@
     SUSPENDED = "suspended"
     INITIALIZING = "initializing"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListClustersRequestOrderBy(str, Enum):
+class ListClustersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NodeTypeStock(str, Enum):
+class NodeTypeStock(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     LOW_STOCK = "low_stock"
     OUT_OF_STOCK = "out_of_stock"
     AVAILABLE = "available"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PrivateNetworkProvisioningMode(str, Enum):
+class PrivateNetworkProvisioningMode(str, Enum, metaclass=StrEnumMeta):
     STATIC = "static"
     IPAM = "ipam"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/registry/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/registry/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/registry/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/registry/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/registry/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/registry/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/registry/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/registry/v1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,81 +6,84 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ImageStatus(str, Enum):
+class ImageStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ImageVisibility(str, Enum):
+class ImageVisibility(str, Enum, metaclass=StrEnumMeta):
     VISIBILITY_UNKNOWN = "visibility_unknown"
     INHERIT = "inherit"
     PUBLIC = "public"
     PRIVATE = "private"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListImagesRequestOrderBy(str, Enum):
+class ListImagesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListNamespacesRequestOrderBy(str, Enum):
+class ListNamespacesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     DESCRIPTION_ASC = "description_asc"
     DESCRIPTION_DESC = "description_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListTagsRequestOrderBy(str, Enum):
+class ListTagsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NamespaceStatus(str, Enum):
+class NamespaceStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class TagStatus(str, Enum):
+class TagStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
 
     def __str__(self) -> str:
```

### Comparing `scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/secret/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/secret/v1alpha1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,53 +6,56 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListSecretsRequestOrderBy(str, Enum):
+class ListSecretsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class Product(str, Enum):
+class Product(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecretStatus(str, Enum):
+class SecretStatus(str, Enum, metaclass=StrEnumMeta):
     READY = "ready"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecretType(str, Enum):
+class SecretType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_SECRET_TYPE = "unknown_secret_type"
     OPAQUE = "opaque"
     CERTIFICATE = "certificate"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class SecretVersionStatus(str, Enum):
+class SecretVersionStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     ENABLED = "enabled"
     DISABLED = "disabled"
     DESTROYED = "destroyed"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/content.py` & `scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/tem/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/tem/v1alpha1/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,73 +6,76 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class DomainLastStatusRecordStatus(str, Enum):
+class DomainLastStatusRecordStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RECORD_STATUS = "unknown_record_status"
     VALID = "valid"
     INVALID = "invalid"
     NOT_FOUND = "not_found"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DomainStatus(str, Enum):
+class DomainStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CHECKED = "checked"
     UNCHECKED = "unchecked"
     INVALID = "invalid"
     LOCKED = "locked"
     REVOKED = "revoked"
     PENDING = "pending"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class EmailFlag(str, Enum):
+class EmailFlag(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_FLAG = "unknown_flag"
     SOFT_BOUNCE = "soft_bounce"
     HARD_BOUNCE = "hard_bounce"
     SPAM = "spam"
     MAILBOX_FULL = "mailbox_full"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class EmailRcptType(str, Enum):
+class EmailRcptType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_RCPT_TYPE = "unknown_rcpt_type"
     TO = "to"
     CC = "cc"
     BCC = "bcc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class EmailStatus(str, Enum):
+class EmailStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     NEW = "new"
     SENDING = "sending"
     SENT = "sent"
     FAILED = "failed"
     CANCELED = "canceled"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListEmailsRequestOrderBy(str, Enum):
+class ListEmailsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_DESC = "created_at_desc"
     CREATED_AT_ASC = "created_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     STATUS_DESC = "status_desc"
     STATUS_ASC = "status_asc"
     MAIL_FROM_DESC = "mail_from_desc"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/test/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/test/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/test/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/test/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/test/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/test/v1/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,40 +3,44 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
-class EyeColors(str, Enum):
+
+class EyeColors(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     AMBER = "amber"
     BLUE = "blue"
     BROWN = "brown"
     GRAY = "gray"
     GREEN = "green"
     HAZEL = "hazel"
     RED = "red"
     VIOLET = "violet"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HumanStatus(str, Enum):
+class HumanStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     STOPPED = "stopped"
     RUNNING = "running"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListHumansRequestOrderBy(str, Enum):
+class ListHumansRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     HEIGHT_ASC = "height_asc"
     HEIGHT_DESC = "height_desc"
```

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v1/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListPrivateNetworksRequestOrderBy(str, Enum):
+class ListPrivateNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v2/__init__.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v2/api.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v2/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpc/v2/types.py` & `scaleway_async-1.1.0/scaleway_async/vpc/v2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class ListPrivateNetworksRequestOrderBy(str, Enum):
+class ListPrivateNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListVPCsRequestOrderBy(str, Enum):
+class ListVPCsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/vpcgw/v1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpcgw/v1/api.py` & `scaleway_async-1.1.0/scaleway_async/vpcgw/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpcgw/v1/content.py` & `scaleway_async-1.1.0/scaleway_async/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpcgw/v1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/vpcgw/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/vpcgw/v1/types.py` & `scaleway_async-1.1.0/scaleway_async/vpcgw/v1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,42 @@
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Zone,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class DHCPEntryType(str, Enum):
+class DHCPEntryType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     RESERVATION = "reservation"
     LEASE = "lease"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class GatewayNetworkStatus(str, Enum):
+class GatewayNetworkStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     CREATED = "created"
     ATTACHING = "attaching"
     CONFIGURING = "configuring"
     READY = "ready"
     DETACHING = "detaching"
     DELETED = "deleted"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class GatewayStatus(str, Enum):
+class GatewayStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     STOPPED = "stopped"
     ALLOCATING = "allocating"
     CONFIGURING = "configuring"
     RUNNING = "running"
     STOPPING = "stopping"
     FAILED = "failed"
@@ -46,83 +49,83 @@
     DELETED = "deleted"
     LOCKED = "locked"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDHCPEntriesRequestOrderBy(str, Enum):
+class ListDHCPEntriesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     IP_ADDRESS_ASC = "ip_address_asc"
     IP_ADDRESS_DESC = "ip_address_desc"
     HOSTNAME_ASC = "hostname_asc"
     HOSTNAME_DESC = "hostname_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListDHCPsRequestOrderBy(str, Enum):
+class ListDHCPsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     SUBNET_ASC = "subnet_asc"
     SUBNET_DESC = "subnet_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListGatewayNetworksRequestOrderBy(str, Enum):
+class ListGatewayNetworksRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListGatewaysRequestOrderBy(str, Enum):
+class ListGatewaysRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     TYPE_ASC = "type_asc"
     TYPE_DESC = "type_desc"
     STATUS_ASC = "status_asc"
     STATUS_DESC = "status_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListIPsRequestOrderBy(str, Enum):
+class ListIPsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     IP_ASC = "ip_asc"
     IP_DESC = "ip_desc"
     REVERSE_ASC = "reverse_asc"
     REVERSE_DESC = "reverse_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListPATRulesRequestOrderBy(str, Enum):
+class ListPATRulesRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     PUBLIC_PORT_ASC = "public_port_asc"
     PUBLIC_PORT_DESC = "public_port_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class PATRuleProtocol(str, Enum):
+class PATRuleProtocol(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     BOTH = "both"
     TCP = "tcp"
     UDP = "udp"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/__init__.py` & `scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/api.py` & `scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/marshalling.py` & `scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-1.0.1/scaleway_async/webhosting/v1alpha1/types.py` & `scaleway_async-1.1.0/scaleway_async/webhosting/v1alpha1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,94 +7,97 @@
 from enum import Enum
 from typing import List, Optional
 
 from scaleway_core.bridge import (
     Money,
     Region,
 )
+from scaleway_core.utils import (
+    StrEnumMeta,
+)
 
 
-class DnsRecordStatus(str, Enum):
+class DnsRecordStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     VALID = "valid"
     INVALID = "invalid"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DnsRecordType(str, Enum):
+class DnsRecordType(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_TYPE = "unknown_type"
     A = "a"
     CNAME = "cname"
     MX = "mx"
     TXT = "txt"
     NS = "ns"
     AAAA = "aaaa"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class DnsRecordsStatus(str, Enum):
+class DnsRecordsStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN = "unknown"
     VALID = "valid"
     INVALID = "invalid"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HostingDnsStatus(str, Enum):
+class HostingDnsStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_DNS_STATUS = "unknown_dns_status"
     VALID = "valid"
     INVALID = "invalid"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class HostingStatus(str, Enum):
+class HostingStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     DELIVERING = "delivering"
     READY = "ready"
     DELETING = "deleting"
     ERROR = "error"
     LOCKED = "locked"
     MIGRATING = "migrating"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListHostingsRequestOrderBy(str, Enum):
+class ListHostingsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class ListOffersRequestOrderBy(str, Enum):
+class ListOffersRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     PRICE_ASC = "price_asc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class NameserverStatus(str, Enum):
+class NameserverStatus(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_STATUS = "unknown_status"
     VALID = "valid"
     INVALID = "invalid"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
-class OfferQuotaWarning(str, Enum):
+class OfferQuotaWarning(str, Enum, metaclass=StrEnumMeta):
     UNKNOWN_QUOTA_WARNING = "unknown_quota_warning"
     EMAIL_COUNT_EXCEEDED = "email_count_exceeded"
     DATABASE_COUNT_EXCEEDED = "database_count_exceeded"
     DISK_USAGE_EXCEEDED = "disk_usage_exceeded"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `scaleway_async-1.0.1/PKG-INFO` & `scaleway_async-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-async
-Version: 1.0.1
+Version: 1.1.0
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

