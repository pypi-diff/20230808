# Comparing `tmp/parsl-2023.7.31.tar.gz` & `tmp/parsl-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.7.31.tar", last modified: Mon Jul 31 22:42:52 2023, max compression
+gzip compressed data, was "parsl-2023.8.7.tar", last modified: Mon Aug  7 22:42:51 2023, max compression
```

## Comparing `parsl-2023.7.31.tar` & `parsl-2023.8.7.tar`

### file list

```diff
@@ -1,485 +1,487 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.138893 parsl-2023.7.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 22:42:47.000000 parsl-2023.7.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 22:42:47.000000 parsl-2023.7.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 22:42:52.138893 parsl-2023.7.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-31 22:42:47.000000 parsl-2023.7.31/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.070890 parsl-2023.7.31/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.070890 parsl-2023.7.31/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.070890 parsl-2023.7.31/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.070890 parsl-2023.7.31/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.074890 parsl-2023.7.31/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.074890 parsl-2023.7.31/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.074890 parsl-2023.7.31/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.074890 parsl-2023.7.31/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.074890 parsl-2023.7.31/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.078890 parsl-2023.7.31/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.078890 parsl-2023.7.31/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.078890 parsl-2023.7.31/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62820 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.078890 parsl-2023.7.31/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.082890 parsl-2023.7.31/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.082890 parsl-2023.7.31/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28361 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32997 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.082890 parsl-2023.7.31/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    50232 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.086891 parsl-2023.7.31/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.086891 parsl-2023.7.31/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/jobs/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.086891 parsl-2023.7.31/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.086891 parsl-2023.7.31/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.090891 parsl-2023.7.31/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.094891 parsl-2023.7.31/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.098891 parsl-2023.7.31/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/serialize/proxystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.102891 parsl-2023.7.31/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.106891 parsl-2023.7.31/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.110892 parsl-2023.7.31/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.110892 parsl-2023.7.31/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.110892 parsl-2023.7.31/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.110892 parsl-2023.7.31/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.110892 parsl-2023.7.31/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.114892 parsl-2023.7.31/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.114892 parsl-2023.7.31/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.114892 parsl-2023.7.31/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.114892 parsl-2023.7.31/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.118892 parsl-2023.7.31/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.118892 parsl-2023.7.31/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.118892 parsl-2023.7.31/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.122892 parsl-2023.7.31/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.122892 parsl-2023.7.31/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.122892 parsl-2023.7.31/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.122892 parsl-2023.7.31/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.122892 parsl-2023.7.31/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_htex/test_htex_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.126893 parsl-2023.7.31/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.126893 parsl-2023.7.31/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.130893 parsl-2023.7.31/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.130893 parsl-2023.7.31/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.130893 parsl-2023.7.31/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.134893 parsl-2023.7.31/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_serialization/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_serialization/test_proxystore_configured.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_serialization/test_proxystore_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.134893 parsl-2023.7.31/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.134893 parsl-2023.7.31/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.138893 parsl-2023.7.31/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-07-31 22:42:47.000000 parsl-2023.7.31/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 22:42:50.000000 parsl-2023.7.31/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:42:52.070890 parsl-2023.7.31/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 22:42:52.000000 parsl-2023.7.31/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 22:42:47.000000 parsl-2023.7.31/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:42:52.138893 parsl-2023.7.31/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2660 2023-07-31 22:42:47.000000 parsl-2023.7.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.368956 parsl-2023.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 22:42:45.000000 parsl-2023.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 22:42:45.000000 parsl-2023.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-07 22:42:51.368956 parsl-2023.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-07 22:42:45.000000 parsl-2023.8.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.308956 parsl-2023.8.7/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.312956 parsl-2023.8.7/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.316956 parsl-2023.8.7/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.320956 parsl-2023.8.7/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.320956 parsl-2023.8.7/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62911 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.320956 parsl-2023.8.7/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.320956 parsl-2023.8.7/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.324956 parsl-2023.8.7/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28361 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32997 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.324956 parsl-2023.8.7/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30113 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/factory_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/taskvine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.324956 parsl-2023.8.7/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.324956 parsl-2023.8.7/parsl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/jobs/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/jobs/simple_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/jobs/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/jobs/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.324956 parsl-2023.8.7/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.328956 parsl-2023.8.7/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.332956 parsl-2023.8.7/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.336956 parsl-2023.8.7/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/serialize/proxystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.340956 parsl-2023.8.7/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.344956 parsl-2023.8.7/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.344956 parsl-2023.8.7/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.344956 parsl-2023.8.7/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.344956 parsl-2023.8.7/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.344956 parsl-2023.8.7/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.348956 parsl-2023.8.7/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.348956 parsl-2023.8.7/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.348956 parsl-2023.8.7/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.352956 parsl-2023.8.7/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.352956 parsl-2023.8.7/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.352956 parsl-2023.8.7/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.352956 parsl-2023.8.7/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.352956 parsl-2023.8.7/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.356956 parsl-2023.8.7/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.356956 parsl-2023.8.7/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.356956 parsl-2023.8.7/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.356956 parsl-2023.8.7/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.356956 parsl-2023.8.7/parsl/tests/test_htex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_htex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_htex/test_htex_zmq_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.360956 parsl-2023.8.7/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.360956 parsl-2023.8.7/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.364956 parsl-2023.8.7/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.364956 parsl-2023.8.7/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.364956 parsl-2023.8.7/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.364956 parsl-2023.8.7/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_serialization/test_2555_caching_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_serialization/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_serialization/test_proxystore_configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_serialization/test_proxystore_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.368956 parsl-2023.8.7/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.368956 parsl-2023.8.7/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.368956 parsl-2023.8.7/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-08-07 22:42:45.000000 parsl-2023.8.7/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-07 22:42:49.000000 parsl-2023.8.7/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:42:51.308956 parsl-2023.8.7/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 22:42:51.000000 parsl-2023.8.7/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 22:42:45.000000 parsl-2023.8.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 22:42:51.368956 parsl-2023.8.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2660 2023-08-07 22:42:45.000000 parsl-2023.8.7/setup.py
```

### Comparing `parsl-2023.7.31/LICENSE` & `parsl-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/PKG-INFO` & `parsl-2023.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.7.31
+Version: 2023.8.7
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.07.31.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.08.07.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.7.31/README.rst` & `parsl-2023.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/__init__.py` & `parsl-2023.8.7/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/addresses.py` & `parsl-2023.8.7/parsl/addresses.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,23 +106,23 @@
     net_interfaces = psutil.net_if_addrs()
 
     s_addresses = set()
     for interface in net_interfaces:
         try:
             s_addresses.add(address_by_interface(interface))
         except Exception:
-            logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
+            logger.info("Ignoring failure to fetch address from interface {}".format(interface))
 
     resolution_functions: List[Callable[[], str]]
     resolution_functions = [address_by_hostname, address_by_route, address_by_query]
     for f in resolution_functions:
         try:
             s_addresses.add(f())
         except Exception:
-            logger.exception("Ignoring an address finder exception")
+            logger.info("Ignoring an address finder exception")
 
     return s_addresses
 
 
 def get_any_address() -> str:
     """ Uses a combination of methods to find any address of the local machine.
 
@@ -133,21 +133,21 @@
 
     addr = ''
     for interface in net_interfaces:
         try:
             addr = address_by_interface(interface)
             return addr
         except Exception:
-            logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
+            logger.info("Ignoring failure to fetch address from interface {}".format(interface))
 
     resolution_functions: List[Callable[[], str]]
     resolution_functions = [address_by_hostname, address_by_route, address_by_query]
     for f in resolution_functions:
         try:
             addr = f()
             return addr
         except Exception:
-            logger.exception("Ignoring an address finder exception")
+            logger.info("Ignoring an address finder exception")
 
     if addr == '':
         raise Exception('Cannot find address of the local machine.')
     return addr
```

### Comparing `parsl-2023.7.31/parsl/app/app.py` & `parsl-2023.8.7/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/app/bash.py` & `parsl-2023.8.7/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/app/errors.py` & `parsl-2023.8.7/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/app/futures.py` & `parsl-2023.8.7/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/app/python.py` & `parsl-2023.8.7/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/benchmark/perf.py` & `parsl-2023.8.7/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/base.py` & `parsl-2023.8.7/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/errors.py` & `parsl-2023.8.7/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/local/local.py` & `parsl-2023.8.7/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.8.7/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/ssh/ssh.py` & `parsl-2023.8.7/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.8.7/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/concurrent/__init__.py` & `parsl-2023.8.7/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/config.py` & `parsl-2023.8.7/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/ASPIRE1.py` & `parsl-2023.8.7/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/Azure.py` & `parsl-2023.8.7/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/ad_hoc.py` & `parsl-2023.8.7/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/bluewaters.py` & `parsl-2023.8.7/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/bridges.py` & `parsl-2023.8.7/parsl/configs/bridges.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from parsl.config import Config
 from parsl.providers import SlurmProvider
 from parsl.launchers import SrunLauncher
 from parsl.executors import HighThroughputExecutor
+from parsl.addresses import address_by_interface
 
 """ This config assumes that it is used to launch parsl tasks from the login nodes
 of Bridges at PSC. Each job submitted to the scheduler will request 2 nodes for 10 minutes.
 """
 
 config = Config(
     executors=[
         HighThroughputExecutor(
             label='Bridges_HTEX_multinode',
+            address=address_by_interface('ens3f0'),
             max_workers=1,
             provider=SlurmProvider(
                 'YOUR_PARTITION_NAME',  # Specify Partition / QOS, for eg. RM-small
                 nodes_per_block=2,
                 init_blocks=1,
                 # string to prepend to #SBATCH blocks in the submit
                 # script to the scheduler eg: '#SBATCH --gres=gpu:type:n'
```

### Comparing `parsl-2023.7.31/parsl/configs/cc_in2p3.py` & `parsl-2023.8.7/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/comet.py` & `parsl-2023.8.7/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/cooley.py` & `parsl-2023.8.7/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/ec2.py` & `parsl-2023.8.7/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/frontera.py` & `parsl-2023.8.7/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/illinoiscluster.py` & `parsl-2023.8.7/parsl/configs/illinoiscluster.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from parsl.config import Config
 from parsl.providers import SlurmProvider
 from parsl.executors import HighThroughputExecutor
 from parsl.launchers import SrunLauncher
-from parsl.addresses import address_by_hostname
 
 """ This config assumes that it is used to launch parsl tasks from the login nodes
 of the Campus Cluster at UIUC. Each job submitted to the scheduler will request 2 nodes for 10 minutes.
 """
 config = Config(
      executors=[
           HighThroughputExecutor(
                label="CC_htex",
                worker_debug=False,
-               address=address_by_hostname(),
                cores_per_worker=16.0,  # each worker uses a full node
                provider=SlurmProvider(
                     partition='secondary-fdr',  # partition
                     nodes_per_block=2,  # number of nodes
                     init_blocks=1,
                     max_blocks=1,
                     scheduler_options='',
```

### Comparing `parsl-2023.7.31/parsl/configs/kubernetes.py` & `parsl-2023.8.7/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/midway.py` & `parsl-2023.8.7/parsl/configs/midway.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from parsl.config import Config
 from parsl.providers import SlurmProvider
 from parsl.launchers import SrunLauncher
 from parsl.executors import HighThroughputExecutor
+from parsl.addresses import address_by_interface
 
 config = Config(
     executors=[
         HighThroughputExecutor(
             label='Midway_HTEX_multinode',
+            address=address_by_interface('bond0'),
             worker_debug=False,
             max_workers=2,
             provider=SlurmProvider(
                 'YOUR_PARTITION',  # Partition name, e.g 'broadwl'
                 launcher=SrunLauncher(),
                 nodes_per_block=2,
                 init_blocks=1,
```

### Comparing `parsl-2023.7.31/parsl/configs/osg.py` & `parsl-2023.8.7/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/polaris.py` & `parsl-2023.8.7/parsl/configs/polaris.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from parsl.addresses import address_by_hostname
+from parsl.addresses import address_by_interface
 from parsl.executors import HighThroughputExecutor
 from parsl.launchers import MpiExecLauncher
 from parsl.providers import PBSProProvider
 from parsl.config import Config
 
 # There are three user parameters to change for the PBSProProvider:
 #  YOUR_ACCOUNT: Account to charge usage
@@ -11,15 +11,15 @@
 
 #  You may also need to change the filesystem if your data is not on Eagle
 
 config = Config(
     executors=[
         HighThroughputExecutor(
             available_accelerators=4,  # Ensures one worker per accelerator
-            address=address_by_hostname(),
+            address=address_by_interface('bond0'),
             cpu_affinity="alternating",  # Prevents thread contention
             prefetch_capacity=0,  # Increase if you have many more tasks than workers
             start_method="spawn",  # Needed to avoid interactions between MPI and os.fork
             provider=PBSProProvider(
                 account="YOUR_ACCOUNT",
                 worker_init="module load conda; conda activate YOUR_ENV",
                 walltime="YOUR_WALLTIME",
```

### Comparing `parsl-2023.7.31/parsl/configs/stampede2.py` & `parsl-2023.8.7/parsl/configs/stampede2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from parsl.config import Config
 from parsl.providers import SlurmProvider
 from parsl.launchers import SrunLauncher
 from parsl.executors import HighThroughputExecutor
 from parsl.data_provider.globus import GlobusStaging
+from parsl.addresses import address_by_interface
 
 
 config = Config(
     executors=[
         HighThroughputExecutor(
             label='Stampede2_HTEX',
+            address=address_by_interface('em3'),
             max_workers=2,
             provider=SlurmProvider(
                 nodes_per_block=2,
                 init_blocks=1,
                 min_blocks=1,
                 max_blocks=1,
                 partition='YOUR_PARTITION',
```

### Comparing `parsl-2023.7.31/parsl/configs/summit.py` & `parsl-2023.8.7/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/theta.py` & `parsl-2023.8.7/parsl/tests/configs/bluewaters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 from parsl.config import Config
-from parsl.providers import CobaltProvider
-from parsl.launchers import AprunLauncher
 from parsl.executors import HighThroughputExecutor
+from parsl.launchers import AprunLauncher
+from parsl.providers import TorqueProvider
+
+from .user_opts import user_opts
+
+
+def fresh_config():
+    config = Config(
+        executors=[
+            HighThroughputExecutor(
+                label="bw_htex",
+                cores_per_worker=1,
+                worker_debug=False,
+                max_workers=1,
+                provider=TorqueProvider(
+                    queue='normal',
+                    launcher=AprunLauncher(overrides="-b -- bwpy-environ --"),
+                    # string to prepend to #SBATCH blocks in the submit
+                    # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
+                    scheduler_options='',
+                    # Command to be run before starting a worker, such as:
+                    # 'module load Anaconda; source activate parsl_env'.
+                    worker_init=user_opts['bluewaters']['worker_init'],
+                    init_blocks=1,
+                    max_blocks=1,
+                    min_blocks=1,
+                    nodes_per_block=2,
+                    walltime='00:30:00',
+                    cmd_timeout=120,
+                ),
+            )
+        ],
+    )
+    return config
 
 
-config = Config(
-    executors=[
-        HighThroughputExecutor(
-            label='theta_local_htex_multinode',
-            max_workers=4,
-            cpu_affinity='block',  # Ensures that workers use cores on the same tile
-            provider=CobaltProvider(
-                queue='YOUR_QUEUE',
-                account='YOUR_ACCOUNT',
-                launcher=AprunLauncher(overrides="-d 64 --cc depth"),
-                walltime='00:30:00',
-                nodes_per_block=2,
-                init_blocks=1,
-                min_blocks=1,
-                max_blocks=1,
-                # string to prepend to #COBALT blocks in the submit
-                # script to the scheduler eg: '#COBALT -t 50'
-                scheduler_options='',
-                # Command to be run before starting a worker, such as:
-                # 'module load Anaconda; source activate parsl_env'.
-                worker_init='',
-                cmd_timeout=120,
-            ),
-        )
-    ],
-)
+config = fresh_config()
```

### Comparing `parsl-2023.7.31/parsl/configs/toss3_llnl.py` & `parsl-2023.8.7/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/vineex_local.py` & `parsl-2023.8.7/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/configs/wqex_local.py` & `parsl-2023.8.7/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/data_manager.py` & `parsl-2023.8.7/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/files.py` & `parsl-2023.8.7/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/ftp.py` & `parsl-2023.8.7/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/globus.py` & `parsl-2023.8.7/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/http.py` & `parsl-2023.8.7/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/rsync.py` & `parsl-2023.8.7/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/data_provider/staging.py` & `parsl-2023.8.7/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/dflow.py` & `parsl-2023.8.7/parsl/dataflow/dflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1124,15 +1124,16 @@
             if self.monitoring and block_ids:
                 new_status = {}
                 for bid in block_ids:
                     new_status[bid] = JobStatus(JobState.PENDING)
                 msg = executor.create_monitoring_info(new_status)
                 logger.debug("Sending monitoring message {} to hub from DFK".format(msg))
                 self.monitoring.send(MessageType.BLOCK_INFO, msg)
-        self.job_status_poller.add_executors(executors)
+        block_executors = [e for e in executors if isinstance(e, BlockProviderExecutor)]
+        self.job_status_poller.add_executors(block_executors)
 
     def atexit_cleanup(self) -> None:
         if not self.cleanup_called:
             logger.info("DFK cleanup because python process is exiting")
             self.cleanup()
         else:
             logger.info("python process is exiting, but DFK has already been cleaned up")
@@ -1193,32 +1194,32 @@
         logger.info("Closing job status poller")
         self.job_status_poller.close()
         logger.info("Terminated job status poller")
 
         logger.info("Scaling in and shutting down executors")
 
         for executor in self.executors.values():
-            if not executor.bad_state_is_set:
-                if isinstance(executor, BlockProviderExecutor):
+            if isinstance(executor, BlockProviderExecutor):
+                if not executor.bad_state_is_set:
                     logger.info(f"Scaling in executor {executor.label}")
                     if executor.provider:
                         job_ids = executor.provider.resources.keys()
                         block_ids = executor.scale_in(len(job_ids))
                         if self.monitoring and block_ids:
                             new_status = {}
                             for bid in block_ids:
                                 new_status[bid] = JobStatus(JobState.CANCELLED)
                             msg = executor.create_monitoring_info(new_status)
                             logger.debug("Sending message {} to hub from DFK".format(msg))
                             self.monitoring.send(MessageType.BLOCK_INFO, msg)
-                logger.info(f"Shutting down executor {executor.label}")
-                executor.shutdown()
-                logger.info(f"Shut down executor {executor.label}")
-            else:  # and bad_state_is_set
-                logger.warning(f"Not shutting down executor {executor.label} because it is in bad state")
+                else:  # and bad_state_is_set
+                    logger.warning(f"Not shutting down executor {executor.label} because it is in bad state")
+            logger.info(f"Shutting down executor {executor.label}")
+            executor.shutdown()
+            logger.info(f"Shut down executor {executor.label}")
 
         logger.info("Terminated executors")
         self.time_completed = datetime.datetime.now()
 
         if self.monitoring:
             logger.info("Sending final monitoring message")
             self.monitoring.send(MessageType.WORKFLOW_INFO,
```

### Comparing `parsl-2023.7.31/parsl/dataflow/errors.py` & `parsl-2023.8.7/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/futures.py` & `parsl-2023.8.7/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/memoization.py` & `parsl-2023.8.7/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/rundirs.py` & `parsl-2023.8.7/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/states.py` & `parsl-2023.8.7/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/dataflow/taskrecord.py` & `parsl-2023.8.7/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/errors.py` & `parsl-2023.8.7/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/base.py` & `parsl-2023.8.7/parsl/executors/status_handling.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,234 +1,236 @@
-from abc import ABCMeta, abstractmethod
+import logging
+import threading
+from itertools import compress
+from abc import abstractmethod, abstractproperty
 from concurrent.futures import Future
-from typing import Any, Callable, Dict, Optional, List
-from typing_extensions import Literal, Self
-
-from parsl.jobs.states import JobStatus
+from typing import List, Any, Dict, Optional, Tuple, Union
 
 import parsl  # noqa F401
+from parsl.executors.base import ParslExecutor
+from parsl.executors.errors import BadStateException, ScalingFailed
+from parsl.jobs.states import JobStatus, JobState
+from parsl.providers.base import ExecutionProvider
+from parsl.utils import AtomicIDCounter
 
+import parsl.jobs.simple_error_handler as error_handler
 
-class ParslExecutor(metaclass=ABCMeta):
-    """Executors are abstractions that represent available compute resources
-    to which you could submit arbitrary App tasks.
-
-    This is an abstract base class that only enforces concrete implementations
-    of functionality by the child classes.
+logger = logging.getLogger(__name__)
 
-    Can be used as a context manager. On exit, calls ``self.shutdown()`` with
-    no arguments and re-raises any thrown exception.
 
-    In addition to the listed methods, a ParslExecutor instance must always
-    have a member field:
+class BlockProviderExecutor(ParslExecutor):
+    """A base class for executors which scale using blocks.
 
-       label: str - a human readable label for the executor, unique
-              with respect to other executors.
+    This base class is intended to help with executors which:
 
-    Per-executor monitoring behaviour can be influenced by exposing:
+    - use blocks of workers to execute tasks
+    - blocks of workers are launched on a batch system through
+      an `ExecutionProvider`
 
-       radio_mode: str - a string describing which radio mode should be used to
-              send task resource data back to the submit side.
+    An implementing class should implement the abstract methods required by
+    `ParslExecutor` to submit tasks, as well as BlockProviderExecutor
+    abstract methods to provide the executor-specific command to start a block
+    of workers (the ``_get_launch_command`` method), and some basic scaling
+    information (``outstanding`` and ``workers_per_node`` properties).
 
-    An executor may optionally expose:
+    This base class provides a ``scale_out`` method which will launch new
+    blocks. It does not provide a ``scale_in`` method, because scale-in
+    behaviour is not well defined in the Parsl scaling model and so behaviour
+    is left to individual executors.
 
-       storage_access: List[parsl.data_provider.staging.Staging] - a list of staging
-              providers that will be used for file staging. In the absence of this
-              attribute, or if this attribute is `None`, then a default value of
-              ``parsl.data_provider.staging.default_staging`` will be used by the
-              staging code.
+    Parsl scaling will provide scaling between min_blocks and max_blocks by
+    invoking scale_out, but it will not initialize the blocks requested by
+    any init_blocks parameter. Subclasses must implement that behaviour
+    themselves.
 
-              Typechecker note: Ideally storage_access would be declared on executor
-              __init__ methods as List[Staging] - however, lists are by default
-              invariant, not co-variant, and it looks like @typeguard cannot be
-              persuaded otherwise. So if you're implementing an executor and want to
-              @typeguard the constructor, you'll have to use List[Any] here.
+    BENC: TODO: block error handling: maybe I want this more user pluggable?
+    I'm not sure of use cases for switchability at the moment beyond "yes or no"
     """
+    def __init__(self, *,
+                 provider: Optional[ExecutionProvider],
+                 block_error_handler: bool):
+        super().__init__()
+        self._provider = provider
+        self.block_error_handler = block_error_handler
+        # errors can happen during the submit call to the provider; this is used
+        # to keep track of such errors so that they can be handled in one place
+        # together with errors reported by status()
+        self._simulated_status: Dict[Any, JobStatus] = {}
+        self._executor_bad_state = threading.Event()
+        self._executor_exception: Optional[Exception] = None
+
+        self._block_id_counter = AtomicIDCounter()
+
+        self._tasks = {}  # type: Dict[object, Future]
+        self.blocks = {}  # type: Dict[str, str]
+        self.block_mapping = {}  # type: Dict[str, str]
+
+    def _make_status_dict(self, block_ids: List[str], status_list: List[JobStatus]) -> Dict[str, JobStatus]:
+        """Given a list of block ids and a list of corresponding status strings,
+        returns a dictionary mapping each block id to the corresponding status
+
+        :param block_ids: the list of block ids
+        :param status_list: the list of job status strings
+        :return: the resulting dictionary
+        """
+        if len(block_ids) != len(status_list):
+            raise IndexError("block id list and status string list differ in size")
+        d = {}
+        for i in range(len(block_ids)):
+            d[block_ids[i]] = status_list[i]
 
-    label: str = "undefined"
-    radio_mode: str = "udp"
-
-    def __enter__(self) -> Self:
-        return self
-
-    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Literal[False]:
-        self.shutdown()
-        return False
-
-    @abstractmethod
-    def start(self) -> Optional[List[str]]:
-        """Start the executor.
-
-        Any spin-up operations (for example: starting thread pools) should be performed here.
-        """
-        pass
-
-    @abstractmethod
-    def submit(self, func: Callable, resource_specification: Dict[str, Any], *args: Any, **kwargs: Any) -> Future:
-        """Submit.
-
-        The executor can optionally set a parsl_executor_task_id attribute on
-        the Future that it returns, and in that case, parsl will log a
-        relationship between the executor's task ID and parsl level try/task
-        IDs.
-        """
-        pass
-
-    @abstractmethod
-    def scale_out(self, blocks: int) -> List[str]:
-        """Scale out method.
-
-        :return: A list of block ids corresponding to the blocks that were added.
-        """
-        pass
-
-    @abstractmethod
-    def scale_in(self, blocks: int) -> List[str]:
-        """Scale in method.
-
-        Cause the executor to reduce the number of blocks by count.
-
-        We should have the scale in method simply take resource object
-        which will have the scaling methods, scale_in itself should be a coroutine, since
-        scaling tasks can be slow.
-
-        :return: A list of block ids corresponding to the blocks that were removed.
-        """
-        pass
-
-    @abstractmethod
-    def shutdown(self) -> bool:
-        """Shutdown the executor.
-
-        This includes all attached resources such as workers and controllers.
-        """
-        pass
-
-    def create_monitoring_info(self, status: Dict[str, JobStatus]) -> List[object]:
-        """Create a monitoring message for each block based on the poll status.
-
-        :return: a list of dictionaries mapping to the info of each block
-        """
-        return []
-
-    def monitor_resources(self) -> bool:
-        """Should resource monitoring happen for tasks on running on this executor?
-
-        Parsl resource monitoring conflicts with execution styles which use threads, and
-        can deadlock while running.
-
-        This function allows resource monitoring to be disabled per executor implementation.
-        """
-        return True
-
-    @abstractmethod
-    def status(self) -> Dict[str, JobStatus]:
-        """Return the status of all jobs/blocks currently known to this executor.
-
-        :return: a dictionary mapping block ids (in string) to job status
-        """
-        pass
+        return d
 
     @property
-    @abstractmethod
-    def status_polling_interval(self) -> int:
+    def status_polling_interval(self):
         """Returns the interval, in seconds, at which the status method should be called. The
         assumption here is that, once initialized, an executor's polling interval is fixed.
         In practice, at least given the current situation, the executor uses a single task provider
         and this method is a delegate to the corresponding method in the provider.
 
         :return: the number of seconds to wait between calls to status() or zero if no polling
                  should be done
         """
-        pass
+        if self._provider is None:
+            return 0
+        else:
+            return self._provider.status_polling_interval
+
+    def _fail_job_async(self, block_id: Any, message: str):
+        """Marks a job that has failed to start but would not otherwise be included in status()
+        as failed and report it in status()
+        """
+        if block_id is None:
+            block_id = str(self._block_id_counter.get_id())
+            logger.info(f"Allocated block ID {block_id} for simulated failure")
+        self._simulated_status[block_id] = JobStatus(JobState.FAILED, message)
+
+    @abstractproperty
+    def outstanding(self) -> int:
+        """This should return the number of tasks that the executor has been given to run (waiting to run, and running now)"""
 
-    @property
-    @abstractmethod
-    def error_management_enabled(self) -> bool:
-        """Indicates whether worker error management is supported by this executor. Worker error
-        management is done externally to the executor. However, the executor must implement
-        certain status handling methods that allow this to function. These methods are:
-
-        :method:handle_errors
-        :method:set_bad_state_and_fail_all
-
-        The basic idea of worker error management is that an external entity maintains a view of
-        the state of the workers by calling :method:status() which is then processed to detect
-        abnormal conditions. This can be done externally, as well as internally, through
-        :method:handle_errors. If an entity external to the executor detects an abnormal condition,
-        it can notify the executor using :method:set_bad_state_and_fail_all(exception).
-
-        Some of the scaffolding needed for implementing error management inside executors,
-        including implementations for the status handling methods above, is available in
-        :class:parsl.executors.status_handling.BlockProviderExecutor, which interested executors
-        should inherit from. Noop versions of methods that are related to status handling and
-        running parsl tasks through workers are implemented by
-        :class:parsl.executors.status_handling.NoStatusHandlingExecutor.
-        """
-        pass
+        raise NotImplementedError("Classes inheriting from BlockProviderExecutor must implement "
+                                  "outstanding()")
 
-    @abstractmethod
-    def handle_errors(self, error_handler: "parsl.jobs.job_error_handler.JobErrorHandler",
-                      status: Dict[str, JobStatus]) -> None:
-        """This method is called by the error management infrastructure after a status poll. The
-        executor implementing this method is then responsible for detecting abnormal conditions
-        based on the status of submitted jobs. If the executor does not implement any special
-        error handling, this method should return False, in which case a generic error handling
-        scheme will be used.
-        :param error_handler: a reference to the generic error handler calling this method
-        :param status: status of all jobs launched by this executor
+    def status(self) -> Dict[str, JobStatus]:
+        """Return the status of all jobs/blocks currently known to this executor.
+
+        :return: a dictionary mapping block ids (in string) to job status
         """
-        pass
+        if self._provider:
+            block_ids, job_ids = self._get_block_and_job_ids()
+            status = self._make_status_dict(block_ids, self._provider.status(job_ids))
+        else:
+            status = {}
+        status.update(self._simulated_status)
 
-    @abstractmethod
-    def set_bad_state_and_fail_all(self, exception: Exception) -> None:
+        return status
+
+    def set_bad_state_and_fail_all(self, exception: Exception):
         """Allows external error handlers to mark this executor as irrecoverably bad and cause
         all tasks submitted to it now and in the future to fail. The executor is responsible
         for checking  :method:bad_state_is_set() in the :method:submit() method and raising the
         appropriate exception, which is available through :method:executor_exception().
         """
-        pass
+        logger.exception("Setting bad state due to exception", exc_info=exception)
+        self._executor_exception = exception
+        # Set bad state to prevent new tasks from being submitted
+        self._executor_bad_state.set()
+        # We set all current tasks to this exception to make sure that
+        # this is raised in the main context.
+        for task in self._tasks:
+            self._tasks[task].set_exception(BadStateException(self, self._executor_exception))
 
     @property
-    @abstractmethod
-    def bad_state_is_set(self) -> bool:
+    def bad_state_is_set(self):
         """Returns true if this executor is in an irrecoverable error state. If this method
         returns true, :property:executor_exception should contain an exception indicating the
         cause.
         """
-        pass
+        return self._executor_bad_state.is_set()
 
     @property
-    @abstractmethod
-    def executor_exception(self) -> Exception:
+    def executor_exception(self):
         """Returns an exception that indicates why this executor is in an irrecoverable state."""
-        pass
+        return self._executor_exception
 
-    @property
-    def run_dir(self) -> str:
-        """Path to the run directory.
-        """
-        return self._run_dir
-
-    @run_dir.setter
-    def run_dir(self, value: str) -> None:
-        self._run_dir = value
-
-    @property
-    def hub_address(self) -> Optional[str]:
-        """Address to the Hub for monitoring.
-        """
-        return self._hub_address
-
-    @hub_address.setter
-    def hub_address(self, value: Optional[str]) -> None:
-        self._hub_address = value
-
-    @property
-    def hub_port(self) -> Optional[int]:
-        """Port to the Hub for monitoring.
+    def handle_errors(self, status: Dict[str, JobStatus]) -> None:
+        """This method is called by the error management infrastructure after a status poll. The
+        executor implementing this method is then responsible for detecting abnormal conditions
+        based on the status of submitted jobs. If the executor does not implement any special
+        error handling, this method should return False, in which case a generic error handling
+        scheme will be used.
+        :param status: status of all jobs launched by this executor
         """
-        return self._hub_port
+        if not self.block_error_handler:
+            return
+        init_blocks = 3
+        if hasattr(self.provider, 'init_blocks'):
+            init_blocks = self.provider.init_blocks
+        if init_blocks < 1:
+            init_blocks = 1
+        error_handler.simple_error_handler(self, status, init_blocks)
+
+    @property
+    def tasks(self) -> Dict[object, Future]:
+        return self._tasks
+
+    @property
+    def provider(self):
+        return self._provider
+
+    def _filter_scale_in_ids(self, to_kill, killed):
+        """ Filter out job id's that were not killed
+        """
+        assert len(to_kill) == len(killed)
+        # Filters first iterable by bool values in second
+        return list(compress(to_kill, killed))
+
+    def scale_out(self, blocks: int = 1) -> List[str]:
+        """Scales out the number of blocks by "blocks"
+        """
+        if not self.provider:
+            raise ScalingFailed(self, "No execution provider available")
+        block_ids = []
+        logger.info(f"Scaling out by {blocks} blocks")
+        for i in range(blocks):
+            block_id = str(self._block_id_counter.get_id())
+            logger.info(f"Allocated block ID {block_id}")
+            try:
+                job_id = self._launch_block(block_id)
+                self.blocks[block_id] = job_id
+                self.block_mapping[job_id] = block_id
+                block_ids.append(block_id)
+            except Exception as ex:
+                self._fail_job_async(block_id,
+                                     "Failed to start block {}: {}".format(block_id, ex))
+        return block_ids
+
+    def _launch_block(self, block_id: str) -> Any:
+        launch_cmd = self._get_launch_command(block_id)
+        job_name = f"parsl.{self.label}.block-{block_id}"
+        logger.debug("Submitting to provider with job_name %s", job_name)
+        job_id = self.provider.submit(launch_cmd, 1, job_name)
+        if job_id:
+            logger.debug(f"Launched block {block_id} on executor {self.label} with job ID {job_id}")
+        else:
+            raise ScalingFailed(self,
+                                "Attempt to provision nodes did not return a job ID")
+        return job_id
+
+    @abstractmethod
+    def _get_launch_command(self, block_id: str) -> str:
+        pass
+
+    def _get_block_and_job_ids(self) -> Tuple[List[str], List[Any]]:
+        # Not using self.blocks.keys() and self.blocks.values() simultaneously
+        # The dictionary may be changed during invoking this function
+        # As scale_in and scale_out are invoked in multiple threads
+        block_ids = list(self.blocks.keys())
+        job_ids = []  # types: List[Any]
+        for bid in block_ids:
+            job_ids.append(self.blocks[bid])
+        return block_ids, job_ids
 
-    @hub_port.setter
-    def hub_port(self, value: Optional[int]) -> None:
-        self._hub_port = value
+    @abstractproperty
+    def workers_per_node(self) -> Union[int, float]:
+        pass
```

### Comparing `parsl-2023.7.31/parsl/executors/errors.py` & `parsl-2023.8.7/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.8.7/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/flux/executor.py` & `parsl-2023.8.7/parsl/executors/flux/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from collections.abc import Mapping, Callable
 from typing import Optional, Any, Dict
 import weakref
 
 import zmq
 
 from parsl.utils import RepresentationMixin
-from parsl.executors.status_handling import NoStatusHandlingExecutor
+from parsl.executors.base import ParslExecutor
 from parsl.executors.flux.execute_parsl_task import __file__ as _WORKER_PATH
 from parsl.executors.flux.flux_instance_manager import __file__ as _MANAGER_PATH
 from parsl.executors.errors import ScalingFailed
 from parsl.providers import LocalProvider
 from parsl.providers.base import ExecutionProvider
 from parsl.serialize import pack_apply_message, deserialize
 from parsl.serialize.errors import SerializationError
@@ -120,15 +120,15 @@
                 future_wrapper.set_result(task_result.returnval)
     else:  # the job exited abnormally
         future_wrapper.set_exception(
             AppException(f"Parsl task exited abnormally: returned {returncode}")
         )
 
 
-class FluxExecutor(NoStatusHandlingExecutor, RepresentationMixin):
+class FluxExecutor(ParslExecutor, RepresentationMixin):
     """Executor that uses Flux to schedule and run jobs.
 
     Every callable submitted to the executor is wrapped into a Flux job.
 
     This executor requires that there be a Flux installation available
     locally, and that it can be located either in PATH or through the
     ``flux_path`` argument.
@@ -185,15 +185,15 @@
         flux_executor_kwargs: Mapping = {},
         flux_path: Optional[str] = None,
         launch_cmd: Optional[str] = None,
     ):
         super().__init__()
         if provider is None:
             provider = LocalProvider()
-        self._provider = provider
+        self.provider = provider
         self.label = label
         if working_dir is None:
             working_dir = self.label + "_" + str(uuid.uuid4())
         self.working_dir = os.path.abspath(working_dir)
         # check that flux_path is an executable, or look for flux in PATH
         if flux_path is None:
             flux_path = shutil.which("flux")
```

### Comparing `parsl-2023.7.31/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.8.7/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/high_throughput/executor.py` & `parsl-2023.8.7/parsl/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/high_throughput/interchange.py` & `parsl-2023.8.7/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/high_throughput/probe.py` & `parsl-2023.8.7/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.8.7/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.8.7/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/errors.py` & `parsl-2023.8.7/parsl/executors/taskvine/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2023.8.7/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.data_provider.files import File
 from parsl.utils import get_std_fname_mode
 import traceback
 import sys
 import pickle
 
-# This scripts executes a parsl function which is pickled in 3 files:
+# This scripts executes a parsl function which is pickled in a file:
 #
 # exec_parsl_function.py map_file function_file result_file
 #
 # map_file: Contains a pickled dictionary that indicates which local_paths the
 #           parsl Files should take.
 #
-# function_file: Contains a pickle parsl function. Function might be serialized in advance.
-# See @parsl.serialize.concretes.py
+# function_file: Contains a pickle parsl function.
 #
-# result_file: A file path, whose content will contain the result of the function, including any
+# result_file: It will contain the result of the function, including any
 #              exception generated. Exceptions will be wrapped with RemoteExceptionWrapper.
 #
 # Exit codes:
 # 0: The function was evaluated to completion. The result or any exception
 #    wrapped with RemoteExceptionWrapper were written to result_file.
 # anything else: There was an error that prevented writing to the result file altogether.
 #                The exit code corresponds to whatever the python interpreter gives.
 #
 
 
-def load_pickled_file(filename: str):
-    """ Load a pickled file and return its pickled object."""
+def load_pickled_file(filename):
     with open(filename, "rb") as f_in:
         return pickle.load(f_in)
 
 
-def dump_result_to_file(result_file: str, result_package):
-    """ Dump a result to the given result file."""
+def dump_result_to_file(result_file, result_package):
     with open(result_file, "wb") as f_out:
         pickle.dump(result_package, f_out)
 
 
 def remap_location(mapping, parsl_file):
-    """ Remap files from local name (on manager) to remote name (on worker)."""
     if not isinstance(parsl_file, File):
         return
     # Below we rewrite .local_path when scheme != file only when the local_name
     # was given by the main parsl process.  This is the case when scheme !=
     # 'file' but .local_path (via filepath) is in mapping.
     if parsl_file.scheme == 'file' or parsl_file.local_path:
         master_location = parsl_file.filepath
         if master_location in mapping:
             parsl_file.local_path = mapping[master_location]
 
 
 def remap_list_of_files(mapping, maybe_files):
-    """ Remap a list of potential files."""
     for maybe_file in maybe_files:
         remap_location(mapping, maybe_file)
 
 
 def remap_all_files(mapping, fn_args, fn_kwargs):
     # remap any positional argument given to the function that looks like a
     # File
@@ -75,48 +70,70 @@
                     fn_kwargs[kwarg] = (mapping[fname], mode)
         else:
             # Treat anything else as a possible File to be remapped.
             remap_location(mapping, maybe_file)
 
 
 def unpack_function(function_info, user_namespace):
-    """ Unpack a function according to its encoding scheme."""
-    return unpack_byte_code_function(function_info, user_namespace)
+    if "source code" in function_info:
+        return unpack_source_code_function(function_info, user_namespace)
+    elif "byte code" in function_info:
+        return unpack_byte_code_function(function_info, user_namespace)
+    else:
+        raise ValueError("Function file does not have a valid function representation.")
+
+
+def unpack_source_code_function(function_info, user_namespace):
+    source_code = function_info["source code"]
+    name = function_info["name"]
+    args = function_info["args"]
+    kwargs = function_info["kwargs"]
+    return (source_code, name, args, kwargs)
 
 
 def unpack_byte_code_function(function_info, user_namespace):
-    """ Returns a function object, a default name, positional arguments, and keyword arguments
-    for a function."""
     from parsl.serialize import unpack_apply_message
     func, args, kwargs = unpack_apply_message(function_info["byte code"], user_namespace, copy=False)
     return (func, 'parsl_function_name', args, kwargs)
 
 
 def encode_function(user_namespace, fn, fn_name, fn_args, fn_kwargs):
-    """ Register the given function to the given namespace."""
     # Returns a tuple (code, result_name)
     # code can be exec in the user_namespace to produce result_name.
     prefix = "parsl_"
     args_name = prefix + "args"
     kwargs_name = prefix + "kwargs"
     result_name = prefix + "result"
 
     # Add variables to the namespace to make function call
     user_namespace.update({args_name: fn_args,
                            kwargs_name: fn_kwargs,
                            result_name: result_name})
 
-    if callable(fn):
+    if isinstance(fn, str):
+        code = encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
+    elif callable(fn):
         code = encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
     else:
         raise ValueError("Function object does not look like a function.")
 
     return (code, result_name)
 
 
+def encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
+    # We drop the first line as it names the parsl decorator used (i.e., @python_app)
+    source = fn.split('\n')[1:]
+    fn_app = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
+
+    source.append(fn_app)
+
+    code = "\n".join(source)
+    return code
+
+
 def encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
     user_namespace.update({fn_name: fn})
     code = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
     return code
 
 
 def load_function(map_file, function_file):
```

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/executor.py` & `parsl-2023.8.7/parsl/executors/workqueue/executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,336 +1,431 @@
-""" TaskVineExecutor utilizes the TaskVine distributed framework developed by the
+""" WorkQueueExecutor utilizes the Work Queue distributed framework developed by the
 Cooperative Computing Lab (CCL) at Notre Dame to provide a fault-tolerant,
 high-throughput system for delegating Parsl tasks to thousands of remote machines
 """
 
-# Import Python built-in libraries
 import threading
 import multiprocessing
 import logging
+from concurrent.futures import Future
+from ctypes import c_bool
+
 import tempfile
 import hashlib
 import subprocess
 import os
+import socket
 import time
 import pickle
 import queue
 import inspect
 import shutil
 import itertools
-import uuid
-from ctypes import c_bool
-from concurrent.futures import Future
-from typing import List, Optional, Union
 
-# Import Parsl constructs
-import parsl.utils as putils
-from parsl.utils import setproctitle
-from parsl.data_provider.staging import Staging
 from parsl.serialize import pack_apply_message
+import parsl.utils as putils
+from parsl.executors.errors import ExecutorError
 from parsl.data_provider.files import File
 from parsl.errors import OptionalModuleMissing
+from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.providers.base import ExecutionProvider
 from parsl.providers import LocalProvider, CondorProvider
+from parsl.executors.workqueue import exec_parsl_function
 from parsl.process_loggers import wrap_with_logs
-from parsl.addresses import get_any_address
-from parsl.executors.errors import ExecutorError
-from parsl.executors.errors import UnsupportedFeatureError
-from parsl.executors.status_handling import BlockProviderExecutor
-from parsl.executors.taskvine import exec_parsl_function
-from parsl.executors.taskvine.manager_config import TaskVineManagerConfig
-from parsl.executors.taskvine.factory_config import TaskVineFactoryConfig
-from parsl.executors.taskvine.errors import TaskVineTaskFailure
-from parsl.executors.taskvine.errors import TaskVineManagerFailure
-from parsl.executors.taskvine.errors import TaskVineFactoryFailure
-from parsl.executors.taskvine.utils import ParslTaskToVine
-from parsl.executors.taskvine.utils import VineTaskToParsl
-from parsl.executors.taskvine.utils import ParslFileToVine
+from parsl.utils import setproctitle
 
-# Import other libraries
 import typeguard
+from typing import Dict, List, Optional, Set, Union
+from parsl.data_provider.staging import Staging
+
+from .errors import WorkQueueTaskFailure
+from .errors import WorkQueueFailure
+
+from collections import namedtuple
 
-# Import TaskVine python modules
 try:
-    from ndcctools.taskvine import cvine
-    from ndcctools.taskvine import Manager
-    from ndcctools.taskvine import Factory
-    from ndcctools.taskvine import Task
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_MAX_THROUGHPUT
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_EXHAUSTIVE_BUCKETING
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_MAX
+    import work_queue as wq
+    from work_queue import WorkQueue
+    from work_queue import WORK_QUEUE_DEFAULT_PORT
+    from work_queue import WORK_QUEUE_ALLOCATION_MODE_MAX_THROUGHPUT
 except ImportError:
-    _taskvine_enabled = False
+    _work_queue_enabled = False
+    WORK_QUEUE_DEFAULT_PORT = 0
 else:
-    _taskvine_enabled = True
+    _work_queue_enabled = True
+
+package_analyze_script = shutil.which("python_package_analyze")
+package_create_script = shutil.which("python_package_create")
+package_run_script = shutil.which("python_package_run")
 
 logger = logging.getLogger(__name__)
 
 
-class TaskVineExecutor(BlockProviderExecutor, putils.RepresentationMixin):
-    """Executor to use TaskVine dynamic workflow system
+# Support structure to communicate parsl tasks to the work queue submit thread.
+ParslTaskToWq = namedtuple('ParslTaskToWq',
+                           'id category cores memory disk gpus priority running_time_min env_pkg map_file function_file result_file input_files output_files')
+
+# Support structure to communicate final status of work queue tasks to parsl
+# result is only valid if result_received is True
+# reason and status are only valid if result_received is False
+WqTaskToParsl = namedtuple('WqTaskToParsl', 'id result_received result reason status')
+
+# Support structure to report parsl filenames to work queue.
+# parsl_name is the local_name or filepath attribute of a parsl file object.
+# stage tells whether the file should be copied by work queue to the workers.
+# cache tells whether the file should be cached at workers. Only valid if stage == True
+ParslFileToWq = namedtuple('ParslFileToWq', 'parsl_name stage cache')
 
-    The TaskVineExecutor system utilizes the TaskVine framework to
+
+class WorkQueueExecutor(BlockProviderExecutor, putils.RepresentationMixin):
+    """Executor to use Work Queue batch system
+
+    The WorkQueueExecutor system utilizes the Work Queue framework to
     efficiently delegate Parsl apps to remote machines in clusters and
     grids using a fault-tolerant system. Users can run the
-    vine_worker program on remote machines to connect to the
-    TaskVineExecutor, and Parsl apps will then be sent out to these
+    work_queue_worker program on remote machines to connect to the
+    WorkQueueExecutor, and Parsl apps will then be sent out to these
     machines for execution and retrieval.
 
-    This Executor sets up configurations for the TaskVine manager, TaskVine
-    factory, and run both in separate processes. Sending tasks and receiving
-    results are done through multiprocessing module native to Python.
 
     Parameters
     ----------
 
         label: str
             A human readable label for the executor, unique
-            with respect to other executors.
-            Default is "TaskVineExecutor".
+            with respect to other Work Queue master programs.
+            Default is "WorkQueueExecutor".
 
-        use_factory: bool
-            Choose to whether use either the Parsl provider or
-            TaskVine factory to scale workers.
+        working_dir: str
+            Location for Parsl to perform app delegation to the Work
+            Queue system. Defaults to current directory.
+
+        project_name: str
+            If a project_name is given, then Work Queue will periodically
+            report its status and performance back to the global WQ catalog,
+            which can be viewed here:  http://ccl.cse.nd.edu/software/workqueue/status
+            Default is None.  Overrides address.
+
+        project_password_file: str
+            Optional password file for the work queue project. Default is None.
+
+        address: str
+            The ip to contact this work queue master process.
+            If not given, uses the address of the current machine as returned
+            by socket.gethostname().
+            Ignored if project_name is specified.
+
+        port: int
+            TCP port on Parsl submission machine for Work Queue workers
+            to connect to. Workers will connect to Parsl using this port.
+
+            If 0, Work Queue will allocate a port number automatically.
+            In this case, environment variables can be used to influence the
+            choice of port, documented here:
+            https://ccl.cse.nd.edu/software/manuals/api/html/work__queue_8h.html#a21714a10bcdfcf5c3bd44a96f5dcbda6
+            Default: WORK_QUEUE_DEFAULT_PORT.
+
+        env: dict{str}
+            Dictionary that contains the environmental variables that
+            need to be set on the Work Queue worker machine.
+
+        shared_fs: bool
+            Define if working in a shared file system or not. If Parsl
+            and the Work Queue workers are on a shared file system, Work
+            Queue does not need to transfer and rename files for execution.
             Default is False.
 
-        manager_config: TaskVineManagerConfig
-            Configuration for the TaskVine manager. Default
-
-        factory_config: TaskVineFactoryConfig
-            Configuration for the TaskVine factory.
-            Use of factory is disabled by default.
-
-        provider: ExecutionProvider
-            The Parsl provider that will spawn worker processes.
-            Default to spawning one local vine worker process.
-
-        storage_access: List[Staging]
-            Define Parsl file staging providers for this executor.
-            Default is None.
+        use_cache: bool
+            Whether workers should cache files that are common to tasks.
+            Warning: Two files are considered the same if they have the same
+            filepath name. Use with care when reusing the executor instance
+            across multiple parsl workflows. Default is False.
+
+        source: bool
+            Choose whether to transfer parsl app information as
+            source code. (Note: this increases throughput for
+            @python_apps, but the implementation does not include
+            functionality for @bash_apps, and thus source=False
+            must be used for programs utilizing @bash_apps.)
+            Default is False. Set to True if pack is True
+
+        pack: bool
+            Use conda-pack to prepare a self-contained Python evironment for
+            each task. This greatly increases task latency, but does not
+            require a common environment or shared FS on execution nodes.
+            Implies source=True.
+
+        extra_pkgs: list
+            List of extra pip/conda package names to include when packing
+            the environment. This may be useful if the app executes other
+            (possibly non-Python) programs provided via pip or conda.
+            Scanning the app source for imports would not detect these
+            dependencies, so they need to be manually specified.
+
+        autolabel: bool
+            Use the Resource Monitor to automatically determine resource
+            labels based on observed task behavior.
+
+        autolabel_window: int
+            Set the number of tasks considered for autolabeling. Work Queue
+            will wait for a series of N tasks with steady resource
+            requirements before making a decision on labels. Increasing
+            this parameter will reduce the number of failed tasks due to
+            resource exhaustion when autolabeling, at the cost of increased
+            resources spent collecting stats.
+
+        autocategory: bool
+            Place each app in its own category by default. If all
+            invocations of an app have similar performance characteristics,
+            this will provide a reasonable set of categories automatically.
+
+        max_retries: int
+            Set the number of retries that Work Queue will make when a task
+            fails. This is distinct from Parsl level retries configured in
+            parsl.config.Config. Set to None to allow Work Queue to retry
+            tasks forever. By default, this is set to 1, so that all retries
+            will be managed by Parsl.
+
+        init_command: str
+            Command line to run before executing a task in a worker.
+            Default is ''.
+
+        worker_options: str
+            Extra options passed to work_queue_worker. Default is ''.
+
+        worker_executable: str
+            The command used to invoke work_queue_worker. This can be used
+            when the worker needs to be wrapped inside some other command
+            (for example, to run the worker inside a container). Default is
+            'work_queue_worker'.
+
+        function_dir: str
+            The directory where serialized function invocations are placed
+            to be sent to workers. If undefined, this defaults to a directory
+            under runinfo/. If shared_filesystem=True, then this directory
+            must be visible from both the submitting side and workers.
+
+        coprocess: bool
+            Use Work Queue's coprocess facility to avoid launching a new Python
+            process for each task. Experimental.
+            This requires a version of Work Queue / cctools after commit
+            874df524516441da531b694afc9d591e8b134b73 (release 7.5.0 is too early).
+            Default is False.
     """
 
     radio_mode = "filesystem"
 
     @typeguard.typechecked
     def __init__(self,
-                 label: str = "TaskVineExecutor",
-                 use_factory: bool = False,
-                 manager_config: TaskVineManagerConfig = TaskVineManagerConfig(),
-                 factory_config: TaskVineFactoryConfig = TaskVineFactoryConfig(),
-                 provider: Optional[ExecutionProvider] = LocalProvider(init_blocks=1),
-                 storage_access: Optional[List[Staging]] = None):
-
-        # If TaskVine factory is used, disable the Parsl provider
-        if use_factory:
-            provider = None
-
-        # Initialize the parent class with the execution provider and block error handling enabled.
+                 label: str = "WorkQueueExecutor",
+                 provider: ExecutionProvider = LocalProvider(),
+                 working_dir: str = ".",
+                 project_name: Optional[str] = None,
+                 project_password_file: Optional[str] = None,
+                 address: Optional[str] = None,
+                 port: int = WORK_QUEUE_DEFAULT_PORT,
+                 env: Optional[Dict] = None,
+                 shared_fs: bool = False,
+                 storage_access: Optional[List[Staging]] = None,
+                 use_cache: bool = False,
+                 source: bool = False,
+                 pack: bool = False,
+                 extra_pkgs: Optional[List[str]] = None,
+                 autolabel: bool = False,
+                 autolabel_window: int = 1,
+                 autocategory: bool = True,
+                 max_retries: int = 1,
+                 init_command: str = "",
+                 worker_options: str = "",
+                 full_debug: bool = True,
+                 worker_executable: str = 'work_queue_worker',
+                 function_dir: Optional[str] = None,
+                 coprocess: bool = False):
         BlockProviderExecutor.__init__(self, provider=provider,
                                        block_error_handler=True)
+        if not _work_queue_enabled:
+            raise OptionalModuleMissing(['work_queue'], "WorkQueueExecutor requires the work_queue module.")
 
-        # Raise an exception if there's a problem importing TaskVine
-        if not _taskvine_enabled:
-            raise OptionalModuleMissing(['taskvine'], "TaskVineExecutor requires the taskvine module.")
-
-        # Executor configurations
         self.label = label
-        self.use_factory = use_factory
-        self.manager_config = manager_config
-        self.factory_config = factory_config
+        self.task_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
+        self.collector_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
+        self.blocks = {}  # type: Dict[str, str]
+        self.address = address
+        self.port = port
+        self.executor_task_counter = -1
+        self.project_name = project_name
+        self.project_password_file = project_password_file
+        self.env = env
+        self.init_command = init_command
+        self.shared_fs = shared_fs
         self.storage_access = storage_access
-
-        # Queue to send ready tasks from TaskVine executor process to TaskVine manager process
-        self.ready_task_queue: multiprocessing.Queue = multiprocessing.Queue()
-
-        # Queue to send finished tasks from TaskVine manager process to TaskVine executor process
-        self.finished_task_queue: multiprocessing.Queue = multiprocessing.Queue()
-
-        # Value to signal whether the manager and factory processes should stop running
+        self.use_cache = use_cache
+        self.working_dir = working_dir
+        self.registered_files: Set[str] = set()
+        self.full_debug = full_debug
+        self.source = True if pack else source
+        self.pack = pack
+        self.extra_pkgs = extra_pkgs or []
+        self.autolabel = autolabel
+        self.autolabel_window = autolabel_window
+        self.autocategory = autocategory
+        self.max_retries = max_retries
         self.should_stop = multiprocessing.Value(c_bool, False)
-
-        # TaskVine manager process
-        self.submit_process = None
-
-        # TaskVine factory process
-        self.factory_process = None
-
-        # Executor thread to collect results from TaskVine manager and set
-        # tasks' futures to done status.
-        self.collector_thread = None
-
-        # track task id of submitted parsl tasks
-        # task ids are incremental and start from 0
-        self.executor_task_counter = 0
-
-        # track number of tasks that are waiting/running
-        self.outstanding_tasks = 0
-
-        # Lock for threads to access self.outstanding_tasks attribute
-        self.outstanding_tasks_lock = threading.Lock()
-
-        # Threading lock to manage self.tasks dictionary object, which maps a task id
-        # to its future object.
-        self.tasks_lock = threading.Lock()
-
-        # Worker command to be given to an execution provider (e.g., local or Condor)
-        self.worker_command = ""
-
-        # Path to directory that holds all tasks' data and results, only used when
-        # manager's task mode is 'regular'.
-        self.function_data_dir = ""
-
-        # helper scripts to prepare package tarballs for Parsl apps
-        self.package_analyze_script = shutil.which("poncho_package_analyze")
-        self.package_create_script = shutil.which("poncho_package_create")
+        self.cached_envs = {}  # type: Dict[int, str]
+        self.worker_options = worker_options
+        self.worker_executable = worker_executable
+        self.function_dir = function_dir
+        self.coprocess = coprocess
+
+        if not self.address:
+            self.address = socket.gethostname()
+
+        if self.project_password_file is not None and not os.path.exists(self.project_password_file):
+            raise WorkQueueFailure('Could not find password file: {}'.format(self.project_password_file))
+
+        if self.project_password_file is not None:
+            if os.path.exists(self.project_password_file) is False:
+                logger.debug("Password File does not exist, no file used")
+                self.project_password_file = None
+
+        # Build foundations of the launch command
+        self.launch_cmd = ("{package_prefix}python3 exec_parsl_function.py {mapping} {function} {result}")
+        if self.init_command != "":
+            self.launch_cmd = self.init_command + "; " + self.launch_cmd
 
     def _get_launch_command(self, block_id):
-        # Implements BlockProviderExecutor's abstract method.
-        # This executor uses different terminology for worker/launch
-        # commands than in htex.
+        # this executor uses different terminology for worker/launch
+        # commands than in htex
         return f"PARSL_WORKER_BLOCK_ID={block_id} {self.worker_command}"
 
-    def __synchronize_manager_factory_comm_settings(self):
-        # Synchronize the communication settings between the manager and the factory
-        # so the factory can direct workers to contact the manager.
-
-        # If the manager can choose any available port (port number = 0),
-        # then it must have a project name
-        # so the factory can look it up. Otherwise the factory process will not know the
-        # port number as it's only chosen when the TaskVine manager process is run.
-        if self.manager_config.port == 0 and self.manager_config.project_name is None:
-            self.manager_config.project_name = "parsl-vine-" + str(uuid.uuid4())
-
-        # guess the host name if the project name is not given
-        if not self.manager_config.project_name:
-            self.manager_config.address = get_any_address()
-
-        # Factory communication settings are overridden by manager communication settings.
-        self.factory_config._project_port = self.manager_config.port
-        self.factory_config._project_address = self.manager_config.address
-        self.factory_config._project_name = self.manager_config.project_name
-        self.factory_config._project_password_file = self.manager_config.project_password_file
-
-    def __create_data_and_logging_dirs(self):
-        # Create neccessary data and logging directories
-
-        # Use the current run directory from Parsl
-        run_dir = self.run_dir
-
-        # Create directories for data and results
-        self.function_data_dir = os.path.join(run_dir, self.label, "function_data")
-        log_dir = os.path.join(run_dir, self.label)
-        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, log_dir))
-        os.makedirs(log_dir)
-        os.makedirs(self.function_data_dir)
-
-        # put TaskVine logs inside run directory of Parsl by default
-        if self.manager_config.vine_log_dir is None:
-            self.manager_config.vine_log_dir = log_dir
-            self.factory_config.scratch_dir = log_dir
-
     def start(self):
         """Create submit process and collector thread to create, send, and
-        retrieve Parsl tasks within the TaskVine system.
+        retrieve Parsl tasks within the Work Queue system.
         """
+        self.tasks_lock = threading.Lock()
 
-        # Synchronize connection and communication settings between the manager and factory
-        self.__synchronize_manager_factory_comm_settings()
+        # Create directories for data and results
+        if not self.function_dir:
+            self.function_data_dir = os.path.join(self.run_dir, self.label, "function_data")
+        else:
+            tp = str(time.time())
+            tx = os.path.join(self.function_dir, tp)
+            os.makedirs(tx)
+            self.function_data_dir = os.path.join(self.function_dir, tp, self.label, "function_data")
+        self.package_dir = os.path.join(self.run_dir, self.label, "package_data")
+        self.wq_log_dir = os.path.join(self.run_dir, self.label)
+        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, self.wq_log_dir))
+        os.makedirs(self.wq_log_dir)
+        os.makedirs(self.function_data_dir)
+        os.makedirs(self.package_dir)
 
-        # Create data and logging dirs
-        self.__create_data_and_logging_dirs()
+        logger.debug("Starting WorkQueueExecutor")
 
-        logger.debug("Starting TaskVineExecutor")
+        self._port_mailbox = multiprocessing.Queue()
 
-        # Create a process to run the TaskVine manager.
-        submit_process_kwargs = {"ready_task_queue": self.ready_task_queue,
-                                 "finished_task_queue": self.finished_task_queue,
+        # Create a Process to perform WorkQueue submissions
+        submit_process_kwargs = {"task_queue": self.task_queue,
+                                 "launch_cmd": self.launch_cmd,
+                                 "data_dir": self.function_data_dir,
+                                 "collector_queue": self.collector_queue,
+                                 "full": self.full_debug,
+                                 "shared_fs": self.shared_fs,
+                                 "autolabel": self.autolabel,
+                                 "autolabel_window": self.autolabel_window,
+                                 "autocategory": self.autocategory,
+                                 "max_retries": self.max_retries,
                                  "should_stop": self.should_stop,
-                                 "manager_config": self.manager_config}
-        self.submit_process = multiprocessing.Process(target=_taskvine_submit_wait,
-                                                      name="TaskVine-Submit-Process",
+                                 "port": self.port,
+                                 "wq_log_dir": self.wq_log_dir,
+                                 "project_password_file": self.project_password_file,
+                                 "project_name": self.project_name,
+                                 "port_mailbox": self._port_mailbox,
+                                 "coprocess": self.coprocess
+                                 }
+        self.submit_process = multiprocessing.Process(target=_work_queue_submit_wait,
+                                                      name="WorkQueue-Submit-Process",
                                                       kwargs=submit_process_kwargs)
 
-        # Create a process to run the TaskVine factory if enabled.
-        if self.use_factory:
-            factory_process_kwargs = {"should_stop": self.should_stop,
-                                      "factory_config": self.factory_config}
-            self.factory_process = multiprocessing.Process(target=_taskvine_factory,
-                                                           name="TaskVine-Factory-Process",
-                                                           kwargs=factory_process_kwargs)
-
-        # Run thread to collect results and set tasks' futures.
-        self.collector_thread = threading.Thread(target=self._collect_taskvine_results,
-                                                 name="TaskVine-Collector-Thread")
-        # Interpreter can exit without waiting for this thread.
+        self.collector_thread = threading.Thread(target=self._collect_work_queue_results,
+                                                 name="WorkQueue-collector-thread")
         self.collector_thread.daemon = True
 
-        # Begin work
+        # Begin both processes
         self.submit_process.start()
+        self.collector_thread.start()
 
-        # Run worker scaler either with Parsl provider or TaskVine factory
-        if self.use_factory:
-            self.factory_process.start()
-        else:
-            self.initialize_scaling()
+        self._chosen_port = self._port_mailbox.get(timeout=60)
 
-        self.collector_thread.start()
+        logger.debug(f"Chosen listening port is {self._chosen_port}")
 
-        logger.debug("All components in TaskVineExecutor started")
+        # Initialize scaling for the provider
+        self.initialize_scaling()
 
     def _path_in_task(self, executor_task_id, *path_components):
-        """
-        Only used when task mode is `regular`.
-        Returns a filename fixed and specific to a task.
+        """Returns a filename specific to a task.
         It is used for the following filename's:
             (not given): The subdirectory per task that contains function, result, etc.
             'function': Pickled file that contains the function to be executed.
             'result': Pickled file that (will) contain the result of the function.
-            'map': Pickled file with a dict between local parsl names, and remote taskvine names.
+            'map': Pickled file with a dict between local parsl names, and remote work queue names.
         """
         task_dir = "{:04d}".format(executor_task_id)
         return os.path.join(self.function_data_dir, task_dir, *path_components)
 
     def submit(self, func, resource_specification, *args, **kwargs):
         """Processes the Parsl app by its arguments and submits the function
-        information to the task queue, to be executed using the TaskVine
+        information to the task queue, to be executed using the Work Queue
         system. The args and kwargs are processed for input and output files to
-        the Parsl app, so that the files are appropriately specified for the TaskVine task.
+        the Parsl app, so that the files are appropriately specified for the Work
+        Queue task.
 
         Parameters
         ----------
 
         func : function
-            Parsl app to be submitted to the TaskVine system
-        resource_specification: dict
-            Dictionary containing relevant info about task.
-            Include information about resources of task, execution mode
-            of task (out of {regular, python, serverless}), and which app
-            type this function was submitted as (out of {python, bash}).
+            Parsl app to be submitted to the Work Queue system
         args : list
             Arguments to the Parsl app
         kwargs : dict
             Keyword arguments to the Parsl app
         """
-
-        # Default execution mode of apps is regular (using TaskVineExecutor serialization and execution mode)
-        exec_mode = resource_specification.get('exec_mode', 'regular')
-
-        logger.debug(f'Got resource specification: {resource_specification}')
-
-        # Detect resources and features of a submitted Parsl app
         cores = None
         memory = None
         disk = None
         gpus = None
         priority = None
         category = None
         running_time_min = None
         if resource_specification and isinstance(resource_specification, dict):
-            for k in resource_specification:
+            logger.debug("Got resource_specification: {}".format(resource_specification))
+
+            required_resource_types = set(['cores', 'memory', 'disk'])
+            acceptable_fields = set(['cores', 'memory', 'disk', 'gpus', 'priority', 'running_time_min'])
+            keys = set(resource_specification.keys())
+
+            if not keys.issubset(acceptable_fields):
+                message = "Task resource specification only accepts these types of resources: {}".format(
+                        ', '.join(acceptable_fields))
+                logger.error(message)
+                raise ExecutorError(self, message)
+
+            # this checks that either all of the required resource types are specified, or
+            # that none of them are: the `required_resource_types` are not actually required,
+            # but if one is specified, then they all must be.
+            key_check = required_resource_types.intersection(keys)
+            required_keys_ok = len(key_check) == 0 or key_check == required_resource_types
+            if not self.autolabel and not required_keys_ok:
+                logger.error("Running with `autolabel=False`. In this mode, "
+                             "task resource specification requires "
+                             "three resources to be specified simultaneously: cores, memory, and disk")
+                raise ExecutorError(self, "Task resource specification requires "
+                                          "three resources to be specified simultaneously: cores, memory, and disk. "
+                                          "Try setting autolabel=True if you are unsure of the resource usage")
+
+            for k in keys:
                 if k == 'cores':
                     cores = resource_specification[k]
                 elif k == 'memory':
                     memory = resource_specification[k]
                 elif k == 'disk':
                     disk = resource_specification[k]
                 elif k == 'gpus':
@@ -338,194 +433,194 @@
                 elif k == 'priority':
                     priority = resource_specification[k]
                 elif k == 'category':
                     category = resource_specification[k]
                 elif k == 'running_time_min':
                     running_time_min = resource_specification[k]
 
-        # Assign executor task id to app
-        executor_task_id = self.executor_task_counter
         self.executor_task_counter += 1
+        executor_task_id = self.executor_task_counter
 
-        # Create a per task directory for the function, map, and result files
+        # Create a per task directory for the function, result, map, and result files
         os.mkdir(self._path_in_task(executor_task_id))
 
         input_files = []
         output_files = []
 
-        # Determine whether to stage input files that will exist at the workers
-        # Input and output files are always cached
+        # Determine the input and output files that will exist at the workes:
         input_files += [self._register_file(f) for f in kwargs.get("inputs", []) if isinstance(f, File)]
         output_files += [self._register_file(f) for f in kwargs.get("outputs", []) if isinstance(f, File)]
 
         # Also consider any *arg that looks like a file as an input:
         input_files += [self._register_file(f) for f in args if isinstance(f, File)]
 
         for kwarg, maybe_file in kwargs.items():
             # Add appropriate input and output files from "stdout" and "stderr" keyword arguments
             if kwarg == "stdout" or kwarg == "stderr":
                 if maybe_file:
-                    output_files.append(self._std_output_to_vine(kwarg, maybe_file))
+                    output_files.append(self._std_output_to_wq(kwarg, maybe_file))
             # For any other keyword that looks like a file, assume it is an input file
             elif isinstance(maybe_file, File):
                 input_files.append(self._register_file(maybe_file))
 
         # Create a Future object and have it be mapped from the task ID in the tasks dictionary
         fu = Future()
         fu.parsl_executor_task_id = executor_task_id
+        logger.debug("Getting tasks_lock to set WQ-level task entry")
         with self.tasks_lock:
+            logger.debug("Got tasks_lock to set WQ-level task entry")
             self.tasks[str(executor_task_id)] = fu
 
-        logger.debug("Creating task {} for function {} of type {} with args {}".format(executor_task_id, func, type(func), args))
+        logger.debug("Creating executor task {} for function {} with args {}".format(executor_task_id, func, args))
 
-        function_file = None
-        result_file = None
-        map_file = None
-        # Use executor's serialization method if app mode is 'regular'
-        if exec_mode == 'regular':
-            # Get path to files that will contain the pickled function, result, and map of input and output files
-            function_file = self._path_in_task(executor_task_id, "function")
-            result_file = self._path_in_task(executor_task_id, "result")
-            map_file = self._path_in_task(executor_task_id, "map")
-
-            logger.debug("Creating executor task {} with function at: {} and result to be found at: {}".format(executor_task_id, function_file, result_file))
+        function_file = self._path_in_task(executor_task_id, "function")
+        result_file = self._path_in_task(executor_task_id, "result")
+        map_file = self._path_in_task(executor_task_id, "map")
 
-            # Pickle the result into object to pass into message buffer
-            self._serialize_function(function_file, func, args, kwargs)
+        logger.debug("Creating executor task {} with function at: {}".format(executor_task_id, function_file))
+        logger.debug("Creating executor task {} with result to be found at: {}".format(executor_task_id, result_file))
 
-            # Construct the map file of local filenames at worker
-            self._construct_map_file(map_file, input_files, output_files)
+        self._serialize_function(function_file, func, args, kwargs)
 
-        # Register a tarball containing all package dependencies for this app if instructed
-        if self.manager_config.app_pack:
+        if self.pack:
             env_pkg = self._prepare_package(func, self.extra_pkgs)
         else:
             env_pkg = None
 
+        logger.debug("Constructing map for local filenames at worker for executor task {}".format(executor_task_id))
+        self._construct_map_file(map_file, input_files, output_files)
+
         if not self.submit_process.is_alive():
-            raise ExecutorError(self, "taskvine Submit Process is not alive")
+            raise ExecutorError(self, "Workqueue Submit Process is not alive")
 
         # Create message to put into the message queue
-        logger.debug("Placing task {} on message queue".format(executor_task_id))
-
-        # Put apps into their categories based on function name if enabled
+        logger.debug("Placing executor task {} on message queue".format(executor_task_id))
         if category is None:
-            category = func.__name__ if self.manager_config.autocategory else 'parsl-default'
-
-        # support for python and serverless exec mode delayed
-        if exec_mode == 'python' or exec_mode == 'serverless':
-            raise UnsupportedFeatureError(f'Execution mode {exec_mode} is not currently supported.', 'TaskVineExecutor', None)
-        task_info = ParslTaskToVine(executor_id=executor_task_id,
-                                    exec_mode=exec_mode,
-                                    category=category,
-                                    input_files=input_files,
-                                    output_files=output_files,
-                                    map_file=map_file,
-                                    function_file=function_file,
-                                    result_file=result_file,
-                                    cores=cores,
-                                    memory=memory,
-                                    disk=disk,
-                                    gpus=gpus,
-                                    priority=priority,
-                                    running_time_min=running_time_min,
-                                    env_pkg=env_pkg)
-
-        # Send ready task to manager process
-        self.ready_task_queue.put_nowait(task_info)
-
-        # Increment outstanding task counter
-        with self.outstanding_tasks_lock:
-            self.outstanding_tasks += 1
+            category = func.__name__ if self.autocategory else 'parsl-default'
+        self.task_queue.put_nowait(ParslTaskToWq(executor_task_id,
+                                                 category,
+                                                 cores,
+                                                 memory,
+                                                 disk,
+                                                 gpus,
+                                                 priority,
+                                                 running_time_min,
+                                                 env_pkg,
+                                                 map_file,
+                                                 function_file,
+                                                 result_file,
+                                                 input_files,
+                                                 output_files))
 
         return fu
 
     def _construct_worker_command(self):
-        worker_command = self.factory_config.worker_executable
-        if self.factory_config._project_password_file:
-            worker_command += ' --password {}'.format(self.factory_config._project_password_file)
-        if self.factory_config.worker_options:
-            worker_command += ' {}'.format(self.factory_config.worker_options)
-        if self.factory_config._project_name:
-            worker_command += ' -M {}'.format(self.factory_config._project_name)
+        worker_command = self.worker_executable
+        if self.coprocess:
+            worker_command += " --coprocess parsl_coprocess.py"
+        if self.project_password_file:
+            worker_command += ' --password {}'.format(self.project_password_file)
+        if self.worker_options:
+            worker_command += ' {}'.format(self.worker_options)
+        if self.project_name:
+            worker_command += ' -M {}'.format(self.project_name)
         else:
-            worker_command += ' {} {}'.format(self.factory_config._project_address, self.factory_config._project_port)
+            worker_command += ' {} {}'.format(self.address, self._chosen_port)
 
         logger.debug("Using worker command: {}".format(worker_command))
         return worker_command
 
     def _patch_providers(self):
         # Add the worker and password file to files that the provider needs to stage.
         # (Currently only for the CondorProvider)
         if isinstance(self.provider, CondorProvider):
-            path_to_worker = shutil.which('vine_worker')
+            path_to_worker = shutil.which('work_queue_worker')
             self.worker_command = './' + self.worker_command
             self.provider.transfer_input_files.append(path_to_worker)
             if self.project_password_file:
                 self.provider.transfer_input_files.append(self.project_password_file)
 
     def _serialize_function(self, fn_path, parsl_fn, parsl_fn_args, parsl_fn_kwargs):
         """Takes the function application parsl_fn(*parsl_fn_args, **parsl_fn_kwargs)
         and serializes it to the file fn_path."""
-        function_info = {"byte code": pack_apply_message(parsl_fn, parsl_fn_args, parsl_fn_kwargs,
-                                                         buffer_threshold=1024 * 1024)}
+
+        # Either build a dictionary with the source of the function, or pickle
+        # the function directly:
+        if self.source:
+            function_info = {"source code": inspect.getsource(parsl_fn),
+                             "name": parsl_fn.__name__,
+                             "args": parsl_fn_args,
+                             "kwargs": parsl_fn_kwargs}
+        else:
+            function_info = {"byte code": pack_apply_message(parsl_fn, parsl_fn_args, parsl_fn_kwargs,
+                                                             buffer_threshold=1024 * 1024)}
 
         with open(fn_path, "wb") as f_out:
             pickle.dump(function_info, f_out)
 
     def _construct_map_file(self, map_file, input_files, output_files):
         """ Map local filepath of parsl files to the filenames at the execution worker.
         If using a shared filesystem, the filepath is mapped to its absolute filename.
-        Otherwise, to its original relative filename. In this later case, taskvine
+        Otherwise, to its original relative filename. In this later case, work queue
         recreates any directory hierarchy needed."""
         file_translation_map = {}
         for spec in itertools.chain(input_files, output_files):
-            local_name = spec.parsl_name
-            if self.manager_config.shared_fs:
+            local_name = spec[0]
+            if self.shared_fs:
                 remote_name = os.path.abspath(local_name)
             else:
                 remote_name = local_name
             file_translation_map[local_name] = remote_name
         with open(map_file, "wb") as f_out:
             pickle.dump(file_translation_map, f_out)
 
     def _register_file(self, parsl_file):
         """Generates a tuple (parsl_file.filepath, stage, cache) to give to
-        taskvine. cache is always True.
-        stage is True if the file has a relative path. (i.e., not
-        a URL or an absolute path)"""
-        to_cache = True
+        work queue. cache is always False if self.use_cache is False.
+        Otherwise, it is set to True if parsl_file is used more than once.
+        stage is True if the file needs to be copied by work queue. (i.e., not
+        a URL or an absolute path)
+
+        It has the side-effect of adding parsl_file to a list of registered
+        files.
+
+        Note: The first time a file is used cache is set to False. Since
+        tasks are generated dynamically, without other information this is
+        the best we can do."""
+        to_cache = False
+        if self.use_cache:
+            to_cache = parsl_file in self.registered_files
+
         to_stage = False
-        if parsl_file.scheme == 'file' or \
-           (parsl_file.local_path and os.path.exists(parsl_file.local_path)):
+        if parsl_file.scheme == 'file' or (parsl_file.local_path and os.path.exists(parsl_file.local_path)):
             to_stage = not os.path.isabs(parsl_file.filepath)
 
-        return ParslFileToVine(parsl_file.filepath, to_stage, to_cache)
+        self.registered_files.add(parsl_file)
 
-    def _std_output_to_vine(self, fdname, stdfspec):
+        return ParslFileToWq(parsl_file.filepath, to_stage, to_cache)
+
+    def _std_output_to_wq(self, fdname, stdfspec):
         """Find the name of the file that will contain stdout or stderr and
-        return a ParslFileToVine with it. These files are never cached"""
+        return a ParslFileToWq with it. These files are never cached"""
         fname, mode = putils.get_std_fname_mode(fdname, stdfspec)
         to_stage = not os.path.isabs(fname)
-        return ParslFileToVine(fname, stage=to_stage, cache=False)
+        return ParslFileToWq(fname, stage=to_stage, cache=False)
 
     def _prepare_package(self, fn, extra_pkgs):
-        """ Look at source code of apps to figure out their package depedencies
-        and output a tarball containing those to send along with tasks for execution."""
         fn_id = id(fn)
         fn_name = fn.__name__
         if fn_id in self.cached_envs:
             logger.debug("Skipping analysis of %s, previously got %s", fn_name, self.cached_envs[fn_id])
             return self.cached_envs[fn_id]
         source_code = inspect.getsource(fn).encode()
         pkg_dir = os.path.join(tempfile.gettempdir(), "python_package-{}".format(os.geteuid()))
         os.makedirs(pkg_dir, exist_ok=True)
         with tempfile.NamedTemporaryFile(suffix='.yaml') as spec:
             logger.info("Analyzing dependencies of %s", fn_name)
-            analyze_cmdline = [self.package_analyze_script, exec_parsl_function.__file__, '-', spec.name]
+            analyze_cmdline = [package_analyze_script, exec_parsl_function.__file__, '-', spec.name]
             for p in extra_pkgs:
                 analyze_cmdline += ["--extra-pkg", p]
             subprocess.run(analyze_cmdline, input=source_code, check=True)
             with open(spec.name, mode='rb') as f:
                 spec_hash = hashlib.sha256(f.read()).hexdigest()
                 logger.debug("Spec hash for %s is %s", fn_name, spec_hash)
                 pkg = os.path.join(pkg_dir, "pack-{}.tar.gz".format(spec_hash))
@@ -533,517 +628,397 @@
                 self.cached_envs[fn_id] = pkg
                 logger.debug("Cached package for %s found at %s", fn_name, pkg)
                 return pkg
             (fd, tarball) = tempfile.mkstemp(dir=pkg_dir, prefix='.tmp', suffix='.tar.gz')
             os.close(fd)
             logger.info("Creating dependency package for %s", fn_name)
             logger.debug("Writing deps for %s to %s", fn_name, tarball)
-            subprocess.run([self.package_create_script, spec.name, tarball], stdout=subprocess.DEVNULL, check=True)
+            subprocess.run([package_create_script, spec.name, tarball], stdout=subprocess.DEVNULL, check=True)
             logger.debug("Done with conda-pack; moving %s to %s", tarball, pkg)
             os.rename(tarball, pkg)
             self.cached_envs[fn_id] = pkg
             return pkg
 
     def initialize_scaling(self):
         """ Compose the launch command and call scale out
 
         Scales the workers to the appropriate nodes with provider
         """
         # Start scaling in/out
-        logger.debug("Starting TaskVineExecutor with provider: %s", self.provider)
+        logger.debug("Starting WorkQueueExecutor with provider: %s", self.provider)
         self.worker_command = self._construct_worker_command()
         self._patch_providers()
 
         if hasattr(self.provider, 'init_blocks'):
             try:
                 self.scale_out(blocks=self.provider.init_blocks)
             except Exception as e:
                 logger.error("Initial block scaling out failed: {}".format(e))
                 raise e
 
     @property
     def outstanding(self) -> int:
-        """Count the number of outstanding tasks."""
-        logger.debug(f"Counted {self.outstanding_tasks} outstanding tasks")
-        return self.outstanding_tasks
+        """Count the number of outstanding tasks. This is inefficiently
+        implemented and probably could be replaced with a counter.
+        """
+        outstanding = 0
+        with self.tasks_lock:
+            for fut in self.tasks.values():
+                if not fut.done():
+                    outstanding += 1
+        logger.debug(f"Counted {outstanding} outstanding tasks")
+        return outstanding
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
     def scale_in(self, count):
-        """Scale in method. Cancel a given number of blocks
+        """Scale in method.
         """
         # Obtain list of blocks to kill
         to_kill = list(self.blocks.keys())[:count]
         kill_ids = [self.blocks[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
             self.provider.cancel(kill_ids)
         else:
             logger.error("No execution provider available to scale")
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
-        collector thread, which shuts down the TaskVine system submission.
+        collector thread, which shuts down the Work Queue system submission.
         """
-        logger.debug("TaskVine shutdown started")
+        logger.debug("Work Queue shutdown started")
         self.should_stop.value = True
 
         # Remove the workers that are still going
         kill_ids = [self.blocks[block] for block in self.blocks.keys()]
         if self.provider:
             logger.debug("Cancelling blocks")
             self.provider.cancel(kill_ids)
 
-        # Join all processes before exiting
         logger.debug("Joining on submit process")
         self.submit_process.join()
         logger.debug("Joining on collector thread")
         self.collector_thread.join()
-        if self.use_factory:
-            logger.debug("Joining on factory process")
-            self.factory_process.join()
 
-        logger.debug("TaskVine shutdown completed")
+        logger.debug("Work Queue shutdown completed")
         return True
 
     @wrap_with_logs
-    def _collect_taskvine_results(self):
-        """Sets the values of tasks' futures completed by taskvine.
+    def _collect_work_queue_results(self):
+        """Sets the values of tasks' futures of tasks completed by work queue.
         """
         logger.debug("Starting Collector Thread")
         try:
             while not self.should_stop.value:
                 if not self.submit_process.is_alive():
-                    raise ExecutorError(self, "taskvine Submit Process is not alive")
+                    raise ExecutorError(self, "Workqueue Submit Process is not alive")
 
-                # Get the result message from the finished_task_queue
+                # Get the result message from the collector_queue
                 try:
-                    task_report = self.finished_task_queue.get(timeout=1)
+                    task_report = self.collector_queue.get(timeout=1)
                 except queue.Empty:
                     continue
 
                 # Obtain the future from the tasks dictionary
                 with self.tasks_lock:
-                    future = self.tasks.pop(task_report.executor_id)
-
-                logger.debug("Updating Future for Parsl Task {}".format(task_report.executor_id))
-                logger.debug(f'task {task_report.executor_id} has result_received set to {task_report.result_received} and result to {task_report.result}')
+                    future = self.tasks.pop(task_report.id)
+                logger.debug("Updating Future for executor task {}".format(task_report.id))
                 if task_report.result_received:
                     future.set_result(task_report.result)
                 else:
                     # If there are no results, then the task failed according to one of
-                    # taskvine modes, such as resource exhaustion.
-                    future.set_exception(TaskVineTaskFailure(task_report.reason, task_report.result))
-
-                # decrement outstanding task counter
-                with self.outstanding_tasks_lock:
-                    self.outstanding_tasks -= 1
+                    # work queue modes, such as resource exhaustion.
+                    future.set_exception(WorkQueueTaskFailure(task_report.reason, task_report.result))
         finally:
-            logger.debug(f"Marking all {self.outstanding} outstanding tasks as failed")
+            logger.debug("Marking all outstanding tasks as failed")
             logger.debug("Acquiring tasks_lock")
             with self.tasks_lock:
                 logger.debug("Acquired tasks_lock")
-                # set exception for tasks waiting for results that taskvine did not execute
+                # set exception for tasks waiting for results that work queue did not execute
                 for fu in self.tasks.values():
                     if not fu.done():
-                        fu.set_exception(TaskVineManagerFailure("taskvine executor failed to execute the task."))
+                        fu.set_exception(WorkQueueFailure("work queue executor failed to execute the task."))
         logger.debug("Exiting Collector Thread")
 
 
 @wrap_with_logs
-def _taskvine_submit_wait(ready_task_queue=None,
-                          finished_task_queue=None,
-                          should_stop=None,
-                          manager_config=None
-                          ):
-    """Process to handle Parsl app submissions to the TaskVine objects.
+def _work_queue_submit_wait(*,
+                            port_mailbox: multiprocessing.Queue,
+                            task_queue: multiprocessing.Queue,
+                            launch_cmd: str,
+                            collector_queue: multiprocessing.Queue,
+                            data_dir: str,
+                            full: bool,
+                            shared_fs: bool,
+                            autolabel: bool,
+                            autolabel_window: int,
+                            autocategory: bool,
+                            max_retries: Optional[int],
+                            should_stop,  # multiprocessing.Value is an awkward type alias from inside multiprocessing
+                            port: int,
+                            wq_log_dir: str,
+                            project_password_file: Optional[str],
+                            project_name: Optional[str],
+                            coprocess: bool) -> int:
+    """Thread to handle Parsl app submissions to the Work Queue objects.
     Takes in Parsl functions submitted using submit(), and creates a
-    TaskVine task with the appropriate specifications, which is then
-    submitted to TaskVine. After tasks are completed, processes the
+    Work Queue task with the appropriate specifications, which is then
+    submitted to Work Queue. After tasks are completed, processes the
     exit status and exit code of the task, and sends results to the
-    TaskVine collector thread.
-    To avoid python's global interpreter lock with taskvine's wait, this
+    Work Queue collector thread.
+    To avoid python's global interpreter lock with work queue's wait, this
     function should be launched as a process, not as a lightweight thread. This
     means that any communication should be done using the multiprocessing
     module capabilities, rather than shared memory.
     """
-    logger.debug("Starting TaskVine Submit/Wait Process")
-    setproctitle("parsl: TaskVine submit/wait")
+    logger.debug("Starting WorkQueue Submit/Wait Process")
+    setproctitle("parsl: Work Queue submit/wait")
 
     # Enable debugging flags and create logging file
-    if manager_config.vine_log_dir is not None:
-        logger.debug("Setting debugging flags and creating logging file at {}".format(manager_config.vine_log_dir))
+    wq_debug_log = None
+    if wq_log_dir is not None:
+        logger.debug("Setting debugging flags and creating logging file")
+        wq_debug_log = os.path.join(wq_log_dir, "debug_log")
 
-    # Create TaskVine queue object
-    logger.debug("Creating TaskVine Object")
+    # Create WorkQueue queue object
+    logger.debug("Creating WorkQueue Object")
     try:
-        logger.debug("Listening on port {}".format(manager_config.port))
-        m = Manager(port=manager_config.port,
-                    name=manager_config.project_name,
-                    run_info_path=manager_config.vine_log_dir)
+        logger.debug("Requested port {}".format(port))
+        q = WorkQueue(port, debug_log=wq_debug_log)
+        port_mailbox.put(q.port)
+        logger.debug("Listening on port {}".format(q.port))
     except Exception as e:
-        logger.error("Unable to create TaskVine object: {}".format(e))
+        logger.error("Unable to create WorkQueue object: {}".format(e))
+        port_mailbox.put(None)
         raise e
 
-    # Specify TaskVine manager attributes
-    if manager_config.project_password_file:
-        m.set_password_file(manager_config.project_password_file)
-
-    # Autolabeling resources require monitoring to be enabled
-    if manager_config.autolabel:
-        m.enable_monitoring()
-        if manager_config.autolabel_window is not None:
-            m.tune('category-steady-n-tasks', manager_config.autolabel_window)
-
-    # Specify number of workers to wait for before sending the first task
-    if manager_config.wait_for_workers:
-        m.tune("wait-for-workers", manager_config.wait_for_workers)
-
-    # Enable peer transfer feature between workers if specified
-    if manager_config.enable_peer_transfers:
-        m.enable_peer_transfers()
+    # Specify WorkQueue queue attributes
+    if project_name:
+        q.specify_name(project_name)
+
+    if project_password_file:
+        q.specify_password_file(project_password_file)
+
+    if autolabel:
+        q.enable_monitoring()
+        if autolabel_window is not None:
+            q.tune('category-steady-n-tasks', autolabel_window)
+
+    # Only write logs when the wq_log_dir is specified, which it most likely will be
+    if wq_log_dir is not None:
+        wq_master_log = os.path.join(wq_log_dir, "master_log")
+        wq_trans_log = os.path.join(wq_log_dir, "transaction_log")
+        if full and autolabel:
+            wq_resource_log = os.path.join(wq_log_dir, "resource_logs")
+            q.enable_monitoring_full(dirname=wq_resource_log)
+        q.specify_log(wq_master_log)
+        q.specify_transactions_log(wq_trans_log)
 
-    # Get parent pid, useful to shutdown this process when its parent, the taskvine
-    # executor process, exits.
     orig_ppid = os.getppid()
 
-    result_file_of_task_id = {}  # Mapping executor task id -> result file for active regular tasks.
-
-    poncho_env_to_file = {}  # Mapping poncho_env file to File object in TaskVine
-
-    # Mapping of parsl local file name to TaskVine File object
-    # dict[str] -> vine File object
-    parsl_file_name_to_vine_file = {}
-
-    # Mapping of tasks from vine id to parsl id
-    # Dict[str] -> str
-    vine_id_to_executor_task_id = {}
-
-    # Find poncho run script to activate an environment tarball
-    poncho_run_script = shutil.which("poncho_package_run")
-
-    # Declare helper scripts as cache-able and peer-transferable
-    package_run_script_file = m.declare_file(poncho_run_script, cache=True, peer_transfer=True)
-    exec_parsl_function_file = m.declare_file(exec_parsl_function.__file__, cache=True, peer_transfer=True)
-
-    logger.debug("Entering main loop of TaskVine manager")
+    result_file_of_task_id = {}  # Mapping executor task id -> result file for active tasks.
 
     while not should_stop.value:
         # Monitor the task queue
         ppid = os.getppid()
         if ppid != orig_ppid:
             logger.debug("new Process")
             break
 
         # Submit tasks
-        while ready_task_queue.qsize() > 0 and not should_stop.value:
-            # Obtain task from ready_task_queue
+        while task_queue.qsize() > 0 and not should_stop.value:
+            # Obtain task from task_queue
             try:
-                task = ready_task_queue.get(timeout=1)
-                logger.debug("Removing executor task from queue")
+                task = task_queue.get(timeout=1)
+                logger.debug("Removing task from queue")
             except queue.Empty:
-                logger.debug("Queue is empty")
                 continue
-            if task.exec_mode == 'regular':
-                # Create command string
-                launch_cmd = "python3 exec_parsl_function.py {mapping} {function} {result}"
-                if manager_config.init_command != '':
-                    launch_cmd = "{init_cmd};" + launch_cmd
-                command_str = launch_cmd.format(init_cmd=manager_config.init_command,
-                                                mapping=os.path.basename(task.map_file),
-                                                function=os.path.basename(task.function_file),
-                                                result=os.path.basename(task.result_file))
-                logger.debug("Sending executor task {} (mode: regular) with command: {}".format(task.executor_id, command_str))
-                try:
-                    t = Task(command_str)
-                except Exception as e:
-                    logger.error("Unable to create executor task (mode:regular): {}".format(e))
-                    finished_task_queue.put_nowait(VineTaskToParsl(executor_id=task.executor_id,
-                                                                   result_received=False,
-                                                                   result=None,
-                                                                   reason="task could not be created by taskvine",
-                                                                   status=-1))
-                    continue
-            else:
-                raise Exception(f'Unrecognized task mode {task.exec_mode}. Exiting...')
 
-            # Add environment file to the task if possible
-            # Prioritize local poncho environment over global poncho environment
-            # (local: use app_pack, global: use env_pack)
-            poncho_env_file = None
-
-            # check if env_pack is specified
-            if manager_config.env_pack is not None:
-                # check if the environment file is not already created
-                if manager_config.env_pack not in poncho_env_to_file:
-                    # if the environment is already packaged as a tarball, then add the file
-                    # otherwise it is an environment name or path, so create a poncho tarball then add it
-                    if not manager_config.env_pack.endswith('.tar.gz'):
-                        env_tarball = str(uuid.uuid4()) + '.tar.gz'
-                        subprocess.run([poncho_run_script, manager_config.env_pack, env_tarball], stdout=subprocess.DEVNULL, check=True)
-                    poncho_env_file = m.declare_poncho(manager_config.env_pack, cache=True, peer_transfer=True)
-                    poncho_env_to_file[manager_config.env_pack] = poncho_env_file
+            try:
+                pkg_pfx = ""
+                if task.env_pkg is not None:
+                    if package_run_script is None:
+                        raise ValueError("package_run_script must be specified")
+                    pkg_pfx = "./{} -e {} ".format(os.path.basename(package_run_script),
+                                                   os.path.basename(task.env_pkg))
+
+                if not coprocess:
+                    # Create command string
+                    logger.debug(launch_cmd)
+                    command_str = launch_cmd.format(package_prefix=pkg_pfx,
+                                                    mapping=os.path.basename(task.map_file),
+                                                    function=os.path.basename(task.function_file),
+                                                    result=os.path.basename(task.result_file))
+                    logger.debug(command_str)
+
+                    # Create WorkQueue task for the command
+                    logger.debug("Sending executor task {} with command: {}".format(task.id, command_str))
+                    t = wq.Task(command_str)
                 else:
-                    poncho_env_file = poncho_env_to_file[manager_config.env_pack]
+                    t = wq.RemoteTask("run_parsl_task",
+                                      "parsl_coprocess",
+                                      os.path.basename(task.map_file),
+                                      os.path.basename(task.function_file),
+                                      os.path.basename(task.result_file))
+                    t.specify_exec_method("direct")
+                    logger.debug("Sending executor task {} to coprocess".format(task.id))
 
-            # check if app_pack is used, override if possible
-            if task.env_pkg is not None:
-                if task.env_pkg not in poncho_env_to_file:
-                    poncho_env_file = m.declare_poncho(task.env_pkg, cache=True, peer_transfer=True)
-                    poncho_env_to_file[task.env_pkg] = poncho_env_file
-                else:
-                    poncho_env_file = poncho_env_to_file[task.env_pkg]
+            except Exception as e:
+                logger.error("Unable to create task: {}".format(e))
+                collector_queue.put_nowait(WqTaskToParsl(id=task.id,
+                                                         result_received=False,
+                                                         result=None,
+                                                         reason="task could not be created by work queue",
+                                                         status=-1))
+                continue
 
-            # Add environment to the task
-            if poncho_env_file is not None:
-                t.add_environment(poncho_env_file)
-                t.add_input(package_run_script_file, "poncho_package_run")
-
-            t.set_category(task.category)
-            if manager_config.autolabel:
-                if manager_config.autolabel_algorithm == 'max-xput':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX_THROUGHPUT)
-                elif manager_config.autolabel_algorithm == 'bucketing':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_EXHAUSTIVE_BUCKETING)
-                elif manager_config.autolabel_algorithm == 'max':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX)
-                else:
-                    logger.warning(f'Unrecognized autolabeling algorithm named {manager_config.autolabel_algorithm} for taskvine manager.')
-                    raise Exception(f'Unrecognized autolabeling algorithm named {manager_config.autolabel_algorithm} for taskvine manager.')
+            t.specify_category(task.category)
+            if autolabel:
+                q.specify_category_mode(task.category, WORK_QUEUE_ALLOCATION_MODE_MAX_THROUGHPUT)
 
             if task.cores is not None:
-                t.set_cores(task.cores)
+                t.specify_cores(task.cores)
             if task.memory is not None:
-                t.set_memory(task.memory)
+                t.specify_memory(task.memory)
             if task.disk is not None:
-                t.set_disk(task.disk)
+                t.specify_disk(task.disk)
             if task.gpus is not None:
-                t.set_gpus(task.gpus)
+                t.specify_gpus(task.gpus)
             if task.priority is not None:
-                t.set_priority(task.priority)
+                t.specify_priority(task.priority)
             if task.running_time_min is not None:
-                t.set_time_min(task.running_time_min)
+                t.specify_running_time_min(task.running_time_min)
 
-            if manager_config.max_retries is not None:
-                logger.debug(f"Specifying max_retries {manager_config.max_retries}")
-                t.set_retries(manager_config.max_retries)
+            if max_retries is not None:
+                logger.debug(f"Specifying max_retries {max_retries}")
+                t.specify_max_retries(max_retries)
             else:
                 logger.debug("Not specifying max_retries")
 
-            # Specify environment variables for the task
-            if manager_config.env_vars is not None:
-                for var in manager_config.env_vars:
-                    t.set_env_var(str(var), str(manager_config.env_vars[var]))
-
-            if task.exec_mode == 'regular':
-                # Add helper files that execute parsl functions on remote nodes
-                # only needed for tasks with 'regular' mode
-                t.add_input(exec_parsl_function_file, "exec_parsl_function.py")
-
-                # Declare and add task-specific function, data, and result files to task
-                task_function_file = m.declare_file(task.function_file, cache=False, peer_transfer=False)
-                t.add_input(task_function_file, "function")
-
-                task_map_file = m.declare_file(task.map_file, cache=False, peer_transfer=False)
-                t.add_input(task_map_file, "map")
-
-                task_result_file = m.declare_file(task.result_file, cache=False, peer_transfer=False)
-                t.add_output(task_result_file, "result")
+            if task.env_pkg is not None:
+                t.specify_input_file(package_run_script, cache=True)
+                t.specify_input_file(task.env_pkg, cache=True)
 
-                result_file_of_task_id[str(task.executor_id)] = task.result_file
+            # Specify script, and data/result files for task
+            t.specify_input_file(exec_parsl_function.__file__, cache=True)
+            t.specify_input_file(task.function_file, cache=False)
+            t.specify_input_file(task.map_file, cache=False)
+            t.specify_output_file(task.result_file, cache=False)
+            t.specify_tag(str(task.id))
+            result_file_of_task_id[str(task.id)] = task.result_file
 
-            logger.debug("Executor task id: {}".format(task.executor_id))
+            logger.debug("Executor task id: {}".format(task.id))
 
             # Specify input/output files that need to be staged.
             # Absolute paths are assumed to be in shared filesystem, and thus
-            # not staged by taskvine.
-            # Files that share the same local path are assumed to be the same
-            # and thus use the same Vine File object if detected.
-            if not manager_config.shared_fs:
+            # not staged by work queue.
+            if not shared_fs:
                 for spec in task.input_files:
                     if spec.stage:
-                        if spec.parsl_name in parsl_file_name_to_vine_file:
-                            task_in_file = parsl_file_name_to_vine_file[spec.parsl_name]
-                        else:
-                            task_in_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
-                            parsl_file_name_to_vine_file[spec.parsl_name] = task_in_file
-                        t.add_input(task_in_file, spec.parsl_name)
-
+                        t.specify_input_file(spec.parsl_name, spec.parsl_name, cache=spec.cache)
                 for spec in task.output_files:
                     if spec.stage:
-                        if spec.parsl_name in parsl_file_name_to_vine_file:
-                            task_out_file = parsl_file_name_to_vine_file[spec.parsl_name]
-                        else:
-                            task_out_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
-                        t.add_output(task_out_file, spec.parsl_name)
+                        t.specify_output_file(spec.parsl_name, spec.parsl_name, cache=spec.cache)
 
-            # Submit the task to the TaskVine object
-            logger.debug("Submitting executor task {}, {} to TaskVine".format(task.executor_id, t))
+            # Submit the task to the WorkQueue object
+            logger.debug("Submitting executor task {} to WorkQueue".format(task.id))
             try:
-                vine_id = m.submit(t)
-                logger.debug("Submitted executor task {} to TaskVine".format(task.executor_id))
-                vine_id_to_executor_task_id[str(vine_id)] = str(task.executor_id), task.exec_mode
+                wq_id = q.submit(t)
             except Exception as e:
-                logger.error("Unable to submit task to taskvine: {}".format(e))
-                finished_task_queue.put_nowait(VineTaskToParsl(executor_id=task.executor_id,
-                                                               result_received=False,
-                                                               result=None,
-                                                               reason="task could not be submited to taskvine",
-                                                               status=-1))
+                logger.error("Unable to submit task to work queue: {}".format(e))
+                collector_queue.put_nowait(WqTaskToParsl(id=task.id,
+                                                         result_received=False,
+                                                         result=None,
+                                                         reason="task could not be submited to work queue",
+                                                         status=-1))
                 continue
+            logger.info("Executor task {} submitted as Work Queue task {}".format(task.id, wq_id))
 
-            logger.debug("Executor task {} submitted as TaskVine task with id {}".format(task.executor_id, vine_id))
-
-        # If the queue is not empty wait on the TaskVine queue for a task
+        # If the queue is not empty wait on the WorkQueue queue for a task
         task_found = True
-        if not m.empty():
+        if not q.empty():
             while task_found and not should_stop.value:
                 # Obtain the task from the queue
-                t = m.wait(1)
+                t = q.wait(1)
                 if t is None:
                     task_found = False
                     continue
-                logger.debug('Found a task')
-                executor_task_id = vine_id_to_executor_task_id[str(t.id)][0]
-                exec_mode_of_task = vine_id_to_executor_task_id[str(t.id)][1]
-                vine_id_to_executor_task_id.pop(str(t.id))
-                # When a task is found
-                if exec_mode_of_task == 'regular':
-                    result_file = result_file_of_task_id.pop(executor_task_id)
-
-                    logger.debug(f"completed executor task info: {executor_task_id}, {t.category}, {t.command}, {t.std_output}")
-
-                    # A tasks completes 'succesfully' if it has result file,
-                    # and it can be loaded. This may mean that the 'success' is
-                    # an exception.
-                    logger.debug("Looking for result in {}".format(result_file))
-                    try:
-                        with open(result_file, "rb") as f_in:
-                            result = pickle.load(f_in)
-                        logger.debug("Found result in {}".format(result_file))
-                        finished_task_queue.put_nowait(VineTaskToParsl(executor_id=executor_task_id,
-                                                                       result_received=True,
-                                                                       result=result,
-                                                                       reason=None,
-                                                                       status=t.exit_code))
-                    # If a result file could not be generated, explain the
-                    # failure according to taskvine error codes. We generate
-                    # an exception and wrap it with RemoteExceptionWrapper, to
-                    # match the positive case.
-                    except Exception as e:
-                        reason = _explain_taskvine_result(t)
-                        logger.debug("Did not find result in {}".format(result_file))
-                        logger.debug("Wrapper Script status: {}\nTaskVine Status: {}"
-                                     .format(t.exit_code, t.result))
-                        logger.debug("Task with executor id {} / vine id {} failed because:\n{}"
-                                     .format(executor_task_id, t.id, reason))
-                        finished_task_queue.put_nowait(VineTaskToParsl(executor_id=executor_task_id,
-                                                                       result_received=False,
-                                                                       result=e,
-                                                                       reason=reason,
-                                                                       status=t.exit_code))
-                else:
-                    raise Exception(f'Unknown exec mode for executor task {executor_task_id}: {exec_mode_of_task}.')
-
-    logger.debug("Exiting TaskVine Monitoring Process")
+                # When a task is found:
+                executor_task_id = t.tag
+                logger.debug("Completed Work Queue task {}, executor task {}".format(t.id, t.tag))
+                result_file = result_file_of_task_id.pop(t.tag)
+
+                # A tasks completes 'succesfully' if it has result file,
+                # and it can be loaded. This may mean that the 'success' is
+                # an exception.
+                logger.debug("Looking for result in {}".format(result_file))
+                try:
+                    with open(result_file, "rb") as f_in:
+                        result = pickle.load(f_in)
+                    logger.debug("Found result in {}".format(result_file))
+                    collector_queue.put_nowait(WqTaskToParsl(id=executor_task_id,
+                                                             result_received=True,
+                                                             result=result,
+                                                             reason=None,
+                                                             status=t.return_status))
+                # If a result file could not be generated, explain the
+                # failure according to work queue error codes. We generate
+                # an exception and wrap it with RemoteExceptionWrapper, to
+                # match the positive case.
+                except Exception as e:
+                    reason = _explain_work_queue_result(t)
+                    logger.debug("Did not find result in {}".format(result_file))
+                    logger.debug("Wrapper Script status: {}\nWorkQueue Status: {}"
+                                 .format(t.return_status, t.result))
+                    logger.debug("Task with executor id {} / Work Queue id {} failed because:\n{}"
+                                 .format(executor_task_id, t.id, reason))
+                    collector_queue.put_nowait(WqTaskToParsl(id=executor_task_id,
+                                                             result_received=False,
+                                                             result=e,
+                                                             reason=reason,
+                                                             status=t.return_status))
+    logger.debug("Exiting WorkQueue Monitoring Process")
     return 0
 
 
-def _explain_taskvine_result(vine_task):
-    """Returns a string with the reason why a task failed according to taskvine."""
+def _explain_work_queue_result(wq_task):
+    """Returns a string with the reason why a task failed according to work queue."""
 
-    vine_result = vine_task.result
+    wq_result = wq_task.result
 
-    reason = "taskvine result: "
-    if vine_result == cvine.VINE_RESULT_SUCCESS:
-        reason += "succesful execution with exit code {}".format(vine_task.return_status)
-    elif vine_result == cvine.VINE_RESULT_OUTPUT_MISSING:
+    reason = "work queue result: "
+    if wq_result == wq.WORK_QUEUE_RESULT_SUCCESS:
+        reason += "succesful execution with exit code {}".format(wq_task.return_status)
+    elif wq_result == wq.WORK_QUEUE_RESULT_OUTPUT_MISSING:
         reason += "The result file was not transfered from the worker.\n"
         reason += "This usually means that there is a problem with the python setup,\n"
         reason += "or the wrapper that executes the function."
-        reason += "\nTrace:\n" + str(vine_task.output)
-    elif vine_result == cvine.VINE_RESULT_INPUT_MISSING:
+        reason += "\nTrace:\n" + str(wq_task.output)
+    elif wq_result == wq.WORK_QUEUE_RESULT_INPUT_MISSING:
         reason += "missing input file"
-    elif vine_result == cvine.VINE_RESULT_STDOUT_MISSING:
+    elif wq_result == wq.WORK_QUEUE_RESULT_STDOUT_MISSING:
         reason += "stdout has been truncated"
-    elif vine_result == cvine.VINE_RESULT_SIGNAL:
+    elif wq_result == wq.WORK_QUEUE_RESULT_SIGNAL:
         reason += "task terminated with a signal"
-    elif vine_result == cvine.VINE_RESULT_RESOURCE_EXHAUSTION:
+    elif wq_result == wq.WORK_QUEUE_RESULT_RESOURCE_EXHAUSTION:
         reason += "task used more resources than requested"
-    elif vine_result == cvine.VINE_RESULT_MAX_END_TIME:
+    elif wq_result == wq.WORK_QUEUE_RESULT_TASK_TIMEOUT:
         reason += "task ran past the specified end time"
-    elif vine_result == cvine.VINE_RESULT_UNKNOWN:
+    elif wq_result == wq.WORK_QUEUE_RESULT_UNKNOWN:
         reason += "result could not be classified"
-    elif vine_result == cvine.VINE_RESULT_FORSAKEN:
+    elif wq_result == wq.WORK_QUEUE_RESULT_FORSAKEN:
         reason += "task failed, but not a task error"
-    elif vine_result == cvine.VINE_RESULT_MAX_RETRIES:
+    elif wq_result == wq.WORK_QUEUE_RESULT_MAX_RETRIES:
         reason += "unable to complete after specified number of retries"
-    elif vine_result == cvine.VINE_RESULT_MAX_WALL_TIME:
+    elif wq_result == wq.WORK_QUEUE_RESULT_TASK_MAX_RUN_TIME:
         reason += "task ran for more than the specified time"
-    elif vine_result == cvine.VINE_RESULT_RMONITOR_ERROR:
+    elif wq_result == wq.WORK_QUEUE_RESULT_DISK_ALLOC_FULL:
+        reason += "task needed more space to complete task"
+    elif wq_result == wq.WORK_QUEUE_RESULT_RMONITOR_ERROR:
         reason += "task failed because the monitor did not produce an output"
-    elif vine_result == cvine.VINE_RESULT_OUTPUT_TRANSFER_ERROR:
-        reason += "task failed because output transfer fails"
-    elif vine_result == cvine.VINE_RESULT_FIXED_LOCATION_MISSING:
-        reason += "task failed because no worker could satisfy the fixed \n"
-        reason += "location input file requirements"
     else:
-        reason += "unable to process TaskVine system failure"
+        reason += "unable to process Work Queue system failure"
     return reason
-
-
-@wrap_with_logs
-def _taskvine_factory(should_stop, factory_config):
-    logger.debug("Starting TaskVine factory process")
-
-    try:
-        # create the factory according to the project name if given
-        if factory_config._project_name:
-            factory = Factory(batch_type=factory_config.batch_type,
-                              manager_name=factory_config._project_name,
-                              )
-        else:
-            factory = Factory(batch_type=factory_config.batch_type,
-                              manager_host_port=f"{factory_config._project_address}:{factory_config._project_port}",
-                             )
-    except Exception as e:
-        raise TaskVineFactoryFailure(f'Cannot create factory with exception {e}')
-
-    # Set attributes of this factory
-    if factory_config._project_password_file:
-        factory.password = factory_config._project_password_file
-    factory.factory_timeout = factory_config.factory_timeout
-    factory.scratch_dir = factory_config.scratch_dir
-    factory.min_workers = factory_config.min_workers
-    factory.max_workers = factory_config.max_workers
-    factory.workers_per_cycle = factory_config.workers_per_cycle
-
-    if factory_config.worker_options:
-        factory.extra_options = factory_config.worker_options
-    factory.timeout = factory_config.worker_timeout
-    if factory_config.cores:
-        factory.cores = factory_config.cores
-    if factory_config.gpus:
-        factory.gpus = factory_config.gpus
-    if factory_config.memory:
-        factory.memory = factory_config.memory
-    if factory_config.disk:
-        factory.disk = factory_config.disk
-    if factory_config.python_env:
-        factory.python_env = factory_config.python_env
-
-    if factory_config.condor_requirements:
-        factory.condor_requirements = factory_config.condor_requirements
-    if factory_config.batch_options:
-        factory.batch_options = factory_config.batch_options
-
-    # setup factory context and sleep for a second in every loop to
-    # avoid wasting CPU
-    with factory:
-        while not should_stop.value:
-            time.sleep(1)
-
-    logger.debug("Exiting TaskVine factory process")
-    return 0
```

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/factory_config.py` & `parsl-2023.8.7/parsl/executors/taskvine/factory_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/manager_config.py` & `parsl-2023.8.7/parsl/executors/taskvine/manager_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         Command line to run before executing a task in a worker.
         Default is ''.
 
     env_pack: Optional[str]
         Used to encapsulate package dependencies of tasks to
         execute them remotely without needing a shared filesystem.
         Recommended way to manage tasks' dependency requirements.
+        All tasks will be executed in the encapsulated environment.
         If an absolute path to a conda environment or a conda
         environment name is given, TaskVine will package the conda
         environment in a tarball and send it along with tasks to be
         executed in a replicated conda environment.
         If a tarball of packages (*.tar.gz) is given, TaskVine
         skips the packaging step and sends the tarball along with
         tasks to be executed in a replicated conda environment.
```

### Comparing `parsl-2023.7.31/parsl/executors/taskvine/utils.py` & `parsl-2023.8.7/parsl/executors/taskvine/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,30 @@
                  executor_id: int,                 # executor id of Parsl function
                  exec_mode: str,                   # execution mode of function, out of {regular, python, serverless}
                  category: str,                    # category of Parsl function
                  input_files: list,                # list of input files to this function
                  output_files: list,               # list of output files to this function
                  map_file: Optional[str],          # pickled file containing mapping of local to remote names of files
                  function_file: Optional[str],     # pickled file containing the function information
+                 argument_file: Optional[str],     # pickled file containing the arguments to the function call
                  result_file: Optional[str],       # path to the pickled result object of the function execution
                  cores: Optional[float],           # number of cores to allocate
                  memory: Optional[int],            # amount of memory in MBs to allocate
                  disk: Optional[int],              # amount of disk in MBs to allocate
                  gpus: Optional[float],            # number of gpus to allocate
                  priority: Optional[float],        # priority of function, the higher the more priority
                  running_time_min: Optional[int],  # minimum amount of time for the function to run on a worker
                  env_pkg: Optional[str],           # path to a poncho environment tarball
                  ):
         self.executor_id = executor_id
         self.exec_mode = exec_mode
         self.category = category
         self.map_file = map_file
         self.function_file = function_file
+        self.argument_file = argument_file
         self.result_file = result_file
         self.input_files = input_files
         self.output_files = output_files
         self.cores = cores
         self.memory = memory
         self.disk = disk
         self.gpus = gpus
@@ -69,7 +71,15 @@
                  parsl_name: str,   # name of file
                  stage: bool,       # whether TaskVine should know about this file
                  cache: bool        # whether TaskVine should cache this file
                  ):
         self.parsl_name = parsl_name
         self.stage = stage
         self.cache = cache
+
+
+def run_parsl_function(map_file, function_file, argument_file, result_file):
+    """
+    Wrapper function to deploy with FunctionCall as serverless tasks.
+    """
+    from parsl.executors.taskvine.exec_parsl_function import run
+    run(map_file, function_file, argument_file, result_file)
```

### Comparing `parsl-2023.7.31/parsl/executors/threads.py` & `parsl-2023.8.7/parsl/executors/threads.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import typeguard
 import concurrent.futures as cf
 
 from typing import List, Optional
 
 from parsl.data_provider.staging import Staging
-from parsl.executors.status_handling import NoStatusHandlingExecutor
+from parsl.executors.base import ParslExecutor
 from parsl.utils import RepresentationMixin
 from parsl.executors.errors import UnsupportedFeatureError
 
 
 logger = logging.getLogger(__name__)
 
 
-class ThreadPoolExecutor(NoStatusHandlingExecutor, RepresentationMixin):
+class ThreadPoolExecutor(ParslExecutor, RepresentationMixin):
     """A thread-based executor.
 
     Parameters
     ----------
     max_threads : int
         Number of threads. Default is 2.
     thread_name_prefix : string
@@ -26,15 +26,15 @@
         Specifications for accessing data this executor remotely.
     """
 
     @typeguard.typechecked
     def __init__(self, label: str = 'threads', max_threads: int = 2,
                  thread_name_prefix: str = '', storage_access: Optional[List[Staging]] = None,
                  working_dir: Optional[str] = None):
-        NoStatusHandlingExecutor.__init__(self)
+        ParslExecutor.__init__(self)
         self.label = label
         self.max_threads = max_threads
         self.thread_name_prefix = thread_name_prefix
 
         # we allow storage_access to be None now, which means something else to [] now
         # None now means that a default storage access list will be used, while
         # [] is a list with no storage access in it at all
```

### Comparing `parsl-2023.7.31/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.8.7/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.data_provider.files import File
 from parsl.utils import get_std_fname_mode
 import traceback
 import sys
 import pickle
 
-# This scripts executes a parsl function which is pickled in a file:
+# This scripts executes a parsl function which is pickled in 3 files:
 #
 # exec_parsl_function.py map_file function_file result_file
 #
 # map_file: Contains a pickled dictionary that indicates which local_paths the
 #           parsl Files should take.
 #
-# function_file: Contains a pickle parsl function.
+# function_file: Contains a pickle parsl function. Function might be serialized in advance.
+# See @parsl.serialize.concretes.py
 #
-# result_file: It will contain the result of the function, including any
+# result_file: A file path, whose content will contain the result of the function, including any
 #              exception generated. Exceptions will be wrapped with RemoteExceptionWrapper.
 #
 # Exit codes:
 # 0: The function was evaluated to completion. The result or any exception
 #    wrapped with RemoteExceptionWrapper were written to result_file.
 # anything else: There was an error that prevented writing to the result file altogether.
 #                The exit code corresponds to whatever the python interpreter gives.
 #
 
 
-def load_pickled_file(filename):
+def load_pickled_file(filename: str):
+    """ Load a pickled file and return its pickled object."""
     with open(filename, "rb") as f_in:
         return pickle.load(f_in)
 
 
-def dump_result_to_file(result_file, result_package):
+def dump_result_to_file(result_file: str, result_package):
+    """ Dump a result to the given result file."""
     with open(result_file, "wb") as f_out:
         pickle.dump(result_package, f_out)
 
 
 def remap_location(mapping, parsl_file):
+    """ Remap files from local name (on manager) to remote name (on worker)."""
     if not isinstance(parsl_file, File):
         return
     # Below we rewrite .local_path when scheme != file only when the local_name
     # was given by the main parsl process.  This is the case when scheme !=
     # 'file' but .local_path (via filepath) is in mapping.
     if parsl_file.scheme == 'file' or parsl_file.local_path:
         master_location = parsl_file.filepath
         if master_location in mapping:
             parsl_file.local_path = mapping[master_location]
 
 
 def remap_list_of_files(mapping, maybe_files):
+    """ Remap a list of potential files."""
     for maybe_file in maybe_files:
         remap_location(mapping, maybe_file)
 
 
 def remap_all_files(mapping, fn_args, fn_kwargs):
     # remap any positional argument given to the function that looks like a
     # File
@@ -69,126 +74,89 @@
                 if fname in mapping:
                     fn_kwargs[kwarg] = (mapping[fname], mode)
         else:
             # Treat anything else as a possible File to be remapped.
             remap_location(mapping, maybe_file)
 
 
-def unpack_function(function_info, user_namespace):
-    if "source code" in function_info:
-        return unpack_source_code_function(function_info, user_namespace)
-    elif "byte code" in function_info:
-        return unpack_byte_code_function(function_info, user_namespace)
-    else:
-        raise ValueError("Function file does not have a valid function representation.")
-
-
-def unpack_source_code_function(function_info, user_namespace):
-    source_code = function_info["source code"]
-    name = function_info["name"]
-    args = function_info["args"]
-    kwargs = function_info["kwargs"]
-    return (source_code, name, args, kwargs)
-
-
-def unpack_byte_code_function(function_info, user_namespace):
-    from parsl.serialize import unpack_apply_message
-    func, args, kwargs = unpack_apply_message(function_info["byte code"], user_namespace, copy=False)
-    return (func, 'parsl_function_name', args, kwargs)
+def unpack_object(serialized_obj, user_namespace):
+    from parsl.serialize import deserialize
+    obj = deserialize(serialized_obj)
+    return obj
 
 
 def encode_function(user_namespace, fn, fn_name, fn_args, fn_kwargs):
+    """ Register the given function to the given namespace."""
     # Returns a tuple (code, result_name)
     # code can be exec in the user_namespace to produce result_name.
     prefix = "parsl_"
     args_name = prefix + "args"
     kwargs_name = prefix + "kwargs"
     result_name = prefix + "result"
 
     # Add variables to the namespace to make function call
     user_namespace.update({args_name: fn_args,
                            kwargs_name: fn_kwargs,
                            result_name: result_name})
 
-    if isinstance(fn, str):
-        code = encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
-    elif callable(fn):
+    if callable(fn):
         code = encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
     else:
         raise ValueError("Function object does not look like a function.")
 
     return (code, result_name)
 
 
-def encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
-    # We drop the first line as it names the parsl decorator used (i.e., @python_app)
-    source = fn.split('\n')[1:]
-    fn_app = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
-
-    source.append(fn_app)
-
-    code = "\n".join(source)
-    return code
-
-
 def encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
     user_namespace.update({fn_name: fn})
     code = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
     return code
 
 
-def load_function(map_file, function_file):
+def load_function(map_file, function_file, argument_file):
     # Decodes the function and its file arguments to be executed into
     # function_code, and updates a user namespace with the function name and
     # the variable named result_name. When the function is executed, its result
     # will be stored in this variable in the user namespace.
     # Returns (namespace, function_code, result_name)
 
     # Create the namespace to isolate the function execution.
     user_ns = locals()
     user_ns.update({'__builtins__': __builtins__})
 
-    function_info = load_pickled_file(function_file)
+    packed_function = load_pickled_file(function_file)
+    packed_argument = load_pickled_file(argument_file)
 
-    (fn, fn_name, fn_args, fn_kwargs) = unpack_function(function_info, user_ns)
+    fn = unpack_object(packed_function, user_ns)
+    args_dict = unpack_object(packed_argument, user_ns)
+    fn_args = args_dict['args']
+    fn_kwargs = args_dict['kwargs']
+    fn_name = 'parsl_tmp_func_name'
 
     mapping = load_pickled_file(map_file)
     remap_all_files(mapping, fn_args, fn_kwargs)
 
     (code, result_name) = encode_function(user_ns, fn, fn_name, fn_args, fn_kwargs)
 
     return (user_ns, code, result_name)
 
 
 def execute_function(namespace, function_code, result_name):
     # On executing the function inside the namespace, its result will be in a
     # variable named result_name.
-
     exec(function_code, namespace, namespace)
     result = namespace.get(result_name)
 
     return result
 
 
-if __name__ == "__main__":
+def run(map_file, function_file, argument_file, result_file):
     try:
-        # parse the three required command line arguments:
-        # map_file: contains a pickled dictionary to map original names to
-        #           names at the execution site.
-        # function_file: contains the pickled parsl function to execute.
-        # result_file: any output (including exceptions) will be written to
-        #              this file.
-        try:
-            (map_file, function_file, result_file) = sys.argv[1:]
-        except ValueError:
-            print("Usage:\n\t{} function result mapping\n".format(sys.argv[0]))
-            raise
-
         try:
-            (namespace, function_code, result_name) = load_function(map_file, function_file)
+            (namespace, function_code, result_name) = load_function(map_file, function_file, argument_file)
         except Exception:
             print("There was an error setting up the function for execution.")
             raise
 
         try:
             result = execute_function(namespace, function_code, result_name)
         except Exception:
@@ -201,7 +169,23 @@
     # Write out function result to the result file
     try:
         dump_result_to_file(result_file, result)
     except Exception:
         print("Could not write to result file.")
         traceback.print_exc()
         sys.exit(1)
+
+
+if __name__ == "__main__":
+    # parse the four required command line arguments:
+    # map_file: contains a pickled dictionary to map original names to
+    #           names at the execution site.
+    # function_file: contains the pickled parsl function to execute.
+    # argument_file: contains the pickled arguments to the function call.
+    # result_file: any output (including exceptions) will be written to
+    #              this file.
+    try:
+        (map_file, function_file, argument_file, result_file) = sys.argv[1:]
+    except ValueError:
+        print("Usage:\n\t{} function argument result mapping\n".format(sys.argv[0]))
+        raise
+    run(map_file, function_file, argument_file, result_file)
```

### Comparing `parsl-2023.7.31/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.8.7/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.8.7/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/jobs/job_status_poller.py` & `parsl-2023.8.7/parsl/jobs/job_status_poller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import logging
 import parsl  # noqa F401 (used in string type annotation)
 import time
 import zmq
 from typing import Dict, Sequence
 from typing import List  # noqa F401 (used in type annotation)
 
-from parsl.executors.base import ParslExecutor
-from parsl.jobs.job_error_handler import JobErrorHandler
 from parsl.jobs.states import JobStatus, JobState
 from parsl.jobs.strategy import Strategy
+from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.monitoring.message_type import MessageType
 
 
 from parsl.utils import Timer
 
 
 logger = logging.getLogger(__name__)
 
 
 class PollItem:
-    def __init__(self, executor: ParslExecutor, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
+    def __init__(self, executor: BlockProviderExecutor, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
         self._executor = executor
         self._dfk = dfk
         self._interval = executor.status_polling_interval
         self._last_poll_time = 0.0
         self._status = {}  # type: Dict[str, JobStatus]
 
         # Create a ZMQ channel to send poll status to monitoring
@@ -67,15 +66,15 @@
         """Return the status of all jobs/blocks of the executor of this poller.
 
         :return: a dictionary mapping block ids (in string) to job status
         """
         return self._status
 
     @property
-    def executor(self) -> ParslExecutor:
+    def executor(self) -> BlockProviderExecutor:
         return self._executor
 
     def scale_in(self, n, force=True, max_idletime=None):
         if force and not max_idletime:
             block_ids = self._executor.scale_in(n)
         else:
             block_ids = self._executor.scale_in(n, force=force, max_idletime=max_idletime)
@@ -103,26 +102,29 @@
 
 class JobStatusPoller(Timer):
     def __init__(self, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
         self._poll_items = []  # type: List[PollItem]
         self.dfk = dfk
         self._strategy = Strategy(strategy=dfk.config.strategy,
                                   max_idletime=dfk.config.max_idletime)
-        self._error_handler = JobErrorHandler()
         super().__init__(self.poll, interval=5, name="JobStatusPoller")
 
     def poll(self):
         self._update_state()
-        self._error_handler.run(self._poll_items)
+        self._run_error_handlers(self._poll_items)
         self._strategy.strategize(self._poll_items)
 
+    def _run_error_handlers(self, status: List[PollItem]):
+        for es in status:
+            es.executor.handle_errors(es.status)
+
     def _update_state(self) -> None:
         now = time.time()
         for item in self._poll_items:
             item.poll(now)
 
-    def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
+    def add_executors(self, executors: Sequence[BlockProviderExecutor]) -> None:
         for executor in executors:
             if executor.status_polling_interval > 0:
                 logger.debug("Adding executor {}".format(executor.label))
                 self._poll_items.append(PollItem(executor, self.dfk))
         self._strategy.add_executors(executors)
```

### Comparing `parsl-2023.7.31/parsl/jobs/states.py` & `parsl-2023.8.7/parsl/jobs/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/jobs/strategy.py` & `parsl-2023.8.7/parsl/jobs/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/launchers/__init__.py` & `parsl-2023.8.7/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/launchers/base.py` & `parsl-2023.8.7/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/launchers/launchers.py` & `parsl-2023.8.7/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/log_utils.py` & `parsl-2023.8.7/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/db_manager.py` & `parsl-2023.8.7/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/monitoring.py` & `parsl-2023.8.7/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/queries/pandas.py` & `parsl-2023.8.7/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/radios.py` & `parsl-2023.8.7/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/remote.py` & `parsl-2023.8.7/parsl/monitoring/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.radios import MonitoringRadio, UDPRadio, HTEXRadio, FilesystemRadio
 from typing import Any, Callable, Dict, List, Sequence, Tuple
 
 logger = logging.getLogger(__name__)
 
-monitoring_wrapper_cache: Dict
-monitoring_wrapper_cache = {}
-
 
 def monitor_wrapper(f: Any,           # per app
                     args: Sequence,   # per invocation
                     kwargs: Dict,     # per invocation
                     x_try_id: int,    # per invocation
                     x_task_id: int,   # per invocation
                     monitoring_hub_url: str,   # per workflow
@@ -29,84 +26,71 @@
                     sleep_dur: float,  # per workflow
                     radio_mode: str,   # per executor
                     monitor_resources: bool,  # per workflow
                     run_dir: str) -> Tuple[Callable, Sequence, Dict]:
     """Wrap the Parsl app with a function that will call the monitor function and point it at the correct pid when the task begins.
     """
 
-    # this makes assumptions that when subsequently executed with the same
-    # cache key, then the relevant parameters will not have changed from the
-    # first invocation with that cache key (otherwise, the resulting cached
-    # closure will be incorrectly cached)
-    cache_key = (run_id, f, radio_mode)
-
-    if cache_key in monitoring_wrapper_cache:
-        wrapped = monitoring_wrapper_cache[cache_key]
-
-    else:
-
-        @wraps(f)
-        def wrapped(*args: List[Any], **kwargs: Dict[str, Any]) -> Any:
-            task_id = kwargs.pop('_parsl_monitoring_task_id')
-            try_id = kwargs.pop('_parsl_monitoring_try_id')
-            terminate_event = Event()
-            # Send first message to monitoring router
-            send_first_message(try_id,
-                               task_id,
-                               monitoring_hub_url,
-                               run_id,
-                               radio_mode,
-                               run_dir)
-
-            if monitor_resources:
-                # create the monitor process and start
-                pp = ForkProcess(target=monitor,
-                                 args=(os.getpid(),
-                                       try_id,
-                                       task_id,
-                                       monitoring_hub_url,
-                                       run_id,
-                                       radio_mode,
-                                       logging_level,
-                                       sleep_dur,
-                                       run_dir,
-                                       terminate_event),
-                                 daemon=True,
-                                 name="Monitor-Wrapper-{}".format(task_id))
-                pp.start()
-                p = pp
-                #  TODO: awkwardness because ForkProcess is not directly a constructor
-                # and type-checking is expecting p to be optional and cannot
-                # narrow down the type of p in this block.
-
-            else:
-                p = None
-
-            try:
-                return f(*args, **kwargs)
-            finally:
-                # There's a chance of zombification if the workers are killed by some signals (?)
-                if p:
-                    terminate_event.set()
-                    p.join(30)  # 30 second delay for this -- this timeout will be hit in the case of an unusually long end-of-loop
-                    if p.exitcode is None:
-                        logger.warn("Event-based termination of monitoring helper took too long. Using process-based termination.")
-                        p.terminate()
-                        # DANGER: this can corrupt shared queues according to docs.
-                        # So, better that the above termination event worked.
-                        # This is why this log message is a warning
-                        p.join()
-
-                send_last_message(try_id,
-                                  task_id,
-                                  monitoring_hub_url,
-                                  run_id,
-                                  radio_mode, run_dir)
-
-        monitoring_wrapper_cache[cache_key] = wrapped
+    @wraps(f)
+    def wrapped(*args: List[Any], **kwargs: Dict[str, Any]) -> Any:
+        task_id = kwargs.pop('_parsl_monitoring_task_id')
+        try_id = kwargs.pop('_parsl_monitoring_try_id')
+        terminate_event = Event()
+        # Send first message to monitoring router
+        send_first_message(try_id,
+                           task_id,
+                           monitoring_hub_url,
+                           run_id,
+                           radio_mode,
+                           run_dir)
+
+        if monitor_resources:
+            # create the monitor process and start
+            pp = ForkProcess(target=monitor,
+                             args=(os.getpid(),
+                                   try_id,
+                                   task_id,
+                                   monitoring_hub_url,
+                                   run_id,
+                                   radio_mode,
+                                   logging_level,
+                                   sleep_dur,
+                                   run_dir,
+                                   terminate_event),
+                             daemon=True,
+                             name="Monitor-Wrapper-{}".format(task_id))
+            pp.start()
+            p = pp
+            #  TODO: awkwardness because ForkProcess is not directly a constructor
+            # and type-checking is expecting p to be optional and cannot
+            # narrow down the type of p in this block.
+
+        else:
+            p = None
+
+        try:
+            return f(*args, **kwargs)
+        finally:
+            # There's a chance of zombification if the workers are killed by some signals (?)
+            if p:
+                terminate_event.set()
+                p.join(30)  # 30 second delay for this -- this timeout will be hit in the case of an unusually long end-of-loop
+                if p.exitcode is None:
+                    logger.warn("Event-based termination of monitoring helper took too long. Using process-based termination.")
+                    p.terminate()
+                    # DANGER: this can corrupt shared queues according to docs.
+                    # So, better that the above termination event worked.
+                    # This is why this log message is a warning
+                    p.join()
+
+            send_last_message(try_id,
+                              task_id,
+                              monitoring_hub_url,
+                              run_id,
+                              radio_mode, run_dir)
 
     new_kwargs = kwargs.copy()
     new_kwargs['_parsl_monitoring_task_id'] = x_task_id
     new_kwargs['_parsl_monitoring_try_id'] = x_try_id
 
     return (wrapped, args, new_kwargs)
```

### Comparing `parsl-2023.7.31/parsl/monitoring/types.py` & `parsl-2023.8.7/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/app.py` & `parsl-2023.8.7/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/models.py` & `parsl-2023.8.7/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.8.7/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.8.7/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.8.7/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.8.7/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.8.7/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/monitoring/visualization/views.py` & `parsl-2023.8.7/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/multiprocessing.py` & `parsl-2023.8.7/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/process_loggers.py` & `parsl-2023.8.7/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/__init__.py` & `parsl-2023.8.7/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.8.7/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/aws/aws.py` & `parsl-2023.8.7/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/azure/azure.py` & `parsl-2023.8.7/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/base.py` & `parsl-2023.8.7/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/cluster_provider.py` & `parsl-2023.8.7/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/cobalt/cobalt.py` & `parsl-2023.8.7/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/condor/condor.py` & `parsl-2023.8.7/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/condor/template.py` & `parsl-2023.8.7/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/errors.py` & `parsl-2023.8.7/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.8.7/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.8.7/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/kubernetes/kube.py` & `parsl-2023.8.7/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/local/local.py` & `parsl-2023.8.7/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/lsf/lsf.py` & `parsl-2023.8.7/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/pbspro/pbspro.py` & `parsl-2023.8.7/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/slurm/slurm.py` & `parsl-2023.8.7/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/providers/torque/torque.py` & `parsl-2023.8.7/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/serialize/base.py` & `parsl-2023.8.7/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/serialize/concretes.py` & `parsl-2023.8.7/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/serialize/errors.py` & `parsl-2023.8.7/parsl/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/serialize/facade.py` & `parsl-2023.8.7/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/serialize/proxystore.py` & `parsl-2023.8.7/parsl/serialize/proxystore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.8.7/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/azure_single_node.py` & `parsl-2023.8.7/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/bluewaters.py` & `parsl-2023.8.7/parsl/tests/configs/theta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from parsl.config import Config
-from parsl.executors import HighThroughputExecutor
+from parsl.providers import CobaltProvider
 from parsl.launchers import AprunLauncher
-from parsl.providers import TorqueProvider
+from parsl.executors import HighThroughputExecutor
 
 from .user_opts import user_opts
 
 
 def fresh_config():
-    config = Config(
+    return Config(
         executors=[
             HighThroughputExecutor(
-                label="bw_htex",
-                cores_per_worker=1,
-                worker_debug=False,
+                label='theta_local_htex_multinode',
                 max_workers=1,
-                provider=TorqueProvider(
-                    queue='normal',
-                    launcher=AprunLauncher(overrides="-b -- bwpy-environ --"),
-                    # string to prepend to #SBATCH blocks in the submit
-                    # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
+                provider=CobaltProvider(
+                    queue=user_opts['theta']['queue'],
+                    account=user_opts['theta']['account'],
+                    launcher=AprunLauncher(overrides="-d 64"),
+                    walltime='00:10:00',
+                    nodes_per_block=2,
+                    init_blocks=1,
+                    max_blocks=1,
+                    # string to prepend to #COBALT blocks in the submit
+                    # script to the scheduler eg: '#COBALT -t 50'
                     scheduler_options='',
                     # Command to be run before starting a worker, such as:
                     # 'module load Anaconda; source activate parsl_env'.
-                    worker_init=user_opts['bluewaters']['worker_init'],
-                    init_blocks=1,
-                    max_blocks=1,
-                    min_blocks=1,
-                    nodes_per_block=2,
-                    walltime='00:30:00',
+                    worker_init=user_opts['theta']['worker_init'],
                     cmd_timeout=120,
                 ),
             )
         ],
     )
-    return config
 
 
 config = fresh_config()
```

### Comparing `parsl-2023.7.31/parsl/tests/configs/bridges.py` & `parsl-2023.8.7/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.8.7/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/comet.py` & `parsl-2023.8.7/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/cooley_htex.py` & `parsl-2023.8.7/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.8.7/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/ec2_spot.py` & `parsl-2023.8.7/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/frontera.py` & `parsl-2023.8.7/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.8.7/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/htex_local.py` & `parsl-2023.8.7/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.8.7/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.8.7/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.8.7/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.8.7/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/midway.py` & `parsl-2023.8.7/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.8.7/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/osg_htex.py` & `parsl-2023.8.7/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/petrelkube.py` & `parsl-2023.8.7/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/summit.py` & `parsl-2023.8.7/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/swan_htex.py` & `parsl-2023.8.7/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/taskvine_ex.py` & `parsl-2023.8.7/parsl/tests/configs/taskvine_ex.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 from parsl.data_provider.http import HTTPInTaskStaging
 from parsl.data_provider.ftp import FTPInTaskStaging
 from parsl.data_provider.file_noop import NoOpFileStaging
 
 
 def fresh_config():
     return Config(executors=[TaskVineExecutor(manager_config=TaskVineManagerConfig(port=9000),
-                                              use_factory=True,
+                                              worker_launch_method='factory',
                                               storage_access=[FTPInTaskStaging(), HTTPInTaskStaging(), NoOpFileStaging()])])
```

### Comparing `parsl-2023.7.31/parsl/tests/configs/theta.py` & `parsl-2023.8.7/parsl/configs/theta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from parsl.config import Config
 from parsl.providers import CobaltProvider
 from parsl.launchers import AprunLauncher
 from parsl.executors import HighThroughputExecutor
+from parsl.addresses import address_by_interface
 
-from .user_opts import user_opts
-
-
-def fresh_config():
-    return Config(
-        executors=[
-            HighThroughputExecutor(
-                label='theta_local_htex_multinode',
-                max_workers=1,
-                provider=CobaltProvider(
-                    queue=user_opts['theta']['queue'],
-                    account=user_opts['theta']['account'],
-                    launcher=AprunLauncher(overrides="-d 64"),
-                    walltime='00:10:00',
-                    nodes_per_block=2,
-                    init_blocks=1,
-                    max_blocks=1,
-                    # string to prepend to #COBALT blocks in the submit
-                    # script to the scheduler eg: '#COBALT -t 50'
-                    scheduler_options='',
-                    # Command to be run before starting a worker, such as:
-                    # 'module load Anaconda; source activate parsl_env'.
-                    worker_init=user_opts['theta']['worker_init'],
-                    cmd_timeout=120,
-                ),
-            )
-        ],
-    )
-
-
-config = fresh_config()
+config = Config(
+    executors=[
+        HighThroughputExecutor(
+            label='theta_local_htex_multinode',
+            address=address_by_interface('vlan2360'),
+            max_workers=4,
+            cpu_affinity='block',  # Ensures that workers use cores on the same tile
+            provider=CobaltProvider(
+                queue='YOUR_QUEUE',
+                account='YOUR_ACCOUNT',
+                launcher=AprunLauncher(overrides="-d 64 --cc depth"),
+                walltime='00:30:00',
+                nodes_per_block=2,
+                init_blocks=1,
+                min_blocks=1,
+                max_blocks=1,
+                # string to prepend to #COBALT blocks in the submit
+                # script to the scheduler eg: '#COBALT -t 50'
+                scheduler_options='',
+                # Command to be run before starting a worker, such as:
+                # 'module load Anaconda; source activate parsl_env'.
+                worker_init='',
+                cmd_timeout=120,
+            ),
+        )
+    ],
+)
```

### Comparing `parsl-2023.7.31/parsl/tests/configs/user_opts.py` & `parsl-2023.8.7/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/configs/workqueue_ex.py` & `parsl-2023.8.7/parsl/tests/configs/workqueue_ex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/conftest.py` & `parsl-2023.8.7/parsl/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/latency.py` & `parsl-2023.8.7/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.8.7/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.8.7/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.8.7/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.8.7/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.8.7/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/scaling_tests/htex_local.py` & `parsl-2023.8.7/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/scaling_tests/test_scale.py` & `parsl-2023.8.7/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2023.8.7/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2023.8.7/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.8.7/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/site_tests/test_provider.py` & `parsl-2023.8.7/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/site_tests/test_site.py` & `parsl-2023.8.7/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_affinity.py` & `parsl-2023.8.7/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_concurrent.py` & `parsl-2023.8.7/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.8.7/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_ec2.py` & `parsl-2023.8.7/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.8.7/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_start_method.py` & `parsl-2023.8.7/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/sites/test_worker_info.py` & `parsl-2023.8.7/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_aalst_patterns.py` & `parsl-2023.8.7/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.8.7/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_callables.py` & `parsl-2023.8.7/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.8.7/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.8.7/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_data/test_file.py` & `parsl-2023.8.7/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.8.7/parsl/tests/test_data/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.8.7/parsl/tests/test_data/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2023.8.7/parsl/tests/test_data/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.8.7/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.8.7/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_flux.py` & `parsl-2023.8.7/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_htex/test_htex_zmq_binding.py` & `parsl-2023.8.7/parsl/tests/test_htex/test_htex_zmq_binding.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.8.7/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.8.7/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.8.7/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.8.7/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2023.8.7/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.8.7/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.8.7/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_1480.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_1653.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_221.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_226.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_2652.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_69a.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_854.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2023.8.7/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2023.8.7/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.8.7/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_serialization/test_2555_caching_deserializer.py` & `parsl-2023.8.7/parsl/tests/test_serialization/test_2555_caching_deserializer.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_serialization/test_basic.py` & `parsl-2023.8.7/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_serialization/test_proxystore_configured.py` & `parsl-2023.8.7/parsl/tests/test_serialization/test_proxystore_configured.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_serialization/test_proxystore_impl.py` & `parsl-2023.8.7/parsl/tests/test_serialization/test_proxystore_impl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.8.7/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_1316.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.8.7/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_summary.py` & `parsl-2023.8.7/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_thread_parallelism.py` & `parsl-2023.8.7/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_threads/test_configs.py` & `parsl-2023.8.7/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.8.7/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/usage_tracking/usage.py` & `parsl-2023.8.7/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl/utils.py` & `parsl-2023.8.7/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/parsl.egg-info/PKG-INFO` & `parsl-2023.8.7/parsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.7.31
+Version: 2023.8.7
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.07.31.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.08.07.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.7.31/parsl.egg-info/SOURCES.txt` & `parsl-2023.8.7/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,28 @@
 parsl/executors/high_throughput/probe.py
 parsl/executors/high_throughput/process_worker_pool.py
 parsl/executors/high_throughput/zmq_pipes.py
 parsl/executors/taskvine/__init__.py
 parsl/executors/taskvine/errors.py
 parsl/executors/taskvine/exec_parsl_function.py
 parsl/executors/taskvine/executor.py
+parsl/executors/taskvine/factory.py
 parsl/executors/taskvine/factory_config.py
+parsl/executors/taskvine/manager.py
 parsl/executors/taskvine/manager_config.py
 parsl/executors/taskvine/utils.py
 parsl/executors/workqueue/__init__.py
 parsl/executors/workqueue/errors.py
 parsl/executors/workqueue/exec_parsl_function.py
 parsl/executors/workqueue/executor.py
 parsl/executors/workqueue/parsl_coprocess.py
 parsl/executors/workqueue/parsl_coprocess_stub.py
 parsl/jobs/__init__.py
-parsl/jobs/job_error_handler.py
 parsl/jobs/job_status_poller.py
+parsl/jobs/simple_error_handler.py
 parsl/jobs/states.py
 parsl/jobs/strategy.py
 parsl/launchers/__init__.py
 parsl/launchers/base.py
 parsl/launchers/errors.py
 parsl/launchers/launchers.py
 parsl/monitoring/__init__.py
```

### Comparing `parsl-2023.7.31/parsl.egg-info/requires.txt` & `parsl-2023.8.7/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.31/setup.py` & `parsl-2023.8.7/setup.py`

 * *Files identical despite different names*

