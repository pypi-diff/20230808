# Comparing `tmp/qiskit-ibm-provider-0.6.2.tar.gz` & `tmp/qiskit-ibm-provider-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-provider-0.6.2.tar", last modified: Tue Jul 25 19:29:49 2023, max compression
+gzip compressed data, was "qiskit-ibm-provider-0.6.3.tar", last modified: Tue Aug  8 19:23:23 2023, max compression
```

## Comparing `qiskit-ibm-provider-0.6.2.tar` & `qiskit-ibm-provider-0.6.3.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.643955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.647955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    40123 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.651955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32106 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.655955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46038 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/type_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.659955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.663955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.643955 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:29:49.000000 qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.667955 qiskit-ibm-provider-0.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.667955 qiskit-ibm-provider-0.6.2/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.671955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:29:49.675955 qiskit-ibm-provider-0.6.2/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-25 19:29:35.000000 qiskit-ibm-provider-0.6.2/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.032479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40087 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.040479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24078 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/type_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.044479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.036479 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-08-08 19:23:23.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 19:23:22.000000 qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.048479 qiskit-ibm-provider-0.6.3/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30377 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:23:23.052479 qiskit-ibm-provider-0.6.3/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-08 19:23:12.000000 qiskit-ibm-provider-0.6.3/test/ws_server.py
```

### Comparing `qiskit-ibm-provider-0.6.2/LICENSE.txt` & `qiskit-ibm-provider-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/PKG-INFO` & `qiskit-ibm-provider-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.2
+Version: 0.6.3
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.2/README.md` & `qiskit-ibm-provider-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class IBMAccountError(IBMError):
     """Account related errors."""
 
     pass
 
 
 class IBMProviderError(IBMError):
-    """Base class for rrrors raise by IBMProvider."""
+    """Base class for errors raise by IBMProvider."""
 
     pass
 
 
 class IBMProviderValueError(IBMProviderError):
     """Value errors raised by IBMProvider."""
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,14 @@
                 "A quantum circuit should be passed in instead."
             )
 
         if isinstance(shots, float):
             shots = int(shots)
         if not self.configuration().simulator:
             circuits = self._deprecate_id_instruction(circuits)
-        options = {"backend": self.name}
 
         run_config_dict = self._get_run_config(
             program_id=program_id,
             init_circuit=init_circuit,
             init_num_resets=init_num_resets,
             header=header,
             shots=shots,
@@ -511,33 +510,33 @@
         if not program_id.startswith(QASM3RUNNERPROGRAMID):
             # Transpiling in circuit-runner is deprecated.
             run_config_dict["skip_transpilation"] = True
 
         return self._runtime_run(
             program_id=program_id,
             inputs=run_config_dict,
-            options=options,
+            backend_name=self.name,
             job_tags=job_tags,
             image=image,
         )
 
     def _runtime_run(
         self,
         program_id: str,
         inputs: Dict,
-        options: Dict,
+        backend_name: str,
         job_tags: Optional[List[str]] = None,
         image: Optional[str] = None,
     ) -> IBMCircuitJob:
         """Runs the runtime program and returns the corresponding job object"""
         hgp_name = self._instance or self.provider._get_hgp().name
         try:
             response = self.provider._runtime_client.program_run(
                 program_id=program_id,
-                backend_name=options["backend"],
+                backend_name=backend_name,
                 params=inputs,
                 hgp=hgp_name,
                 job_tags=job_tags,
                 image=image,
             )
         except RequestsApiError as ex:
             raise IBMBackendApiError("Error submitting job: {}".format(str(ex))) from ex
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     validate_job_tags,
     filter_data,
     api_status_to_job_status,
 )
 from .utils.hgp import to_instance_format
 
 logger = logging.getLogger(__name__)
+PAGE_SIZE = 50
 
 
 class IBMBackendService:
     """Backend namespace for an IBM Quantum account.
 
     Represent a namespace that provides backend related services for the IBM
     Quantum backends available to this account. An instance of
@@ -318,15 +319,14 @@
             status
             and status not in ["PENDING", "COMPLETED"]
             and (
                 status in all_job_statuses or all(x in all_job_statuses for x in status)
             )
         )
         job_list = []
-        original_limit = limit
         while True:
             job_responses = self._get_jobs(
                 api_filter=api_filter,
                 limit=limit,
                 skip=skip,
                 descending=descending,
                 legacy=legacy,
@@ -358,17 +358,17 @@
                     if job is None:
                         logger.warning(
                             'Discarding job "%s" because it contains invalid data.',
                             job_info.get("job_id", ""),
                         )
                         continue
                     job_list.append(job)
-                    if len(job_list) == original_limit:
+                    if limit and len(job_list) == limit:
                         return job_list
-            skip += limit
+            skip += len(job_responses)
         return job_list
 
     def _get_jobs(
         self,
         api_filter: Dict,
         limit: Optional[int] = 10,
         skip: int = 0,
@@ -387,15 +387,17 @@
 
         Returns:
             A list of raw API response.
         """
         # Retrieve the requested number of jobs, using pagination. The server
         # might limit the number of jobs per request.
         job_responses: List[Dict[str, Any]] = []
-        current_page_limit = limit if (limit is not None and limit <= 50) else 50
+        current_page_limit = (
+            limit if (limit is not None and limit <= PAGE_SIZE) else PAGE_SIZE
+        )
         while True:
             if legacy:
                 job_page = self._default_hgp._api_client.list_jobs(
                     limit=current_page_limit,
                     skip=skip,
                     descending=descending,
                     extra_filter=api_filter,
@@ -416,15 +418,15 @@
             job_responses += job_page
             if limit:
                 if len(job_responses) >= limit:
                     # Stop if we have reached the limit.
                     break
                 current_page_limit = limit - len(job_responses)
             else:
-                current_page_limit = 50
+                current_page_limit = PAGE_SIZE
             skip = len(job_responses)
         return job_responses
 
     def _restore_circuit_job(
         self, job_info: Dict, raise_error: bool, legacy: bool = False
     ) -> Optional[IBMCircuitJob]:
         """Restore a circuit job from the API response.
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         self._status = None
         self._params: Dict[str, Any] = None
         self._queue_info: QueueInfo = None
         if status is not None:
             self._status = api_status_to_job_status(status)
         self._client_version = self._extract_client_version(client_info)
         self._set_result(result)
+        self._usage_estimation: Dict[str, Any] = {}
 
         # Properties used for caching.
         self._cancelled = False
         self._job_error_msg = None  # type: Optional[str]
         self._refreshed = False
 
         self._ws_client_future = None  # type: Optional[futures.Future]
@@ -368,17 +369,21 @@
             return self._job_error_msg
 
         # First try getting error message from the runtime job data
         response = self._runtime_client.job_get(job_id=self.job_id())
         if api_status_to_job_status(response["state"]["status"]) != JobStatus.ERROR:
             return None
         reason = response["state"].get("reason")
+        reason_code = response["state"].get("reason_code")
         # If there is a meaningful reason, return it
         if reason is not None and reason != "Error":
-            self._job_error_msg = reason
+            if reason_code:
+                self._job_error_msg = f"Error code {reason_code}; {reason}"
+            else:
+                self._job_error_msg = reason
             return self._job_error_msg
 
         # Now try parsing a meaningful reason from the results, if possible
         api_result = self._download_external_result(
             self._runtime_client.job_results(self.job_id())
         )
         reason = self._parse_result_for_errors(api_result)
@@ -509,14 +514,28 @@
             Client version in dictionary format, where the key is the name
                 of the client and the value is the version.
         """
         if not self._client_version and not self._refreshed:
             self.refresh()
         return self._client_version
 
+    @property
+    def usage_estimation(self) -> Dict[str, Any]:
+        """Return usage estimation information for this job.
+
+        Returns:
+            ``quantum_seconds`` which is the estimated quantum time
+            of the job in seconds. Quantum time represents the time that
+            the QPU complex is occupied exclusively by the job.
+        """
+        if not self._usage_estimation:
+            self.refresh()
+
+        return self._usage_estimation
+
     def refresh(self) -> None:
         """Obtain the latest job information from the server.
 
         This method may add additional attributes to this job instance, if new
         information becomes available.
 
         Raises:
@@ -532,14 +551,17 @@
             api_response.pop("id")
             self._creation_date = dateutil.parser.isoparse(api_response.pop("created"))
             self._api_status = api_response.pop("state")["status"]
         except (KeyError, TypeError) as err:
             raise IBMJobApiError(
                 "Unexpected return value received " "from the server: {}".format(err)
             ) from err
+        self._usage_estimation = {
+            "quantum_seconds": api_response.pop("estimated_running_time_seconds", None),
+        }
         self._time_per_step = api_metadata.get("timestamps", None)
         self._tags = api_response.pop("tags", [])
         self._status = api_status_to_job_status(self._api_status)
         self._params = api_response.get("params", {})
         self._client_version = self._extract_client_version(
             api_metadata.get("qiskit_version", None)
         )
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from collections import defaultdict
 import numpy as np
 
 from qiskit import circuit as circuit_mod
 from qiskit import extensions
 from qiskit.circuit import library, controlflow, CircuitInstruction
+from qiskit.circuit.classical import expr
 from qiskit.circuit.classicalregister import ClassicalRegister, Clbit
 from qiskit.circuit.gate import Gate
 from qiskit.circuit.controlledgate import ControlledGate
 from qiskit.circuit.instruction import Instruction
 from qiskit.circuit.quantumcircuit import QuantumCircuit
 from qiskit.circuit.quantumregister import QuantumRegister, Qubit
 from qiskit.extensions import quantum_initializer
@@ -153,15 +154,22 @@
         # TODO This uses little endian. Should be fixed in the next QPY version.
         param = struct.unpack("<d", data_bytes)[0]
     elif type_key == type_keys.Value.REGISTER:
         param = _loads_register_param(
             data_bytes.decode(common.ENCODE), circuit, registers
         )
     else:
-        param = value.loads_value(type_key, data_bytes, version, vectors)
+        param = value.loads_value(
+            type_key,
+            data_bytes,
+            version,
+            vectors,
+            clbits=circuit.clbits,
+            cregs=registers["c"],
+        )
 
     return param
 
 
 def _loads_register_param(data_bytes, circuit, registers):  # type: ignore[no-untyped-def]
     # If register name prefixed with null character it's a clbit index for single bit condition.
     if data_bytes[0] == "\x00":
@@ -191,21 +199,26 @@
     label = file_obj.read(instruction.label_size).decode(common.ENCODE)
     condition_register = file_obj.read(instruction.condition_register_size).decode(
         common.ENCODE
     )
     qargs = []
     cargs = []
     params = []
-    condition_tuple = None
-    if instruction.has_condition:
-        # If register name prefixed with null character it's a clbit index for single bit condition.
-        condition_tuple = (
+    condition = None
+    if (version < 5 and instruction.has_condition) or (
+        version >= 5 and instruction.conditional_key == type_keys.Condition.TWO_TUPLE
+    ):
+        condition = (
             _loads_register_param(condition_register, circuit, registers),
             instruction.condition_value,
         )
+    elif version >= 5 and instruction.conditional_key == type_keys.Condition.EXPRESSION:
+        condition = value.read_value(
+            file_obj, version, vectors, clbits=circuit.clbits, cregs=registers["c"]
+        )
     if circuit is not None:
         qubit_indices = dict(enumerate(circuit.qubits))
         clbit_indices = dict(enumerate(circuit.clbits))
     else:
         qubit_indices = {}
         clbit_indices = {}
 
@@ -241,26 +254,26 @@
         params.append(param)
 
     # Load Gate object
     if gate_name in {"Gate", "Instruction", "ControlledGate"}:
         inst_obj = _parse_custom_operation(
             custom_operations, gate_name, params, version, vectors, registers
         )
-        inst_obj.condition = condition_tuple
+        inst_obj.condition = condition
         if instruction.label_size > 0:
             inst_obj.label = label
         if circuit is None:
             return inst_obj
         circuit._append(inst_obj, qargs, cargs)
         return None
     elif gate_name in custom_operations:
         inst_obj = _parse_custom_operation(
             custom_operations, gate_name, params, version, vectors, registers
         )
-        inst_obj.condition = condition_tuple
+        inst_obj.condition = condition
         if instruction.label_size > 0:
             inst_obj.label = label
         if circuit is None:
             return inst_obj
         circuit._append(inst_obj, qargs, cargs)
         return None
     elif hasattr(library, gate_name):
@@ -273,30 +286,30 @@
         gate_class = getattr(quantum_initializer, gate_name)
     elif hasattr(controlflow, gate_name):
         gate_class = getattr(controlflow, gate_name)
     else:
         raise AttributeError("Invalid instruction type: %s" % gate_name)
 
     if gate_name in {"IfElseOp", "WhileLoopOp"}:
-        gate = gate_class(condition_tuple, *params)
+        gate = gate_class(condition, *params)
     elif version >= 5 and issubclass(gate_class, ControlledGate):
         if gate_name in {
             "MCPhaseGate",
             "MCU1Gate",
             "MCXGrayCode",
             "MCXGate",
             "MCXRecursive",
             "MCXVChain",
         }:
             gate = gate_class(*params, instruction.num_ctrl_qubits)
         else:
             gate = gate_class(*params)
             gate.num_ctrl_qubits = instruction.num_ctrl_qubits
             gate.ctrl_state = instruction.ctrl_state
-        gate.condition = condition_tuple
+        gate.condition = condition
     else:
         if gate_name in {
             "Initialize",
             "StatePreparation",
             "UCRXGate",
             "UCRYGate",
             "UCRZGate",
@@ -305,15 +318,15 @@
             gate = gate_class(params)
         else:
             if gate_name == "Barrier":
                 params = [len(qargs)]
             elif gate_name in {"BreakLoopOp", "ContinueLoopOp"}:
                 params = [len(qargs), len(cargs)]
             gate = gate_class(*params)
-        gate.condition = condition_tuple
+        gate.condition = condition
     if instruction.label_size > 0:
         gate.label = label
     if circuit is None:
         return gate
     if not isinstance(gate, Instruction):
         circuit.append(gate, qargs, cargs)
     else:
@@ -542,15 +555,15 @@
         # TODO This uses little endian. This should be fixed in next QPY version.
         type_key = type_keys.Value.FLOAT
         data_bytes = struct.pack("<d", param)
     elif isinstance(param, (Clbit, ClassicalRegister)):
         type_key = type_keys.Value.REGISTER
         data_bytes = _dumps_register(param, index_map)
     else:
-        type_key, data_bytes = value.dumps_value(param)
+        type_key, data_bytes = value.dumps_value(param, index_map=index_map)
 
     return type_key, data_bytes
 
 
 # pylint: disable=too-many-boolean-expressions
 def _write_instruction(  # type: ignore[no-untyped-def]
     file_obj, instruction, custom_operations, index_map
@@ -576,23 +589,26 @@
         gate_class_name = instruction.operation.name
 
     elif isinstance(instruction.operation, library.PauliEvolutionGate):
         gate_class_name = r"###PauliEvolutionGate_" + str(uuid.uuid4())
         custom_operations[gate_class_name] = instruction.operation
         custom_operations_list.append(gate_class_name)
 
-    has_condition = False
+    condition_type = type_keys.Condition.NONE
     condition_register = b""
     condition_value = 0
-    if getattr(instruction.operation, "condition", None):
-        has_condition = True
-        condition_register = _dumps_register(
-            instruction.operation.condition[0], index_map
-        )
-        condition_value = int(instruction.operation.condition[1])
+    if (op_condition := getattr(instruction.operation, "condition", None)) is not None:
+        if isinstance(op_condition, expr.Expr):
+            condition_type = type_keys.Condition.EXPRESSION
+        else:
+            condition_type = type_keys.Condition.TWO_TUPLE
+            condition_register = _dumps_register(
+                instruction.operation.condition[0], index_map
+            )
+            condition_value = int(instruction.operation.condition[1])
 
     gate_class_name = gate_class_name.encode(common.ENCODE)
     label = getattr(instruction.operation, "label")
     if label:
         label_raw = label.encode(common.ENCODE)
     else:
         label_raw = b""
@@ -612,24 +628,27 @@
     instruction_raw = struct.pack(
         formats.CIRCUIT_INSTRUCTION_V2_PACK,
         len(gate_class_name),
         len(label_raw),
         len(instruction_params),
         instruction.operation.num_qubits,
         instruction.operation.num_clbits,
-        has_condition,
+        condition_type.value,
         len(condition_register),
         condition_value,
         num_ctrl_qubits,
         ctrl_state,
     )
     file_obj.write(instruction_raw)
     file_obj.write(gate_class_name)
     file_obj.write(label_raw)
-    file_obj.write(condition_register)
+    if condition_type is type_keys.Condition.EXPRESSION:
+        value.write_value(file_obj, op_condition, index_map=index_map)
+    else:
+        file_obj.write(condition_register)
     # Encode instruciton args
     for qbit in instruction.qubits:
         instruction_arg_raw = struct.pack(
             formats.CIRCUIT_INSTRUCTION_ARG_PACK, b"q", index_map["q"][qbit]
         )
         file_obj.write(instruction_arg_raw)
     for clbit in instruction.clbits:
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 
 """Read and write schedule and schedule instructions."""
 import json
 import struct
 import zlib
 import warnings
 
+from io import BytesIO
 import numpy as np
 
 from qiskit.pulse import library, channels, instructions
 from qiskit.pulse.schedule import ScheduleBlock
 from qiskit.utils import optionals as _optional
+from qiskit.pulse.configuration import Kernel, Discriminator
 from .. import formats, common, type_keys
 from ..exceptions import QpyError
 from . import value
 
 
 if _optional.HAS_SYMENGINE:
     import symengine as sym
@@ -58,14 +60,60 @@
         samples=samples,
         name=name,
         epsilon=header.epsilon,
         limit_amplitude=header.amp_limited,
     )
 
 
+def _loads_obj(type_key, binary_data, version, vectors):  # type: ignore[no-untyped-def]
+    """Wraps `value.loads_value` to deserialize binary data to dictionary
+    or list objects which are not supported by `value.loads_value`.
+    """
+    if type_key == b"D":
+        with BytesIO(binary_data) as container:
+            return common.read_mapping(
+                file_obj=container,
+                deserializer=_loads_obj,
+                version=version,
+                vectors=vectors,
+            )
+    elif type_key == b"l":
+        with BytesIO(binary_data) as container:
+            return common.read_sequence(
+                file_obj=container,
+                deserializer=_loads_obj,
+                version=version,
+                vectors=vectors,
+            )
+    else:
+        return value.loads_value(type_key, binary_data, version, vectors)
+
+
+def _read_kernel(file_obj, version):  # type: ignore[no-untyped-def]
+    params = common.read_mapping(
+        file_obj=file_obj,
+        deserializer=_loads_obj,
+        version=version,
+        vectors={},
+    )
+    name = value.read_value(file_obj, version, {})
+    return Kernel(name=name, **params)
+
+
+def _read_discriminator(file_obj, version):  # type: ignore[no-untyped-def]
+    params = common.read_mapping(
+        file_obj=file_obj,
+        deserializer=_loads_obj,
+        version=version,
+        vectors={},
+    )
+    name = value.read_value(file_obj, version, {})
+    return Discriminator(name=name, **params)
+
+
 def _loads_symbolic_expr(expr_bytes):  # type: ignore[no-untyped-def]
     from sympy import parse_expr  # pylint: disable=import-outside-toplevel
 
     if expr_bytes == b"":
         return None
 
     expr_txt = zlib.decompress(expr_bytes).decode(common.ENCODE)
@@ -231,14 +279,15 @@
 
     instance = object.__new__(context_cls)
     instance._context_params = tuple(context_params)
 
     return instance
 
 
+# pylint: disable=too-many-return-statements
 def _loads_operand(type_key, data_bytes, version):  # type: ignore[no-untyped-def]
     if type_key == type_keys.ScheduleOperand.WAVEFORM:
         return common.data_from_binary(data_bytes, _read_waveform, version=version)
     if type_key == type_keys.ScheduleOperand.SYMBOLIC_PULSE:
         if version < 6:
             return common.data_from_binary(
                 data_bytes, _read_symbolic_pulse, version=version
@@ -247,14 +296,26 @@
             return common.data_from_binary(
                 data_bytes, _read_symbolic_pulse_v6, version=version
             )
     if type_key == type_keys.ScheduleOperand.CHANNEL:
         return common.data_from_binary(data_bytes, _read_channel, version=version)
     if type_key == type_keys.ScheduleOperand.OPERAND_STR:
         return data_bytes.decode(common.ENCODE)
+    if type_key == type_keys.ScheduleOperand.KERNEL:
+        return common.data_from_binary(
+            data_bytes,
+            _read_kernel,
+            version=version,
+        )
+    if type_key == type_keys.ScheduleOperand.DISCRIMINATOR:
+        return common.data_from_binary(
+            data_bytes,
+            _read_discriminator,
+            version=version,
+        )
 
     return value.loads_value(type_key, data_bytes, version, {})
 
 
 def _read_element(file_obj, version, metadata_deserializer):  # type: ignore[no-untyped-def]
     type_key = common.read_type_key(file_obj)
 
@@ -310,14 +371,48 @@
         data._limit_amplitude,
     )
     file_obj.write(header)
     file_obj.write(samples_bytes)
     value.write_value(file_obj, data.name)
 
 
+def _dumps_obj(obj):  # type: ignore[no-untyped-def]
+    """Wraps `value.dumps_value` to serialize dictionary and list objects
+    which are not supported by `value.dumps_value`.
+    """
+    if isinstance(obj, dict):
+        with BytesIO() as container:
+            common.write_mapping(file_obj=container, mapping=obj, serializer=_dumps_obj)
+            binary_data = container.getvalue()
+        return b"D", binary_data
+    elif isinstance(obj, list):
+        with BytesIO() as container:
+            common.write_sequence(
+                file_obj=container, sequence=obj, serializer=_dumps_obj
+            )
+            binary_data = container.getvalue()
+        return b"l", binary_data
+    else:
+        return value.dumps_value(obj)
+
+
+def _write_kernel(file_obj, data):  # type: ignore[no-untyped-def]
+    name = data.name
+    params = data.params
+    common.write_mapping(file_obj=file_obj, mapping=params, serializer=_dumps_obj)
+    value.write_value(file_obj, name)
+
+
+def _write_discriminator(file_obj, data):  # type: ignore[no-untyped-def]
+    name = data.name
+    params = data.params
+    common.write_mapping(file_obj=file_obj, mapping=params, serializer=_dumps_obj)
+    value.write_value(file_obj, name)
+
+
 def _dumps_symbolic_expr(expr):  # type: ignore[no-untyped-def]
     from sympy import srepr, sympify  # pylint: disable=import-outside-toplevel
 
     if expr is None:
         return b""
 
     expr_bytes = srepr(sympify(expr)).encode(common.ENCODE)
@@ -374,14 +469,20 @@
         data_bytes = common.data_to_binary(operand, _write_symbolic_pulse)
     elif isinstance(operand, channels.Channel):
         type_key = type_keys.ScheduleOperand.CHANNEL
         data_bytes = common.data_to_binary(operand, _write_channel)
     elif isinstance(operand, str):
         type_key = type_keys.ScheduleOperand.OPERAND_STR
         data_bytes = operand.encode(common.ENCODE)
+    elif isinstance(operand, Kernel):
+        type_key = type_keys.ScheduleOperand.KERNEL
+        data_bytes = common.data_to_binary(operand, _write_kernel)
+    elif isinstance(operand, Discriminator):
+        type_key = type_keys.ScheduleOperand.DISCRIMINATOR
+        data_bytes = common.data_to_binary(operand, _write_discriminator)
     else:
         type_key, data_bytes = value.dumps_value(operand)
 
     return type_key, data_bytes
 
 
 def _write_element(file_obj, element, metadata_serializer):  # type: ignore[no-untyped-def]
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 """
 Common functions across several serialization and deserialization modules.
 """
 
 import io
 import struct
 
+from typing import Any
 from . import formats
 
-QPY_VERSION = 8
+QPY_VERSION = 9
 ENCODE = "utf8"
 
 
 def read_generic_typed_data(file_obj):  # type: ignore[no-untyped-def]
     """Read a single data chunk from the file like object.
 
     Args:
@@ -249,15 +250,15 @@
     with io.BytesIO() as container:
         write_mapping(container, mapping, serializer, **kwargs)
         binary_data = container.getvalue()
 
     return binary_data
 
 
-def data_from_binary(binary_data, deserializer, **kwargs):  # type: ignore[no-untyped-def]
+def data_from_binary(binary_data, deserializer, **kwargs) -> Any:  # type: ignore[no-untyped-def]
     """Load object from binary data with specified deserializer.
 
     Args:
         binary_data (bytes): Binary data to deserialize.
         deserializer (Callable): Deserializer callback that can handle input object type.
         **kwargs: Options set to the deserializer.
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/formats.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,22 +100,22 @@
     "CIRCUIT_INSTRUCTION",
     [
         "name_size",
         "label_size",
         "num_parameters",
         "num_qargs",
         "num_cargs",
-        "has_condition",
+        "conditional_key",
         "condition_register_size",
         "condition_value",
         "num_ctrl_qubits",
         "ctrl_state",
     ],
 )
-CIRCUIT_INSTRUCTION_V2_PACK = "!HHHII?HqII"
+CIRCUIT_INSTRUCTION_V2_PACK = "!HHHIIBHqII"
 CIRCUIT_INSTRUCTION_V2_SIZE = struct.calcsize(CIRCUIT_INSTRUCTION_V2_PACK)
 
 
 # CIRCUIT_INSTRUCTION_ARG
 CIRCUIT_INSTRUCTION_ARG = namedtuple("CIRCUIT_INSTRUCTION_ARG", ["type", "size"])
 CIRCUIT_INSTRUCTION_ARG_PACK = "!1cI"
 CIRCUIT_INSTRUCTION_ARG_SIZE = struct.calcsize(CIRCUIT_INSTRUCTION_ARG_PACK)
@@ -288,7 +288,63 @@
 )
 LAYOUT_PACK = "!?iiiI"
 LAYOUT_SIZE = struct.calcsize(LAYOUT_PACK)
 
 INITIAL_LAYOUT_BIT = namedtuple("INITIAL_LAYOUT_BIT", ["index", "register_size"])
 INITIAL_LAYOUT_BIT_PACK = "!ii"
 INITIAL_LAYOUT_BIT_SIZE = struct.calcsize(INITIAL_LAYOUT_BIT_PACK)
+
+
+# EXPRESSION
+
+EXPRESSION_DISCRIMINATOR_SIZE = 1
+
+EXPRESSION_CAST = namedtuple("EXPRESSION_CAST", ["implicit"])
+EXPRESSION_CAST_PACK = "!?"
+EXPRESSION_CAST_SIZE = struct.calcsize(EXPRESSION_CAST_PACK)
+
+EXPRESSION_UNARY = namedtuple("EXPRESSION_UNARY", ["opcode"])
+EXPRESSION_UNARY_PACK = "!B"
+EXPRESSION_UNARY_SIZE = struct.calcsize(EXPRESSION_UNARY_PACK)
+
+EXPRESSION_BINARY = namedtuple("EXPRESSION_BINARY", ["opcode"])
+EXPRESSION_BINARY_PACK = "!B"
+EXPRESSION_BINARY_SIZE = struct.calcsize(EXPRESSION_BINARY_PACK)
+
+
+# EXPR_TYPE
+
+EXPR_TYPE_DISCRIMINATOR_SIZE = 1
+
+EXPR_TYPE_BOOL = namedtuple("EXPR_TYPE_BOOL", [])
+EXPR_TYPE_BOOL_PACK = "!"
+EXPR_TYPE_BOOL_SIZE = struct.calcsize(EXPR_TYPE_BOOL_PACK)
+
+EXPR_TYPE_UINT = namedtuple("EXPR_TYPE_UINT", ["width"])  # type: ignore[no-untyped-def]
+EXPR_TYPE_UINT_PACK = "!L"
+EXPR_TYPE_UINT_SIZE = struct.calcsize(EXPR_TYPE_UINT_PACK)
+
+
+# EXPR_VAR
+
+EXPR_VAR_DISCRIMINATOR_SIZE = 1
+
+EXPR_VAR_CLBIT = namedtuple("EXPR_VAR_CLBIT", ["index"])
+EXPR_VAR_CLBIT_PACK = "!L"
+EXPR_VAR_CLBIT_SIZE = struct.calcsize(EXPR_VAR_CLBIT_PACK)
+
+EXPR_VAR_REGISTER = namedtuple("EXPR_VAR_REGISTER", ["reg_name_size"])
+EXPR_VAR_REGISTER_PACK = "!H"
+EXPR_VAR_REGISTER_SIZE = struct.calcsize(EXPR_VAR_REGISTER_PACK)
+
+
+# EXPR_VALUE
+
+EXPR_VALUE_DISCRIMINATOR_SIZE = 1
+
+EXPR_VALUE_BOOL = namedtuple("EXPR_VALUE_BOOL", ["value"])
+EXPR_VALUE_BOOL_PACK = "!?"
+EXPR_VALUE_BOOL_SIZE = struct.calcsize(EXPR_VALUE_BOOL_PACK)
+
+EXPR_VALUE_INT = namedtuple("EXPR_VALUE_INT", ["num_bytes"])
+EXPR_VALUE_INT_PACK = "!B"
+EXPR_VALUE_INT_SIZE = struct.calcsize(EXPR_VALUE_INT_PACK)
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
-
 """User interface of qpy serializer."""
 
 from json import JSONEncoder, JSONDecoder
 from typing import Union, List, BinaryIO, Type, Optional
 from collections.abc import Iterable
 import struct
 import warnings
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,40 +13,42 @@
 # pylint: disable=too-many-return-statements
 
 """
 QPY Type keys for several namespace.
 """
 
 from abc import abstractmethod
-from enum import Enum
+from enum import Enum, IntEnum
 
 import numpy as np
 
 from qiskit.circuit import (
     Gate,
     Instruction,
     QuantumCircuit,
     ControlledGate,
     CASE_DEFAULT,
     Clbit,
     ClassicalRegister,
 )
 from qiskit.circuit.library import PauliEvolutionGate
 from qiskit.circuit.parameter import Parameter
+from qiskit.circuit.classical import expr, types
 from qiskit.circuit.parameterexpression import ParameterExpression
 from qiskit.circuit.parametervector import ParameterVectorElement
 from qiskit.pulse.channels import (
     Channel,
     DriveChannel,
     MeasureChannel,
     ControlChannel,
     AcquireChannel,
     MemorySlot,
     RegisterSlot,
 )
+from qiskit.pulse.configuration import Discriminator, Kernel
 from qiskit.pulse.instructions import (
     Acquire,
     Play,
     Delay,
     SetFrequency,
     ShiftFrequency,
     SetPhase,
@@ -100,14 +102,15 @@
     COMPLEX = b"c"
     NUMPY_OBJ = b"n"
     PARAMETER = b"p"
     PARAMETER_VECTOR = b"v"
     PARAMETER_EXPRESSION = b"e"
     STRING = b"s"
     NULL = b"z"
+    EXPRESSION = b"x"
     CASE_DEFAULT = b"d"
     REGISTER = b"R"
 
     @classmethod
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, int):
             return cls.INTEGER
@@ -127,24 +130,38 @@
             return cls.STRING
         if isinstance(obj, (Clbit, ClassicalRegister)):
             return cls.REGISTER
         if obj is None:
             return cls.NULL
         if obj is CASE_DEFAULT:
             return cls.CASE_DEFAULT
+        if isinstance(obj, expr.Expr):
+            return cls.EXPRESSION
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
         raise NotImplementedError
 
 
+class Condition(IntEnum):
+    """Type keys for the ``conditional_key`` field of the INSTRUCTION struct."""
+
+    # This class is deliberately raw integers and not in terms of ASCII characters for backwards
+    # compatiblity in the form as an old Boolean value was expanded; `NONE` and `TWO_TUPLE` must
+    # have the enumeration values 0 and 1.
+
+    NONE = 0
+    TWO_TUPLE = 1
+    EXPRESSION = 2
+
+
 class Container(TypeKeyBase):
     """Typle key enum for container-like object."""
 
     RANGE = b"r"
     TUPLE = b"t"
 
     @classmethod
@@ -310,18 +327,16 @@
 
 class ScheduleOperand(TypeKeyBase):
     """Type key enum for schedule instruction operand object."""
 
     WAVEFORM = b"w"
     SYMBOLIC_PULSE = b"s"
     CHANNEL = b"c"
-
-    # Discriminator and Acquire instance are not serialzied.
-    # Data format of these object is somewhat opaque and not defiend well.
-    # It's rarely used in the Qiskit experiements. Of course these can be added later.
+    KERNEL = b"k"
+    DISCRIMINATOR = b"d"
 
     # We need to have own string type definition for operands of schedule instruction.
     # Note that string type is already defined in the Value namespace,
     # but its key "s" conflicts with the SYMBOLIC_PULSE in the ScheduleOperand namespace.
     # New in QPY version 7.
     OPERAND_STR = b"o"
 
@@ -329,14 +344,20 @@
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, Waveform):
             return cls.WAVEFORM
         if isinstance(obj, SymbolicPulse):
             return cls.SYMBOLIC_PULSE
         if isinstance(obj, Channel):
             return cls.CHANNEL
+        if isinstance(obj, str):
+            return cls.OPERAND_STR
+        if isinstance(obj, Kernel):
+            return cls.KERNEL
+        if isinstance(obj, Discriminator):
+            return cls.DISCRIMINATOR
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
@@ -410,7 +431,96 @@
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
         raise NotImplementedError
+
+
+class Expression(TypeKeyBase):
+    """Type keys for the ``EXPRESSION`` QPY item."""
+
+    VAR = b"x"
+    VALUE = b"v"
+    CAST = b"c"
+    UNARY = b"u"
+    BINARY = b"b"
+
+    @classmethod
+    def assign(cls, obj):  # type: ignore[no-untyped-def]
+        if (
+            isinstance(obj, expr.Expr)
+            and (key := getattr(cls, obj.__class__.__name__.upper(), None)) is not None
+        ):
+            return key
+        raise exceptions.QpyError(
+            f"Object '{obj}' is not supported in {cls.__name__} namespace."
+        )
+
+    @classmethod
+    def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
+        raise NotImplementedError
+
+
+class ExprType(TypeKeyBase):
+    """Type keys for the ``EXPR_TYPE`` QPY item."""
+
+    BOOL = b"b"
+    UINT = b"u"
+
+    @classmethod
+    def assign(cls, obj):  # type: ignore[no-untyped-def]
+        if (
+            isinstance(obj, types.Type)
+            and (key := getattr(cls, obj.__class__.__name__.upper(), None)) is not None
+        ):
+            return key
+        raise exceptions.QpyError(
+            f"Object '{obj}' is not supported in {cls.__name__} namespace."
+        )
+
+    @classmethod
+    def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
+        raise NotImplementedError
+
+
+class ExprVar(TypeKeyBase):
+    """Type keys for the ``EXPR_VAR`` QPY item."""
+
+    CLBIT = b"C"
+    REGISTER = b"R"
+
+    @classmethod
+    def assign(cls, obj):  # type: ignore[no-untyped-def]
+        if isinstance(obj, Clbit):
+            return cls.CLBIT
+        if isinstance(obj, ClassicalRegister):
+            return cls.REGISTER
+        raise exceptions.QpyError(
+            f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
+        )
+
+    @classmethod
+    def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
+        raise NotImplementedError
+
+
+class ExprValue(TypeKeyBase):
+    """Type keys for the ``EXPR_VALUE`` QPY item."""
+
+    BOOL = b"b"
+    INT = b"i"
+
+    @classmethod
+    def assign(cls, obj):  # type: ignore[no-untyped-def]
+        if isinstance(obj, bool):
+            return cls.BOOL
+        if isinstance(obj, int):
+            return cls.INT
+        raise exceptions.QpyError(
+            f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
+        )
+
+    @classmethod
+    def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
+        raise NotImplementedError
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,14 @@
                 dag.substitute_node(
                     node,
                     node.op.replace_blocks(dag_to_circuit(block) for block in new_dags),
                     inplace=True,
                 )
             elif isinstance(node.op, IGate):
                 delay_op = Delay(self._get_duration(qubit_index_map[node.qargs[0]]))
-                delay_op.condition = node.op.condition
                 dag.substitute_node(node, delay_op, inplace=True)
 
                 modified = True
 
         return modified
 
     def _get_duration(self, qubit: int) -> int:
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 
 """Dynamical decoupling insertion pass for IBM (dynamic circuit) backends."""
 
 import warnings
 from typing import Dict, List, Optional, Union
 
 import numpy as np
+import rustworkx as rx
 from qiskit.circuit import Qubit, Gate
 from qiskit.circuit.delay import Delay
 from qiskit.circuit.library.standard_gates import IGate, UGate, U3Gate
 from qiskit.circuit.reset import Reset
 from qiskit.dagcircuit import DAGCircuit, DAGNode, DAGInNode, DAGOpNode
 from qiskit.quantum_info.operators.predicates import matrix_equal
 from qiskit.quantum_info.synthesis import OneQubitEulerDecomposer
 from qiskit.transpiler.exceptions import TranspilerError
 from qiskit.transpiler.instruction_durations import InstructionDurations
 from qiskit.transpiler.passes.optimization import Optimize1qGates
+from qiskit.transpiler import CouplingMap
 
 from .block_base_padder import BlockBasePadder
 
 
 class PadDynamicalDecoupling(BlockBasePadder):
     """Dynamical decoupling insertion pass for IBM dynamic circuit backends.
 
@@ -113,14 +115,16 @@
         qubits: Optional[List[int]] = None,
         spacings: Optional[Union[List[List[float]], List[float]]] = None,
         skip_reset_qubits: bool = True,
         pulse_alignment: int = 16,
         extra_slack_distribution: str = "middle",
         sequence_min_length_ratios: Optional[Union[int, List[int]]] = None,
         insert_multiple_cycles: bool = False,
+        coupling_map: CouplingMap = None,
+        alt_spacings: Optional[Union[List[List[float]], List[float]]] = None,
     ):
         """Dynamical decoupling initializer.
 
         Args:
             durations: Durations of instructions to be used in scheduling.
             dd_sequences: Sequence of gates to apply in idle spots.
                 Alternatively a list of gate sequences may be supplied that
@@ -129,15 +133,17 @@
                 ``sequence_min_length_ratios``.
             qubits: Physical qubits on which to apply DD.
                 If None, all qubits will undergo DD (when possible).
             spacings: A list of lists of spacings between the DD gates.
                 The available slack will be divided according to this.
                 The list length must be one more than the length of dd_sequence,
                 and the elements must sum to 1. If None, a balanced spacing
-                will be used [d/2, d, d, ..., d, d, d/2].
+                will be used [d/2, d, d, ..., d, d, d/2]. This spacing only
+                applies to the first subcircuit, if a ``coupling_map`` is
+                specified
             skip_reset_qubits: If True, does not insert DD on idle periods that
                 immediately follow initialized/reset qubits
                 (as qubits in the ground state are less susceptible to decoherence).
             pulse_alignment: The hardware constraints for gate timing allocation.
                 This is usually provided from ``backend.configuration().timing_constraints``.
                 If provided, the delay length, i.e. ``spacing``, is implicitly adjusted to
                 satisfy this constraint.
@@ -157,45 +163,71 @@
                 in order to insert the DD sequence. For example if the X-X dynamical decoupling sequence
                 is 320dt samples long and the available delay is 384dt it has a ratio of 384dt/320dt=1.2.
                 From the perspective of dynamical decoupling this is likely to add more control noise
                 than decoupling error rate reductions. The defaults value is 2.0.
             insert_multiple_cycles: If the available duration exceeds
                 2*sequence_min_length_ratio*duration(dd_sequence) enable the insertion of multiple
                 rounds of the dynamical decoupling sequence in that delay.
+            coupling_map: directed graph representing the coupling map for the device. Specifying a
+                coupling map partitions the device into subcircuits, in order to apply DD sequences
+                with different pulse spacings within each. Currently support 2 subcircuits.
+            alt_spacings: A list of lists of spacings between the DD gates, for the second subcircuit,
+                as determined by the coupling map. If None, a balanced spacing that is staggered with
+                respect to the first subcircuit will be used [d, d, d, ..., d, d, 0].
         Raises:
             TranspilerError: When invalid DD sequence is specified.
             TranspilerError: When pulse gate with the duration which is
                 non-multiple of the alignment constraint value is found.
+            TranspilerError: When the coupling map is not supported (i.e., if degree > 3)
         """
 
         super().__init__()
         self._durations = durations
+
         # Enforce list of DD sequences
         if dd_sequences:
             try:
                 iter(dd_sequences[0])
             except TypeError:
                 dd_sequences = [dd_sequences]
         self._dd_sequences = dd_sequences
         self._qubits = qubits
         self._skip_reset_qubits = skip_reset_qubits
         self._alignment = pulse_alignment
+        self._coupling_map = coupling_map
+        self._coupling_coloring = None
 
         if spacings is not None:
             try:
                 iter(spacings[0])  # type: ignore
             except TypeError:
                 spacings = [spacings]  # type: ignore
+        if alt_spacings is not None:
+            try:
+                iter(alt_spacings[0])  # type: ignore
+            except TypeError:
+                alt_spacings = [alt_spacings]  # type: ignore
         self._spacings = spacings
+        self._alt_spacings = alt_spacings
 
         if self._spacings and len(self._spacings) != len(self._dd_sequences):
             raise TranspilerError(
                 "Number of sequence spacings must equal number of DD sequences."
             )
 
+        if self._alt_spacings:
+            if not self._coupling_map:
+                warnings.warn(
+                    "Alternate spacings are ignored because a coupling map was not provided"
+                )
+            elif len(self._alt_spacings) != len(self._dd_sequences):
+                raise TranspilerError(
+                    "Number of alternate sequence spacings must equal number of DD sequences."
+                )
+
         self._extra_slack_distribution = extra_slack_distribution
 
         self._dd_sequence_lengths: Dict[Qubit, List[List[Gate]]] = {}
         self._sequence_phase = 0
 
         if sequence_min_length_ratios is None:
             # Use 2.0 as a sane default
@@ -213,17 +245,34 @@
             )
 
         self._insert_multiple_cycles = insert_multiple_cycles
 
     def _pre_runhook(self, dag: DAGCircuit) -> None:
         super()._pre_runhook(dag)
 
+        if self._coupling_map:
+            physical_qubits = [dag.qubits.index(q) for q in dag.qubits]
+            sub_coupling_map = self._coupling_map.reduce(physical_qubits)
+            self._coupling_coloring = rx.graph_greedy_color(
+                sub_coupling_map.graph.to_undirected()
+            )
+            if any(c > 1 for c in self._coupling_coloring.values()):
+                raise TranspilerError(
+                    "This circuit topology is not supported for staggered dynamical decoupling."
+                    "The maximum connectivity is 3 nearest neighbors per qubit."
+                )
+
         spacings_required = self._spacings is None
         if spacings_required:
             self._spacings = []  # type: ignore
+        alt_spacings_required = (
+            self._alt_spacings is None and self._coupling_map is not None
+        )
+        if alt_spacings_required:
+            self._alt_spacings = []  # type: ignore
 
         for seq_idx, seq in enumerate(self._dd_sequences):
             num_pulses = len(self._dd_sequences[seq_idx])
 
             # Check if physical circuit is given
             if len(dag.qregs) != 1 or dag.qregs.get("q", None) is None:
                 raise TranspilerError("DD runs on physical circuits only.")
@@ -238,14 +287,27 @@
                     a < 0 for a in self._spacings[seq_idx]  # type: ignore
                 ):
                     raise TranspilerError(
                         "The spacings must be given in terms of fractions "
                         "of the slack period and sum to 1."
                     )
 
+            if self._coupling_map:
+                if alt_spacings_required:
+                    mid = 1 / num_pulses
+                    self._alt_spacings.append([mid] * num_pulses + [0])  # type: ignore
+                else:
+                    if sum(self._alt_spacings[seq_idx]) != 1 or any(  # type: ignore
+                        a < 0 for a in self._alt_spacings[seq_idx]  # type: ignore
+                    ):
+                        raise TranspilerError(
+                            "The spacings must be given in terms of fractions "
+                            "of the slack period and sum to 1."
+                        )
+
             # Check if DD sequence is identity
             if num_pulses != 1:
                 if num_pulses % 2 != 0:
                     raise TranspilerError(
                         "DD sequence must contain an even number of gates (or 1)."
                     )
                 # TODO: this check should use the quantum info package in Qiskit.
@@ -359,14 +421,19 @@
 
         for sequence_idx, _ in enumerate(self._dd_sequences):
             dd_sequence = self._dd_sequences[sequence_idx]
             seq_lengths = self._dd_sequence_lengths[qubit][sequence_idx]
             seq_length = np.sum(seq_lengths)
             seq_ratio = self._sequence_min_length_ratios[sequence_idx]
             spacings = self._spacings[sequence_idx]
+            alt_spacings = (
+                np.asarray(self._alt_spacings[sequence_idx])
+                if self._coupling_map
+                else None
+            )
 
             # Verify the delay duration exceeds the minimum time to insert
             if time_interval / seq_length <= seq_ratio:
                 continue
 
             if self._insert_multiple_cycles:
                 num_sequences = max(int(time_interval // (seq_length * seq_ratio)), 1)
@@ -379,17 +446,17 @@
                     num_sequences = 1
             else:
                 num_sequences = 1
 
             # multiple dd sequences may be inserted
             if num_sequences > 1:
                 dd_sequence = list(dd_sequence) * num_sequences
-                spacings = spacings * num_sequences
                 seq_lengths = seq_lengths * num_sequences
                 seq_length = np.sum(seq_lengths)
+                spacings = spacings * num_sequences
 
             spacings = np.asarray(spacings) / num_sequences
             slack = time_interval - seq_length
             sequence_gphase = self._sequence_phase
 
             if slack <= 0:
                 continue
@@ -427,16 +494,24 @@
                         qubit,
                     )
                     return
 
             def _constrained_length(values: np.array) -> np.array:
                 return self._alignment * np.floor(values / self._alignment)
 
+            if self._coupling_map:
+                if self._coupling_coloring[qubit.index] == 0:
+                    sub_spacings = spacings
+                else:
+                    sub_spacings = alt_spacings
+            else:
+                sub_spacings = spacings
+
             # (1) Compute DD intervals satisfying the constraint
-            taus = _constrained_length(slack * spacings)
+            taus = _constrained_length(slack * sub_spacings)
             extra_slack = slack - np.sum(taus)
             # (2) Distribute extra slack
             if self._extra_slack_distribution == "middle":
                 mid_ind = int((len(taus) - 1) / 2)
                 to_middle = _constrained_length(extra_slack)
                 taus[mid_ind] += to_middle
                 if extra_slack - to_middle:
@@ -476,25 +551,17 @@
                 ):
                     gate = dd_sequence[dd_ind]
                     gate_length = seq_lengths[dd_ind]
                     self._apply_scheduled_op(block_idx, idle_after, gate, qubit)
                     idle_after += gate_length
                     dd_ind += 1
 
-            self._block_dag.global_phase = self._mod_2pi(
+            self._block_dag.global_phase = (
                 self._block_dag.global_phase + sequence_gphase
             )
             return
 
         # DD could not be applied, delay instead
         self._apply_scheduled_op(
             block_idx, t_start, Delay(time_interval, self._block_dag.unit), qubit
         )
         return
-
-    @staticmethod
-    def _mod_2pi(angle: float, atol: float = 0) -> float:
-        """Wrap angle into interval [-π,π). If within atol of the endpoint, clamp to -π"""
-        wrapped = (angle + np.pi) % (2 * np.pi) - np.pi
-        if abs(wrapped - np.pi) < atol:
-            wrapped = -np.pi
-        return wrapped
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_decoder.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.2
+Version: 0.6.3
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.2/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.6.3/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/setup.cfg` & `qiskit-ibm-provider-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/setup.py` & `qiskit-ibm-provider-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Setup qiskit_ibm_provider"""
 
 import os
 
 import setuptools
 
 REQUIREMENTS = [
-    "qiskit-terra>=0.24.2",
+    "qiskit-terra>=0.25.0",
     "requests>=2.19",
     "requests-ntlm>=1.1.0",
     "numpy>=1.13",
     "urllib3>=1.21.1",
     "python-dateutil>=2.8.0",
     "websocket-client>=1.5.1",
     "websockets>=10.0",
```

### Comparing `qiskit-ibm-provider-0.6.2/test/__init__.py` & `qiskit-ibm-provider-0.6.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/account.py` & `qiskit-ibm-provider-0.6.3/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/contextmanagers.py` & `qiskit-ibm-provider-0.6.3/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/decorators.py` & `qiskit-ibm-provider-0.6.3/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.6.3/test/e2e/test_real_devices.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.6.3/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/fake_account_client.py` & `qiskit-ibm-provider-0.6.3/test/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/http_server.py` & `qiskit-ibm-provider-0.6.3/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/ibm_test_case.py` & `qiskit-ibm-provider-0.6.3/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_backend.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_composite_job.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_ibm_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_ibm_job_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,19 @@
         )
         self.assertRaises(
             IBMBackendValueError,
             self.dependencies.provider.backend.jobs,
             job_tags=[1, 2, 3],
         )
 
+    def test_cost_estimation(self):
+        """Test cost estimation is returned correctly."""
+        self.assertTrue(self.sim_job.usage_estimation)
+        self.assertIn("quantum_seconds", self.sim_job.usage_estimation)
+
     @skip("TODO refactor fake client")
     def test_missing_required_fields(self):
         """Test response data is missing required fields."""
         saved_api = self.sim_backend._api_client
         try:
             self.sim_backend._api_client = BaseFakeAccountClient(
                 job_class=MissingFieldFakeJob
```

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_ibm_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from qiskit_ibm_provider import hub_group_project
 from qiskit_ibm_provider.api.clients import AccountClient, RuntimeClient
 from qiskit_ibm_provider.api.exceptions import RequestsApiError
 
 from qiskit_ibm_provider.job.ibm_job import IBMJob
 from qiskit_ibm_provider.ibm_backend import IBMBackend
-from qiskit_ibm_provider.ibm_backend_service import IBMBackendService
+from qiskit_ibm_provider.ibm_backend_service import IBMBackendService, PAGE_SIZE
 from qiskit_ibm_provider.ibm_provider import IBMProvider
 from ..account import temporary_account_config_file
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
     integration_test_setup_with_backend,
 )
@@ -196,14 +196,51 @@
         self.assertTrue(len(jobs) > 0)
 
     def test_get_backend(self):
         """Test getting a backend from the provider."""
         backend = self.dependencies.provider.get_backend(name=self.backend_name)
         self.assertEqual(backend.name, self.backend_name)
 
+    def test_jobs_filter(self):
+        """Test limit filters when accessing jobs from the provider."""
+        num_jobs = PAGE_SIZE + 1
+        small_limit = PAGE_SIZE // 2
+        large_limit = PAGE_SIZE * 2
+        backend_name = self.backend_name
+        backend = self.dependencies.provider.get_backend(name=backend_name)
+        circuit = QuantumCircuit(1)
+        circuit.h(0)
+
+        start_time = datetime.now()
+        for _ in range(num_jobs):
+            backend.run(circuit, job_tags=["ibm-provider-test"], shots=1)
+        end_time = datetime.now()
+
+        recent_jobs_small_limit = self.dependencies.provider.jobs(
+            backend_name=backend_name,
+            limit=small_limit,
+            start_datetime=start_time,
+            end_datetime=end_time,
+        )
+        recent_jobs_large_limit = self.dependencies.provider.jobs(
+            backend_name=backend_name,
+            limit=large_limit,
+            start_datetime=start_time,
+            end_datetime=end_time,
+        )
+        recent_jobs_no_limit = self.dependencies.provider.jobs(
+            backend_name=backend_name,
+            limit=None,
+            start_datetime=start_time,
+            end_datetime=end_time,
+        )
+        self.assertEqual(len(recent_jobs_small_limit), small_limit)
+        self.assertEqual(len(recent_jobs_large_limit), num_jobs)
+        self.assertEqual(len(recent_jobs_no_limit), num_jobs)
+
     def test_backend_instance(self):
         """Test that the instance is saved correctly."""
         backend = self.dependencies.provider.get_backend(
             name=self.backend_name, instance=self.instance
         )
         backends = self.dependencies.provider.backends(instance=self.instance)
         job = backend.run(ReferenceCircuits.bell())
```

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_ibm_qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.6.3/test/integration/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/jobtestcase.py` & `qiskit-ibm-provider-0.6.3/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/proxy_server.py` & `qiskit-ibm-provider-0.6.3/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.6.3/test/unit/mock/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.6.3/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_account.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_backend.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_ibm_job_states.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.6.3/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py` & `qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/control_flow_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ddt import ddt, data
 from qiskit import pulse
 from qiskit.circuit import QuantumCircuit, Delay
 from qiskit.circuit.library import XGate, YGate, RXGate, UGate
 from qiskit.quantum_info import Operator
 from qiskit.transpiler.passmanager import PassManager
 from qiskit.transpiler.exceptions import TranspilerError
+from qiskit.transpiler.coupling import CouplingMap
 
 from qiskit_ibm_provider.transpiler.passes.scheduling.dynamical_decoupling import (
     PadDynamicalDecoupling,
 )
 from qiskit_ibm_provider.transpiler.passes.scheduling.scheduler import (
     ASAPScheduleAnalysis,
 )
@@ -71,14 +72,16 @@
                 ("u", None, 100),
                 ("rx", None, 100),
                 ("measure", None, 840),
                 ("reset", None, 1340),
             ]
         )
 
+        self.coupling_map = CouplingMap([[0, 1], [1, 2], [2, 3]])
+
     def test_insert_dd_ghz(self):
         """Test DD gates are inserted in correct spots."""
         dd_sequence = [XGate(), XGate()]
         pm = PassManager(
             [
                 ASAPScheduleAnalysis(self.durations),
                 PadDynamicalDecoupling(
@@ -849,7 +852,120 @@
         expected.delay(225, 0)
         expected.delay(225, 0)
         expected.x(0)
         expected.delay(450, 0)
         expected.x(0)
         expected.delay(225, 0)
         self.assertEqual(qc_dd, expected)
+
+    def test_staggered_dd(self):
+        """Test that timing on DD can be staggered if coupled with each other"""
+        dd_sequence = [XGate(), XGate()]
+        pm = PassManager(
+            [
+                ASAPScheduleAnalysis(self.durations),
+                PadDynamicalDecoupling(
+                    self.durations,
+                    dd_sequence,
+                    coupling_map=self.coupling_map,
+                    alt_spacings=[0.1, 0.8, 0.1],
+                ),
+            ]
+        )
+
+        qc_barriers = QuantumCircuit(4, 1)
+        qc_barriers.x(0)
+        qc_barriers.x(1)
+        qc_barriers.x(2)
+        qc_barriers.x(3)
+        qc_barriers.barrier()
+        qc_barriers.measure(0, 0)
+        qc_barriers.delay(14, 0)
+        qc_barriers.x(1)
+        qc_barriers.x(2)
+        qc_barriers.x(3)
+        qc_barriers.barrier()
+
+        qc_dd = pm.run(qc_barriers)
+
+        expected = QuantumCircuit(4, 1)
+        expected.x(0)
+        expected.x(1)
+        expected.x(2)
+        expected.x(3)
+        expected.barrier()
+        expected.x(1)
+        expected.delay(208, 1)
+        expected.x(1)
+        expected.delay(448, 1)
+        expected.x(1)
+        expected.delay(208, 1)
+        expected.x(2)
+        expected.delay(80, 2)  # q1-q2 are coupled, staggered delays
+        expected.x(2)
+        expected.delay(704, 2)
+        expected.x(2)
+        expected.delay(80, 2)  # q2-q3 are uncoupled, same delays
+        expected.x(3)
+        expected.delay(208, 3)
+        expected.x(3)
+        expected.delay(448, 3)
+        expected.x(3)
+        expected.delay(208, 3)
+        expected.measure(0, 0)
+        expected.delay(14, 0)
+        expected.barrier()
+
+        self.assertEqual(qc_dd, expected)
+
+    def test_insert_dd_bad_spacings(self):
+        """Test DD raises when spacings don't add up to 1."""
+        dd_sequence = [XGate(), XGate()]
+        pm = PassManager(
+            [
+                ASAPScheduleAnalysis(self.durations),
+                PadDynamicalDecoupling(
+                    self.durations,
+                    dd_sequence,
+                    spacings=[0.1, 0.9, 0.1],
+                    coupling_map=self.coupling_map,
+                ),
+            ]
+        )
+
+        with self.assertRaises(TranspilerError):
+            pm.run(self.ghz4)
+
+    def test_insert_dd_bad_alt_spacings(self):
+        """Test DD raises when alt_spacings don't add up to 1."""
+        dd_sequence = [XGate(), XGate()]
+        pm = PassManager(
+            [
+                ASAPScheduleAnalysis(self.durations),
+                PadDynamicalDecoupling(
+                    self.durations,
+                    dd_sequence,
+                    alt_spacings=[0.1, 0.9, 0.1],
+                    coupling_map=self.coupling_map,
+                ),
+            ]
+        )
+
+        with self.assertRaises(TranspilerError):
+            pm.run(self.ghz4)
+
+    def test_unsupported_coupling_map(self):
+        """Test DD raises if coupling map is not supported."""
+        dd_sequence = [XGate(), XGate()]
+        pm = PassManager(
+            [
+                ASAPScheduleAnalysis(self.durations),
+                PadDynamicalDecoupling(
+                    self.durations,
+                    dd_sequence,
+                    coupling_map=CouplingMap([[0, 1], [0, 2], [1, 2], [2, 3]]),
+                ),
+            ]
+        )
+
+        with self.assertRaises(TranspilerError):
+            pm.run(self.ghz4)
```

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.6.3/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.6.3/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/utils.py` & `qiskit-ibm-provider-0.6.3/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.2/test/ws_server.py` & `qiskit-ibm-provider-0.6.3/test/ws_server.py`

 * *Files identical despite different names*

