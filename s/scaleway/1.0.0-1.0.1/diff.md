# Comparing `tmp/scaleway-1.0.0.tar.gz` & `tmp/scaleway-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway-1.0.0.tar", max compression
+gzip compressed data, was "scaleway-1.0.1.tar", max compression
```

## Comparing `scaleway-1.0.0.tar` & `scaleway-1.0.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-r--r--   0        0        0       76 2023-08-07 09:31:24.813265 scaleway-1.0.0/README.md
--rw-r--r--   0        0        0     1117 2023-08-07 09:31:44.829183 scaleway-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      905 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/__init__.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/__init__.py
--rw-r--r--   0        0        0      382 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v2/__init__.py
--rw-r--r--   0        0        0     8582 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v2/api.py
--rw-r--r--   0        0        0     2500 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v2/marshalling.py
--rw-r--r--   0        0        0     2636 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v2/types.py
--rw-r--r--   0        0        0      396 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v3/__init__.py
--rw-r--r--   0        0        0     8252 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v3/api.py
--rw-r--r--   0        0        0     2560 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v3/marshalling.py
--rw-r--r--   0        0        0     2676 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/account/v3/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/__init__.py
--rw-r--r--   0        0        0      968 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    17978 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      497 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     6527 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7305 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/__init__.py
--rw-r--r--   0        0        0     3212 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    52870 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/v1/api.py
--rw-r--r--   0        0        0     1066 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/v1/content.py
--rw-r--r--   0        0        0    26856 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    28859 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/billing/__init__.py
--rw-r--r--   0        0        0      698 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/billing/v2alpha1/__init__.py
--rw-r--r--   0        0        0     4370 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/billing/v2alpha1/api.py
--rw-r--r--   0        0        0     3385 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/billing/v2alpha1/marshalling.py
--rw-r--r--   0        0        0     4206 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/billing/v2alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/__init__.py
--rw-r--r--   0        0        0     1468 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    26429 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      419 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    15740 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0    10634 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/__init__.py
--rw-r--r--   0        0        0     3386 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    64998 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/v1beta1/api.py
--rw-r--r--   0        0        0     1587 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/v1beta1/content.py
--rw-r--r--   0        0        0    26245 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    28456 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/__init__.py
--rw-r--r--   0        0        0     8426 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    86540 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1955 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/v2beta1/content.py
--rw-r--r--   0        0        0    88058 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    40494 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/__init__.py
--rw-r--r--   0        0        0      978 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20597 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      651 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     7038 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     9176 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/__init__.py
--rw-r--r--   0        0        0     3642 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    64078 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/v1beta1/api.py
--rw-r--r--   0        0        0     1579 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/v1beta1/content.py
--rw-r--r--   0        0        0    28021 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    30155 2023-08-07 09:31:24.817265 scaleway-1.0.0/scaleway/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iam/__init__.py
--rw-r--r--   0        0        0     2300 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    74207 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    26114 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    30264 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/__init__.py
--rw-r--r--   0        0        0     8194 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/__init__.py
--rw-r--r--   0        0        0   130160 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/api.py
--rw-r--r--   0        0        0     2660 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/api_utils.py
--rw-r--r--   0        0        0     2210 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/content.py
--rw-r--r--   0        0        0    97574 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/marshalling.py
--rw-r--r--   0        0        0      712 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/marshalling_utils.py
--rw-r--r--   0        0        0    57214 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/types.py
--rw-r--r--   0        0        0    11049 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/__init__.py
--rw-r--r--   0        0        0     3456 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/v1/__init__.py
--rw-r--r--   0        0        0    61702 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/v1/api.py
--rw-r--r--   0        0        0      364 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/v1/content.py
--rw-r--r--   0        0        0    31989 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/v1/marshalling.py
--rw-r--r--   0        0        0    33256 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/iot/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/__init__.py
--rw-r--r--   0        0        0     3430 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/__init__.py
--rw-r--r--   0        0        0    57678 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/api.py
--rw-r--r--   0        0        0      937 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/content.py
--rw-r--r--   0        0        0    34447 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    45370 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/types.py
--rw-r--r--   0        0        0      540 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/k8s/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/__init__.py
--rw-r--r--   0        0        0     5060 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/v1/__init__.py
--rw-r--r--   0        0        0   224407 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/v1/api.py
--rw-r--r--   0        0        0     1111 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/v1/content.py
--rw-r--r--   0        0        0    83655 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/v1/marshalling.py
--rw-r--r--   0        0        0   102503 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/lb/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/__init__.py
--rw-r--r--   0        0        0      636 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v1/__init__.py
--rw-r--r--   0        0        0     4094 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v1/api.py
--rw-r--r--   0        0        0     5360 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v1/marshalling.py
--rw-r--r--   0        0        0     3161 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v1/types.py
--rw-r--r--   0        0        0      948 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    14707 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v2/api.py
--rw-r--r--   0        0        0     5380 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     5365 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/mnq/__init__.py
--rw-r--r--   0        0        0     1008 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/mnq/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18375 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/mnq/v1alpha1/api.py
--rw-r--r--   0        0        0     8332 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/mnq/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     9028 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/mnq/v1alpha1/types.py
--rw-r--r--   0        0        0        0 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/py.typed
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/rdb/__init__.py
--rw-r--r--   0        0        0     5874 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/rdb/v1/__init__.py
--rw-r--r--   0        0        0   116807 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/rdb/v1/api.py
--rw-r--r--   0        0        0     1956 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/rdb/v1/content.py
--rw-r--r--   0        0        0    50774 2023-08-07 09:31:24.821265 scaleway-1.0.0/scaleway/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    53443 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/__init__.py
--rw-r--r--   0        0        0     2130 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/v1/__init__.py
--rw-r--r--   0        0        0    44073 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/v1/api.py
--rw-r--r--   0        0        0      489 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/v1/content.py
--rw-r--r--   0        0        0    20527 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/v1/marshalling.py
--rw-r--r--   0        0        0    19830 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/redis/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/__init__.py
--rw-r--r--   0        0        0     1190 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/v1/__init__.py
--rw-r--r--   0        0        0    28659 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/v1/api.py
--rw-r--r--   0        0        0      713 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/v1/content.py
--rw-r--r--   0        0        0     7013 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/v1/marshalling.py
--rw-r--r--   0        0        0    11691 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/registry/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/secret/__init__.py
--rw-r--r--   0        0        0      946 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    42442 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/secret/v1alpha1/api.py
--rw-r--r--   0        0        0     9169 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    16883 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/secret/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/__init__.py
--rw-r--r--   0        0        0     1522 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    24693 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      551 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/v1alpha1/content.py
--rw-r--r--   0        0        0    11457 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    14380 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/__init__.py
--rw-r--r--   0        0        0      598 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/v1/__init__.py
--rw-r--r--   0        0        0    11907 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/v1/api.py
--rw-r--r--   0        0        0      350 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/v1/content.py
--rw-r--r--   0        0        0     5840 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/v1/marshalling.py
--rw-r--r--   0        0        0     3303 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/test/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/__init__.py
--rw-r--r--   0        0        0      416 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v1/__init__.py
--rw-r--r--   0        0        0    11743 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v1/api.py
--rw-r--r--   0        0        0     2898 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     4346 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v1/types.py
--rw-r--r--   0        0        0      820 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v2/__init__.py
--rw-r--r--   0        0        0    29295 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v2/api.py
--rw-r--r--   0        0        0     9247 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v2/marshalling.py
--rw-r--r--   0        0        0    10566 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpc/v2/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/__init__.py
--rw-r--r--   0        0        0     2168 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    78648 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/v1/api.py
--rw-r--r--   0        0        0      757 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/v1/content.py
--rw-r--r--   0        0        0    25219 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    35284 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/vpcgw/v1/types.py
--rw-r--r--   0        0        0      127 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/__init__.py
--rw-r--r--   0        0        0     1378 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/v1alpha1/__init__.py
--rw-r--r--   0        0        0    16992 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/v1alpha1/api.py
--rw-r--r--   0        0        0      422 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/v1alpha1/content.py
--rw-r--r--   0        0        0     8924 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    10942 2023-08-07 09:31:24.825265 scaleway-1.0.0/scaleway/webhosting/v1alpha1/types.py
--rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 scaleway-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-08-07 09:35:26.684022 scaleway-1.0.1/README.md
+-rw-r--r--   0        0        0     1117 2023-08-07 09:35:46.192148 scaleway-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      905 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/__init__.py
+-rw-r--r--   0        0        0      382 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v2/__init__.py
+-rw-r--r--   0        0        0     8582 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v2/api.py
+-rw-r--r--   0        0        0     2500 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2636 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v2/types.py
+-rw-r--r--   0        0        0      396 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v3/__init__.py
+-rw-r--r--   0        0        0     8252 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v3/api.py
+-rw-r--r--   0        0        0     2560 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v3/marshalling.py
+-rw-r--r--   0        0        0     2676 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/account/v3/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/__init__.py
+-rw-r--r--   0        0        0      968 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    17978 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      497 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0     6527 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7305 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/__init__.py
+-rw-r--r--   0        0        0     3212 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    52870 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1066 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/v1/content.py
+-rw-r--r--   0        0        0    26856 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    28859 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/billing/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/billing/v2alpha1/__init__.py
+-rw-r--r--   0        0        0     4370 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/billing/v2alpha1/api.py
+-rw-r--r--   0        0        0     3385 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/billing/v2alpha1/marshalling.py
+-rw-r--r--   0        0        0     4206 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/billing/v2alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/__init__.py
+-rw-r--r--   0        0        0     1468 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    26429 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      419 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    15740 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    10634 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/__init__.py
+-rw-r--r--   0        0        0     3386 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    64998 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1587 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/v1beta1/content.py
+-rw-r--r--   0        0        0    26245 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    28456 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/__init__.py
+-rw-r--r--   0        0        0     8426 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    86540 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1955 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    88058 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    40494 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/__init__.py
+-rw-r--r--   0        0        0      978 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20597 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      651 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     7038 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9176 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/__init__.py
+-rw-r--r--   0        0        0     3642 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    64078 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1579 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/v1beta1/content.py
+-rw-r--r--   0        0        0    28021 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    30155 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.688022 scaleway-1.0.1/scaleway/iam/__init__.py
+-rw-r--r--   0        0        0     2300 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    74207 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    26114 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    30264 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/__init__.py
+-rw-r--r--   0        0        0     8194 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/__init__.py
+-rw-r--r--   0        0        0   130160 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/api.py
+-rw-r--r--   0        0        0     2660 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/api_utils.py
+-rw-r--r--   0        0        0     2210 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/content.py
+-rw-r--r--   0        0        0    97574 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/marshalling.py
+-rw-r--r--   0        0        0      712 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/marshalling_utils.py
+-rw-r--r--   0        0        0    57214 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/types.py
+-rw-r--r--   0        0        0    11049 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/__init__.py
+-rw-r--r--   0        0        0     3456 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/v1/__init__.py
+-rw-r--r--   0        0        0    61702 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/v1/api.py
+-rw-r--r--   0        0        0      364 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/v1/content.py
+-rw-r--r--   0        0        0    31989 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    33256 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/__init__.py
+-rw-r--r--   0        0        0     3430 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    57678 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/api.py
+-rw-r--r--   0        0        0      937 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/content.py
+-rw-r--r--   0        0        0    34447 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    45370 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/types.py
+-rw-r--r--   0        0        0      540 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/k8s/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/__init__.py
+-rw-r--r--   0        0        0     5060 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/v1/__init__.py
+-rw-r--r--   0        0        0   224407 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/v1/api.py
+-rw-r--r--   0        0        0     1111 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/v1/content.py
+-rw-r--r--   0        0        0    83655 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/v1/marshalling.py
+-rw-r--r--   0        0        0   102503 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/__init__.py
+-rw-r--r--   0        0        0      636 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v1/__init__.py
+-rw-r--r--   0        0        0     4094 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v1/api.py
+-rw-r--r--   0        0        0     5360 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v1/marshalling.py
+-rw-r--r--   0        0        0     3161 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v1/types.py
+-rw-r--r--   0        0        0      948 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    14707 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v2/api.py
+-rw-r--r--   0        0        0     5380 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     5365 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/mnq/__init__.py
+-rw-r--r--   0        0        0     1008 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/mnq/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18375 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/mnq/v1alpha1/api.py
+-rw-r--r--   0        0        0     8332 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/mnq/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9028 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/mnq/v1alpha1/types.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/py.typed
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/__init__.py
+-rw-r--r--   0        0        0     5874 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   116807 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/v1/api.py
+-rw-r--r--   0        0        0     1956 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/v1/content.py
+-rw-r--r--   0        0        0    50774 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    53443 2023-08-07 09:35:26.692022 scaleway-1.0.1/scaleway/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/__init__.py
+-rw-r--r--   0        0        0     2130 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/v1/__init__.py
+-rw-r--r--   0        0        0    44073 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/v1/api.py
+-rw-r--r--   0        0        0      489 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/v1/content.py
+-rw-r--r--   0        0        0    20527 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    19830 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/__init__.py
+-rw-r--r--   0        0        0     1190 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/v1/__init__.py
+-rw-r--r--   0        0        0    28659 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/v1/api.py
+-rw-r--r--   0        0        0      713 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/v1/content.py
+-rw-r--r--   0        0        0     7013 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    11691 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/secret/__init__.py
+-rw-r--r--   0        0        0      946 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    42442 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0     9169 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    16883 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/__init__.py
+-rw-r--r--   0        0        0     1522 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    24693 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      551 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0    11457 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    14380 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/__init__.py
+-rw-r--r--   0        0        0      598 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/v1/__init__.py
+-rw-r--r--   0        0        0    11907 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/v1/api.py
+-rw-r--r--   0        0        0      350 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/v1/content.py
+-rw-r--r--   0        0        0     5840 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3303 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/test/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/__init__.py
+-rw-r--r--   0        0        0      416 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    11743 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v1/api.py
+-rw-r--r--   0        0        0     2898 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4346 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v1/types.py
+-rw-r--r--   0        0        0      820 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v2/__init__.py
+-rw-r--r--   0        0        0    29295 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v2/api.py
+-rw-r--r--   0        0        0     9247 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v2/marshalling.py
+-rw-r--r--   0        0        0    10566 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpc/v2/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/__init__.py
+-rw-r--r--   0        0        0     2168 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    78648 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      757 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    25219 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    35284 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/__init__.py
+-rw-r--r--   0        0        0     1378 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    16992 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      422 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0     8924 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    10942 2023-08-07 09:35:26.696022 scaleway-1.0.1/scaleway/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 scaleway-1.0.1/PKG-INFO
```

### Comparing `scaleway-1.0.0/pyproject.toml` & `scaleway-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway"
-version = "1.0.0"
+version = "1.0.1"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway-1.0.0/scaleway/__init__.py` & `scaleway-1.0.1/scaleway/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v2/api.py` & `scaleway-1.0.1/scaleway/account/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v2/marshalling.py` & `scaleway-1.0.1/scaleway/account/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v2/types.py` & `scaleway-1.0.1/scaleway/account/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v3/api.py` & `scaleway-1.0.1/scaleway/account/v3/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v3/marshalling.py` & `scaleway-1.0.1/scaleway/account/v3/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/account/v3/types.py` & `scaleway-1.0.1/scaleway/account/v3/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/applesilicon/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/applesilicon/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/applesilicon/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/applesilicon/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/applesilicon/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/applesilicon/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/applesilicon/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/applesilicon/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/baremetal/v1/__init__.py` & `scaleway-1.0.1/scaleway/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/baremetal/v1/api.py` & `scaleway-1.0.1/scaleway/baremetal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/baremetal/v1/content.py` & `scaleway-1.0.1/scaleway/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/baremetal/v1/marshalling.py` & `scaleway-1.0.1/scaleway/baremetal/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/baremetal/v1/types.py` & `scaleway-1.0.1/scaleway/baremetal/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/billing/v2alpha1/__init__.py` & `scaleway-1.0.1/scaleway/billing/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/billing/v2alpha1/api.py` & `scaleway-1.0.1/scaleway/billing/v2alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/billing/v2alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/billing/v2alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/billing/v2alpha1/types.py` & `scaleway-1.0.1/scaleway/billing/v2alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/cockpit/v1beta1/__init__.py` & `scaleway-1.0.1/scaleway/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/cockpit/v1beta1/api.py` & `scaleway-1.0.1/scaleway/cockpit/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/cockpit/v1beta1/marshalling.py` & `scaleway-1.0.1/scaleway/cockpit/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/cockpit/v1beta1/types.py` & `scaleway-1.0.1/scaleway/cockpit/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/container/v1beta1/__init__.py` & `scaleway-1.0.1/scaleway/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/container/v1beta1/api.py` & `scaleway-1.0.1/scaleway/container/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/container/v1beta1/content.py` & `scaleway-1.0.1/scaleway/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/container/v1beta1/marshalling.py` & `scaleway-1.0.1/scaleway/container/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/container/v1beta1/types.py` & `scaleway-1.0.1/scaleway/container/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/domain/v2beta1/__init__.py` & `scaleway-1.0.1/scaleway/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/domain/v2beta1/api.py` & `scaleway-1.0.1/scaleway/domain/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/domain/v2beta1/content.py` & `scaleway-1.0.1/scaleway/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/domain/v2beta1/marshalling.py` & `scaleway-1.0.1/scaleway/domain/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/domain/v2beta1/types.py` & `scaleway-1.0.1/scaleway/domain/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/flexibleip/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/flexibleip/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/flexibleip/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/flexibleip/v1alpha1/content.py` & `scaleway-1.0.1/scaleway/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/flexibleip/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/flexibleip/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/flexibleip/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/flexibleip/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/function/v1beta1/__init__.py` & `scaleway-1.0.1/scaleway/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/function/v1beta1/api.py` & `scaleway-1.0.1/scaleway/function/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/function/v1beta1/content.py` & `scaleway-1.0.1/scaleway/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/function/v1beta1/marshalling.py` & `scaleway-1.0.1/scaleway/function/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/function/v1beta1/types.py` & `scaleway-1.0.1/scaleway/function/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iam/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/iam/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iam/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/iam/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iam/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/iam/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iam/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/iam/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/__init__.py` & `scaleway-1.0.1/scaleway/instance/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/api.py` & `scaleway-1.0.1/scaleway/instance/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/api_utils.py` & `scaleway-1.0.1/scaleway/instance/v1/api_utils.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/content.py` & `scaleway-1.0.1/scaleway/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/marshalling.py` & `scaleway-1.0.1/scaleway/instance/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/marshalling_utils.py` & `scaleway-1.0.1/scaleway/instance/v1/marshalling_utils.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/types.py` & `scaleway-1.0.1/scaleway/instance/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/instance/v1/types_private.py` & `scaleway-1.0.1/scaleway/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iot/v1/__init__.py` & `scaleway-1.0.1/scaleway/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iot/v1/api.py` & `scaleway-1.0.1/scaleway/iot/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iot/v1/marshalling.py` & `scaleway-1.0.1/scaleway/iot/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/iot/v1/types.py` & `scaleway-1.0.1/scaleway/iot/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/__init__.py` & `scaleway-1.0.1/scaleway/k8s/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/api.py` & `scaleway-1.0.1/scaleway/k8s/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/content.py` & `scaleway-1.0.1/scaleway/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/marshalling.py` & `scaleway-1.0.1/scaleway/k8s/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/types.py` & `scaleway-1.0.1/scaleway/k8s/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/k8s/v1/types_private.py` & `scaleway-1.0.1/scaleway/k8s/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/lb/v1/__init__.py` & `scaleway-1.0.1/scaleway/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/lb/v1/api.py` & `scaleway-1.0.1/scaleway/lb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/lb/v1/content.py` & `scaleway-1.0.1/scaleway/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/lb/v1/marshalling.py` & `scaleway-1.0.1/scaleway/lb/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/lb/v1/types.py` & `scaleway-1.0.1/scaleway/lb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v1/__init__.py` & `scaleway-1.0.1/scaleway/marketplace/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v1/api.py` & `scaleway-1.0.1/scaleway/marketplace/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v1/marshalling.py` & `scaleway-1.0.1/scaleway/marketplace/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v1/types.py` & `scaleway-1.0.1/scaleway/marketplace/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v2/__init__.py` & `scaleway-1.0.1/scaleway/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v2/api.py` & `scaleway-1.0.1/scaleway/marketplace/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v2/marshalling.py` & `scaleway-1.0.1/scaleway/marketplace/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/marketplace/v2/types.py` & `scaleway-1.0.1/scaleway/marketplace/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/mnq/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/mnq/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/mnq/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/mnq/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/mnq/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/mnq/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/mnq/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/mnq/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/rdb/v1/__init__.py` & `scaleway-1.0.1/scaleway/rdb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/rdb/v1/api.py` & `scaleway-1.0.1/scaleway/rdb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/rdb/v1/content.py` & `scaleway-1.0.1/scaleway/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/rdb/v1/marshalling.py` & `scaleway-1.0.1/scaleway/rdb/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/rdb/v1/types.py` & `scaleway-1.0.1/scaleway/rdb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/redis/v1/__init__.py` & `scaleway-1.0.1/scaleway/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/redis/v1/api.py` & `scaleway-1.0.1/scaleway/redis/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/redis/v1/marshalling.py` & `scaleway-1.0.1/scaleway/redis/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/redis/v1/types.py` & `scaleway-1.0.1/scaleway/redis/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/registry/v1/__init__.py` & `scaleway-1.0.1/scaleway/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/registry/v1/api.py` & `scaleway-1.0.1/scaleway/registry/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/registry/v1/content.py` & `scaleway-1.0.1/scaleway/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/registry/v1/marshalling.py` & `scaleway-1.0.1/scaleway/registry/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/registry/v1/types.py` & `scaleway-1.0.1/scaleway/registry/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/secret/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/secret/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/secret/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/secret/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/secret/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/secret/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/secret/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/tem/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/tem/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/tem/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/tem/v1alpha1/content.py` & `scaleway-1.0.1/scaleway/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/tem/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/tem/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/tem/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/tem/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/test/v1/__init__.py` & `scaleway-1.0.1/scaleway/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/test/v1/api.py` & `scaleway-1.0.1/scaleway/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/test/v1/marshalling.py` & `scaleway-1.0.1/scaleway/test/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/test/v1/types.py` & `scaleway-1.0.1/scaleway/test/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v1/api.py` & `scaleway-1.0.1/scaleway/vpc/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v1/marshalling.py` & `scaleway-1.0.1/scaleway/vpc/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v1/types.py` & `scaleway-1.0.1/scaleway/vpc/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v2/__init__.py` & `scaleway-1.0.1/scaleway/vpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v2/api.py` & `scaleway-1.0.1/scaleway/vpc/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v2/marshalling.py` & `scaleway-1.0.1/scaleway/vpc/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpc/v2/types.py` & `scaleway-1.0.1/scaleway/vpc/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpcgw/v1/__init__.py` & `scaleway-1.0.1/scaleway/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpcgw/v1/api.py` & `scaleway-1.0.1/scaleway/vpcgw/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpcgw/v1/content.py` & `scaleway-1.0.1/scaleway/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpcgw/v1/marshalling.py` & `scaleway-1.0.1/scaleway/vpcgw/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/vpcgw/v1/types.py` & `scaleway-1.0.1/scaleway/vpcgw/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/webhosting/v1alpha1/__init__.py` & `scaleway-1.0.1/scaleway/webhosting/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/webhosting/v1alpha1/api.py` & `scaleway-1.0.1/scaleway/webhosting/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/webhosting/v1alpha1/marshalling.py` & `scaleway-1.0.1/scaleway/webhosting/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/scaleway/webhosting/v1alpha1/types.py` & `scaleway-1.0.1/scaleway/webhosting/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-1.0.0/PKG-INFO` & `scaleway-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

