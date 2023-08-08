# Comparing `tmp/ml-starter-0.1.49.tar.gz` & `tmp/ml-starter-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.49.tar", last modified: Tue Aug  8 16:07:54 2023, max compression
+gzip compressed data, was "ml-starter-0.1.50.tar", last modified: Tue Aug  8 20:50:53 2023, max compression
```

## Comparing `ml-starter-0.1.49.tar` & `ml-starter-0.1.50.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 16:07:42.000000 ml-starter-0.1.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 16:07:42.000000 ml-starter-0.1.49/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 16:07:54.075945 ml-starter-0.1.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 16:07:42.000000 ml-starter-0.1.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.071944 ml-starter-0.1.49/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28186 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.071944 ml-starter-0.1.49/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/grad_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 16:07:42.000000 ml-starter-0.1.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 16:07:54.079944 ml-starter-0.1.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-08 16:07:42.000000 ml-starter-0.1.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.654168 ml-starter-0.1.50/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 20:50:39.000000 ml-starter-0.1.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 20:50:39.000000 ml-starter-0.1.50/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 20:50:53.654168 ml-starter-0.1.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 20:50:39.000000 ml-starter-0.1.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.630166 ml-starter-0.1.50/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.630166 ml-starter-0.1.50/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.630166 ml-starter-0.1.50/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.634167 ml-starter-0.1.50/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.634167 ml-starter-0.1.50/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.634167 ml-starter-0.1.50/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.634167 ml-starter-0.1.50/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.638167 ml-starter-0.1.50/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.638167 ml-starter-0.1.50/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.638167 ml-starter-0.1.50/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.638167 ml-starter-0.1.50/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.642167 ml-starter-0.1.50/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.646168 ml-starter-0.1.50/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28162 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.646168 ml-starter-0.1.50/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/grad_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.650168 ml-starter-0.1.50/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.654168 ml-starter-0.1.50/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.654168 ml-starter-0.1.50/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-08 20:50:39.000000 ml-starter-0.1.50/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:50:53.654168 ml-starter-0.1.50/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 20:50:53.000000 ml-starter-0.1.50/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-08 20:50:53.000000 ml-starter-0.1.50/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:50:53.000000 ml-starter-0.1.50/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 20:50:53.000000 ml-starter-0.1.50/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-08 20:50:53.000000 ml-starter-0.1.50/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 20:50:39.000000 ml-starter-0.1.50/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 20:50:53.654168 ml-starter-0.1.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-08 20:50:39.000000 ml-starter-0.1.50/setup.py
```

### Comparing `ml-starter-0.1.49/LICENSE` & `ml-starter-0.1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/PKG-INFO` & `ml-starter-0.1.50/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.49
+Version: 0.1.50
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.49/README.md` & `ml-starter-0.1.50/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/api.py` & `ml-starter-0.1.50/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/core/common_types.py` & `ml-starter-0.1.50/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/core/config.py` & `ml-starter-0.1.50/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/core/env.py` & `ml-starter-0.1.50/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/core/registry.py` & `ml-starter-0.1.50/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/core/state.py` & `ml-starter-0.1.50/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/launchers/base.py` & `ml-starter-0.1.50/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/launchers/mp.py` & `ml-starter-0.1.50/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/launchers/sagemaker.py` & `ml-starter-0.1.50/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/launchers/slurm.py` & `ml-starter-0.1.50/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/launchers/torchrun.py` & `ml-starter-0.1.50/ml/launchers/torchrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from ml.core.config import conf_field
 from ml.core.registry import project_dirs, register_launcher, register_trainer
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.utils.networking import get_unused_port
 
 logger: logging.Logger = logging.getLogger(__name__)
 
+DEFAULT_PORT = 29500
+
 TORCHRUN_TEMPLATE: str = """
 #!/usr/bin/env python
 
 from pathlib import Path
 
 from omegaconf import OmegaConf
 
@@ -58,15 +60,15 @@
     @classmethod
     def resolve(cls: type["TorchRunLauncherConfig"], config: "TorchRunLauncherConfig") -> None:
         super().resolve(config)
 
         if OmegaConf.is_missing(config, "nproc_per_node"):
             config.nproc_per_node = torch.cuda.device_count()
         if OmegaConf.is_missing(config, "master_port"):
-            config.master_port = get_unused_port()
+            config.master_port = get_unused_port(DEFAULT_PORT)
         if OmegaConf.is_missing(config, "torchrun_path"):
             torchrun_path = shutil.which("torchrun")
             if torchrun_path is None:
                 raise ValueError("Could not find torchrun in PATH")
             config.torchrun_path = torchrun_path
```

### Comparing `ml-starter-0.1.49/ml/loggers/base.py` & `ml-starter-0.1.50/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/loggers/meter.py` & `ml-starter-0.1.50/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/loggers/multi.py` & `ml-starter-0.1.50/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/loggers/stdout.py` & `ml-starter-0.1.50/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/loggers/tensorboard.py` & `ml-starter-0.1.50/ml/loggers/tensorboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import atexit
 import datetime
 import functools
 import logging
 import os
 import re
+import shutil
 import subprocess
 import threading
 import time
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, Iterable, Iterator, TypeVar, cast
@@ -112,23 +113,16 @@
     return "\n".join([header_str, header_sep_str, rows_str])
 
 
 @dataclass
 class TensorboardLoggerConfig(BaseLoggerConfig):
     flush_seconds: float = conf_field(10.0, help="How often to flush logs")
     wait_seconds: float = conf_field(0.0, help="Time to wait before starting Tensorboard process")
-    log_id: str = conf_field(MISSING, help="Unique log ID")
     start_in_subprocess: bool = conf_field(True, help="Start TensorBoard subprocess")
 
-    @classmethod
-    def resolve(cls, config: "TensorboardLoggerConfig") -> None:
-        if OmegaConf.is_missing(config, "log_id"):
-            config.log_id = datetime.datetime.now().strftime("%H-%M-%S")
-        super().resolve(config)
-
 
 @register_logger("tensorboard", TensorboardLoggerConfig)
 class TensorboardLogger(BaseLogger[TensorboardLoggerConfig]):
     def __init__(self, config: TensorboardLoggerConfig) -> None:
         super().__init__(config)
 
         self.scalars: dict[Phase, dict[str, Callable[[], int | float | Tensor]]] = defaultdict(dict)
@@ -225,15 +219,15 @@
             self.proc = None
 
     def __del__(self) -> None:
         self.cleanup()
 
     @property
     def tensorboard_log_directory(self) -> Path:
-        return self.log_directory / "tensorboard" / self.config.log_id
+        return self.log_directory / "tensorboard"
 
     @functools.cached_property
     def train_writer(self) -> SummaryWriter:
         return SummaryWriter(
             self.tensorboard_log_directory / "train",
             flush_secs=self.config.flush_seconds,
         )
@@ -248,14 +242,22 @@
     @functools.cached_property
     def test_writer(self) -> SummaryWriter:
         return SummaryWriter(
             self.tensorboard_log_directory / "test",
             flush_secs=self.config.flush_seconds,
         )
 
+    def clear_logs(self) -> None:
+        if not self.tensorboard_log_directory.exists():
+            return
+        if not any(child.is_dir() for child in self.tensorboard_log_directory.iterdir()):
+            return
+        logger.info("Clearing TensorBoard logs in %s", self.tensorboard_log_directory)
+        shutil.rmtree(self.tensorboard_log_directory)
+
     def get_writer(self, phase: Phase) -> SummaryWriter:
         self._start()
         if phase == "train":
             return self.train_writer
         if phase == "valid":
             return self.valid_writer
         if phase == "test":
@@ -283,14 +285,17 @@
     def log_point_cloud(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
         self.point_clouds[state.phase][f"{namespace}/{key}"] = value
 
     def log_config(self, config: DictConfig) -> None:
         self.run_config = config
 
     def write(self, state: State) -> None:
+        if state.num_steps == 0:
+            self.clear_logs()
+
         if self.line_str is not None:
             cur_time = state.elapsed_time_s
             if cur_time - self.last_tensorboard_write_time > WRITE_PROC_TEXT_EVERY_N_SECONDS:
                 logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str], "light-green", "cyan"))
                 self.last_tensorboard_write_time = cur_time
 
         writer = self.get_writer(state.phase)
```

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/base.py` & `ml-starter-0.1.50/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/constant.py` & `ml-starter-0.1.50/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.50/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.50/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/gan.py` & `ml-starter-0.1.50/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/linear.py` & `ml-starter-0.1.50/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.50/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.50/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/activations.py` & `ml-starter-0.1.50/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/architectures/bifpn.py` & `ml-starter-0.1.50/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/architectures/unet.py` & `ml-starter-0.1.50/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/base.py` & `ml-starter-0.1.50/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/codebook.py` & `ml-starter-0.1.50/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/embeddings.py` & `ml-starter-0.1.50/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/gan.py` & `ml-starter-0.1.50/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/init.py` & `ml-starter-0.1.50/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/kmeans.py` & `ml-starter-0.1.50/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/lora.py` & `ml-starter-0.1.50/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/modules.py` & `ml-starter-0.1.50/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/norms.py` & `ml-starter-0.1.50/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/models/parallel.py` & `ml-starter-0.1.50/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/adam.py` & `ml-starter-0.1.50/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/adan.py` & `ml-starter-0.1.50/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/base.py` & `ml-starter-0.1.50/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/common.py` & `ml-starter-0.1.50/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/gan.py` & `ml-starter-0.1.50/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/lion.py` & `ml-starter-0.1.50/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/sgd.py` & `ml-starter-0.1.50/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/optimizers/shampoo.py` & `ml-starter-0.1.50/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/scripts/cli.py` & `ml-starter-0.1.50/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/scripts/stage.py` & `ml-starter-0.1.50/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/scripts/train.py` & `ml-starter-0.1.50/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/base.py` & `ml-starter-0.1.50/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.50/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.50/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/collate.py` & `ml-starter-0.1.50/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.50/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.50/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.50/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.50/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.50/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.50/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.50/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.50/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/environments/base.py` & `ml-starter-0.1.50/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/environments/utils.py` & `ml-starter-0.1.50/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/environments/worker.py` & `ml-starter-0.1.50/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/gan/base.py` & `ml-starter-0.1.50/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/losses/audio.py` & `ml-starter-0.1.50/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/losses/image.py` & `ml-starter-0.1.50/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/losses/kl.py` & `ml-starter-0.1.50/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/losses/loss.py` & `ml-starter-0.1.50/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/rl/base.py` & `ml-starter-0.1.50/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/rl/replay.py` & `ml-starter-0.1.50/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/tasks/sl/base.py` & `ml-starter-0.1.50/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/base.py` & `ml-starter-0.1.50/ml/trainers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,27 +528,27 @@
                             if to_remove not in metadata:
                                 removed[to_remove] = kept_name
                             del state_dict[to_remove]
                     metadata["removed"] = json.dumps(removed)
 
                     self.update_state_dict(state_dict, metadata)
 
-                    if last_ckpt_path.exists():
-                        if self.checkpoint_config.only_save_most_recent:
-                            base_ckpt = last_ckpt_path.resolve()
-                            if base_ckpt.is_file():
-                                base_ckpt.unlink()
-                        last_ckpt_path.unlink()
-
                     safetensors_save_file(state_dict, ckpt_path, metadata)
 
                 except Exception:
                     logger.exception("Saving with safetensors failed, falling back to torch.save")
                     torch.save({"state": state_dict, "metadata": metadata}, ckpt_path)
 
+                if last_ckpt_path.exists():
+                    if self.checkpoint_config.only_save_most_recent:
+                        base_ckpt = last_ckpt_path.resolve()
+                        if base_ckpt.is_file():
+                            base_ckpt.unlink()
+                    last_ckpt_path.unlink()
+
                 try:
                     last_ckpt_path.symlink_to(ckpt_path)
                 except FileExistsError:
                     logger.exception("Exception while trying to update %s", ckpt_path)
                 self.add_lock_file("ckpt", exists_ok=True)
                 task.on_after_save_checkpoint(ckpt_path)
```

### Comparing `ml-starter-0.1.49/ml/trainers/gan.py` & `ml-starter-0.1.50/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/learning.py` & `ml-starter-0.1.50/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/compile.py` & `ml-starter-0.1.50/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.50/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.50/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.50/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/grad_balancer.py` & `ml-starter-0.1.50/ml/trainers/mixins/grad_balancer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.50/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.50/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.50/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.50/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.50/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/rl.py` & `ml-starter-0.1.50/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/trainers/sl.py` & `ml-starter-0.1.50/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/amp.py` & `ml-starter-0.1.50/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/argparse.py` & `ml-starter-0.1.50/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/atomic.py` & `ml-starter-0.1.50/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/attention.py` & `ml-starter-0.1.50/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/audio.py` & `ml-starter-0.1.50/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/augmentation.py` & `ml-starter-0.1.50/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/caching.py` & `ml-starter-0.1.50/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/checkpoint.py` & `ml-starter-0.1.50/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/cli.py` & `ml-starter-0.1.50/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/colors.py` & `ml-starter-0.1.50/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/containers.py` & `ml-starter-0.1.50/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/data.py` & `ml-starter-0.1.50/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/datetime.py` & `ml-starter-0.1.50/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/device/auto.py` & `ml-starter-0.1.50/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/device/base.py` & `ml-starter-0.1.50/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/device/cpu.py` & `ml-starter-0.1.50/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/device/gpu.py` & `ml-starter-0.1.50/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/device/metal.py` & `ml-starter-0.1.50/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/distributed.py` & `ml-starter-0.1.50/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/exceptions.py` & `ml-starter-0.1.50/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/image.py` & `ml-starter-0.1.50/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/io.py` & `ml-starter-0.1.50/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/large_models.py` & `ml-starter-0.1.50/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/logging.py` & `ml-starter-0.1.50/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/meter.py` & `ml-starter-0.1.50/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/mixed_precision.py` & `ml-starter-0.1.50/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/networking.py` & `ml-starter-0.1.50/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/numpy.py` & `ml-starter-0.1.50/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/parallel.py` & `ml-starter-0.1.50/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/spectrogram.py` & `ml-starter-0.1.50/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/staging.py` & `ml-starter-0.1.50/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/testing.py` & `ml-starter-0.1.50/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/timer.py` & `ml-starter-0.1.50/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/tokens.py` & `ml-starter-0.1.50/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/torch_distributed.py` & `ml-starter-0.1.50/ml/utils/torch_distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from ml.core.config import conf_field
 from ml.utils.checkpoint import is_missing
 from ml.utils.distributed import get_init_method, get_rank, get_world_size, set_dist
 from ml.utils.logging import INFOALL, configure_logging
 from ml.utils.networking import get_unused_port
 from ml.utils.parallel import init_parallelism
 
+DEFAULT_PORT = 29500
+
 logger: logging.Logger = logging.getLogger(__name__)
 
 P = ParamSpec("P")
 
 
 @dataclass
 class MultiprocessConfig:
@@ -53,15 +55,15 @@
     def resolve(cls, config: "MultiprocessConfig") -> None:
         device_count = torch.cuda.device_count() if torch.cuda.is_available() else 1
         if is_missing(config, "world_size"):
             config.world_size = device_count
         if is_missing(config, "local_world_size"):
             config.local_world_size = min(device_count, config.world_size)
         if is_missing(config, "master_port"):
-            config.master_port = get_unused_port()
+            config.master_port = get_unused_port(DEFAULT_PORT)
 
 
 def init_process_group_from_backend(backend: str | dist.Backend | None = None) -> None:
     if backend is None:
         backend = get_distributed_backend()
     init_method, world_size, rank = get_init_method(), get_world_size(), get_rank()
```

### Comparing `ml-starter-0.1.49/ml/utils/triton/kmeans.py` & `ml-starter-0.1.50/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/triton/lion.py` & `ml-starter-0.1.50/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml/utils/video.py` & `ml-starter-0.1.50/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.50/ml_starter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.49
+Version: 0.1.50
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.49/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.50/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/pyproject.toml` & `ml-starter-0.1.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.49/setup.py` & `ml-starter-0.1.50/setup.py`

 * *Files identical despite different names*

