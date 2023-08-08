# Comparing `tmp/msticpy-2.6.0.tar.gz` & `tmp/msticpy-2.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msticpy-2.6.0.tar", last modified: Tue Jul 25 01:04:56 2023, max compression
+gzip compressed data, was "msticpy-2.7.0rc1.tar", last modified: Tue Aug  8 18:51:11 2023, max compression
```

## Comparing `msticpy-2.6.0.tar` & `msticpy-2.7.0rc1.tar`

### file list

```diff
@@ -1,419 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-25 01:04:41.000000 msticpy-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 01:04:41.000000 msticpy-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-07-25 01:04:41.000000 msticpy-2.6.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-25 01:04:56.175965 msticpy-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-07-25 01:04:41.000000 msticpy-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/anomalous.py
--rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/sessionize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/cluster_auditd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/code_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/polling_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/analysis/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/azure_auth_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/cloud_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/cred_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyring_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyvault_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/keyvault_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/msal_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/auth/secret_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.135965 msticpy-2.6.0/msticpy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/check_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/pkg_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/provider_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/proxy_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/common/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/utility/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/common/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_azure_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_msticpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_other_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_simple_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_ti_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/ce_user_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/comp_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/compound_ctrls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/config/mp_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.139965 msticpy-2.6.0/msticpy/context/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.143965 msticpy-2.6.0/msticpy/context/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_ti.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_watchlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/azure/sentinel_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.143965 msticpy-2.6.0/msticpy/context/contextproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/context_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/http_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/contextproviders/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/lookup_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/preprocess_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/context/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/alienvault_otx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/azure_sent_byoti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/greynoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ibm_xforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/intsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/kql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/mblookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/open_page_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/pulsedive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/result_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/riskiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ti_http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/tor_exit_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/tiproviders/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/context/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookupv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/azure_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.147965 msticpy-2.6.0/msticpy/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/data_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/data_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/param_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_provider_connections_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_provider_utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/core/query_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/data_obfus.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/data_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37132 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/azure_kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/azure_monitor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/cybereason_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/driver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/elastic_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/kql_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_data_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_osquery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/local_velociraptor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/mdatp_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/mordor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/odata_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/resource_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/security_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/sentinel_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/splunk_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/drivers/sumologic_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.127965 msticpy-2.6.0/msticpy/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/cybereason/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_processes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/localdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/localdata/local_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.151965 msticpy-2.6.0/msticpy/data/queries/m365d/
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/mde/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/msgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/msgraph/graph_alerts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/mssentinel/
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/resourcegraph/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/splunk/splunk_queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/queries/sumologic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/queries/sumologic/sumologic_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/query_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/sql_to_kql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/storage/azure_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.155965 msticpy-2.6.0/msticpy/data/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/loganalytics_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/splunk_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/data/uploaders/uploader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.159965 msticpy-2.6.0/msticpy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.159965 msticpy-2.6.0/msticpy/datamodel/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/azure_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/cloud_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/cloud_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/entity_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/file_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/graph_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/host_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mail_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/malware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/registry_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/registry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/submission_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/threat_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/unknown_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/entities/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/datamodel/soc/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/datamodel/soc/sentinel_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/azure_ml_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/azure_synapse_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/mp_pandas_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/mp_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/nbinit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/nbmagics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/pivot_core/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_magic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_core/pivot_register_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.163965 msticpy-2.6.0/msticpy/init/pivot_init/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/pivot_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/pivot_ti_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/pivot_init/vt_pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/init/user_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/msticpyconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/nbtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/entityschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/nbwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_alert_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/security_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbtools/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/nbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/get_environment_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/get_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/lookback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/option_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/query_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/nbwidgets/select_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.167965 msticpy-2.6.0/msticpy/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/WinSecurityEvent.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/cmd_line_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/mp_pivot_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/mpconfig_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/resources/obfuscation_cols.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/proc_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/sectools_magics.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.171965 msticpy-2.6.0/msticpy/sectools/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtlookupv3.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/msticpy/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/transform/process_tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.175965 msticpy-2.6.0/msticpy/vis/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/code_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/data_viewer_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/entity_graph_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/figure_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/matrix_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/mordor_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/mp_pandas_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/network_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/query_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeline_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-25 01:04:42.000000 msticpy-2.6.0/msticpy/vis/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:04:56.131965 msticpy-2.6.0/msticpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:04:55.000000 msticpy-2.6.0/msticpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 01:04:56.000000 msticpy-2.6.0/msticpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 01:04:42.000000 msticpy-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-25 01:04:42.000000 msticpy-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-25 01:04:56.179965 msticpy-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-25 01:04:42.000000 msticpy-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.417724 msticpy-2.7.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   487752 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17488 2023-08-08 18:51:11.417724 msticpy-2.7.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.341723 msticpy-2.7.0rc1/msticpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.341723 msticpy-2.7.0rc1/msticpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.341723 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/anomalous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29469 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/sessionize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.345723 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/cluster_auditd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/code_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/polling_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/analysis/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.345723 msticpy-2.7.0rc1/msticpy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/azure_auth_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/cloud_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/cred_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/keyring_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/keyvault_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/keyvault_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/msal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/auth/secret_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.349723 msticpy-2.7.0rc1/msticpy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/pkg_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/provider_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/proxy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.349723 msticpy-2.7.0rc1/msticpy/common/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/utility/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/utility/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/utility/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/common/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.353723 msticpy-2.7.0rc1/msticpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_azure_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_msticpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_other_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_simple_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_ti_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/ce_user_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/comp_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/compound_ctrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/mp_config_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/mp_config_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/mp_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35348 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/config/query_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.357723 msticpy-2.7.0rc1/msticpy/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.361723 msticpy-2.7.0rc1/msticpy/context/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35954 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_dynamic_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_dynamic_summary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_ti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_watchlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/azure/sentinel_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/contextlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.361723 msticpy-2.7.0rc1/msticpy/context/contextproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/contextproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/contextproviders/context_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/contextproviders/http_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/contextproviders/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/lookup_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/preprocess_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.365723 msticpy-2.7.0rc1/msticpy/context/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/abuseipdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/alienvault_otx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/azure_sent_byoti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/crowdsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/greynoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/ibm_xforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/intsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/kql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/mblookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/open_page_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/pulsedive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/result_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/riskiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/ti_http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/tor_exit_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/tiproviders/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.369723 msticpy-2.7.0rc1/msticpy/context/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtlookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtlookupv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.369723 msticpy-2.7.0rc1/msticpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.369723 msticpy-2.7.0rc1/msticpy/data/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/azure_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.373723 msticpy-2.7.0rc1/msticpy/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/data_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/param_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_provider_connections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_provider_utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/core/query_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/data_obfus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/data_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.377723 msticpy-2.7.0rc1/msticpy/data/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37124 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/azure_kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/azure_monitor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/cybereason_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/elastic_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22798 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/kql_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/local_data_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/local_osquery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/local_velociraptor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/mdatp_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/mordor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/odata_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/resource_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/security_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/sentinel_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/splunk_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/drivers/sumologic_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.337723 msticpy-2.7.0rc1/msticpy/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.377723 msticpy-2.7.0rc1/msticpy/data/queries/cybereason/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_connections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_hosts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_processes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.377723 msticpy-2.7.0rc1/msticpy/data/queries/localdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/localdata/local_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.381723 msticpy-2.7.0rc1/msticpy/data/queries/m365d/
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_identity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.381723 msticpy-2.7.0rc1/msticpy/data/queries/mde/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.381723 msticpy-2.7.0rc1/msticpy/data/queries/msgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/msgraph/graph_alerts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/queries/resourcegraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/queries/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_alert_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/queries/sumologic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/queries/sumologic/sumologic_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/sql_to_kql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/storage/azure_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/data/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/uploaders/loganalytics_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/uploaders/splunk_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/data/uploaders/uploader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.389723 msticpy-2.7.0rc1/msticpy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.397724 msticpy-2.7.0rc1/msticpy/datamodel/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/azure_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/cloud_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/cloud_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/entity_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/entity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/file_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/graph_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/host_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/mail_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/malware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/registry_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/registry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/submission_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/threat_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/unknown_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/entities/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.401723 msticpy-2.7.0rc1/msticpy/datamodel/soc/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/soc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/soc/incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/datamodel/soc/sentinel_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.401723 msticpy-2.7.0rc1/msticpy/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/azure_ml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/azure_synapse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/mp_pandas_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/mp_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/nbinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/nbmagics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.405723 msticpy-2.7.0rc1/msticpy/init/pivot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_magic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_register_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.405723 msticpy-2.7.0rc1/msticpy/init/pivot_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_init/pivot_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_init/pivot_ti_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/pivot_init/vt_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/init/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/msticpyconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.409723 msticpy-2.7.0rc1/msticpy/nbtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/entityschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/nbwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/security_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/security_alert_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/security_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/security_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbtools/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.409723 msticpy-2.7.0rc1/msticpy/nbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/get_environment_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/get_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/lookback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/option_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/query_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/select_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/select_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/nbwidgets/select_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.409723 msticpy-2.7.0rc1/msticpy/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   104245 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/resources/WinSecurityEvent.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/resources/cmd_line_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/resources/mp_pivot_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/resources/mpconfig_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/resources/obfuscation_cols.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.413724 msticpy-2.7.0rc1/msticpy/sectools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/proc_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/sectools_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.413724 msticpy-2.7.0rc1/msticpy/sectools/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/vtlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.413724 msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtlookupv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.413724 msticpy-2.7.0rc1/msticpy/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/transform/process_tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.417724 msticpy-2.7.0rc1/msticpy/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/code_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/data_viewer_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/entity_graph_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/figure_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/matrix_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/mordor_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/mp_pandas_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/network_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/query_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeline_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeline_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/msticpy/vis/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:51:11.341723 msticpy-2.7.0rc1/msticpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17488 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 18:51:11.000000 msticpy-2.7.0rc1/msticpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-08 18:51:11.417724 msticpy-2.7.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-08 18:50:59.000000 msticpy-2.7.0rc1/setup.py
```

### Comparing `msticpy-2.6.0/LICENSE` & `msticpy-2.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/NOTICE.txt` & `msticpy-2.7.0rc1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/PKG-INFO` & `msticpy-2.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.6.0
+Version: 2.7.0rc1
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.6.0/README.md` & `msticpy-2.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/__init__.py` & `msticpy-2.7.0rc1/msticpy/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/__init__.py` & `msticpy-2.7.0rc1/msticpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/anomalous.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/anomalous.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/model.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/model.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/sessionize.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/sessionize.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py` & `msticpy-2.7.0rc1/msticpy/analysis/anomalous_sequence/utils/probabilities.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/cluster_auditd.py` & `msticpy-2.7.0rc1/msticpy/analysis/cluster_auditd.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/code_cleanup.py` & `msticpy-2.7.0rc1/msticpy/analysis/code_cleanup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/eventcluster.py` & `msticpy-2.7.0rc1/msticpy/analysis/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/observationlist.py` & `msticpy-2.7.0rc1/msticpy/analysis/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/outliers.py` & `msticpy-2.7.0rc1/msticpy/analysis/outliers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/polling_detection.py` & `msticpy-2.7.0rc1/msticpy/analysis/polling_detection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/syslog_utils.py` & `msticpy-2.7.0rc1/msticpy/analysis/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/analysis/timeseries.py` & `msticpy-2.7.0rc1/msticpy/analysis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/__init__.py` & `msticpy-2.7.0rc1/msticpy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/azure_auth.py` & `msticpy-2.7.0rc1/msticpy/auth/azure_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     tenant_id : str, optional
         The tenant to authenticate against. If not supplied, the default
         tenant for the identity will be used.
     silent : bool, optional
         Set True to hide all output during connection, by default False
     credential : AzureCredential
         If an Azure credential is passed, it will be used directly.
+    cloud : str, optional
+        What Azure cloud to connect to.
+        By default it will attempt to use the cloud setting from config file.
+        If this is not set it will default to Azure Public Cloud
 
     Returns
     -------
     AzCredentials
         Named tuple of:
         - legacy (ADAL) credentials
         - modern (MSAL) credentials
@@ -70,15 +74,15 @@
         If chained token credential creation fails.
 
     See Also
     --------
     list_auth_methods
 
     """
-    az_cloud_config = AzureCloudConfig()
+    az_cloud_config = AzureCloudConfig(cloud=kwargs.get("cloud"))
     # Use auth_methods param or configuration defaults
     data_provs = get_provider_settings(config_section="DataProviders")
     auth_methods = auth_methods or az_cloud_config.auth_methods
 
     # Ignore AzCLI settings except for authentication creds for EnvCred
     az_cli_config = data_provs.get("AzureCLI")
     if (
```

### Comparing `msticpy-2.6.0/msticpy/auth/azure_auth_core.py` & `msticpy-2.7.0rc1/msticpy/auth/azure_auth_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/cloud_mappings.py` & `msticpy-2.7.0rc1/msticpy/auth/cloud_mappings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/cred_wrapper.py` & `msticpy-2.7.0rc1/msticpy/auth/cred_wrapper.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/keyring_client.py` & `msticpy-2.7.0rc1/msticpy/auth/keyring_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/keyvault_client.py` & `msticpy-2.7.0rc1/msticpy/auth/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/keyvault_settings.py` & `msticpy-2.7.0rc1/msticpy/auth/keyvault_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/msal_auth.py` & `msticpy-2.7.0rc1/msticpy/auth/msal_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/auth/secret_settings.py` & `msticpy-2.7.0rc1/msticpy/auth/secret_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/__init__.py` & `msticpy-2.7.0rc1/msticpy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/azure_auth.py` & `msticpy-2.7.0rc1/msticpy/common/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/check_version.py` & `msticpy-2.7.0rc1/msticpy/common/check_version.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/data_types.py` & `msticpy-2.7.0rc1/msticpy/common/data_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/data_utils.py` & `msticpy-2.7.0rc1/msticpy/common/data_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/exceptions.py` & `msticpy-2.7.0rc1/msticpy/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/pkg_config.py` & `msticpy-2.7.0rc1/msticpy/common/pkg_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/provider_settings.py` & `msticpy-2.7.0rc1/msticpy/common/provider_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/proxy_settings.py` & `msticpy-2.7.0rc1/msticpy/common/proxy_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/settings.py` & `msticpy-2.7.0rc1/msticpy/common/settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/timespan.py` & `msticpy-2.7.0rc1/msticpy/common/timespan.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     def _parse_time(time_val, prop_name):
         if time_val is None:
             return None
         if isinstance(time_val, datetime):
             return time_val
         with contextlib.suppress(ValueError, ParserError):
             if isinstance(time_val, str):
-                return pd.to_datetime(time_val, infer_datetime_format=True)
+                return pd.to_datetime(time_val)
         raise ValueError(f"'{prop_name}' must be a datetime or a datetime string.")
 
     @staticmethod
     def _parse_timedelta(time_val):
         if time_val is None:
             return None
         if isinstance(time_val, timedelta):
```

### Comparing `msticpy-2.6.0/msticpy/common/utility/__init__.py` & `msticpy-2.7.0rc1/msticpy/common/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/utility/format.py` & `msticpy-2.7.0rc1/msticpy/common/utility/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     -------
     str
         The de-fanged observable.
 
     """
     de_fanged = ioc
     if ioc_type == "email":
-        de_fanged = de_fanged.replace("@", "AT")
+        de_fanged = de_fanged.replace("@", "[AT]")
     elif ioc_type == "url":
         de_fanged = de_fanged.replace("http", "hXXp").replace("ftp", "fXp")
     return de_fanged.replace(".", "[.]")
 
 
 @export
 def refang_ioc(ioc: str, ioc_type: str = None) -> str:
@@ -137,11 +137,11 @@
     -------
     str
         The re-fanged observable.
 
     """
     re_fanged = ioc
     if ioc_type == "email":
-        re_fanged = re_fanged.replace("AT", "@")
+        re_fanged = re_fanged.replace("[AT]", "@")
     elif ioc_type == "url":
         re_fanged = re_fanged.replace("hXXp", "http").replace("fXp", "ftp")
     return re_fanged.replace("[.]", ".")
```

### Comparing `msticpy-2.6.0/msticpy/common/utility/ipython.py` & `msticpy-2.7.0rc1/msticpy/common/utility/ipython.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/utility/package.py` & `msticpy-2.7.0rc1/msticpy/common/utility/package.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/utility/types.py` & `msticpy-2.7.0rc1/msticpy/common/utility/types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/common/wsconfig.py` & `msticpy-2.7.0rc1/msticpy/common/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/__init__.py` & `msticpy-2.7.0rc1/msticpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_azure.py` & `msticpy-2.7.0rc1/msticpy/config/ce_azure.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_azure_sentinel.py` & `msticpy-2.7.0rc1/msticpy/config/ce_azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_common.py` & `msticpy-2.7.0rc1/msticpy/config/ce_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_data_providers.py` & `msticpy-2.7.0rc1/msticpy/config/ce_data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_keyvault.py` & `msticpy-2.7.0rc1/msticpy/config/ce_keyvault.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_msticpy.py` & `msticpy-2.7.0rc1/msticpy/config/ce_msticpy.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_other_providers.py` & `msticpy-2.7.0rc1/msticpy/config/ce_other_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_provider_base.py` & `msticpy-2.7.0rc1/msticpy/config/ce_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_simple_settings.py` & `msticpy-2.7.0rc1/msticpy/config/ce_simple_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_ti_providers.py` & `msticpy-2.7.0rc1/msticpy/config/ce_ti_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/ce_user_defaults.py` & `msticpy-2.7.0rc1/msticpy/config/ce_user_defaults.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/comp_edit.py` & `msticpy-2.7.0rc1/msticpy/config/comp_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/compound_ctrls.py` & `msticpy-2.7.0rc1/msticpy/config/compound_ctrls.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/file_browser.py` & `msticpy-2.7.0rc1/msticpy/config/file_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/mp_config_control.py` & `msticpy-2.7.0rc1/msticpy/config/mp_config_control.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/mp_config_edit.py` & `msticpy-2.7.0rc1/msticpy/config/mp_config_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/config/mp_config_file.py` & `msticpy-2.7.0rc1/msticpy/config/mp_config_file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/__init__.py` & `msticpy-2.7.0rc1/msticpy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/azure/azure_data.py` & `msticpy-2.7.0rc1/msticpy/context/azure/azure_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Uses the Azure Python SDK to collect and return details related to Azure."""
 import datetime
+import logging
 from typing import Any, Dict, List, Optional, Tuple
 
 import attr
 import numpy as np
 import pandas as pd
 from azure.common.exceptions import CloudError
 from azure.core.exceptions import ClientAuthenticationError
@@ -51,14 +52,16 @@
         title="Error importing azure module",
         extra="azure",
     ) from imp_err
 
 __version__ = VERSION
 __author__ = "Pete Bryan"
 
+logger = logging.getLogger(__name__)
+
 _CLIENT_MAPPING = {
     "sub_client": SubscriptionClient,
     "resource_client": ResourceManagementClient,
     "network_client": NetworkManagementClient,
     "monitoring_client": MonitorManagementClient,
     "compute_client": ComputeManagementClient,
 }
@@ -125,60 +128,77 @@
         self.sub_client: Optional[SubscriptionClient] = None
         self.resource_client: Optional[ResourceManagementClient] = None
         self.network_client: Optional[NetworkManagementClient] = None
         self.monitoring_client: Optional[MonitorManagementClient] = None
         self.compute_client: Optional[ComputeManagementClient] = None
         self.cloud = cloud or AzureCloudConfig().cloud
         self.endpoints = get_all_endpoints(self.cloud)  # type: ignore
+        logger.info("Initialized AzureData")
         if connect:
             self.connect()
 
     def connect(
         self,
         auth_methods: Optional[List] = None,
         tenant_id: Optional[str] = None,
         silent: bool = False,
+        **kwargs,
     ):
         """
         Authenticate to the Azure SDK.
 
         Parameters
         ----------
         auth_methods : List, optional
             list of preferred authentication methods to use, by default None
         tenant_id : str, optional
             The tenant to authenticate against. If not supplied, the default
             tenant for the identity will be used.
         silent : bool, optional
             Set true to prevent output during auth process, by default False
+        cloud : str, optional
+            What Azure cloud to connect to.
+            By default it will attempt to use the cloud setting from config file.
+            If this is not set it will default to Azure Public Cloud
+        **kwargs
+            Additional keyword arguments to pass to the az_connect function.
 
         Raises
         ------
         CloudError
             If no valid credentials are found or if subscription client can't be created
 
+        See Also
+        --------
+        msticpy.auth.azure_auth.az_connect : function to authenticate to Azure SDK
+
         """
+        if kwargs.get("cloud"):
+            logger.info("Setting cloud to %s", kwargs["cloud"])
+            self.cloud = kwargs["cloud"]
+            self.azure_cloud_config = AzureCloudConfig(self.cloud)
         auth_methods = auth_methods or self.az_cloud_config.auth_methods
         tenant_id = tenant_id or self.az_cloud_config.tenant_id
         self.credentials = az_connect(
-            auth_methods=auth_methods, tenant_id=tenant_id, silent=silent
+            auth_methods=auth_methods, tenant_id=tenant_id, silent=silent, **kwargs
         )
         if not self.credentials:
             raise CloudError("Could not obtain credentials.")
         self._check_client("sub_client")
         if only_interactive_cred(self.credentials.modern) and not silent:
             print("Check your default browser for interactive sign-in prompt.")
 
         self.sub_client = SubscriptionClient(
             credential=self.credentials.modern,
             base_url=self.endpoints.resource_manager,
             credential_scopes=[self.az_cloud_config.token_uri],
         )
         if not self.sub_client:
             raise CloudError("Could not create a Subscription client.")
+        logger.info("Connected to Azure Subscription Client")
         self.connected = True
 
     def get_subscriptions(self) -> pd.DataFrame:
         """
         Get details of all subscriptions within the tenant.
 
         Returns
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_analytics.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             "enabled": str(enabled).lower(),
         }
         data = _build_sent_data(data_items, props=True)
         data["kind"] = "Scheduled"
         params = {"api-version": "2020-01-01"}
         response = httpx.put(
             analytic_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code != 201:
             raise CloudError(response=response)
         print("Analytic Created.")
@@ -301,15 +301,15 @@
         """
         self.check_connected()  # type: ignore
         analytic_id = self._get_analytic_id(analytic_rule)
         analytic_url = self.sent_urls["alert_rules"] + f"/{analytic_id}"  # type: ignore
         params = {"api-version": "2020-01-01"}
         response = httpx.delete(
             analytic_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code != 200:
             raise CloudError(response=response)
         print("Analytic Deleted.")
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_bookmarks.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_bookmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             data_items["notes"] = notes
         if labels:
             data_items["labels"] = labels
         data = _build_sent_data(data_items, props=True)
         params = {"api-version": "2020-01-01"}
         response = httpx.put(
             bookmark_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code == 200:
             print("Bookmark created.")
             return response.json().get("name")
@@ -119,15 +119,15 @@
         """
         self.check_connected()  # type: ignore
         bookmark_id = self._get_bookmark_id(bookmark)
         bookmark_url = self.sent_urls["bookmarks"] + f"/{bookmark_id}"  # type: ignore
         params = {"api-version": "2020-01-01"}
         response = httpx.delete(
             bookmark_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code == 200:
             print("Bookmark deleted.")
         else:
             raise CloudError(response=response)
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_core.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_provider_utils_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,307 +1,379 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-"""Uses the Microsoft Sentinel APIs to interact with Microsoft Sentinel Workspaces."""
-
-import contextlib
-from typing import Any, Dict, List, Optional
-
-import pandas as pd
+"""Query Provider mixin methods."""
+import re
+from collections import abc
+from typing import Dict, Iterable, List, NamedTuple, Optional, Pattern, Protocol, Union
 
 from ..._version import VERSION
-from ...common.exceptions import MsticpyUserConfigError
-from ...common.wsconfig import WorkspaceConfig
-from .azure_data import AzureData, get_token
-from .sentinel_analytics import SentinelAnalyticsMixin, SentinelHuntingMixin
-from .sentinel_bookmarks import SentinelBookmarksMixin
-from .sentinel_dynamic_summary import SentinelDynamicSummaryMixin, SentinelQueryProvider
-from .sentinel_incidents import SentinelIncidentsMixin
-from .sentinel_search import SentinelSearchlistsMixin
-from .sentinel_ti import SentinelTIMixin
-from .sentinel_utils import (
-    _PATH_MAPPING,
-    SentinelUtilsMixin,
-    parse_resource_id,
-    validate_res_id,
-)
-from .sentinel_watchlists import SentinelWatchlistsMixin
-from .sentinel_workspaces import SentinelWorkspacesMixin
+from ...common.utility.package import lazy_import
+from ..drivers.driver_base import DriverBase
+from .query_defns import DataEnvironment
+from .query_source import QuerySource
+from .query_store import QueryStore
 
 __version__ = VERSION
-__author__ = "Pete Bryan"
+__author__ = "Ian Hellen"
 
+query_browser = lazy_import("msticpy.vis.query_browser", "browse_queries")
 
-# pylint: disable=too-many-ancestors, too-many-instance-attributes
-class MicrosoftSentinel(
-    SentinelAnalyticsMixin,
-    SentinelHuntingMixin,
-    SentinelBookmarksMixin,
-    SentinelDynamicSummaryMixin,
-    SentinelIncidentsMixin,
-    SentinelUtilsMixin,
-    SentinelWatchlistsMixin,
-    SentinelSearchlistsMixin,
-    SentinelWorkspacesMixin,
-    SentinelTIMixin,
-    AzureData,
-):
-    """Class for returning key Microsoft Sentinel elements."""
 
-    def __init__(
-        self,
-        res_id: Optional[str] = None,
-        connect: Optional[bool] = False,
-        cloud: Optional[str] = None,
-        sub_id: Optional[str] = None,
-        res_grp: Optional[str] = None,
-        ws_name: Optional[str] = None,
-        **kwargs,
-    ):
+# pylint: disable=too-few-public-methods
+class QueryProviderProtocol(Protocol):
+    """Protocol for required properties of QueryProvider class."""
+
+    _query_provider: DriverBase
+    query_store: QueryStore
+
+    def _add_query_functions(self):
+        pass
+
+
+class QueryParam(NamedTuple):
+    """
+    Named tuple for custom query parameters.
+
+    name and data_type are mandatory.
+    description and default are optional.
+
+    """
+
+    name: str
+    data_type: str
+    description: Optional[str] = None
+    default: Optional[str] = None
+
+
+# pylint: disable=super-init-not-called
+class QueryProviderUtilsMixin(QueryProviderProtocol):
+    """Mixin utility methods for QueryProvider class."""
+
+    create_param = QueryParam
+
+    @property
+    def connected(self) -> bool:
+        """
+        Return True if the provider is connected.
+
+        Returns
+        -------
+        bool
+            True if the provider is connected.
+
+        """
+        return self._query_provider.connected
+
+    @property
+    def connection_string(self) -> str:
+        """
+        Return provider connection string.
+
+        Returns
+        -------
+        str
+            Provider connection string.
+
+        """
+        return self._query_provider.current_connection
+
+    @property
+    def schema(self) -> Dict[str, Dict]:
+        """
+        Return current data schema of connection.
+
+        Returns
+        -------
+        Dict[str, Dict]
+            Data schema of current connection.
+
+        """
+        return self._query_provider.schema
+
+    @property
+    def schema_tables(self) -> List[str]:
+        """
+        Return list of tables in the data schema of the connection.
+
+        Returns
+        -------
+        List[str]
+            Tables in the of current connection.
+
+        """
+        return list(self._query_provider.schema.keys())
+
+    @property
+    def instance(self) -> Optional[str]:
+        """
+        Return instance name, if any for provider.
+
+        Returns
+        -------
+        Optional[str]
+            The instance name or None for drivers that do not
+            support multiple instances.
+
+        """
+        return self._query_provider.instance
+
+    def import_query_file(self, query_file: str):
+        """
+        Import a yaml data source definition.
+
+        Parameters
+        ----------
+        query_file : str
+            Path to the file to import
+
+        """
+        self.query_store.import_file(query_file)
+        self._add_query_functions()
+
+    def driver_help(self):
+        """Display help for the driver."""
+        print(self._query_provider.__doc__)
+
+    @classmethod
+    def list_data_environments(cls) -> List[str]:
+        """
+        Return list of current data environments.
+
+        Returns
+        -------
+        List[str]
+            List of current data environments
+
+        """
+        # pylint: disable=not-an-iterable
+        return [
+            de
+            for de in dir(DataEnvironment)
+            if de != "Unknown" and not de.startswith("_")
+        ]
+        # pylint: enable=not-an-iterable
+
+    def list_queries(self, substring: Optional[str] = None) -> List[str]:
         """
-        Initialize connector for Azure APIs.
+        Return list of family.query in the store.
 
         Parameters
         ----------
-        res_id : str, optional
-            Set the Sentinel workspace resource ID you want to use, if not specified
-            defaults will be looked for or details can be passed separately with functions.
-        connect : bool, optional
-            Set true if you want to connect to API on initialization, by default False
-        cloud : str, optional
-            Specify cloud to use, overriding any configuration value.
-            Default is to use configuration setting or public cloud if no
-            configuration setting is available.
-        sub_id : str, optional
-            If not specifying a resource ID the Subscription ID of the Sentinel Workspace
-            by default None
-        res_grp : str, optional
-            If not specifying a resource ID the Resource Group name of the
-            Sentinel Workspace, by default None
-        ws_name : str, optional
-            If not specifying a resource ID, the Workspace name of the
-            Sentinel Workspace, by default None
-        workspace : str, optional
-            Alias of ws_name
-
-        """
-        self.user_cloud = cloud
-        super().__init__(connect=False, cloud=self.user_cloud)
-        self.base_url = self.endpoints.resource_manager
-        self.default_subscription: Optional[str] = None
-        self._resource_id = res_id
-        self._default_resource_group: Optional[str] = None
-        self.sent_urls: Dict[str, str] = {}
-        self.sent_data_query: Optional[SentinelQueryProvider] = None  # type: ignore
-        self.url: Optional[str] = None
-
-        workspace = kwargs.get("workspace", ws_name)
-        self._default_workspace: Optional[str] = workspace
-        self.workspace_config = WorkspaceConfig(workspace)
-
-        if self._resource_id:
-            # If a resource ID is supplied, use that
-            self.url = self._build_sent_paths(self._resource_id, self.base_url)  # type: ignore
-            res_id_parts = parse_resource_id(self._resource_id)
-            self.default_subscription = res_id_parts["subscription_id"]
-            self._default_resource_group = res_id_parts["resource_group"]
-            self._default_workspace = workspace or res_id_parts["workspace_name"]
-            if self._default_workspace in WorkspaceConfig.list_workspaces():
-                self.workspace_config = WorkspaceConfig(
-                    workspace=self._default_workspace
+        substring : Optional[str]
+            Optional pattern - will return only queries matching the pattern,
+            default None.
+
+        Returns
+        -------
+        List[str]
+            List of queries
+
+        """
+        if substring:
+            return list(
+                filter(
+                    lambda x: substring in x.lower(),  # type: ignore
+                    self.query_store.query_names,
                 )
-        else:
-            # Otherwise - use details from specified workspace or default from settings
-            self.default_subscription = self.workspace_config.get(
-                "subscription_id", sub_id
-            )
-            self._default_resource_group = self.workspace_config.get(
-                "resource_group", res_grp
-            )
-            workspace_name = self.workspace_config.get("workspace_name", workspace)
-            self._resource_id = self._build_sent_res_id(
-                sub_id=self.default_subscription,
-                res_grp=self._default_resource_group,
-                ws_name=workspace_name,
-            )
-            self._default_workspace = workspace_name
-            self.url = self._build_sent_paths(
-                self._resource_id, self.base_url  # type: ignore
             )
+        return list(self.query_store.query_names)
 
-        if connect:
-            self.connect()
-
-    def connect(
+    def search(
         self,
-        auth_methods: Optional[List] = None,
-        tenant_id: Optional[str] = None,
-        silent: bool = False,
-        **kwargs,
-    ):
+        search: Union[str, Iterable[str]] = None,
+        table: Union[str, Iterable[str]] = None,
+        param: Union[str, Iterable[str]] = None,
+        ignore_case: bool = True,
+    ) -> List[str]:
         """
-        Authenticate with the SDK & API.
+        Search queries for match properties.
 
         Parameters
         ----------
-        auth_methods : List, optional
-            list of preferred authentication methods to use, by default None
-        tenant_id : str, optional
-            Specify cloud tenant to use
-        silent : bool, optional
-            Set true to prevent output during auth process, by default False
+        search : Union[str, Iterable[str]], optional
+            String or iterable of search terms to match on
+            any property of the query, by default None.
+            The properties include: name, description, table,
+            parameter names and query_text.
+        table : Union[str, Iterable[str]], optional
+            String or iterable of search terms to match on
+            the query table name, by default None
+        param : Union[str, Iterable[str]], optional
+            String or iterable of search terms to match on
+            the query parameter names, by default None
+        ignore_case : bool
+            Use case-insensitive search, default is True.
+
+        Returns
+        -------
+        List[str]
+            A list of matched queries
+
+        Notes
+        -----
+        Search terms are treated as regular expressions.
+        Supplying multiple parameters returns the intersection
+        of matches for each category. For example:
+        `qry_prov.search(search="account", table="syslog")` will
+        match queries that have a table parameter of "syslog" AND
+        have the term "Account" somewhere in the query properties.
 
         """
-        if workspace := kwargs.get("workspace"):
-            # override any previous default setting
-            self.workspace_config = WorkspaceConfig(workspace)
-        if not self.workspace_config:
-            self.workspace_config = WorkspaceConfig()
-        tenant_id = (
-            tenant_id or self.workspace_config[WorkspaceConfig.CONF_TENANT_ID_KEY]
-        )
+        if not (search or table or param):
+            return []
 
-        super().connect(auth_methods=auth_methods, tenant_id=tenant_id, silent=silent)
-        if "token" in kwargs:
-            self.token = kwargs["token"]
-        else:
-            self.token = get_token(
-                self.credentials, tenant_id=tenant_id, cloud=self.user_cloud  # type: ignore
+        glob_searches = _normalize_to_regex(search, ignore_case)
+        table_searches = _normalize_to_regex(table, ignore_case)
+        param_searches = _normalize_to_regex(param, ignore_case)
+        search_hits: List[str] = []
+        for query, search_data in self.query_store.search_items.items():
+            glob_match = (not glob_searches) or any(
+                re.search(term, prop)
+                for term in glob_searches
+                for prop in search_data.values()
             )
-
-        with contextlib.suppress(KeyError):
-            self.default_subscription = self.workspace_config[
-                WorkspaceConfig.CONF_SUB_ID_KEY
-            ]
-            self.set_default_workspace(
-                self.default_subscription,
-                self.workspace_config[WorkspaceConfig.CONF_WS_NAME_KEY],
+            table_match = (not table_searches) or any(
+                re.search(term, search_data["table"]) for term in table_searches
             )
-        self._create_api_paths_for_workspace(
-            az_resource_id=None,
-            subscription_id=self.workspace_config.get(WorkspaceConfig.CONF_SUB_ID_KEY),
-            resource_group=self.workspace_config.get(
-                WorkspaceConfig.CONF_RES_GROUP_KEY
-            ),
-            workspace_name=self.workspace_config.get(WorkspaceConfig.CONF_WS_NAME_KEY),
-        )
-
-    def _create_api_paths_for_workspace(
-        self,
-        az_resource_id: Optional[str] = None,
-        subscription_id: Optional[str] = None,
-        resource_group: Optional[str] = None,
-        workspace_name: Optional[str] = None,
-    ):
-        """Save configuration and build API URLs for workspace."""
-        if workspace_name:
-            self.workspace_config = WorkspaceConfig(workspace=workspace_name)
-        az_resource_id = az_resource_id or self._resource_id
-        if not az_resource_id:
-            az_resource_id = self._build_sent_res_id(
-                subscription_id, resource_group, workspace_name  # type: ignore
+            param_match = (not param_searches) or any(
+                re.search(term, search_data["params"]) for term in param_searches
             )
-        az_resource_id = validate_res_id(az_resource_id)
-        self.url = self._build_sent_paths(az_resource_id, self.base_url)  # type: ignore
+            if glob_match and table_match and param_match:
+                search_hits.append(query)
+        return sorted(search_hits)
 
-        self.sent_urls = {
-            name: f"{self.url}{mapping}" for name, mapping in _PATH_MAPPING.items()
-        }
+    def query_help(self, query_name: str):
+        """
+        Print help for `query_name`.
 
-    def set_default_subscription(self, subscription_id: str):
-        """Set the default subscription to use to `subscription_id`."""
-        subs_df = self.get_subscriptions()
-        if subscription_id in subs_df["Subscription ID"].values:
-            self.default_subscription = subscription_id
-        else:
-            print(f"Subscription ID {subscription_id} not found.")
-            print(
-                f"Subscriptions found: {', '.join(subs_df['Subscription ID'].values)}"
-            )
+        Parameters
+        ----------
+        query_name : str
+            The name of the query.
 
-    def set_default_workspace(
-        self, sub_id: Optional[str], workspace: Optional[str] = None
-    ):
         """
-        Set the default workspace.
+        self.query_store[query_name].help()
+
+    def get_query(self, query_name: str) -> str:
+        """
+        Return the raw query text for `query_name`.
 
         Parameters
         ----------
-        sub_id : Optional[str], optional
-            Subscription ID containing the workspace. If not specified,
-            the subscription will be taken from the `default_subscription`
-            or from configuration.
-        workspace : Optional[str], optional
-            Name of the workspace, by default None.
-            If not specified and there is only one workspace in the
-            subscription, this will be set as the default.
-
-        Raises
-        ------
-        ValueError
-            If no current or default subscription has been set.
-
-        """
-        sub_id = sub_id or self.default_subscription
-        if not sub_id:
-            raise MsticpyUserConfigError(
-                "No current or default subscription ID set.",
-                "Please configure the subscription ID for your workspace in your"
-                "msticpyconfig.yaml",
-            )
-        self._default_workspace = workspace
-        ws_res_id: Optional[str] = None
-        # if workspace not supplied trying looking up in subscription
-        if not workspace:
-            workspaces = self.get_sentinel_workspaces(sub_id=sub_id)
-            if len(workspaces) == 1:
-                # if only one, use that one
-                name, ws_res_id = next(iter(workspaces.items()))
-                self._default_workspace = name
-
-        # if workspace is one that we have configuration for, get the details from there.
-        if self._default_workspace in WorkspaceConfig.list_workspaces():
-            self.workspace_config = WorkspaceConfig(workspace=self._default_workspace)
-        elif ws_res_id:
-            # otherwise construct partial settings
-            res_id_parts = parse_resource_id(ws_res_id)
-            self.workspace_config = WorkspaceConfig.from_settings(
-                {
-                    "WorkspaceName": self._default_workspace
-                    or res_id_parts["workspace_name"],
-                    "SubscriptionId": res_id_parts["subscription_id"],
-                    "ResourceGroup": res_id_parts["resource_group"],
-                }
-            )
+        query_name : str
+            The name of the query.
 
-    @property
-    def default_workspace_settings(self) -> Optional[Dict[str, Any]]:
-        """Return current default workspace settings."""
-        return self.workspace_config.mp_settings
-
-    @property
-    def default_workspace_name(self):
-        """Return the default workspace name."""
-        return self._default_workspace
+        """
+        return self.query_store[query_name].query
 
-    def list_data_connectors(self) -> pd.DataFrame:
+    def browse_queries(self, **kwargs):
         """
-        List deployed data connectors.
+        Return QueryProvider query browser.
+
+        Other Parameters
+        ----------------
+        kwargs :
+            passed to SelectItem constructor.
 
         Returns
         -------
-        pd.DataFrame
-            A DataFrame containing the deployed data connectors
+        SelectItem
+            SelectItem browser for TI Data.
+
+        """
+        return query_browser()(self, **kwargs)
 
-        Raises
-        ------
-        CloudError
-            If a valid result is not returned.
+    # alias for browse_queries
+    browse = browse_queries
 
+    def add_custom_query(
+        self,
+        name: str,
+        query: str,
+        family: Union[str, Iterable[str]],
+        description: Optional[str] = None,
+        parameters: Optional[Iterable[QueryParam]] = None,
+    ):
         """
-        return self._list_items(item_type="data_connectors")
+        Add a custom function to the provider.
+
+        Parameters
+        ----------
+        name : str
+            The name of the query.
+        query : str
+            The query text (optionally parameterized).
+        family : Union[str, Iterable[str]]
+            The query group/family or list of families. The query will
+            be added to attributes of the query provider with these
+            names.
+        description : Optional[str], optional
+            Optional description (for query help), by default None
+        parameters : Optional[Iterable[QueryParam]], optional
+            Optional list of parameter definitions, by default None.
+            If the query is parameterized you must supply definitions
+            for the parameters here - at least name and type.
+            Parameters can be the named tuple QueryParam (also
+            exposed as QueryProvider.Param) or a 4-value
+
+        Examples
+        --------
+        >>> qp = QueryProvider("MSSentinel")
+        >>> qp_host = qp.create_param("host_name", "str", "Name of Host")
+        >>> qp_start = qp.create_param("start", "datetime")
+        >>> qp_end = qp.create_param("end", "datetime")
+        >>> qp_evt = qp.create_param("event_id", "int", None, 4688)
+        >>>
+        >>> query = '''
+        >>> SecurityEvent
+        >>> | where EventID == {event_id}
+        >>> | where TimeGenerated between (datetime({start}) .. datetime({end}))
+        >>> | where Computer has "{host_name}"
+        >>> '''
+        >>>
+        >>> qp.add_custom_query(
+        >>>     name="test_host_proc",
+        >>>     query=query,
+        >>>     family="Custom",
+        >>>     parameters=[qp_host, qp_start, qp_end, qp_evt]
+        >>> )
+
+        """
+        if parameters:
+            param_dict = {
+                param[0]: {
+                    "type": param[1],
+                    "default": param[2],
+                    "description": param[3],
+                }
+                for param in parameters
+            }
+        else:
+            param_dict = {}
+        source = {
+            "args": {"query": query},
+            "description": description,
+            "parameters": param_dict,
+        }
+        metadata = {"data_families": [family] if isinstance(family, str) else family}
+        query_source = QuerySource(
+            name=name, source=source, defaults={}, metadata=metadata
+        )
+        self.query_store.add_data_source(query_source)
+        self._add_query_functions()
 
 
-# Alias for old class name
-AzureSentinel = MicrosoftSentinel
+def _normalize_to_regex(
+    search_term: Union[str, Iterable[str], None], ignore_case: bool
+) -> List[Pattern[str]]:
+    """Return iterable or str search term as list of compiled reg expressions."""
+    if not search_term:
+        return []
+    regex_opts = [re.IGNORECASE] if ignore_case else []
+    if isinstance(search_term, str):
+        return [re.compile(search_term, *regex_opts)]
+    if isinstance(search_term, abc.Iterable):
+        return [re.compile(term, *regex_opts) for term in set(search_term)]
+    return []
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_dynamic_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 )
 
         dyn_sum_url = self.sent_urls["dynamic_summary"] + f"/{summary_id}"  # type: ignore
 
         params = {"api-version": _DYN_SUM_API_VERSION}
         response = httpx.get(
             dyn_sum_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code == 200:
             logger.info("Query API for summary id %s", summary_id)
             return DynamicSummary.from_json(response.json())
         logger.info(
@@ -215,15 +215,15 @@
         dyn_sum_url = "/".join(
             [self.sent_urls["dynamic_summary"], summary.summary_id]  # type: ignore
         )
 
         params = {"api-version": _DYN_SUM_API_VERSION}
         response = httpx.put(
             dyn_sum_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=summary.to_json_api(),
             timeout=get_http_timeout(),
         )
         logger.info(
             "_create_dynamic_summary (DynamicSummary) status %d", response.status_code
         )
@@ -321,15 +321,15 @@
         """
         self.check_connected()  # type: ignore
 
         dyn_sum_url = f"{self.sent_urls['dynamic_summary']}/{summary_id}"  # type: ignore
         params = {"api-version": _DYN_SUM_API_VERSION}
         response = httpx.delete(
             dyn_sum_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         logger.info(
             "delete_dynamic_summary %s - status %d", summary_id, response.status_code
         )
         if response.status_code == 200:
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_dynamic_summary_types.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_dynamic_summary_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_incidents.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_incidents.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """
         self.check_connected()  # type: ignore
         incident_id = self._get_incident_id(incident)
         entities_url = self.sent_urls["incidents"] + f"/{incident_id}/entities"  # type: ignore
         ent_parameters = {"api-version": "2021-04-01"}
         ents = httpx.post(
             entities_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=ent_parameters,
             timeout=get_http_timeout(),
         )
         return (
             [(ent["kind"], ent["properties"]) for ent in ents.json()["entities"]]
             if ents.status_code == 200
             else []
@@ -130,15 +130,15 @@
         """
         self.check_connected()  # type: ignore
         incident_id = self._get_incident_id(incident)
         alerts_url = self.sent_urls["incidents"] + f"/{incident_id}/alerts"  # type: ignore
         alerts_parameters = {"api-version": "2021-04-01"}
         alerts_resp = httpx.post(
             alerts_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=alerts_parameters,
             timeout=get_http_timeout(),
         )
         return (
             [
                 {
                     "ID": alrts["properties"]["systemAlertId"],
@@ -248,15 +248,15 @@
         if "title" not in update_items.keys():
             update_items["title"] = incident_dets.iloc[0]["properties.title"]
         if "status" not in update_items.keys():
             update_items["status"] = incident_dets.iloc[0]["properties.status"]
         data = _build_sent_data(update_items, etag=incident_dets.iloc[0]["etag"])
         response = httpx.put(
             incident_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         print("Incident updated.")
@@ -325,15 +325,15 @@
         if first_activity_time:
             data_items["firstActivityTimeUtc"] = first_activity_time.isoformat()
         if last_activity_time:
             data_items["lastActivityTimeUtc"] = last_activity_time.isoformat()
         data = _build_sent_data(data_items, props=True)
         response = httpx.put(
             incident_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         if bookmarks:
@@ -343,15 +343,15 @@
                 mark_res_id = self.sent_urls["bookmarks"] + f"/{bookmark_id}"  # type: ignore
                 relations_url = incident_url + f"/relations/{relation_id}"
                 bkmark_data_items = {"relatedResourceId": mark_res_id}
                 data = _build_sent_data(bkmark_data_items, props=True)
                 params = {"api-version": "2021-04-01"}
                 response = httpx.put(
                     relations_url,
-                    headers=get_api_headers(self.token),  # type: ignore
+                    headers=get_api_headers(self._token),  # type: ignore
                     params=params,
                     content=str(data),
                     timeout=get_http_timeout(),
                 )
         print("Incident created.")
         return response.json().get("name")
 
@@ -422,15 +422,15 @@
         comment_url = (
             self.sent_urls["incidents"] + f"/{incident_id}/comments/{uuid4()}"  # type: ignore
         )
         params = {"api-version": "2020-01-01"}
         data = _build_sent_data({"message": comment})
         response = httpx.put(
             comment_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         print("Comment posted.")
@@ -463,15 +463,15 @@
         bkmark_data_items = {
             "relatedResourceId": mark_res_id.split("https://management.azure.com")[1]
         }
         data = _build_sent_data(bkmark_data_items, props=True)
         params = {"api-version": "2021-04-01"}
         response = httpx.put(
             bookmark_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         print("Bookmark added to incident.")
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_search.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 "startSearchTime": f"{search_start.isoformat()}",
                 "endSearchTime": f"{search_end.isoformat()}",
             }
         }
         search_body = _build_sent_data(search_items)
         search_create_response = httpx.put(
             search_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             json=search_body,
             timeout=60,
         )
         if search_create_response.status_code != 202:
             raise CloudError(response=search_create_response)
         print(f"Search job created with for {search_name}_SRCH.")
 
@@ -104,15 +104,15 @@
         """
         search_name = search_name.strip("_SRCH")
         search_url = (
             self.sent_urls["search"]  # type: ignore
             + f"/{search_name}_SRCH?api-version=2021-12-01-preview"
         )
         search_check_response = httpx.get(
-            search_url, headers=get_api_headers(self.token)  # type: ignore
+            search_url, headers=get_api_headers(self._token)  # type: ignore
         )
         if search_check_response.status_code != 200:
             raise CloudError(response=search_check_response)
 
         check_result = search_check_response.json()["properties"]["provisioningState"]
         print(f"{search_name}_SRCH status is '{check_result}'")
         if check_result == "Succeeded":
@@ -136,12 +136,12 @@
         """
         search_name = search_name.strip("_SRCH")
         search_url = (
             self.sent_urls["search"]  # type: ignore
             + f"/{search_name}_SRCH?api-version=2021-12-01-preview"
         )
         search_delete_response = httpx.delete(
-            search_url, headers=get_api_headers(self.token)  # type: ignore
+            search_url, headers=get_api_headers(self._token)  # type: ignore
         )
         if search_delete_response.status_code != 202:
             raise CloudError(response=search_delete_response)
         print(f"{search_name}_SRCH set for deletion.")
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_ti.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_ti.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             "source": "MSTICPy",
         }
         data_items.update(_build_additional_indicator_items(**kwargs))
         data = _build_sent_data(data_items, props=True)
         data["kind"] = "indicator"
         response = httpx.post(
             ti_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         if not silent:
@@ -243,15 +243,15 @@
 
         """
         self.check_connected()  # type: ignore
         ti_url = self.sent_urls["ti"] + f"/indicators/{indicator_id}"  # type: ignore
         params = {"api-version": "2021-10-01"}
         response = httpx.get(
             ti_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code != 200:
             raise CloudError(response=response)
         return response.json()
 
@@ -298,15 +298,15 @@
         full_data_items = _add_missing_items(data_items, indicator_details)
         data = _build_sent_data(full_data_items, props=True)
         data["etag"] = indicator_details["etag"]
         data["kind"] = "indicator"
         params = {"api-version": "2021-10-01"}
         response = httpx.put(
             ti_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data),
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 201):
             raise CloudError(response=response)
         print("Indicator updated.")
@@ -346,15 +346,15 @@
 
         """
         self.check_connected()  # type: ignore
         ti_url = self.sent_urls["ti"] + f"/indicators/{indicator_id}"  # type: ignore
         params = {"api-version": "2021-10-01"}
         response = httpx.delete(
             ti_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code not in (200, 204):
             raise CloudError(response=response)
         print("Indicator deleted.")
 
@@ -402,15 +402,15 @@
         """
         self.check_connected()  # type: ignore
         ti_url = self.sent_urls["ti"] + "/queryIndicators"  # type: ignore
         data_items = dict(kwargs)
         params = {"api-version": "2021-10-01"}
         response = httpx.post(
             ti_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(data_items),
             timeout=get_http_timeout(),
         )
         if response.status_code != 200:
             raise CloudError(response=response)
         return _azs_api_result_to_df(response)
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_utils.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def _get_items(self, url: str, params: Optional[dict] = None) -> httpx.Response:
         """Get items from the API."""
         self.check_connected()  # type: ignore
         if params is None:
             params = {"api-version": "2020-01-01"}
         return httpx.get(
             url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
 
     def _list_items(
         self,
         item_type: str,
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_watchlists.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_watchlists.py`

 * *Files 18% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         }  # type: Dict[str, str]
         if isinstance(data, pd.DataFrame) and not data.empty:
             data_csv = data.to_csv(index=False)
             data_items["rawContent"] = str(data_csv)
         request_data = _build_sent_data(data_items, props=True)
         response = httpx.put(
             watchlist_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             content=str(request_data),
             timeout=get_http_timeout(),
         )
         if response.status_code != 200:
             raise CloudError(response=response)
 
@@ -218,15 +218,15 @@
 
             watchlist_url = (
                 self.sent_urls["watchlists"]  # type: ignore
                 + f"/{watchlist_name}/watchlistItems/{watchlist_id}"
             )
             response = httpx.put(
                 watchlist_url,
-                headers=get_api_headers(self.token),  # type: ignore
+                headers=get_api_headers(self._token),  # type: ignore
                 params={"api-version": "2021-04-01"},
                 content=str({"properties": {"itemsKeyValue": item}}),
                 timeout=get_http_timeout(),
             )
             if response.status_code != 200:
                 raise CloudError(response=response)
 
@@ -256,22 +256,61 @@
         # Check requested watchlist actually exists
         if not self._check_watchlist_exists(watchlist_name):
             raise MsticpyUserError(f"Watchlist {watchlist_name} does not exist.")
         watchlist_url = self.sent_urls["watchlists"] + f"/{watchlist_name}"  # type: ignore
         params = {"api-version": "2021-04-01"}
         response = httpx.delete(
             watchlist_url,
-            headers=get_api_headers(self.token),  # type: ignore
+            headers=get_api_headers(self._token),  # type: ignore
             params=params,
             timeout=get_http_timeout(),
         )
         if response.status_code != 200:
             raise CloudError(response=response)
         print(f"Watchlist {watchlist_name} deleted")
 
+    def delete_watchlist_item(self, watchlist_name: str, watchlist_item_id: str):
+        """
+        Delete a Watchlist item.
+
+        Parameters
+        ----------
+        watchlist_name : str
+            The name of the watchlist with the item to be deleted
+        watchlist_item_id : str
+            The watchlist item ID to delete
+
+        Raises
+        ------
+        MsticpyUserError
+            If the specified Watchlist does not exist.
+        CloudError
+            If the API returns an error.
+
+        """
+        self.check_connected()  # type: ignore
+        # Check requested watchlist actually exists
+        if not self._check_watchlist_exists(watchlist_name):
+            raise MsticpyUserError(f"Watchlist {watchlist_name} does not exist.")
+
+        watchlist_url = (
+            self.sent_urls["watchlists"]  # type: ignore
+            + f"/{watchlist_name}/watchlistItems/{watchlist_item_id}"
+        )
+        response = httpx.delete(
+            watchlist_url,
+            headers=get_api_headers(self._token),  # type: ignore
+            params={"api-version": "2023-02-01"},
+            timeout=get_http_timeout(),
+        )
+        if response.status_code != 200:
+            raise CloudError(response=response)
+
+        print(f"Item deleted from {watchlist_name}")
+
     def _check_watchlist_exists(
         self,
         watchlist_name: str,
     ):
         """
         Check whether a Watchlist exists or not.
```

### Comparing `msticpy-2.6.0/msticpy/context/azure/sentinel_workspaces.py` & `msticpy-2.7.0rc1/msticpy/context/azure/sentinel_workspaces.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/contextlookup.py` & `msticpy-2.7.0rc1/msticpy/context/contextlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/contextproviders/context_provider_base.py` & `msticpy-2.7.0rc1/msticpy/context/contextproviders/context_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/contextproviders/http_context_provider.py` & `msticpy-2.7.0rc1/msticpy/context/contextproviders/http_context_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/contextproviders/servicenow.py` & `msticpy-2.7.0rc1/msticpy/context/contextproviders/servicenow.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/domain_utils.py` & `msticpy-2.7.0rc1/msticpy/context/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/geoip.py` & `msticpy-2.7.0rc1/msticpy/context/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/http_provider.py` & `msticpy-2.7.0rc1/msticpy/context/http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/ip_utils.py` & `msticpy-2.7.0rc1/msticpy/context/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/lookup.py` & `msticpy-2.7.0rc1/msticpy/context/lookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/lookup_result.py` & `msticpy-2.7.0rc1/msticpy/context/lookup_result.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/preprocess_observable.py` & `msticpy-2.7.0rc1/msticpy/context/preprocess_observable.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/provider_base.py` & `msticpy-2.7.0rc1/msticpy/context/provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tilookup.py` & `msticpy-2.7.0rc1/msticpy/context/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/__init__.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from ..preprocess_observable import preprocess_observable  # noqa:F401
 from .ti_http_provider import HttpTIProvider  # noqa:F401
 from .ti_provider_base import TIProvider  # noqa:F401
 
 __version__ = VERSION
 
 TI_PROVIDERS: Dict[str, Tuple[str, str]] = {
+    "CrowdSec": ("crowdsec", "CrowdSec"),
     "OTX": ("alienvault_otx", "OTX"),
     "AzSTI": ("azure_sent_byoti", "AzSTI"),
     "GreyNoise": ("greynoise", "GreyNoise"),
     "XForce": ("ibm_xforce", "XForce"),
     "IntSights": ("intsights", "IntSights"),
     "OPR": ("open_page_rank", "OPR"),
     "Tor": ("tor_exit_nodes", "Tor"),
     "VirusTotal": ("virustotal", "VirusTotal"),
     "RiskIQ": ("riskiq", "RiskIQ"),
     "Pulsedive": ("pulsedive", "Pulsedive"),
+    "AbuseIPDB": ("abuseipdb", "AbuseIPDB"),
 }
```

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/alienvault_otx.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/alienvault_otx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/azure_sent_byoti.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/azure_sent_byoti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/greynoise.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/greynoise.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/ibm_xforce.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/ibm_xforce.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/intsights.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/intsights.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/kql_base.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/kql_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/mblookup.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/mblookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/open_page_rank.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/open_page_rank.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/pulsedive.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/pulsedive.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/result_severity.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/result_severity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/riskiq.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/riskiq.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/ti_http_provider.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/ti_http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/ti_provider_base.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/tor_exit_nodes.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/tor_exit_nodes.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/tiproviders/virustotal.py` & `msticpy-2.7.0rc1/msticpy/context/tiproviders/virustotal.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/vtlookupv3/__init__.py` & `msticpy-2.7.0rc1/msticpy/context/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/vtlookupv3/vtfile_behavior.py` & `msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookup.py` & `msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/context/vtlookupv3/vtlookupv3.py` & `msticpy-2.7.0rc1/msticpy/context/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/__init__.py` & `msticpy-2.7.0rc1/msticpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure/__init__.py` & `msticpy-2.7.0rc1/msticpy/data/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure/azure_blob_storage.py` & `msticpy-2.7.0rc1/msticpy/data/azure/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure/azure_data.py` & `msticpy-2.7.0rc1/msticpy/data/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure_blob_storage.py` & `msticpy-2.7.0rc1/msticpy/data/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure_data.py` & `msticpy-2.7.0rc1/msticpy/data/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/azure_sentinel.py` & `msticpy-2.7.0rc1/msticpy/data/azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/data_providers.py` & `msticpy-2.7.0rc1/msticpy/data/core/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/data_query_reader.py` & `msticpy-2.7.0rc1/msticpy/data/core/data_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/param_extractor.py` & `msticpy-2.7.0rc1/msticpy/data/core/param_extractor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/query_container.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/query_defns.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_defns.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,19 +84,20 @@
 
     Used to identify which queries are relevant for which
     data sources.
     """
 
     Unknown = 0
     MSSentinel = 1
-    AzureSentinel = 1  # alias of LogAnalytics
-    LogAnalytics = 1
-    Kusto = 2
+    AzureSentinel = 1  # alias of MSSentinel
+    LogAnalytics = 1  # alias of MSSentinel
+    MSSentinel_New = 1  # alias of MSSentinel
+    Kusto = 2  # alias of Kusto
     AzureDataExplorer = 2  # alias of Kusto
-    AzureSecurityCenter = 3
+    Kusto_New = 2  # alias of Kusto
     MSGraph = 4
     SecurityGraph = 4
     MDE = 5
     MDATP = 5  # alias of MDE
     LocalData = 6
     Splunk = 7
     OTRF = 8
@@ -104,16 +105,18 @@
     ResourceGraph = 9
     Sumologic = 10
     M365D = 11
     Cybereason = 12
     Elastic = 14
     OSQueryLogs = 15
     OSQuery = 15
-    MSSentinel_New = 16
-    Kusto_New = 17
+    MSSentinel_Legacy = 16
+    MSSentinel_KQLM = 16
+    Kusto_Legacy = 17
+    Kusto_KQLM = 17
     VelociraptorLogs = 18
     Velociraptor = 18
 
     @classmethod
     def parse(cls, value: Union[str, int]) -> "DataEnvironment":
         """
         Convert string or int to enum.
```

### Comparing `msticpy-2.6.0/msticpy/data/core/query_provider_connections_mixin.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_provider_connections_mixin.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/query_source.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_source.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/query_store.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_store.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/core/query_template.py` & `msticpy-2.7.0rc1/msticpy/data/core/query_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """MSTICPy query template definition."""
-from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from dataclasses import field
+from typing import Any, Dict, List, Optional, Union
+
+from pydantic.dataclasses import dataclass
 
 from ..._version import VERSION
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
+# pylint: disable=too-many-instance-attributes
 @dataclass
-class Metadata:
+class QueryMetadata:
     """Metadata for query definitions."""
 
     version: int
     description: str
     data_environments: List[str]
     data_families: List[str]
     database: Optional[str] = None
     cluster: Optional[str] = None
     clusters: Optional[List[str]] = None
+    cluster_groups: Optional[List[str]] = None
     tags: List[str] = field(default_factory=list)
     data_source: Optional[str] = None
+    aliases: Optional[Union[str, List[str]]] = None
+    query_macros: Optional[Dict[str, Any]] = None
 
 
 @dataclass
-class Parameter:
+class QueryParameter:
     """Query parameter."""
 
     description: str
     datatype: str
     default: Any = None
-    required: Optional[bool] = None
+    aliases: Optional[List[str]] = None
 
 
 @dataclass
-class Defaults:
+class QueryDefaults:
     """Default values for query definitions."""
 
     metadata: Optional[Dict[str, Any]] = None
-    parameters: Dict[str, Parameter] = field(default_factory=dict)
+    parameters: Dict[str, QueryParameter] = field(default_factory=dict)
 
 
 @dataclass
-class Args:
+class QueryArgs:
     """Query arguments."""
 
     query: str = ""
+    uri: Optional[str] = None
 
 
 @dataclass
 class Query:
     """A Query definition."""
 
     description: str
-    metadata: Dict[str, Any] = field(default_factory=dict)
-    args: Args = field(default_factory=Args)
-    parameters: Dict[str, Parameter] = field(default_factory=dict)
+    args: QueryArgs = field(default_factory=QueryArgs)
+    metadata: Optional[Dict[str, Any]] = field(default_factory=dict)  # type: ignore
+    parameters: Optional[Dict[str, QueryParameter]] = field(default_factory=dict)  # type: ignore
 
 
 @dataclass
 class QueryCollection:
     """Query Collection class - a query template."""
 
-    file_name: str
-    metadata: Metadata
-    defaults: Optional[Defaults] = None
+    metadata: QueryMetadata
+    defaults: Optional[QueryDefaults] = None
     sources: Dict[str, Query] = field(default_factory=dict)
+    file_name: Optional[str] = None
```

### Comparing `msticpy-2.6.0/msticpy/data/data_obfus.py` & `msticpy-2.7.0rc1/msticpy/data/data_obfus.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/data_providers.py` & `msticpy-2.7.0rc1/msticpy/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/__init__.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 
 # flake8: noqa: F403
 from .driver_base import DriverBase
 
 __version__ = VERSION
 
 _ENVIRONMENT_DRIVERS = {
-    DataEnvironment.LogAnalytics: ("kql_driver", "KqlDriver"),
-    DataEnvironment.AzureSecurityCenter: ("kql_driver", "KqlDriver"),
+    DataEnvironment.LogAnalytics: ("azure_monitor_driver", "AzureMonitorDriver"),
     DataEnvironment.SecurityGraph: ("security_graph_driver", "SecurityGraphDriver"),
-    DataEnvironment.Kusto: ("kusto_driver", "KustoDriver"),
+    DataEnvironment.Kusto: ("azure_kusto_driver", "AzureKustoDriver"),
     DataEnvironment.MDATP: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.MDE: ("mdatp_driver", "MDATPDriver"),
     DataEnvironment.LocalData: ("local_data_driver", "LocalDataDriver"),
     DataEnvironment.OSQueryLogs: ("local_osquery_driver", "OSQueryLogDriver"),
     DataEnvironment.Splunk: ("splunk_driver", "SplunkDriver"),
     DataEnvironment.Mordor: ("mordor_driver", "MordorDriver"),
     DataEnvironment.Sumologic: ("sumologic_driver", "SumologicDriver"),
@@ -34,14 +33,16 @@
     DataEnvironment.Elastic: ("elastic_driver", "ElasticDriver"),
     DataEnvironment.MSSentinel_New: ("azure_monitor_driver", "AzureMonitorDriver"),
     DataEnvironment.Kusto_New: ("azure_kusto_driver", "AzureKustoDriver"),
     DataEnvironment.VelociraptorLogs: (
         "local_velociraptor_driver",
         "VelociraptorLogDriver",
     ),
+    DataEnvironment.MSSentinel_Legacy: ("kql_driver", "KqlDriver"),
+    DataEnvironment.Kusto_Legacy: ("kusto_driver", "KustoDriver"),
 }
 
 CUSTOM_PROVIDERS: Dict[str, type] = {}
 
 
 @singledispatch
 def import_driver(data_environment) -> type:
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/azure_kusto_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/azure_kusto_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         debug : bool
             print out additional diagnostic information.
         timeout : int
             Query timeout in seconds, default is 240 seconds (4 minutes)
             Maximum is 3600 seconds (1 hour).
             (can be set here or in connect and overridden in query methods)
         proxies : Dict[str, str]
-            Proxy settings for log analytics queries.
+            Proxy settings for Kusto queries.
             Dictionary format is {protocol: proxy_url}
             Where protocol is https, http, etc. and proxy_url can contain
             optional authentication information in the format
             "https://username:password@proxy_host:port"
             If you have a proxy configuration in msticpyconfig.yaml and
             you do not want to use it, set this to an empty dictionary.
             (can be overridden in connect method)
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/azure_monitor_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/azure_monitor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/cybereason_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/cybereason_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/driver_base.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/driver_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/elastic_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/elastic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/kql_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/kql_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 import contextlib
 import json
 import logging
 import os
 import re
 import warnings
-from datetime import datetime
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from azure.core.exceptions import ClientAuthenticationError
 from IPython import get_ipython
 
 from ..._version import VERSION
 from ...auth.azure_auth import AzureCloudConfig, az_connect, only_interactive_cred
@@ -114,28 +113,27 @@
             print out additional diagnostic information.
 
         """
         self._ip = get_ipython()
         self._debug = kwargs.get("debug", False)
         super().__init__(**kwargs)
         self.workspace_id: Optional[str] = None
-        self.set_driver_property(
-            DriverProps.FORMATTERS,
-            {"datetime": self._format_datetime, "list": self._format_list},
-        )
         self._loaded = self._is_kqlmagic_loaded()
 
         os.environ["KQLMAGIC_LOAD_MODE"] = "silent"
         if not self._loaded:
             self._load_kql_magic()
 
         self._set_kql_option("request_user_agent_tag", MSTICPY_USER_AGENT)
         self._set_kql_env_option("enable_add_items_to_help", False)
         self._schema: Dict[str, Any] = {}
         self.environment = kwargs.pop("data_environment", DataEnvironment.MSSentinel)
+        self.set_driver_property(
+            DriverProps.EFFECTIVE_ENV, DataEnvironment.MSSentinel.name
+        )
         self.kql_cloud, self.az_cloud = self._set_kql_cloud()
         for option, value in kwargs.items():
             self._set_kql_option(option, value)
 
         self.current_connection = ""
         self.current_connection_args: Dict[str, Any] = {}
         if connection_str:
@@ -299,15 +297,15 @@
         ----------
         query : str
             The kql query to execute
 
         Returns
         -------
         Tuple[pd.DataFrame, results.ResultSet]
-            A DataFrame (if successfull) and
+            A DataFrame (if successful) and
             Kql ResultSet.
 
         """
         debug = kwargs.pop("debug", self._debug)
         if debug:
             print(query)
 
@@ -453,30 +451,14 @@
         az_cloud = AzureCloudConfig().cloud
         kql_cloud = _KQL_CLOUD_MAP.get(az_cloud, "public")
         if kql_cloud != self._get_kql_option("cloud"):
             self._set_kql_option("cloud", kql_cloud)
         return kql_cloud, az_cloud
 
     @staticmethod
-    def _format_datetime(date_time: datetime) -> str:
-        """Return datetime-formatted string."""
-        return date_time.isoformat(sep="T") + "Z"
-
-    @staticmethod
-    def _format_list(param_list: Iterable[Any]):
-        """Return formatted list parameter."""
-        fmt_list = []
-        for item in param_list:
-            if isinstance(item, str):
-                fmt_list.append(f"'{item}'")
-            else:
-                fmt_list.append(f"{item}")
-        return ", ".join(fmt_list)
-
-    @staticmethod
     def _raise_query_failure(query, result):
         """Raise query failure exception."""
         err_contents = []
         if hasattr(result, "completion_query_info"):
             q_info = result.completion_query_info
             if "StatusDescription" in q_info:
                 err_contents = [
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/kusto_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/kusto_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyParameterError, MsticpyUserConfigError
 from ...common.provider_settings import ProviderArgs, get_provider_settings
 from ...common.utility import export
 from ..core.query_defns import DataEnvironment
-from .kql_driver import KqlDriver, QuerySource
+from .kql_driver import DriverProps, KqlDriver, QuerySource
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 _KCS_CODE = "code;"
 _KCS_APP = "tenant='{tenant_id}';clientid='{client_id}';clientsecret='{clientsecret}';"
 _KCS_TEMPLATE = "azure_data-Explorer://{auth}cluster='{cluster}';database='{database}'"
@@ -42,14 +42,15 @@
         ----------------
         debug : bool
             print out additional diagnostic information.
 
         """
         super().__init__(connection_str=connection_str, **kwargs)
         self.environment = kwargs.get("data_environment", DataEnvironment.Kusto)
+        self.set_driver_property(DriverProps.EFFECTIVE_ENV, DataEnvironment.Kusto.name)
         self._connected = True
         self._kusto_settings: KustoClusterSettings = _get_kusto_settings()
         self._cluster_uri = None
 
     def connect(self, connection_str: Optional[str] = None, **kwargs):
         """
         Connect to data source.
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/local_data_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/local_data_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,15 @@
         file_path = self.data_files.get(query.casefold())
         if not file_path:
             raise FileNotFoundError(
                 f"Data file ({query}) for query {query_name} not found."
             )
         if file_path.endswith("csv"):
             try:
-                return pd.read_csv(
-                    file_path, infer_datetime_format=True, parse_dates=["TimeGenerated"]
-                )
+                return pd.read_csv(file_path, parse_dates=["TimeGenerated"])
             except ValueError:
                 return pd.read_csv(file_path)
         data_df = pd.read_pickle(file_path)  # nosec
         if isinstance(data_df, pd.DataFrame):
             return data_df
         return f"{query} is not a DataFrame ({file_path})."
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/local_osquery_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/local_osquery_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pickle  # nosec
 import re
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
-from pandas import to_datetime
+from pandas import to_datetime, to_numeric
 from tqdm.auto import tqdm
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyDataQueryError, MsticpyNoDataSourceError
 from ...common.provider_settings import get_provider_settings
 from ...common.utility import export, valid_pyname
 from .driver_base import DriverBase, QuerySource
@@ -264,17 +264,16 @@
 
     def _extract_event_type(self, df_all_queries: pd.DataFrame, event_name: str):
         """Extract tidied DF from all queries."""
         query_df = df_all_queries[df_all_queries["name"] == event_name].dropna(
             axis=1, how="all"
         )
         for date_column in self.OS_QUERY_DATEIME_COLS & set(query_df.columns):
-            query_df[date_column] = pd.to_datetime(
-                query_df[date_column],
-                unit="s",
+            query_df[date_column] = to_datetime(
+                to_numeric(query_df[date_column]),
                 origin="unix",
                 utc=True,
             )
         return query_df
 
     def _read_log_file(self, log_path: str):
         """Read log file into cache."""
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/local_velociraptor_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/local_velociraptor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/mdatp_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/mdatp_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/mordor_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/mordor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/odata_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/odata_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/resource_graph_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/resource_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/security_graph_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/security_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/sentinel_query_reader.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/sentinel_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/drivers/splunk_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/splunk_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,17 @@
 
         # default to unlimited query unless count is specified
         count = kwargs.pop("count", 0)
 
         # Get sets of N results at a time, N=100 by default
         page_size = kwargs.pop("page_size", 100)
 
+        # default to 60s unless timeout is specified
+        timeout = kwargs.pop("timeout", 60)
+
         # Normal (non-blocking) searches or oneshot (blocking) searches.
         # Defaults to Normal(non-blocking)
 
         # Oneshot is a blocking search that is scheduled to run immediately.
         # Instead of returning a search job, this mode returns the results
         # of the search once completed.
         # Because this is a blocking search, the results are not available
@@ -251,15 +254,17 @@
             resp_rows = [row for row in reader if isinstance(row, dict)]
         else:
             # Set mode and initialize async job
             kwargs_normalsearch = {"exec_mode": "normal"}
             query_job = self.service.jobs.create(
                 query, count=count, **kwargs_normalsearch
             )
-            resp_rows, reader = self._exec_async_search(query_job, page_size, **kwargs)
+            resp_rows, reader = self._exec_async_search(
+                query_job, page_size, timeout=timeout
+            )
 
         if len(resp_rows) == 0 or not resp_rows:
             print("Warning - query did not return any results.")
             return [row for row in reader if isinstance(row, sp_results.Message)]
         return pd.DataFrame(resp_rows)
 
     def query_with_results(self, query: str, **kwargs) -> Tuple[pd.DataFrame, Any]:
@@ -329,15 +334,15 @@
                     "query_paths": "SavedSearches",
                     "description": "",
                 }
                 for search in self.service.saved_searches
             ]
         return []
 
-    def _exec_async_search(self, query_job, page_size, timeout=60):
+    def _exec_async_search(self, query_job, page_size, timeout):
         """Execute an async search and return results."""
         # Initiate progress bar and start while loop, waiting for async query to complete
         progress_bar = tqdm(total=100, desc="Waiting Splunk job to complete")
         prev_progress = 0
         offset = 0  # Start at result 0
         start_time = datetime.now()
         end_time = start_time + timedelta(seconds=timeout)
```

### Comparing `msticpy-2.6.0/msticpy/data/drivers/sumologic_driver.py` & `msticpy-2.7.0rc1/msticpy/data/drivers/sumologic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_connections.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_connections.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_hosts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/cybereason/cybereason_processes.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/cybereason/cybereason_processes.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/localdata/local_data.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/localdata/local_data.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_file.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_file.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         | where SHA1 == "{file_hash}" or SHA256 == "{file_hash}" or MD5 == "{file_hash}"
         {add_query_items}'
       uri: None
     parameters:
       file_hash:
         description: Hash of file
         type: str
-        aliases: hash
+        aliases:
+          - hash
   list_file_events_for_host:
     description: Lists all file events for a host/device
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
```

### Comparing `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_network.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_network.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         {add_query_items}"
       uri: None
     parameters:
   host_connections:
-    description: Returns connections by for a specified hostname
+    description: Returns connections by a specified hostname
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
         | where {time_column} <= datetime({end})
         | where DeviceName has "{host_name}"
```

### Comparing `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_process.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/m365d/kql_m365_user.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/m365d/kql_m365_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_file.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_file.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         | where SHA1 == "{file_hash}" or SHA256 == "{file_hash}" or MD5 == "{file_hash}"
         {add_query_items}'
       uri: None
     parameters:
       file_hash:
         description: Hash of file
         type: str
-        aliases: hash
+        aliases:
+          - hash
   list_file_events_for_filename:
     description: Lists all file events by filename
     metadata:
     args:
       query: '
         {table}
         | where {time_column} >= datetime({start})
```

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_hunting.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_network.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_process.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mde/kql_mdatp_user.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mde/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/msgraph/graph_alerts.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/msgraph/graph_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_alert.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_azure.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_net.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_o365.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/resourcegraph/sentinel_resources.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_alert_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_authentication_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/splunk/splunk_queries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/splunk/splunk_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/queries/sumologic/sumologic_queries.yaml` & `msticpy-2.7.0rc1/msticpy/data/queries/sumologic/sumologic_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/query_container.py` & `msticpy-2.7.0rc1/msticpy/data/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/query_defns.py` & `msticpy-2.7.0rc1/msticpy/data/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/sql_to_kql.py` & `msticpy-2.7.0rc1/msticpy/data/sql_to_kql.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/storage/azure_blob_storage.py` & `msticpy-2.7.0rc1/msticpy/data/storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/uploaders/__init__.py` & `msticpy-2.7.0rc1/msticpy/data/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/uploaders/loganalytics_uploader.py` & `msticpy-2.7.0rc1/msticpy/data/uploaders/loganalytics_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/data/uploaders/splunk_uploader.py` & `msticpy-2.7.0rc1/msticpy/data/uploaders/splunk_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,15 @@
         if not self.connected:
             raise MsticpyConnectionError(
                 "Splunk host not connected, please call .connect before proceeding.",
                 title="Splunk host not connected",
             )
         if not host:
             host = "Upload"
-        create_idx = kwargs.get("create_index", False)
-        index = self._load_index(index_name, create_idx)
+        index = self._load_index(index_name, kwargs.get("create_index", False))
         progress = tqdm(total=len(data.index), desc="Rows", position=0)
         for row in data.iterrows():
             data = row[1].to_csv()
             try:
                 data.encode(encoding="latin-1")
             except UnicodeEncodeError:
                 data = data.encode(encoding="utf-8")
```

### Comparing `msticpy-2.6.0/msticpy/data/uploaders/uploader_base.py` & `msticpy-2.7.0rc1/msticpy/data/uploaders/uploader_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/__init__.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/account.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/account.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/alert.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/azure_resource.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/azure_resource.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/cloud_application.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/cloud_application.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/cloud_logon_session.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/cloud_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/dns.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/dns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/entity.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/entity_enums.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/entity_enums.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/entity_graph.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/entity_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/file.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/file.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/file_hash.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/file_hash.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/geo_location.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/geo_location.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/graph_property.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/graph_property.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/host.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/host.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/host_logon_session.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/host_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/iot_device.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/iot_device.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/ip_address.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/ip_address.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/mail_cluster.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/mail_cluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/mail_message.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/mail_message.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/mailbox.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/mailbox.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/malware.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/malware.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/network_connection.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/network_connection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/process.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/process.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/registry_key.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/registry_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/registry_value.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/registry_value.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/security_group.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/security_group.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/submission_mail.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/submission_mail.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/threat_intelligence.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/unknown_entity.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/unknown_entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/entities/url.py` & `msticpy-2.7.0rc1/msticpy/datamodel/entities/url.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/pivot.py` & `msticpy-2.7.0rc1/msticpy/datamodel/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/soc/incident.py` & `msticpy-2.7.0rc1/msticpy/datamodel/soc/incident.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/datamodel/soc/sentinel_alert.py` & `msticpy-2.7.0rc1/msticpy/datamodel/soc/sentinel_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/__init__.py` & `msticpy-2.7.0rc1/msticpy/init/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/azure_ml_tools.py` & `msticpy-2.7.0rc1/msticpy/init/azure_ml_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/azure_synapse_tools.py` & `msticpy-2.7.0rc1/msticpy/init/azure_synapse_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/logging.py` & `msticpy-2.7.0rc1/msticpy/init/logging.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/mp_pandas_accessors.py` & `msticpy-2.7.0rc1/msticpy/init/mp_pandas_accessors.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     """Msticpy pandas accessor for core functions."""
 
     def __init__(self, pandas_obj):
         """Initialize the extension."""
         self._df = pandas_obj
         self._ioc = IoCExtract()
 
+        self._data_viewer_class: Any = None
+
     def b64extract(self, column: str, **kwargs) -> pd.DataFrame:
         """
         Base64-decode strings taken from a pandas dataframe.
 
         Parameters
         ----------
         data : pd.DataFrame
@@ -237,7 +239,59 @@
         Returns
         -------
         pd.DataFrame
             Output DataFrame with results in added columns.
 
         """
         return get_whois_df(data=self._df, ip_column=ip_column, **kwargs)
+
+    def view(self, **kwargs):
+        """
+        Initialize the DataViewer class.
+
+        Parameters
+        ----------
+        data : pd.DataFrame
+            The DataFrame to view
+        selected_cols : List[str], optional
+            Initial subset of columns to show, by default None (all cols)
+
+        Other Parameters
+        ----------------
+        selectable : Union[bool, str], optional
+            Whether rows should be selectable, by default "checkbox"
+        show_index : bool, optional
+            If True show the DataFrame index as a column, by default  True.
+        show_tenant_id : bool, optional
+            If True show the TenantId column, by default  True.
+        max_col_width : int, optional
+            Sets the maximum column width to display, by default 500
+        detail_cols : List[str]
+            List of columns for which details are displayed in collapsible
+            field beneath each table row.
+        kwargs :
+            Other keyword arguments are passed to the panel
+            Tabulator control.
+
+        Notes
+        -----
+        Main attributes:
+        value - original dataframe
+        selected - indexes of currently selected rows
+        selected_dataframe - currently selected rows
+        current_view - current dataframe after filtering and sorting
+        selection - indexes of currently selected rows
+
+        See Also
+        --------
+        Tabulator - https://panel.holoviz.org/reference/widgets/Tabulator.html
+
+        """
+        if self._data_viewer_class is None:
+            try:
+                # pylint: disable=import-outside-toplevel
+                from ..vis.data_viewer_panel import DataViewer
+            except ImportError:
+                print("This component needs the panel package.")
+                return self._df
+            self._data_viewer_class = DataViewer
+        return self._data_viewer_class(data=self._df, **kwargs)
```

### Comparing `msticpy-2.6.0/msticpy/init/mp_plugins.py` & `msticpy-2.7.0rc1/msticpy/init/mp_plugins.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/nbinit.py` & `msticpy-2.7.0rc1/msticpy/init/nbinit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/nbmagics.py` & `msticpy-2.7.0rc1/msticpy/init/nbmagics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot.py` & `msticpy-2.7.0rc1/msticpy/init/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_browser.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_container.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_magic_core.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_magic_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_pd_accessor.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_pipeline.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_pipeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_register.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_register.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_core/pivot_register_reader.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_core/pivot_register_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_init/pivot_data_queries.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_init/pivot_data_queries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_init/pivot_ti_provider.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_init/pivot_ti_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/pivot_init/vt_pivot.py` & `msticpy-2.7.0rc1/msticpy/init/pivot_init/vt_pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/init/user_config.py` & `msticpy-2.7.0rc1/msticpy/init/user_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/__init__.py` & `msticpy-2.7.0rc1/msticpy/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/data_viewer.py` & `msticpy-2.7.0rc1/msticpy/nbtools/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/entityschema.py` & `msticpy-2.7.0rc1/msticpy/nbtools/entityschema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/foliummap.py` & `msticpy-2.7.0rc1/msticpy/nbtools/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/morph_charts.py` & `msticpy-2.7.0rc1/msticpy/nbtools/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/nbdisplay.py` & `msticpy-2.7.0rc1/msticpy/nbtools/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/nbwidgets.py` & `msticpy-2.7.0rc1/msticpy/nbtools/nbwidgets.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/observationlist.py` & `msticpy-2.7.0rc1/msticpy/nbtools/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/process_tree.py` & `msticpy-2.7.0rc1/msticpy/nbtools/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/security_alert.py` & `msticpy-2.7.0rc1/msticpy/nbtools/security_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/security_alert_graph.py` & `msticpy-2.7.0rc1/msticpy/nbtools/security_alert_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/security_base.py` & `msticpy-2.7.0rc1/msticpy/nbtools/security_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/security_event.py` & `msticpy-2.7.0rc1/msticpy/nbtools/security_event.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/ti_browser.py` & `msticpy-2.7.0rc1/msticpy/nbtools/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/timeline.py` & `msticpy-2.7.0rc1/msticpy/nbtools/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/timeline_duration.py` & `msticpy-2.7.0rc1/msticpy/nbtools/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/timeline_pd_accessor.py` & `msticpy-2.7.0rc1/msticpy/nbtools/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/timeseries.py` & `msticpy-2.7.0rc1/msticpy/nbtools/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/utility.py` & `msticpy-2.7.0rc1/msticpy/nbtools/utility.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbtools/wsconfig.py` & `msticpy-2.7.0rc1/msticpy/nbtools/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/__init__.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/core.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/get_environment_key.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/get_environment_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/get_text.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/get_text.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/lookback.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/lookback.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/option_buttons.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/option_buttons.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/progress.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/query_time.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/query_time.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/select_alert.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/select_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/select_item.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/select_item.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/nbwidgets/select_subset.py` & `msticpy-2.7.0rc1/msticpy/nbwidgets/select_subset.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/resources/WinSecurityEvent.json` & `msticpy-2.7.0rc1/msticpy/resources/WinSecurityEvent.json`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/resources/mp_pivot_reg.yaml` & `msticpy-2.7.0rc1/msticpy/resources/mp_pivot_reg.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/resources/mpconfig_defaults.yaml` & `msticpy-2.7.0rc1/msticpy/resources/mpconfig_defaults.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/resources/obfuscation_cols.yaml` & `msticpy-2.7.0rc1/msticpy/resources/obfuscation_cols.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/__init__.py` & `msticpy-2.7.0rc1/msticpy/sectools/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/auditdextract.py` & `msticpy-2.7.0rc1/msticpy/sectools/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/base64unpack.py` & `msticpy-2.7.0rc1/msticpy/sectools/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/cmd_line.py` & `msticpy-2.7.0rc1/msticpy/sectools/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/domain_utils.py` & `msticpy-2.7.0rc1/msticpy/sectools/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/eventcluster.py` & `msticpy-2.7.0rc1/msticpy/sectools/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/geoip.py` & `msticpy-2.7.0rc1/msticpy/sectools/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/iocextract.py` & `msticpy-2.7.0rc1/msticpy/sectools/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/ip_utils.py` & `msticpy-2.7.0rc1/msticpy/sectools/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/proc_tree_build_mde.py` & `msticpy-2.7.0rc1/msticpy/sectools/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/proc_tree_build_winlx.py` & `msticpy-2.7.0rc1/msticpy/sectools/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/proc_tree_builder.py` & `msticpy-2.7.0rc1/msticpy/sectools/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/proc_tree_schema.py` & `msticpy-2.7.0rc1/msticpy/sectools/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/proc_tree_utils.py` & `msticpy-2.7.0rc1/msticpy/sectools/proc_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/sectools_magics.py` & `msticpy-2.7.0rc1/msticpy/sectools/sectools_magics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/syslog_utils.py` & `msticpy-2.7.0rc1/msticpy/sectools/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/tilookup.py` & `msticpy-2.7.0rc1/msticpy/sectools/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/tiproviders/ti_provider_base.py` & `msticpy-2.7.0rc1/msticpy/sectools/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/vtlookup.py` & `msticpy-2.7.0rc1/msticpy/sectools/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/vtlookupv3/__init__.py` & `msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py` & `msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtlookupv3.py` & `msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/sectools/vtlookupv3/vtobject_browser.py` & `msticpy-2.7.0rc1/msticpy/sectools/vtlookupv3/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/auditdextract.py` & `msticpy-2.7.0rc1/msticpy/transform/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/base64unpack.py` & `msticpy-2.7.0rc1/msticpy/transform/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/cmd_line.py` & `msticpy-2.7.0rc1/msticpy/transform/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/iocextract.py` & `msticpy-2.7.0rc1/msticpy/transform/iocextract.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,17 +129,18 @@
     IPV4_DF_REGEX = r"(?P<ipaddress>(?:[0-9]{1,3}\[?\.\]?){3}[0-9]{1,3})"
     IPV6_REGEX = r"(?<![:.\w])(?:[A-F0-9]{0,4}:){2,7}[A-F0-9]{0,4}(?![:.\w])"
     DNS_REGEX = r"((?=[a-z0-9-]{1,63}\.)[a-z0-9]+(-[a-z0-9]+)*\.){1,126}[a-z]{2,63}"
     DNS_DF_REGEX = (
         r"((?=[a-z0-9-]{1,63}\[?\.\]?)[a-z0-9]+(-[a-z0-9]+)*\[?\.\]?){1,126}[a-z]{2,63}"
     )
 
-    EMAIL_USER_REGEX = r"(?P<user>[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+)(@|AT)"
-    EMAIL_REGEX = f"{EMAIL_USER_REGEX}(?P<domain>{DNS_REGEX})"
-    EMAIL_DF_REGEX = f"{EMAIL_USER_REGEX}(?P<domain>{DNS_DF_REGEX})"
+    EMAIL_USER_REGEX = r"(?P<user>[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+)"
+    EMAIL_REGEX = f"{EMAIL_USER_REGEX}@(?P<domain>{DNS_REGEX})"
+    DF_AT = r"(@|\[at\])"
+    EMAIL_DF_REGEX = f"{EMAIL_USER_REGEX}{DF_AT}(?P<domain>{DNS_DF_REGEX})"
 
     URL_REGEX = r"""
             (?P<protocol>(https?|s?ftps?|telnet|ldap|file)://)
             (?P<userinfo>([a-z0-9-._~!$&\'()*+,;=:]|%[0-9A-F]{2})*@)?
             (?P<host>([a-z0-9-._~!$&\'()*+,;=]|%[0-9A-F]{2})*)
             (:(?P<port>\d*))?
             (/(?P<path>([^?\#"<>\s]|%[0-9A-F]{2})*/?))?
@@ -171,41 +172,53 @@
             (?P<file>[^/\0<>|\r\n ]+)
     """
     MD5_REGEX = r"(?:^|[^A-Fa-f0-9])(?P<hash>[A-Fa-f0-9]{32})(?:$|[^A-Fa-f0-9])"
     SHA1_REGEX = r"(?:^|[^A-Fa-f0-9])(?P<hash>[A-Fa-f0-9]{40})(?:$|[^A-Fa-f0-9])"
     SHA256_REGEX = r"(?:^|[^A-Fa-f0-9])(?P<hash>[A-Fa-f0-9]{64})(?:$|[^A-Fa-f0-9])"
 
     _content_regex: Dict[str, IoCPattern] = {}
+    _content_df_regex: Dict[str, IoCPattern] = {}
 
     def __init__(self, defanged: bool = True):
-        """Initialize new instance of IoCExtract."""
+        """
+        Initialize new instance of IoCExtract.
+
+        Parameters
+        ----------
+        defanged : bool, optional
+            If True, the regex will be used to match defanged IoC patterns
+
+        """
         # IP Addresses
         self.add_ioc_type(
+            IoCType.ipv4.name, self.IPV4_REGEX, 0, "ipaddress", defang_pattern=False
+        )
+        self.add_ioc_type(
             IoCType.ipv4.name,
-            self.IPV4_DF_REGEX if defanged else self.IPV4_REGEX,
+            self.IPV4_DF_REGEX,
             0,
             "ipaddress",
+            defang_pattern=True,
         )
         self.add_ioc_type(IoCType.ipv6.name, self.IPV6_REGEX, 0)
 
         # Dns Domains
         # This also matches IP addresses but IPs have higher
         # priority both matching on the same substring will defer
         # to the IP regex
-        self.add_ioc_type(
-            IoCType.dns.name, self.DNS_DF_REGEX if defanged else self.DNS_REGEX, 2
-        )
+        self.add_ioc_type(IoCType.dns.name, self.DNS_REGEX, 2, defang_pattern=False)
+        self.add_ioc_type(IoCType.dns.name, self.DNS_DF_REGEX, 2, defang_pattern=True)
 
         # URLs
-        self.add_ioc_type(
-            IoCType.url.name, self.URL_DF_REGEX if defanged else self.URL_REGEX, 0
-        )
+        self.add_ioc_type(IoCType.url.name, self.URL_REGEX, 0, defang_pattern=False)
+        self.add_ioc_type(IoCType.url.name, self.URL_DF_REGEX, 0, defang_pattern=True)
         # Email addresses (lower priority than URLs)
+        self.add_ioc_type(IoCType.email.name, self.EMAIL_REGEX, 1, defang_pattern=False)
         self.add_ioc_type(
-            IoCType.email.name, self.EMAIL_DF_REGEX if defanged else self.EMAIL_REGEX, 1
+            IoCType.email.name, self.EMAIL_DF_REGEX, 1, defang_pattern=True
         )
         # File paths
         self.add_ioc_type(IoCType.windows_path.name, self.WINPATH_REGEX, 3)
         self.add_ioc_type(IoCType.linux_path.name, self.LXPATH_REGEX, 4)
 
         # MD5, SHA1, SHA256 hashes
         self.add_ioc_type(IoCType.md5_hash.name, self.MD5_REGEX, 1, "hash")
@@ -215,18 +228,24 @@
         # inline import due to circular dependency
         # pylint: disable=import-outside-toplevel
         from ..context.domain_utils import DomainValidator
 
         # pylint: enable=import-outside-toplevel
         self._dom_validator = DomainValidator()
         self._ignore_tld = False
+        self._defanged = defanged
 
     # Public members
     def add_ioc_type(
-        self, ioc_type: str, ioc_regex: str, priority: int = 0, group: str = None
+        self,
+        ioc_type: str,
+        ioc_regex: str,
+        priority: int = 0,
+        group: str = None,
+        defang_pattern: Optional[bool] = None,
     ):
         """
         Add an IoC type and regular expression to use to the built-in set.
 
         Parameters
         ----------
         ioc_type : str
@@ -235,14 +254,18 @@
             A regular expression used to search for the type
         priority : int, optional
             Priority of the regex match vs. other ioc_patterns. 0 is
             the highest priority (the default is 0).
         group : str, optional
             The regex group to match (the default is None,
             which will match on the whole expression)
+        defang_pattern : bool, optional
+            If True, the regex will be used to match defanged patterns
+            If False, the regex will be used to match non-defanged patterns
+            If None, the regex will be used to match both defanged and non-defanged patterns
 
         Notes
         -----
         Pattern priorities.
             If two IocType patterns match on the same substring, the matched
             substring is assigned to the pattern/IocType with the highest
             priority. E.g. `foo.bar.com` will match types: `dns`, `windows_path`
@@ -251,34 +274,51 @@
 
         """
         if ioc_type is None or ioc_type.strip() is None:
             raise ValueError("No value supplied for ioc_type parameter")
         if ioc_regex is None or ioc_regex.strip() is None:
             raise ValueError("No value supplied for ioc_regex parameter")
 
-        self._content_regex[ioc_type] = IoCPattern(
+        ioc_pattern = IoCPattern(
             ioc_type=ioc_type,
             comp_regex=_compile_regex(regex=ioc_regex),
             priority=priority,
             group=group,
         )
+        if not defang_pattern:
+            self._content_regex[ioc_type] = ioc_pattern
+        if defang_pattern or defang_pattern is None:
+            self._content_df_regex[ioc_type] = ioc_pattern
 
     @property
     def ioc_types(self) -> dict:
         """
         Return the current set of IoC types and regular expressions.
 
         Returns
         -------
         dict
             dict of IoC Type names and regular expressions
 
         """
         return self._content_regex
 
+    @property
+    def ioc_df_types(self) -> dict:
+        """
+        Return current set of IoC types and regular expressions for defanged IoCs.
+
+        Returns
+        -------
+        dict
+            dict of IoC Type names and regular expressions
+
+        """
+        return self._content_df_regex
+
     # pylint: disable=too-many-locals
     def extract(
         self,
         src: str = None,
         data: pd.DataFrame = None,
         columns: List[str] = None,
         **kwargs,
@@ -309,16 +349,16 @@
             and 'linux_path'). If `ioc_types` is specified
             this parameter is ignored.
         ignore_tlds : bool, optional
             If True, ignore the official Top Level Domains
             list when determining whether a domain name is
             a legal domain.
         defanged : bool, optional
-            If False will remove any [] from email, dns and ip
-            entities.
+            If True will match defanged versions of from email, dns,
+            url and ip entities.
 
         Returns
         -------
         Any
             dict of found observables (if input is a string) or
             DataFrame of observables
 
@@ -343,18 +383,18 @@
 
         """
         check_kwargs(kwargs, ["ioc_types", "include_paths", "ignore_tlds", "defanged"])
         ioc_types = kwargs.get("ioc_types")
         include_paths = kwargs.get("include_paths", False)
         ignore_tld_current = self._ignore_tld
         self._ignore_tld = kwargs.get("ignore_tlds", False)
-        defanged = kwargs.get("defanged", True)
+        defanged = kwargs.get("defanged", self._defanged)
 
         if src and src.strip():
-            return self._scan_for_iocs(src=src, ioc_types=ioc_types, defang=defanged)
+            return self._scan_for_iocs(src=src, ioc_types=ioc_types, defanged=defanged)
 
         if data is None:
             raise ValueError("No source data was supplied to extract")
 
         if columns is None:
             raise ValueError("No values were supplied for the columns parameter")
 
@@ -423,14 +463,17 @@
             (the default is false - excludes 'windows_path'
             and 'linux_path'). If `ioc_types` is specified
             this parameter is ignored.
         ignore_tlds : bool, optional
             If True, ignore the official Top Level Domains
             list when determining whether a domain name is
             a legal domain.
+        defanged : bool, optional
+            If True will match defanged versions of from email, dns,
+            url and ip entities.
 
         Returns
         -------
         pd.DataFrame
             DataFrame of observables
 
         Notes
@@ -452,15 +495,15 @@
 
         """
         check_kwargs(kwargs, ["ioc_types", "include_paths", "ignore_tlds", "defanged"])
         ioc_types = kwargs.get("ioc_types")
         include_paths = kwargs.get("include_paths", False)
         ignore_tld_current = self._ignore_tld
         self._ignore_tld = kwargs.get("ignore_tlds", False)
-        defanged = kwargs.get("defanged", False)
+        defanged = kwargs.get("defanged", self._defanged)
 
         ioc_types_to_use = self._get_ioc_types_to_use(ioc_types, include_paths)
         if isinstance(columns, str):
             columns = [columns]
         col_set = set(columns)
         if col_set > set(data.columns):
             missing_cols = [elem for elem in col_set if elem not in data.columns]
@@ -480,38 +523,45 @@
     def _get_ioc_types_to_use(
         self, ioc_types: Optional[List[str]], include_paths: bool
     ) -> List[str]:
         # Use only requested IoC Type patterns
         if ioc_types:
             ioc_types_to_use = list(set(ioc_types))
         else:
-            ioc_types_to_use = list(set(self._content_regex.keys()))
+            ioc_types_to_use = list(set(self.ioc_types.keys()))
             # don't include linux paths unless explicitly included
             ioc_types_to_use.remove(IoCType.linux_path.name)
             if not include_paths:
                 # windows path matching is less noisy
                 ioc_types_to_use.remove(IoCType.windows_path.name)
         return ioc_types_to_use
 
     def validate(
-        self, input_str: str, ioc_type: str, ignore_tlds: bool = False
+        self,
+        input_str: str,
+        ioc_type: str,
+        ignore_tlds: bool = False,
+        defanged: Optional[bool] = None,
     ) -> bool:
         """
         Check that `input_str` matches the regex for the specified `ioc_type`.
 
         Parameters
         ----------
         input_str : str
             the string to test
         ioc_type : str
             the regex pattern to use
         ignore_tlds : bool, optional
             If True, ignore the official Top Level Domains
             list when determining whether a domain name is
             a legal domain.
+        defanged : bool, optional
+            If True, the input string will also match
+            defanged versions of the IoC, default is False.
 
         Returns
         -------
         bool
             True if match.
 
         """
@@ -519,20 +569,24 @@
         self._ignore_tld = ignore_tlds
         if ioc_type == IoCType.file_hash.name:
             val_type = self.file_hash_type(input_str).name
         elif ioc_type == IoCType.hostname.name:
             val_type = "dns"
         else:
             val_type = ioc_type
-        if val_type not in self._content_regex:
+        if val_type not in self.ioc_types:
             raise KeyError(
                 f"Unknown type {ioc_type}.",
-                f"Valid types are: {list(self._content_regex.keys())}",
+                f"Valid types are: {list(self.ioc_types.keys())}",
             )
-        rgx = self._content_regex[val_type]
+        use_defanged = defanged if defanged is not None else self._defanged
+        if use_defanged:
+            rgx = self._content_df_regex[val_type]
+        else:
+            rgx = self._content_regex[val_type]
         pattern_match = rgx.comp_regex.fullmatch(input_str)
         validated = self._validate_tld(input_str) if val_type == "dns" else True
         self._ignore_tld = ignore_tld_current
         return pattern_match and validated
 
     @staticmethod
     def file_hash_type(file_hash: str) -> IoCType:
@@ -569,50 +623,49 @@
 
         Returns
         -------
         str
             The IoC type enumeration (unknown, if no match)
 
         """
-        results = self._scan_for_iocs(src=observable)
-
-        if not results:
-            results = self._scan_for_iocs(
-                src=observable, ioc_types=[IoCType.linux_path.name]
-            )
+        results = self._scan_for_iocs(src=observable) or self._scan_for_iocs(
+            src=observable, ioc_types=[IoCType.linux_path.name]
+        )
         if not results:
             return IoCType.unknown.name
 
-        # we need to select the type that is an exact match for the whole
-        # observable string (_scan_for_iocs will return matching substrings)
-        for ioc_type, match_set in results.items():
-            if observable in match_set:
-                return ioc_type
-
-        return IoCType.unknown.name
+        return next(
+            (
+                ioc_type
+                for ioc_type, match_set in results.items()
+                if observable in match_set
+            ),
+            IoCType.unknown.name,
+        )
 
     # Private methods
     def _validate_tld(self, domain: str) -> bool:
         """If validate TLDS check with TLD list."""
         if self._ignore_tld:
             return True
         return self._dom_validator.validate_tld(domain.replace("[.]", "."))
 
     def _scan_for_iocs(
         self,
         src: str,
         ioc_types: List[str] = None,
-        defang: bool = True,
+        defanged: bool = True,
     ) -> Dict[str, Set[str]]:
         """Return IoCs found in the string."""
         ioc_results: Dict[str, Set] = defaultdict(set)
         iocs_found: Dict[str, Tuple[str, int]] = {}
 
         # pylint: disable=too-many-nested-blocks
-        for ioc_type, rgx_def in self._content_regex.items():
+        ioc_regexes = self._content_df_regex if defanged else self._content_regex
+        for ioc_type, rgx_def in ioc_regexes.items():
             if ioc_types and ioc_type not in ioc_types:
                 continue
 
             match_pos = 0
             for rgx_match in rgx_def.comp_regex.finditer(src, match_pos):
                 if rgx_match is None:
                     break
@@ -628,30 +681,36 @@
 
                 self._add_highest_pri_match(iocs_found, match_str, rgx_def)
                 if ioc_type == "url":
                     self._check_decode_url(match_str, rgx_def, match_pos, iocs_found)
                 match_pos = rgx_match.end()
 
         for ioc, ioc_result in iocs_found.items():
-            if not defang and ioc_result[0] in ["ipv4", "ipv6", "url", "dns", "email"]:
+            if not defanged and ioc_result[0] in [
+                "ipv4",
+                "ipv6",
+                "url",
+                "dns",
+                "email",
+            ]:
                 ioc = refang_ioc(ioc, ioc_result[0])
             ioc_results[ioc_result[0]].add(ioc)
 
         return ioc_results
 
     def _check_decode_url(self, match_str, rgx_def, match_pos, iocs_found):
         """Get any other IoCs from decoded URL."""
         decoded_url = unquote(match_str)
         for url_match in rgx_def.comp_regex.finditer(decoded_url, match_pos):
             if url_match is not None:
                 self._add_highest_pri_match(iocs_found, url_match.group(), rgx_def)
                 self._add_highest_pri_match(
                     iocs_found,
                     url_match.groupdict()["host"],
-                    self._content_regex["dns"],
+                    self._content_df_regex["dns"],
                 )
 
     @staticmethod
     def _add_highest_pri_match(
         iocs_found: dict, current_match: str, current_def: IoCPattern
     ):
         # if we already found a match for this item and the previous
```

### Comparing `msticpy-2.6.0/msticpy/transform/network.py` & `msticpy-2.7.0rc1/msticpy/transform/network.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/proc_tree_build_mde.py` & `msticpy-2.7.0rc1/msticpy/transform/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/proc_tree_build_winlx.py` & `msticpy-2.7.0rc1/msticpy/transform/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/proc_tree_builder.py` & `msticpy-2.7.0rc1/msticpy/transform/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/proc_tree_schema.py` & `msticpy-2.7.0rc1/msticpy/transform/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/transform/process_tree_utils.py` & `msticpy-2.7.0rc1/msticpy/transform/process_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/__init__.py` & `msticpy-2.7.0rc1/msticpy/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/code_view.py` & `msticpy-2.7.0rc1/msticpy/vis/code_view.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/data_viewer.py` & `msticpy-2.7.0rc1/msticpy/vis/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/data_viewer_panel.py` & `msticpy-2.7.0rc1/msticpy/vis/data_viewer_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             Other keyword arguments are passed to the panel
             Tabulator control.
 
         Notes
         -----
         Main attributes:
         value - original dataframe
+        selected - indexes of currently selected rows
         selected_dataframe - currently selected rows
         current_view - current dataframe after filtering and sorting
         selection - indexes of currently selected rows
 
         See Also
         --------
         Tabulator - https://panel.holoviz.org/reference/widgets/Tabulator.html
```

### Comparing `msticpy-2.6.0/msticpy/vis/entity_graph_tools.py` & `msticpy-2.7.0rc1/msticpy/vis/entity_graph_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Creates an entity graph for a Microsoft Sentinel Incident."""
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import List, Optional, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from bokeh.io import output_notebook, show
 from bokeh.layouts import column
 from bokeh.models import Circle, HoverTool, Label, LayoutDOM  # type: ignore
 from bokeh.plotting import figure, from_networkx
+from dateutil import parser
 
 from .._version import VERSION
 from ..common.exceptions import MsticpyUserError
 from ..common.utility import export
 from ..datamodel.entities import Entity
 from ..datamodel.entities.alert import Alert
 from ..datamodel.soc.incident import Incident
@@ -131,25 +132,26 @@
         LayoutDOM
             A Bokeh figure object
 
         """
         timeline = None
         tl_df = self.to_df()
         tl_type = "duration"
+        # pylint: disable=unsubscriptable-object
         if len(tl_df["EndTime"].unique()) == 1 and not tl_df["EndTime"].unique()[0]:
             tl_type = "discreet"
             if (
                 len(tl_df["TimeGenerated"].unique()) == 1
                 and not tl_df["TimeGenerated"].unique()[0]
             ):
                 print("No timestamps available to create timeline")
                 return self._plot_no_timeline(timeline=False, hide=hide, **kwargs)
-        tl_df["TimeGenerated"] = pd.to_datetime(tl_df["TimeGenerated"], utc=True)
-        tl_df["StartTime"] = pd.to_datetime(tl_df["StartTime"], utc=True)
-        tl_df["EndTime"] = pd.to_datetime(tl_df["EndTime"], utc=True)
+        # tl_df["TimeGenerated"] = pd.to_datetime(tl_df["TimeGenerated"], utc=True)
+        # tl_df["StartTime"] = pd.to_datetime(tl_df["StartTime"], utc=True)
+        # tl_df["EndTime"] = pd.to_datetime(tl_df["EndTime"], utc=True)
         graph = self._plot_no_timeline(hide=True, **kwargs)
         if tl_type == "duration":
             timeline = display_timeline_duration(
                 tl_df.dropna(subset=["TimeGenerated"]),
                 group_by="Name",
                 title="Entity Timeline",
                 time_column="StartTime",
@@ -316,43 +318,28 @@
         if name in self.alertentity_graph.nodes():
             self.alertentity_graph.remove_node(name)
         else:
             raise MsticpyUserError(f"Node named {name} not found")
 
     def to_df(self) -> pd.DataFrame:
         """Generate a dataframe of nodes in the graph."""
-        names = [node[1]["Name"] for node in self.alertentity_graph.nodes.items()]
-        descs = [
-            node[1]["Description"] for node in self.alertentity_graph.nodes.items()
-        ]
-        types = [node[1]["Type"] for node in self.alertentity_graph.nodes.items()]
-        times = [
-            node[1]["TimeGenerated"] if "TimeGenerated" in node[1] else None
-            for node in self.alertentity_graph.nodes.items()
-        ]
-        starttimes = [
-            node[1]["StartTime"] if "StartTime" in node[1] else node[1]["TimeGenerated"]
-            for node in self.alertentity_graph.nodes.items()
-        ]
-        endtimes = [
-            node[1]["EndTime"] if "EndTime" in node[1] else None
-            for node in self.alertentity_graph.nodes.items()
-        ]
-        tl_df = pd.DataFrame(
+        node_list = [
             {
-                "Name": names,
-                "Description": descs,
-                "Type": types,
-                "TimeGenerated": times,
-                "EndTime": endtimes,
-                "StartTime": starttimes,
+                "Name": node.get("Name"),
+                "Description": node.get("Description"),
+                "Type": node.get("Type"),
+                "TimeGenerated": _convert_to_tz_aware_ts(node.get("TimeGenerated")),
+                "EndTime": _convert_to_tz_aware_ts(node.get("EndTime")),
+                "StartTime": _convert_to_tz_aware_ts(
+                    node.get("StartTime", node.get("TimeGenerated"))
+                ),
             }
-        )
-        tl_df.replace("None", np.NaN, inplace=True)
-        return tl_df
+            for node in self.alertentity_graph.nodes.values()
+        ]
+        return pd.DataFrame(node_list).replace("None", np.NaN)
 
     def _add_incident_or_alert_node(self, incident: Union[Incident, Alert, None]):
         """Check what type of entity is passed in and creates relevant graph."""
         if isinstance(incident, Incident):
             self._add_incident_node(incident)
         elif isinstance(incident, Alert):
             self._add_alert_node(incident)
@@ -398,14 +385,24 @@
 
     @property
     def graph(self) -> nx.Graph:
         """Return the raw NetworkX graph."""
         return self.alertentity_graph
 
 
+def _convert_to_tz_aware_ts(date_string: Optional[str]) -> Optional[datetime]:
+    """Convert a date string to a timezone aware datetime object."""
+    if date_string is None:
+        return None
+    date_time = parser.parse(date_string)
+    if date_time.tzinfo is None:
+        return date_time.replace(tzinfo=timezone.utc)
+    return date_time
+
+
 def _dedupe_entities(alerts, ents) -> list:
     """Deduplicate incident and alert entities."""
     alert_entities = []
     for alert in alerts:
         if alert["Entities"]:
             alert_entities += [hash(ent) for ent in alert["Entities"]]
     for ent in ents:
```

### Comparing `msticpy-2.6.0/msticpy/vis/figure_dimension.py` & `msticpy-2.7.0rc1/msticpy/vis/figure_dimension.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/foliummap.py` & `msticpy-2.7.0rc1/msticpy/vis/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/matrix_plot.py` & `msticpy-2.7.0rc1/msticpy/vis/matrix_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/mordor_browser.py` & `msticpy-2.7.0rc1/msticpy/vis/mordor_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/morph_charts.py` & `msticpy-2.7.0rc1/msticpy/vis/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/mp_pandas_plot.py` & `msticpy-2.7.0rc1/msticpy/vis/mp_pandas_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/nbdisplay.py` & `msticpy-2.7.0rc1/msticpy/vis/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/network_plot.py` & `msticpy-2.7.0rc1/msticpy/vis/network_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/process_tree.py` & `msticpy-2.7.0rc1/msticpy/vis/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/query_browser.py` & `msticpy-2.7.0rc1/msticpy/vis/query_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/ti_browser.py` & `msticpy-2.7.0rc1/msticpy/vis/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeline.py` & `msticpy-2.7.0rc1/msticpy/vis/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeline_common.py` & `msticpy-2.7.0rc1/msticpy/vis/timeline_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeline_duration.py` & `msticpy-2.7.0rc1/msticpy/vis/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeline_pd_accessor.py` & `msticpy-2.7.0rc1/msticpy/vis/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeline_values.py` & `msticpy-2.7.0rc1/msticpy/vis/timeline_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/timeseries.py` & `msticpy-2.7.0rc1/msticpy/vis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy/vis/vtobject_browser.py` & `msticpy-2.7.0rc1/msticpy/vis/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/msticpy.egg-info/PKG-INFO` & `msticpy-2.7.0rc1/msticpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.6.0
+Version: 2.7.0rc1
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
```

### Comparing `msticpy-2.6.0/msticpy.egg-info/SOURCES.txt` & `msticpy-2.7.0rc1/msticpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 msticpy/config/ce_user_defaults.py
 msticpy/config/comp_edit.py
 msticpy/config/compound_ctrls.py
 msticpy/config/file_browser.py
 msticpy/config/mp_config_control.py
 msticpy/config/mp_config_edit.py
 msticpy/config/mp_config_file.py
+msticpy/config/query_editor.py
 msticpy/context/__init__.py
 msticpy/context/contextlookup.py
 msticpy/context/domain_utils.py
 msticpy/context/geoip.py
 msticpy/context/http_provider.py
 msticpy/context/ip_utils.py
 msticpy/context/lookup.py
@@ -107,16 +108,18 @@
 msticpy/context/azure/sentinel_watchlists.py
 msticpy/context/azure/sentinel_workspaces.py
 msticpy/context/contextproviders/__init__.py
 msticpy/context/contextproviders/context_provider_base.py
 msticpy/context/contextproviders/http_context_provider.py
 msticpy/context/contextproviders/servicenow.py
 msticpy/context/tiproviders/__init__.py
+msticpy/context/tiproviders/abuseipdb.py
 msticpy/context/tiproviders/alienvault_otx.py
 msticpy/context/tiproviders/azure_sent_byoti.py
+msticpy/context/tiproviders/crowdsec.py
 msticpy/context/tiproviders/greynoise.py
 msticpy/context/tiproviders/ibm_xforce.py
 msticpy/context/tiproviders/intsights.py
 msticpy/context/tiproviders/kql_base.py
 msticpy/context/tiproviders/mblookup.py
 msticpy/context/tiproviders/open_page_rank.py
 msticpy/context/tiproviders/pulsedive.py
@@ -175,14 +178,15 @@
 msticpy/data/queries/cybereason/cybereason_connections.yaml
 msticpy/data/queries/cybereason/cybereason_hosts.yaml
 msticpy/data/queries/cybereason/cybereason_processes.yaml
 msticpy/data/queries/localdata/local_data.yaml
 msticpy/data/queries/m365d/kql_m365_alerts.yaml
 msticpy/data/queries/m365d/kql_m365_file.yaml
 msticpy/data/queries/m365d/kql_m365_hunting.yaml
+msticpy/data/queries/m365d/kql_m365_identity.yaml
 msticpy/data/queries/m365d/kql_m365_network.yaml
 msticpy/data/queries/m365d/kql_m365_process.yaml
 msticpy/data/queries/m365d/kql_m365_user.yaml
 msticpy/data/queries/mde/kql_mdatp_alerts.yaml
 msticpy/data/queries/mde/kql_mdatp_file.yaml
 msticpy/data/queries/mde/kql_mdatp_hunting.yaml
 msticpy/data/queries/mde/kql_mdatp_network.yaml
```

### Comparing `msticpy-2.6.0/msticpy.egg-info/requires.txt` & `msticpy-2.7.0rc1/msticpy.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 attrs>=18.2.0
 azure-common>=1.1.18
 azure-core>=1.24.0
 azure-identity>=1.10.0
+azure-keyvault-secrets>=4.0.0
+azure-kusto-data<=5.0.0,>=4.0.0
+azure-mgmt-keyvault>=2.0.0
 azure-mgmt-subscription>=3.0.0
+azure-monitor-query<=2.0.0,>=1.0.0
 beautifulsoup4>=4.0.0
 bokeh<4.0.0,>=1.4.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython<3.0.0,>=2.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.1
+httpx<1.0.0,>=0.23.0
 html5lib
 ipywidgets<9.0.0,>=7.4.2
-KqlmagicCustom[auth_code_clipboard,jupyter-basic]>=0.1.114.post22
+keyring>=13.2.1
 lxml>=4.6.5
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4
-pandas<2.0.0,>=1.4.0
+pandas<3.0.0,>=1.4.0
+pydantic<2.0.0,>=1.8.0
 pygments>=2.0.0
 pyjwt>=2.3.0
 python-dateutil>=2.8.1
 pytz>=2019.2
 pyyaml>=3.13
 setuptools>=40.6.3
 tldextract>=2.2.2
@@ -47,26 +52,21 @@
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-storage-blob>=12.5.0
 azure-mgmt-resourcegraph>=8.0.0
 
 [all]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
-keyring>=13.2.1
 matplotlib>=3.0.0
 mo-sql-parsing<9.0.0,>=8
 nest_asyncio>=1.4.0
 openpyxl>=3.0
 panel>=0.14.4
 passivetotal>=2.5.3
 scikit-learn>=1.0.0
@@ -75,59 +75,42 @@
 statsmodels>=0.11.1
 sumologic-sdk>=0.1.11
 vt-graph-api>=2.0
 vt-py>=0.6.1
 
 [azsentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
-keyring>=13.2.1
 
 [azure]
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
-keyring>=13.2.1
 
 [azure_query]
-azure-kusto-data>=4.0.0
-azure-monitor-query>=1.0.0
 
 [azuresentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
-keyring>=13.2.1
 
 [dev]
 aiohttp>=3.7.4
 async-cache>=1.1.1
 bandit>=1.7.0
 beautifulsoup4>=4.0.0
 black>=20.8b1
@@ -137,15 +120,15 @@
 flake8>=3.8.4
 isort>=5.10.1
 markdown>=3.3.4
 mccabe>=0.6.1
 mypy>=0.812
 nbdime>=2.1.0
 nbconvert>=6.1.0
-pandas<2.0.0,>=1.4.0
+pandas<3.0.0,>=1.4.0
 pep8-naming>=0.10.0
 pep8>=1.7.1
 pipreqs>=0.4.9
 pre-commit>=2.7.1
 pycodestyle>=2.6.0
 pydocstyle>=6.0.0
 pyflakes>=2.2.0
@@ -160,17 +143,14 @@
 responses>=0.13.2
 respx>=0.20.1
 sphinx-rtd-theme>=1.0.0
 sphinx>=5.0.1
 types-attrs>=19.0.0
 
 [keyvault]
-azure-keyvault-secrets>=4.0.0
-azure-mgmt-keyvault>=2.0.0
-keyring>=13.2.1
 
 [kql]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 
 [ml]
 scikit-learn>=1.0.0
 scipy>=1.1.0
@@ -181,26 +161,21 @@
 panel>=0.14.4
 
 [riskiq]
 passivetotal>=2.5.3
 
 [sentinel]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
-keyring>=13.2.1
 
 [splunk]
 splunk-sdk>=1.6.0
 
 [sql2kql]
 mo-sql-parsing<9.0.0,>=8
 
@@ -208,44 +183,39 @@
 sumologic-sdk>=0.1.11
 openpyxl>=3.0
 
 [test]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 aiohttp>=3.7.4
 async-cache>=1.1.1
-azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
-azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
-azure-monitor-query>=1.0.0
 azure-storage-blob>=12.5.0
 bandit>=1.7.0
 beautifulsoup4>=4.0.0
 black>=20.8b1
 coverage>=5.5
 docutils<0.20.0
 filelock>=3.0.0
 flake8>=3.8.4
 isort>=5.10.1
-keyring>=13.2.1
 markdown>=3.3.4
 matplotlib>=3.0.0
 mccabe>=0.6.1
 mo-sql-parsing<9.0.0,>=8
 mypy>=0.812
 nbconvert>=6.1.0
 nbdime>=2.1.0
 nest_asyncio>=1.4.0
 openpyxl>=3.0
-pandas<2.0.0,>=1.4.0
+pandas<3.0.0,>=1.4.0
 panel>=0.14.4
 passivetotal>=2.5.3
 pep8-naming>=0.10.0
 pep8>=1.7.1
 pipreqs>=0.4.9
 pre-commit>=2.7.1
 pycodestyle>=2.6.0
```

### Comparing `msticpy-2.6.0/requirements-all.txt` & `msticpy-2.7.0rc1/requirements-all.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 attrs>=18.2.0
 azure-common>=1.1.18
 azure-core>=1.24.0
 azure-identity>=1.10.0
 azure-keyvault-secrets>=4.0.0
-azure-kusto-data>=4.0.0
+azure-kusto-data>=4.0.0, <=5.0.0
 azure-mgmt-compute>=4.6.2
 azure-mgmt-core>=1.2.1
 azure-mgmt-keyvault>=2.0.0
 azure-mgmt-monitor>=2.0.0
 azure-mgmt-network>=2.7.0
 azure-mgmt-resource>=16.1.0
 azure-mgmt-resourcegraph>=8.0.0
 azure-mgmt-subscription>=3.0.0
-azure-monitor-query>=1.0.0
+azure-monitor-query>=1.0.0, <=2.0.0
 azure-storage-blob>=12.5.0
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <4.0.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.1
+httpx>=0.23.0, <1.0.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <9.0.0
 keyring>=13.2.1
-KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 lxml>=4.6.5
 matplotlib>=3.0.0
 mo-sql-parsing>=8, <9.0.0
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4  # pandas
 openpyxl>=3.0
-pandas>=1.4.0, <2.0.0
+pandas>=1.4.0, <3.0.0
 panel>=0.14.4
 passivetotal>=2.5.3
+pydantic>=1.8.0, <2.0.0
 pygments>=2.0.0
 pyjwt>=2.3.0
 python-dateutil>=2.8.1  # pandas
 pytz>=2019.2  # pandas
 pyyaml>=3.13
 scikit-learn>=1.0.0
 scipy>=1.1.0
```

### Comparing `msticpy-2.6.0/requirements-dev.txt` & `msticpy-2.7.0rc1/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 flake8>=3.8.4
 isort>=5.10.1
 markdown>=3.3.4
 mccabe>=0.6.1
 mypy>=0.812
 nbdime>=2.1.0
 nbconvert>=6.1.0
-pandas>=1.4.0, <2.0.0
+pandas>=1.4.0, <3.0.0
 pep8-naming>=0.10.0
 pep8>=1.7.1
 pipreqs>=0.4.9
 pre-commit>=2.7.1
 pycodestyle>=2.6.0
 pydocstyle>=6.0.0
 pyflakes>=2.2.0
```

### Comparing `msticpy-2.6.0/requirements.txt` & `msticpy-2.7.0rc1/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 attrs>=18.2.0
 azure-common>=1.1.18
 azure-core>=1.24.0
 azure-identity>=1.10.0
+azure-keyvault-secrets>=4.0.0
+azure-kusto-data>=4.0.0, <=5.0.0
+azure-mgmt-keyvault>=2.0.0
 azure-mgmt-subscription>=3.0.0
+azure-monitor-query>=1.0.0, <=2.0.0
 beautifulsoup4>=4.0.0
 bokeh>=1.4.0, <4.0.0
 cryptography>=3.1
 deprecated>=1.2.4
 dnspython>=2.0.0, <3.0.0
 folium>=0.9.0
 geoip2>=2.9.0
-httpx==0.24.1
+httpx>=0.23.0, <1.0.0
 html5lib
 ipython >= 7.1.1; python_version < "3.8"
 ipython >= 7.23.1; python_version >= "3.8"
 ipywidgets>=7.4.2, <9.0.0
-KqlmagicCustom[jupyter-basic,auth_code_clipboard]>=0.1.114.post22
+keyring>=13.2.1
 lxml>=4.6.5
 msal>=1.12.0
 msal_extensions>=0.3.0
 msrest>=0.6.0
 msrestazure>=0.6.0
 nest_asyncio>=1.4.0
 networkx>=2.2
 numpy>=1.15.4  # pandas
-pandas>=1.4.0, <2.0.0
+pandas>=1.4.0, <3.0.0
+pydantic>=1.8.0, <2.0.0
 pygments>=2.0.0
 pyjwt>=2.3.0
 python-dateutil>=2.8.1  # pandas
 pytz>=2019.2  # pandas
 pyyaml>=3.13
 setuptools>=40.6.3
 tldextract>=2.2.2
```

### Comparing `msticpy-2.6.0/setup.cfg` & `msticpy-2.7.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `msticpy-2.6.0/setup.py` & `msticpy-2.7.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Setup script for msticpy."""
+
 import re
 
 import setuptools
 
 with open("msticpy/_version.py", "r", encoding="utf-8") as fd:
     v_match = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE)
-    __version__ = v_match.group(1) if v_match else "no version"
+    __version__ = v_match[1] if v_match else "no version"
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     INSTALL_REQUIRES = fh.readlines()
 
 with open("requirements-dev.txt", "r", encoding="utf-8") as fh:
     INSTALL_DEV_REQUIRES = fh.readlines()
 
@@ -37,23 +38,16 @@
         "azure-mgmt-core>=1.2.1",
         "azure-mgmt-monitor>=2.0.0",
         "azure-mgmt-network>=2.7.0",
         "azure-mgmt-resource>=16.1.0",
         "azure-storage-blob>=12.5.0",
         "azure-mgmt-resourcegraph>=8.0.0",
     ],
-    "azure_query": [
-        "azure-kusto-data>=4.0.0",
-        "azure-monitor-query>=1.0.0",
-    ],
-    "keyvault": [
-        "azure-keyvault-secrets>=4.0.0",
-        "azure-mgmt-keyvault>=2.0.0",
-        "keyring>=13.2.1",  # needed by Key Vault package
-    ],
+    "azure_query": [],
+    "keyvault": [],
     "ml": [
         "scikit-learn>=1.0.0",
         "scipy>=1.1.0",
         "statsmodels>=0.11.1",
         "matplotlib>=3.0.0",
     ],
     "sql2kql": ["mo-sql-parsing>=8, <9.0.0"],
```

