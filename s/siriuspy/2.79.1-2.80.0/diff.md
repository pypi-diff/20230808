# Comparing `tmp/siriuspy-2.79.1.tar.gz` & `tmp/siriuspy-2.80.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.79.1.tar", last modified: Tue Aug  1 18:59:56 2023, max compression
+gzip compressed data, was "siriuspy-2.80.0.tar", last modified: Tue Aug  8 13:27:30 2023, max compression
```

## Comparing `siriuspy-2.79.1.tar` & `siriuspy-2.80.0.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-08-01 18:59:48.000000 siriuspy-2.79.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-08-01 18:59:48.000000 siriuspy-2.79.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-01 18:59:56.740632 siriuspy-2.79.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-01 18:59:48.000000 siriuspy-2.79.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-01 18:59:48.000000 siriuspy-2.79.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 18:59:56.740632 siriuspy-2.79.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-08-01 18:59:48.000000 siriuspy-2.79.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    49080 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   124502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.716632 siriuspy-2.79.1/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/afc_acq_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    40718 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    19400 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51455 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    46088 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/fofb_acq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36084 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8522 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    25271 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    24724 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    70231 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/gensumm_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/savedata_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    17480 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33336 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2433 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3886 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5018 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-08-08 13:27:17.000000 siriuspy-2.80.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-08-08 13:27:17.000000 siriuspy-2.80.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-08 13:27:30.751659 siriuspy-2.80.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-08 13:27:17.000000 siriuspy-2.80.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-08 13:27:17.000000 siriuspy-2.80.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 13:27:30.751659 siriuspy-2.80.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-08-08 13:27:17.000000 siriuspy-2.80.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.715658 siriuspy-2.80.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.715658 siriuspy-2.80.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.715658 siriuspy-2.80.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.719658 siriuspy-2.80.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9600 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.719658 siriuspy-2.80.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49080 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   124502 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.719658 siriuspy-2.80.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.723658 siriuspy-2.80.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.723658 siriuspy-2.80.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.723658 siriuspy-2.80.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/afc_acq_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12787 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40718 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14051 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19405 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51455 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46088 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/fofb_acq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38555 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36084 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8522 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25271 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.727658 siriuspy-2.80.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.731658 siriuspy-2.80.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16681 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25927 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70811 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/gensumm_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/savedata_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.735659 siriuspy-2.80.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.739658 siriuspy-2.80.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.739658 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.739658 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.739658 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.739658 siriuspy-2.80.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.743659 siriuspy-2.80.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17480 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.743659 siriuspy-2.80.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.743659 siriuspy-2.80.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.743659 siriuspy-2.80.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.743659 siriuspy-2.80.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20613 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33336 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-08-08 13:27:17.000000 siriuspy-2.80.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.715658 siriuspy-2.80.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-08 13:27:30.000000 siriuspy-2.80.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.747659 siriuspy-2.80.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2433 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3886 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:30.751659 siriuspy-2.80.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5018 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-08-08 13:27:17.000000 siriuspy-2.80.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.79.1/LICENSE` & `siriuspy-2.80.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/PKG-INFO` & `siriuspy-2.80.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.79.1
+Version: 2.80.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.79.1/README.md` & `siriuspy-2.80.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/setup.py` & `siriuspy-2.80.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/__init__.py` & `siriuspy-2.80.0/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/commands.py` & `siriuspy-2.80.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/constants.py` & `siriuspy-2.80.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/entities.py` & `siriuspy-2.80.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/exceptions.py` & `siriuspy-2.80.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/serial.py` & `siriuspy-2.80.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/bsmp/types.py` & `siriuspy-2.80.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/callbacks.py` & `siriuspy-2.80.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientarch/client.py` & `siriuspy-2.80.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientarch/devices.py` & `siriuspy-2.80.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientarch/exceptions.py` & `siriuspy-2.80.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientarch/pvarch.py` & `siriuspy-2.80.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientarch/time.py` & `siriuspy-2.80.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import _templates
 
 
 class ConfigDBClient:
     """Perform operation on configuration database."""
 
-    _TIMEOUT_DEFAULT = 2.0
+    _TIMEOUT_DEFAULT = 30.0
     _INVALID_CHARACTERS = '\\/:;,?!$'
 
     def __init__(self, url=None, config_type=None):
         """Class constructor.
 
         Parameters
         ----------
```

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.80.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/clientweb/implementation.py` & `siriuspy-2.80.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/csdev.py` & `siriuspy-2.80.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/currinfo/csdev.py` & `siriuspy-2.80.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.80.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/currinfo/main.py` & `siriuspy-2.80.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/__init__.py` & `siriuspy-2.80.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.80.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/conn.py` & `siriuspy-2.80.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.80.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.80.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/main.py` & `siriuspy-2.80.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/cycle/util.py` & `siriuspy-2.80.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/__init__.py` & `siriuspy-2.80.0/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/afc_acq_core.py` & `siriuspy-2.80.0/siriuspy/devices/afc_acq_core.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/bbb.py` & `siriuspy-2.80.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/blctrl.py` & `siriuspy-2.80.0/siriuspy/devices/modltr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,94 @@
-"""Beamline Control."""
+"""LI PU device."""
+
+import time as _time
 
 from .device import DeviceNC as _DeviceNC
+from ..csdev import Const as _Const
+
 
+class LIModltr(_DeviceNC):
+    """LI LLRF."""
 
-class BLPPSCtrl(_DeviceNC):
-    """Beamline Control."""
+    DEF_TIMEOUT = 10  # [s]
 
     class DEVICES:
         """Devices names."""
 
-        CAX = 'CAX'
-        ALL = (CAX, )
+        LI_MOD1 = 'LI-01:PU-Modltr-1'
+        LI_MOD2 = 'LI-01:PU-Modltr-2'
+        ALL = (LI_MOD1, LI_MOD2)
 
     _properties = (
-        'F:PPS01:FOEOPEN',  # Enviar 1 para abrir o Front-end completo (abre o gamma e o photon)
-        'F:PPS01:FOECLOSE',  # Enviar 1 para fechar o Front-end completo (fecha o photon e o gamma)
-        'F:PPS01:GS_X_STATUS',  # Status gamma shutter front-end – 0 indica aberto
-        'F:PPS01:PS_STATUS',  # Status photon shutter front-end – 0 indica aberto
-        'A:PPS01:OEAOPENCLOSE',  # shutter da cabana a - Enviar 1 –se estiver fechado abre – se estiver aberto fecha
-        'A:PPS01:PG_STATUS',  # Status do gamma shutter da cabana A – 0 indica aberto
-        'M:PPS01:HABILITACAO_MAQUINA',  # Status da liberação do gamma pela máquina – 1 indica liberado
-        'A:PPS01:SEARCH_OK',  # status da procura cabana A – 1 indica procura feita
-        'B:PPS01:SEARCH_OK',  # status da procura cabana B – 1 indica procura feita
-    )
+        'Remote', 'OutPut_Status', 'RESET',
+        'Run/Stop', 'PreHeat', 'Charge_Allowed', 'TrigOut_Allowed',
+        'Emer_Stop', 'CPS_ALL', 'Thy_Heat', 'Kly_Heat', 'LV_Rdy_OK',
+        'HV_Rdy_OK', 'TRIG_Rdy_OK', 'MOD_Self_Fault', 'MOD_Sys_Ready',
+        'TRIG_Norm', 'Pulse_Current',
+        'RUN_STOP', 'PREHEAT', 'CHARGE', 'TRIGOUT',
+        'WRITE_I', 'READI', 'WRITE_V', 'READV')
 
-    def __init__(self, devname, *args, **kwargs):
-        """Init."""
+    def __init__(self, devname):
+        """."""
         # check if device exists
-        if devname not in BLPPSCtrl.DEVICES.ALL:
+        if devname not in LIModltr.DEVICES.ALL:
             raise NotImplementedError(devname)
+
         # call base class constructor
-        super().__init__(devname, properties=self._properties, *args, **kwargs)
+        super().__init__(devname, properties=LIModltr._properties)
 
     @property
-    def is_hutchA_intlk_search_done(self):
-        """."""
-        return self['A:PPS01:SEARCH_OK'] == 1
+    def run_stop(self):
+        """RUN_STOP."""
+        return self['RUN_STOP']
 
     @property
-    def is_hutchB_intlk_search_done(self):
-        """."""
-        return self['B:PPS01:SEARCH_OK'] == 1
+    def preheat(self):
+        """PREHEAT."""
+        return self['PREHEAT']
 
     @property
-    def is_machine_gamma_enabled(self):
-        """."""
-        return self['M:PPS01:HABILITACAO_MAQUINA'] == 1
+    def charge(self):
+        """CHARGE."""
+        return self['CHARGE']
+
+    @charge.setter
+    def charge(self, value):
+        self._enum_setter('CHARGE', value, _Const.OffOn)
 
     @property
-    def is_frontend_gamma_shutter_opened(self):
-        """."""
-        return self['F:PPS01:GS_X_STATUS'] == 0
+    def trigout(self):
+        """TRIGOUT."""
+        return self['TRIGOUT']
+
+    @trigout.setter
+    def trigout(self, value):
+        self._enum_setter('TRIGOUT', value, _Const.OffOn)
 
     @property
-    def is_frontend_photon_shutter_opened(self):
-        """."""
-        return self['F:PPS01:PS_STATUS'] == 0
-    
+    def voltage(self):
+        """READV."""
+        return self['READV']
+
+    @voltage.setter
+    def voltage(self, value):
+        """WRITE_V."""
+        self['WRITE_V'] = value
+
     @property
-    def is_hutchA_gamma_shutter_opened(self):
-        """."""
-        return self['A:PPS01:PG_STATUS'] == 0
-    
-    def cmd_frontend_gamma_and_photon_open(self):
-        """"."""
-        self['F:PPS01:FOEOPEN'] = 1
-
-    def cmd_frontend_gamma_and_photon_close(self):
-        """"."""
-        self['F:PPS01:FOECLOSE'] = 1
-
-    def cmd_hutchA_gamma_open(self):
-        """"."""
-        if not self.is_hutchA_gamma_shutter_opened:
-            self['A:PPS01:OEAOPENCLOSE'] = 1
-
-    def cmd_hutchA_gamma_close(self):
-        """"."""
-        if self.is_hutchA_gamma_shutter_opened:
-            self['A:PPS01:OEAOPENCLOSE'] = 1
-
-    def cmd_frontend_gamma_and_photon_close(self):
-        """"."""
-        self['F:PPS01:FOECLOSE'] = 1
+    def current(self):
+        """READI."""
+        return self['READI']
+
+    @current.setter
+    def current(self, value):
+        """WRITE_I."""
+        self['WRITE_I'] = value
+
+    def cmd_reset(self, timeout=DEF_TIMEOUT):
+        """Reset."""
+        self['RESET'] = 1
+        if not self._wait('RESET', 1, timeout/2):
+            return False
+        _time.sleep(1)
+        self['RESET'] = 0
+        return self._wait('RESET', 0, timeout/2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `siriuspy-2.79.1/siriuspy/devices/bpm.py` & `siriuspy-2.80.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/currinfo.py` & `siriuspy-2.80.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/dcct.py` & `siriuspy-2.80.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/device.py` & `siriuspy-2.80.0/siriuspy/devices/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,38 +182,39 @@
             in_sim = _Simulation.pv_check(pvname)
             pvclass = _PVSim if in_sim else _PV
             pvs[propty] = pvclass(
                 pvname, auto_monitor=auto_monitor,
                 connection_timeout=Device.CONNECTION_TIMEOUT)
         return devname, pvs
 
-    def _wait(self, propty, value, timeout=_DEF_TIMEOUT, comp='eq'):
+    def _wait(self, propty, value, timeout=None, comp='eq'):
         """."""
         def comp_(val):
             boo = comp(self[propty], val)
             if isinstance(boo, _np.ndarray):
                 boo = _np.all(boo)
             return boo
 
         if isinstance(comp, str):
             comp = getattr(_opr, comp)
 
         if comp_(value):
             return True
 
+        timeout = _DEF_TIMEOUT if timeout is None else timeout
         ntrials = int(timeout/_TINY_INTERVAL)
         for _ in range(ntrials):
             _time.sleep(_TINY_INTERVAL)
             if comp_(value):
                 return True
         return False
 
     def _wait_float(
             self, propty, value, rel_tol=0.0, abs_tol=0.1,
-            timeout=_DEF_TIMEOUT):
+            timeout=None):
         """Wait until float value gets close enough of desired value."""
         func = _partial(_math.isclose, abs_tol=abs_tol, rel_tol=rel_tol)
         return self._wait(propty, value, comp=func, timeout=timeout)
 
     def _get_pvname(self, devname, propty):
         if devname:
             func = devname.substitute
@@ -396,20 +397,21 @@
         for dev, val in dev2val.items():
             if dev.pv_object(propty).wait_for_connection():
                 dev[propty] = val
                 _time.sleep(wait)
 
     def _wait_devices_propty(
             self, devices, propty, values, comp='eq',
-            timeout=_DEF_TIMEOUT, return_prob=False):
+            timeout=None, return_prob=False):
         """Wait for devices property to reach value(s)."""
         if isinstance(comp, str):
             comp = getattr(_opr, comp)
         dev2val = self._get_dev_2_val(devices, values)
 
+        timeout = _DEF_TIMEOUT if timeout is None else timeout
         tini = _time.time()
         for _ in range(int(timeout/_TINY_INTERVAL)):
             okdevs = set()
             for k, v in dev2val.items():
                 boo = comp(k[propty], v)
                 if isinstance(boo, _np.ndarray):
                     boo = _np.all(boo)
```

### Comparing `siriuspy-2.79.1/siriuspy/devices/dvf.py` & `siriuspy-2.80.0/siriuspy/devices/dvf.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         self['cam1:Gain'] = value
 
     @property
     def gain_auto(self):
         """Return camera gain auto."""
         return self['cam1:GainAuto_RBV']
 
-    @gain.setter
+    @gain_auto.setter
     def gain_auto(self, value):
         """Set camera gain auto."""
         self['cam1:GainAuto'] = value
 
     @property
     def pixel_format(self):
         """Return camera pixel format."""
```

### Comparing `siriuspy-2.79.1/siriuspy/devices/egun.py` & `siriuspy-2.80.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/energy.py` & `siriuspy-2.80.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/fofb.py` & `siriuspy-2.80.0/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/fofb_acq.py` & `siriuspy-2.80.0/siriuspy/devices/fofb_acq.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/ict.py` & `siriuspy-2.80.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/idff.py` & `siriuspy-2.80.0/siriuspy/devices/idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/ids.py` & `siriuspy-2.80.0/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/injctrl.py` & `siriuspy-2.80.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/injsys.py` & `siriuspy-2.80.0/siriuspy/devices/injsys.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,16 +460,23 @@
 
         devices = self._llrf_devs + self._moddevs
         devices.append(self._limps)
 
         # call base class constructor
         super().__init__('', tuple(devices), hltiming=hltiming)
 
+        # NOTE: Triggers ordering is important so that LINAC LLRF does
+        # not have any transient during source migration between events
+        # Linac and RmpBO.
         self._trig_names = HLTimeSearch.get_hl_triggers(
-            {'sec': 'LI', 'dev': '(Mod|LLRF|SSAmp|Osc)'})
+            {'sec': 'LI', 'dev': '(Mod|Osc)'})
+        self._trig_names += HLTimeSearch.get_hl_triggers(
+            {'sec': 'LI', 'dev': 'SSAmp'})
+        self._trig_names += HLTimeSearch.get_hl_triggers(
+            {'sec': 'LI', 'dev': 'LLRF'})
 
         self._on_values = dict()
         for dev in self._llrf_devs:
             self._on_values[dev] = {
                 'GET_INTEGRAL_ENABLE': _Const.DsblEnbl.Enbl,
                 'GET_FB_MODE': _Const.DsblEnbl.Enbl}
         for mdev in self._moddevs:
@@ -618,20 +625,20 @@
             text = 'Check for LI LLRF Feedback Mode to be on '\
                    'timed out without success! Verify LI LLRF!'
             return [False, text, retval[1]]
 
         return True, '', []
 
     def change_trigs_to_linac_evt(self):
-        """."""
+        """Change triggers source to Linac."""
         return self.hltiming.change_triggers_source(
-            self._trig_names, new_src='Linac')
+            self._trig_names[::-1], new_src='Linac')
 
     def change_trigs_to_rmpbo_evt(self):
-        """."""
+        """Change triggers source to RmpBO."""
         return self.hltiming.change_triggers_source(
             self._trig_names, new_src='RmpBO')
 
     def check_mps_status(self):
         """."""
         # check if mps status is ok
         _t0 = _time.time()
```

### Comparing `siriuspy-2.79.1/siriuspy/devices/lienergy.py` & `siriuspy-2.80.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/lillrf.py` & `siriuspy-2.80.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/machshift.py` & `siriuspy-2.80.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.80.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/posang.py` & `siriuspy-2.80.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/psconv.py` & `siriuspy-2.80.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/pssofb.py` & `siriuspy-2.80.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/pstesters.py` & `siriuspy-2.80.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/pwrsupply.py` & `siriuspy-2.80.0/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/rf.py` & `siriuspy-2.80.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/scraper.py` & `siriuspy-2.80.0/siriuspy/devices/scraper.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/screen.py` & `siriuspy-2.80.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/sofb.py` & `siriuspy-2.80.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/syncd.py` & `siriuspy-2.80.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/timing.py` & `siriuspy-2.80.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/devices/tune.py` & `siriuspy-2.80.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.80.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.80.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.80.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.80.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.80.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/app.py` & `siriuspy-2.80.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.80.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.80.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.80.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.80.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.80.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.80.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.80.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.80.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.80.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/pvs.py` & `siriuspy-2.80.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.80.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.80.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.80.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.80.0/siriuspy/dvfimgproc/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/dvfimgproc/main.py` & `siriuspy-2.80.0/siriuspy/dvfimgproc/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.80.0/siriuspy/dvfimgproc/meas.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/envars.py` & `siriuspy-2.80.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/epics/multiproc.py` & `siriuspy-2.80.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/epics/properties.py` & `siriuspy-2.80.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/epics/pv_fake.py` & `siriuspy-2.80.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.80.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/fofb/csdev.py` & `siriuspy-2.80.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/fofb/main.py` & `siriuspy-2.80.0/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/idff/config.py` & `siriuspy-2.80.0/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/idff/csdev.py` & `siriuspy-2.80.0/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/idff/main.py` & `siriuspy-2.80.0/siriuspy/idff/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.80.0/siriuspy/injctrl/bias_feedback.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,17 @@
             'ModelDataBias-SP': self.set_data_bias,
             'ModelDataInjCurr-SP': self.set_data_injcurr,
             'LinModAngCoeff-SP': self.set_lin_ang_coeff,
             'LinModOffCoeff-SP': self.set_lin_off_coeff,
             'GPModNoiseStd-SP': self.set_gp_noise_std,
             'GPModKernStd-SP': self.set_gp_kern_std,
             'GPModKernLenScl-SP': self.set_gp_kern_leng,
+            'GPModNoiseStdFit-Sel': self.set_gp_noise_std_fit,
+            'GPModKernStdFit-Sel': self.set_gp_kern_std_fit,
+            'GPModKernLenSclFit-Sel': self.set_gp_kern_leng_fit,
             }
 
     def init_database(self):
         """Set initial PV values."""
         for key, pvdbase in self.database.items():
             pvname = key.split(_Const.BIASFB_PROPTY_PREFIX)[1]
             self.run_callbacks(pvname, pvdbase['value'])
@@ -237,14 +240,38 @@
     def set_gp_kern_leng(self, value):
         """."""
         self.gpmodel.kern.lengthscale = value
         self._update_models()
         self.run_callbacks('GPModKernLenScl-RB', value)
         return True
 
+    def set_gp_noise_std_fit(self, value):
+        """."""
+        if bool(value):
+            self.gpmodel.likelihood.variance.unfix()
+        else:
+            self.gpmodel.likelihood.variance.fix()
+        self.run_callbacks('GPModNoiseStdFit-Sts')
+
+    def set_gp_kern_std_fit(self, value):
+        """."""
+        if bool(value):
+            self.gpmodel.kern.variance.unfix()
+        else:
+            self.gpmodel.kern.variance.fix()
+        self.run_callbacks('GPModKernStdFit-Sts')
+
+    def set_gp_kern_leng_fit(self, value):
+        """."""
+        if bool(value):
+            self.gpmodel.kern.lengthscale.unfix()
+        else:
+            self.gpmodel.kern.lengthscale.fix()
+        self.run_callbacks('GPModKernLenSclFit-Sts')
+
     # ############ Auxiliary Methods ############
     def _callback_to_thread(self, **kwgs):
         if not self.do_update_models or not self.model_update_data:
             return
         _Thread(target=self._update_data, kwargs=kwgs, daemon=True).start()
 
     def _initialize_models(self):
@@ -260,23 +287,37 @@
         x = self.bias_data[:, None].copy()
         y = self.injc_data[:, None].copy()
 
         kernel = gpy.kern.RBF(input_dim=1)
         db_ = self.database['BiasFBGPModKernStd-RB']
         kernel.variance.constrain_bounded(db_['lolim']**2, db_['hilim']**2)
         kernel.variance = db_['value']**2
+        if bool(self.database['BiasFBGPModKernStdFit-Sts']['value']):
+            kernel.variance.unfix()
+        else:
+            kernel.variance.fix()
+
         db_ = self.database['BiasFBGPModKernLenScl-RB']
         kernel.lengthscale.constrain_bounded(db_['lolim'], db_['hilim'])
         kernel.lengthscale = db_['value']
+        if bool(self.database['BiasFBGPModKernLenSclFit-Sts']['value']):
+            kernel.lengthscale.unfix()
+        else:
+            kernel.lengthscale.fix()
 
         gpmodel = gpy.models.GPRegression(x, y, kernel)
         db_ = self.database['BiasFBGPModNoiseStd-RB']
         gpmodel.likelihood.variance.constrain_bounded(
             db_['lolim']**2, db_['hilim']**2)
         gpmodel.likelihood.variance = db_['value']**2
+        if bool(self.database['BiasFBGPModNoiseStdFit-Sts']['value']):
+            gpmodel.likelihood.variance.unfix()
+        else:
+            gpmodel.likelihood.variance.fix()
+
         self.gpmodel = gpmodel
         self._update_predictions()
 
     def _update_data(self, **kwgs):
         bias = self._injctrl.egun_dev.bias.voltage
         dcurr = kwgs['value']
         if None in {bias, dcurr}:
```

### Comparing `siriuspy-2.79.1/siriuspy/injctrl/csdev.py` & `siriuspy-2.80.0/siriuspy/injctrl/csdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         'Off', 'Waiting', 'TurningOn', 'Injecting', 'TurningOff', 'Skipping')
     ACCUMSTS = ('Off', 'Waiting', 'TurningOn', 'Injecting')
     INJSYSCMDSTS = ('Idle', 'On', 'Off')
     RFKILLBEAMMON = ('Idle', 'Kill')
     IDLERUNNING = ('Idle', 'Running')
     IDLEINJECTING = ('Idle', 'Injecting')
     BIASFB_MODEL_TYPES = ('Linear', 'GaussianProcess')
+    FIXED_UNFIXED = ('Fixed', 'Unfixed')
     STANDBY_INJECT = ('Standby', 'Inject')
 
 
 _et = ETypes
 
 
 # --- Const class ---
@@ -41,14 +42,15 @@
     AccumSts = _csdev.Const.register('AccumSts', _et.ACCUMSTS)
     InjSysCmdSts = _csdev.Const.register('InjSysCmdSts', _et.INJSYSCMDSTS)
     RFKillBeamMon = _csdev.Const.register('RFKillBeamMon', _et.RFKILLBEAMMON)
     IdleRunning = _csdev.Const.register('IdleRunning', _et.IDLERUNNING)
     IdleInjecting = _csdev.Const.register('IdleInjecting', _et.IDLEINJECTING)
     BiasFBModelTypes = _csdev.Const.register(
         'ModelTypes', _et.BIASFB_MODEL_TYPES)
+    FixedUnfixed = _csdev.Const.register('FixedUnfixed', _et.FIXED_UNFIXED)
     StandbyInject = _csdev.Const.register('StandbyInject', _et.STANDBY_INJECT)
 
     GEN_STATUS_LABELS = ('LI', 'TB', 'BO', 'TS', 'SI', 'AS')
     LI_STATUS_LABELS = ('Egun', 'PS', 'PU', 'RF', 'TI')
     TL_STATUS_LABELS = ('PS', 'PU', 'TI')
     SR_STATUS_LABELS = ('PS', 'PU', 'RF', 'TI')
     AS_STATUS_LABELS = ('TI', )
@@ -515,40 +517,62 @@
         # Generally ploted in Bias x InjCurr graphs to check model sanity
         'LinModPredBias-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'V'},
         'LinModPredInjCurrAvg-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'mA'},
 
         'GPModNoiseStd-SP': {
-            'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
+            'type': 'float', 'value': 0.0316, 'unit': 'mA', 'prec': 4,
             'lolim': 0.005, 'hilim': 0.5},
         'GPModNoiseStd-RB': {
-            'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
+            'type': 'float', 'value': 0.0316, 'unit': 'mA', 'prec': 4,
             'lolim': 0.005, 'hilim': 0.5},
         'GPModNoiseStd-Mon': {
-            'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
+            'type': 'float', 'value': 0.0316, 'unit': 'mA', 'prec': 4,
             'lolim': 0.005, 'hilim': 0.5},
         'GPModKernStd-SP': {
-            'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
+            'type': 'float', 'value': 0.432, 'unit': 'mA', 'prec': 3,
             'lolim': 0.05, 'hilim': 1},
         'GPModKernStd-RB': {
-            'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
+            'type': 'float', 'value': 0.432, 'unit': 'mA', 'prec': 3,
             'lolim': 0.05, 'hilim': 1},
         'GPModKernStd-Mon': {
-            'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
+            'type': 'float', 'value': 0.432, 'unit': 'mA', 'prec': 3,
             'lolim': 0.05, 'hilim': 1},
         'GPModKernLenScl-SP': {
-            'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'hilim': 10},
+            'type': 'float', 'value': 4, 'unit': 'V', 'prec': 3,
+            'lolim': 2, 'hilim': 10},
         'GPModKernLenScl-RB': {
-            'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'hilim': 10},
+            'type': 'float', 'value': 4, 'unit': 'V', 'prec': 3,
+            'lolim': 2, 'hilim': 10},
         'GPModKernLenScl-Mon': {
-            'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'hilim': 10},
+            'type': 'float', 'value': 4, 'unit': 'V', 'prec': 3,
+            'lolim': 2, 'hilim': 10},
+
+        # These properties are used to fix or unfix the fitting of the
+        # gp parameters.
+        'GPModNoiseStdFit-Sel': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Unfixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+        'GPModNoiseStdFit-Sts': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Unfixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+        'GPModKernStdFit-Sel': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Unfixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+        'GPModKernStdFit-Sts': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Unfixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+        'GPModKernLenSclFit-Sel': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Fixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+        'GPModKernLenSclFit-Sts': {
+            'type': 'enum', 'value': _ct.FixedUnfixed.Fixed,
+            'enums': _et.FIXED_UNFIXED, 'unit': 'Fixed_Unfixed'},
+
 
         # These are used to give the model inference about the bias
         # Generally ploted in Injcurr X Bias graphs
         'GPModInferenceInjCurr-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'mA'},
         'GPModInferenceBias-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'V'},
```

### Comparing `siriuspy-2.79.1/siriuspy/injctrl/main.py` & `siriuspy-2.80.0/siriuspy/injctrl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,37 +437,36 @@
             self._stop_topup_job()
             self._setting_mode = False
         if self._accum_job and self._accum_job.is_alive():
             self._setting_mode = True
             self._stop_accum_job()
             self._setting_mode = False
 
+        if self._pumode != _Const.PUMode.Accumulation and \
+                value == _Const.InjMode.TopUp:
+            self._update_log('ERR:Set PUMode to Accumulation before')
+            self._update_log('ERR:changing mode to top-up')
+            return False
+
         if value != _Const.InjMode.Decay:
             stg = 'top-up' if value == _Const.InjMode.TopUp else 'accumulation'
-
-            if self._pumode != _Const.PUMode.Accumulation:
-                self._update_log('ERR:Set PUMode to Accumulation before')
-                self._update_log(f'ERR:changing mode to {stg:s}')
-                return False
-
             self._update_log('Configuring EVG RepeatBucketList...')
             self._evg_dev['RepeatBucketList-SP'] = 1
             self._update_log(f'...done. Ready to start {stg:s}.')
 
         self._mode = value
         self.run_callbacks('Mode-Sts', self._mode)
         return True
 
     def set_type(self, value):
         """Set injection type."""
         if not 0 <= value < len(_ETypes.INJTYPE):
             return False
         if self._mode != _Const.InjMode.Decay:
-            self._update_log(
-                f'ERR:InjType can only be changed in Decay mode.')
+            self._update_log('ERR:InjType can only be changed in Decay mode.')
             return False
         if self._p2w['Type']['watcher'] is not None and \
                 self._p2w['Type']['watcher'].is_alive():
             self._update_log('WARN:Interrupting type change command..')
             self.egun_dev.cmd_abort_chg_type()
             self._p2w['Type']['watcher'].join()
 
@@ -565,17 +564,17 @@
         self._launch_watch_dev_thread()
         return True
 
     def set_pumode(self, value):
         """Set PU mode."""
         if not 0 <= value < len(_ETypes.PUMODE):
             return False
-        if self._mode != _Const.InjMode.Decay:
-            self._update_log(
-                f'ERR:PUMode can only be changed in Decay mode.')
+        if self._mode == _Const.InjMode.TopUp and \
+                value != _Const.PUMode.Accumulation:
+            self._update_log('ERR:In TopUp mode PUMode must be Accumulation.')
             return False
         if self._p2w['PUMode']['watcher'] is not None and \
                 self._p2w['PUMode']['watcher'].is_alive():
             self._update_log('WARN:Interrupting PUMode change command')
             self._pumode_dev.cmd_abort()
             self._p2w['PUMode']['watcher'].join()
 
@@ -1297,48 +1296,64 @@
         self._handle_aspu_standby_state(_Const.StandbyInject.Inject)
         self._handle_liti_warmup_state(_Const.StandbyInject.Inject)
         self._handle_bops_standby_state(_Const.StandbyInject.Inject)
         self._handle_borf_standby_state(_Const.StandbyInject.Inject)
 
         while self._mode == _Const.InjMode.Accum:
             t0_ = _time.time()
-            if not self.currinfo_dev.connected:
-                self._update_log('ERR:CurrInfo device disconnected.')
-                break
-            if self.currinfo_dev.current >= self._target_current:
-                self._update_log(
-                    'Target Current reached. Stopping accumulation...')
-                break
-
-            if not self._check_allok_2_inject():
+            if not self._continue_accum():
                 break
 
             self.run_callbacks('AccumState-Sts', _Const.AccumSts.TurningOn)
             if not self._start_injection():
                 break
 
             self.run_callbacks('AccumState-Sts', _Const.AccumSts.Injecting)
             if not self._wait_injection():
                 break
             self._update_bucket_list(nrpulses=1)
 
             dt_ = self._accum_period - (_time.time() - t0_)
-            if dt_ > 0:
-                self.run_callbacks('AccumState-Sts', _Const.AccumSts.Waiting)
-                self._update_log('Waiting for next injection...')
-                _time.sleep(dt_)
+            if dt_ <= 0:
+                continue
+            self.run_callbacks('AccumState-Sts', _Const.AccumSts.Waiting)
+            self._update_log('Waiting for next injection...')
+
+            while dt_ > 0:
+                self.run_callbacks('Log-Mon', f'Remaining time: {dt_:.2f}s')
+                slp = min(1, dt_)
+                _time.sleep(slp)
+                if not self._continue_accum():
+                    break
+                dt_ = self._accum_period - (_time.time() - t0_)
+            else:
+                self.run_callbacks('Log-Mon', 'Remaining time: 0s')
+                continue
+            break
 
         self._handle_liti_warmup_state(_Const.StandbyInject.Standby)
 
         # update top-up status
         self.run_callbacks('AccumState-Sts', _Const.AccumSts.Off)
         self._update_log('Stopped accumulation loop.')
         if not self._abort or self._setting_mode:
             self.run_callbacks('AccumState-Sel', _Const.OffOn.Off)
 
+    def _continue_accum(self):
+        if not self.currinfo_dev.connected:
+            self._update_log('ERR:CurrInfo device disconnected.')
+            return False
+        if self.currinfo_dev.current >= self._target_current:
+            self._update_log(
+                'Target Current reached. Stopping accumulation...')
+            return False
+        if not self._check_allok_2_inject():
+            return False
+        return True
+
     # --- auxiliary top-up methods ---
 
     def _launch_topup_job(self):
         while self._abort:
             _time.sleep(0.1)
         self._update_log('Launching top-up thread...')
         self._topup_job = _epics.ca.CAThread(
```

### Comparing `siriuspy-2.79.1/siriuspy/machshift/csdev.py` & `siriuspy-2.80.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/gensumm_macreport.py` & `siriuspy-2.80.0/siriuspy/machshift/gensumm_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/macreport.py` & `siriuspy-2.80.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/macschedule.py` & `siriuspy-2.80.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/main.py` & `siriuspy-2.80.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/savedata_macreport.py` & `siriuspy-2.80.0/siriuspy/machshift/savedata_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/machshift/utils.py` & `siriuspy-2.80.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/magnet/data.py` & `siriuspy-2.80.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/magnet/excdata.py` & `siriuspy-2.80.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/magnet/factory.py` & `siriuspy-2.80.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/magnet/normalizer.py` & `siriuspy-2.80.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/magnet/util.py` & `siriuspy-2.80.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/csdev.py` & `siriuspy-2.80.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.80.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/liemit/main.py` & `siriuspy-2.80.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.80.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/lienergy/main.py` & `siriuspy-2.80.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/meas/util.py` & `siriuspy-2.80.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/namesys/implementation.py` & `siriuspy-2.80.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/optics/lattice_survey.py` & `siriuspy-2.80.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/base.py` & `siriuspy-2.80.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/chrom.py` & `siriuspy-2.80.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/csdev.py` & `siriuspy-2.80.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.80.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/tune.py` & `siriuspy-2.80.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/opticscorr/utils.py` & `siriuspy-2.80.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.80.0/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.80.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/posang/csdev.py` & `siriuspy-2.80.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/posang/main.py` & `siriuspy-2.80.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/posang/utils.py` & `siriuspy-2.80.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/data.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/factory.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.80.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/conn.py` & `siriuspy-2.80.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/magnet.py` & `siriuspy-2.80.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/ramp.py` & `siriuspy-2.80.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.80.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.80.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/testwfm.py` & `siriuspy-2.80.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/util.py` & `siriuspy-2.80.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/ramp/waveform.py` & `siriuspy-2.80.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/bpms_search.py` & `siriuspy-2.80.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/hl_time_search.py` & `siriuspy-2.80.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/id_search.py` & `siriuspy-2.80.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/ioc_search.py` & `siriuspy-2.80.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/ll_time_search.py` & `siriuspy-2.80.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/ma_search.py` & `siriuspy-2.80.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/search/ps_search.py` & `siriuspy-2.80.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/simul/simfactory.py` & `siriuspy-2.80.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/simul/simps.py` & `siriuspy-2.80.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/simul/simpv.py` & `siriuspy-2.80.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/simul/simulation.py` & `siriuspy-2.80.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/simul/simulator.py` & `siriuspy-2.80.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/base_class.py` & `siriuspy-2.80.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/bpms.py` & `siriuspy-2.80.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/correctors.py` & `siriuspy-2.80.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/csdev.py` & `siriuspy-2.80.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/main.py` & `siriuspy-2.80.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/matrix.py` & `siriuspy-2.80.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/orbit.py` & `siriuspy-2.80.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/sofb/utils.py` & `siriuspy-2.80.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/stabinfo/csdev.py` & `siriuspy-2.80.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/stabinfo/main.py` & `siriuspy-2.80.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/thread.py` & `siriuspy-2.80.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/timesys/csdev.py` & `siriuspy-2.80.0/siriuspy/timesys/csdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,19 +601,21 @@
         dbase['Direction-Sel'] = _dcopy(dic_)
         dbase['Direction-Sts'] = dic_
 
     dbase['Status-Mon'] = {'type': 'int', 'value': 0b1111111111}
     dbase['InInjTable-Mon'] = {
         'type': 'enum', 'enums': _et.ININJTAB, 'value': 0}
 
+    # NOTE: we need to add plus 1 to the PVs count due to some unexpected
+    # behavior of pcaspy
+    labs = '\n'.join(Const.HLTrigStatusLabels)
     dbase['StatusLabels-Cte'] = {
-        'type': 'char', 'count': 1000,
-        'value': '\n'.join(Const.HLTrigStatusLabels)
-        }
+        'type': 'char', 'count': len(labs)+1, 'value': labs}
+
     ll_trigs = '\n'.join(ll_trig_names)
     dbase['LowLvlTriggers-Cte'] = {
-        'type': 'char', 'count': 5000, 'value': ll_trigs}
+        'type': 'char', 'count': len(ll_trigs)+1, 'value': ll_trigs}
     channels = '\n'.join(_HLTimeSearch.get_hl_trigger_channels(hl_trigger))
     dbase['CtrldChannels-Cte'] = {
-        'type': 'char', 'count': 5000, 'value': channels}
+        'type': 'char', 'count': len(channels)+1, 'value': channels}
 
     return {prefix + pv: dt for pv, dt in dbase.items()}
```

### Comparing `siriuspy-2.79.1/siriuspy/timesys/hl_classes.py` & `siriuspy-2.80.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/timesys/ll_classes.py` & `siriuspy-2.80.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/timesys/plot_network.py` & `siriuspy-2.80.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/timesys/static_table.py` & `siriuspy-2.80.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy/util.py` & `siriuspy-2.80.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.80.0/siriuspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.79.1
+Version: 2.80.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.79.1/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.80.0/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/bsmp/test_bsmp.py` & `siriuspy-2.80.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/bsmp/test_commands.py` & `siriuspy-2.80.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/bsmp/test_entities.py` & `siriuspy-2.80.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/bsmp/test_serial.py` & `siriuspy-2.80.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/bsmp/test_types.py` & `siriuspy-2.80.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.80.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/clientweb/test_implementation.py` & `siriuspy-2.80.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.80.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/currinfo/test_csdev.py` & `siriuspy-2.80.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/currinfo/test_main.py` & `siriuspy-2.80.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/magnet/test_factory.py` & `siriuspy-2.80.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/magnet/tests_normalizer.py` & `siriuspy-2.80.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/mock_servweb.py` & `siriuspy-2.80.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/namesys/test_implementation.py` & `siriuspy-2.80.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/opticscorr/test_chrom.py` & `siriuspy-2.80.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/opticscorr/test_csdev.py` & `siriuspy-2.80.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.80.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/opticscorr/test_tune.py` & `siriuspy-2.80.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/opticscorr/test_utils.py` & `siriuspy-2.80.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/posang/test_csdev.py` & `siriuspy-2.80.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/posang/test_main.py` & `siriuspy-2.80.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/db.py` & `siriuspy-2.80.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.80.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.80.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/test_csdev.py` & `siriuspy-2.80.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/test_data.py` & `siriuspy-2.80.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/test_siggen.py` & `siriuspy-2.80.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/pwrsupply/variables.py` & `siriuspy-2.80.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/ramp/test_magnet.py` & `siriuspy-2.80.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/ramp/test_waveform.py` & `siriuspy-2.80.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/search/test_hl_time_search.py` & `siriuspy-2.80.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/search/test_init.py` & `siriuspy-2.80.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/search/test_ll_time_search.py` & `siriuspy-2.80.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/search/test_ma_search.py` & `siriuspy-2.80.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/search/test_ps_search.py` & `siriuspy-2.80.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/test_callbacks.py` & `siriuspy-2.80.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/test_csdev.py` & `siriuspy-2.80.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/test_envars.py` & `siriuspy-2.80.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/test_util.py` & `siriuspy-2.80.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/timesys/test_csdev.py` & `siriuspy-2.80.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.1/tests/timesys/test_plot_network.py` & `siriuspy-2.80.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

