# Comparing `tmp/ml-starter-0.1.48.tar.gz` & `tmp/ml-starter-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.48.tar", last modified: Mon Aug  7 23:13:45 2023, max compression
+gzip compressed data, was "ml-starter-0.1.49.tar", last modified: Tue Aug  8 16:07:54 2023, max compression
```

## Comparing `ml-starter-0.1.48.tar` & `ml-starter-0.1.49.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 23:13:28.000000 ml-starter-0.1.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 23:13:28.000000 ml-starter-0.1.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 23:13:45.926980 ml-starter-0.1.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-07 23:13:28.000000 ml-starter-0.1.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.890980 ml-starter-0.1.48/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.894980 ml-starter-0.1.48/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.894980 ml-starter-0.1.48/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.914980 ml-starter-0.1.48/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.914980 ml-starter-0.1.48/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/grad_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.922980 ml-starter-0.1.48/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-07 23:13:28.000000 ml-starter-0.1.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 23:13:45.926980 ml-starter-0.1.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-07 23:13:28.000000 ml-starter-0.1.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 16:07:42.000000 ml-starter-0.1.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 16:07:42.000000 ml-starter-0.1.49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 16:07:54.075945 ml-starter-0.1.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 16:07:42.000000 ml-starter-0.1.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.059944 ml-starter-0.1.49/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.063944 ml-starter-0.1.49/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.067944 ml-starter-0.1.49/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.071944 ml-starter-0.1.49/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28186 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.071944 ml-starter-0.1.49/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/grad_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-08 16:07:42.000000 ml-starter-0.1.49/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:07:54.075945 ml-starter-0.1.49/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-08 16:07:54.000000 ml-starter-0.1.49/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 16:07:42.000000 ml-starter-0.1.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 16:07:54.079944 ml-starter-0.1.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-08 16:07:42.000000 ml-starter-0.1.49/setup.py
```

### Comparing `ml-starter-0.1.48/LICENSE` & `ml-starter-0.1.49/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/PKG-INFO` & `ml-starter-0.1.49/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.48
+Version: 0.1.49
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.48/README.md` & `ml-starter-0.1.49/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/api.py` & `ml-starter-0.1.49/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/core/common_types.py` & `ml-starter-0.1.49/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/core/config.py` & `ml-starter-0.1.49/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/core/env.py` & `ml-starter-0.1.49/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/core/registry.py` & `ml-starter-0.1.49/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/core/state.py` & `ml-starter-0.1.49/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/launchers/base.py` & `ml-starter-0.1.49/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/launchers/mp.py` & `ml-starter-0.1.49/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/launchers/sagemaker.py` & `ml-starter-0.1.49/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/launchers/slurm.py` & `ml-starter-0.1.49/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/launchers/torchrun.py` & `ml-starter-0.1.49/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/loggers/base.py` & `ml-starter-0.1.49/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/loggers/meter.py` & `ml-starter-0.1.49/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/loggers/multi.py` & `ml-starter-0.1.49/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/loggers/stdout.py` & `ml-starter-0.1.49/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/loggers/tensorboard.py` & `ml-starter-0.1.49/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/base.py` & `ml-starter-0.1.49/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/constant.py` & `ml-starter-0.1.49/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.49/ml/lr_schedulers/cosine.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from ml.core.registry import register_lr_scheduler
 from ml.core.state import State
 from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
 
 
 @dataclass
 class CosineLRSchedulerConfig(BaseLRSchedulerConfig):
-    phase: int = conf_field(II("task.max_steps"), help="Number of steps in a phase")
+    total_steps: int = conf_field(II("task.max_steps"), help="Total number of steps to run")
+    num_resets: int = conf_field(0, help="Number of times to reset learning")
+    phase: int = conf_field(MISSING, help="Number of steps in a phase")
     ramp_up_percent: float = conf_field(0.05, help="Percent of phase to spend ramping up")
     ramp_up_steps: int = conf_field(MISSING, help="Number of steps to spend ramping up")
     eta_min: float = conf_field(0.01, help="Minimum learning rate scale")
     eta_max: float = conf_field(1.0, help="Maximum learning rate scale")
 
     @classmethod
     def resolve(cls, config: "CosineLRSchedulerConfig") -> None:
+        if OmegaConf.is_missing(config, "phase"):
+            config.phase = int(config.total_steps / (config.num_resets + 1))
         if OmegaConf.is_missing(config, "ramp_up_steps"):
             assert 0 <= config.ramp_up_percent < 1
             config.ramp_up_steps = int(config.phase * config.ramp_up_percent)
         else:
             assert config.ramp_up_steps < config.phase
         return super().resolve(config)
```

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.49/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/gan.py` & `ml-starter-0.1.49/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/linear.py` & `ml-starter-0.1.49/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.49/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.49/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/activations.py` & `ml-starter-0.1.49/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/architectures/bifpn.py` & `ml-starter-0.1.49/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/architectures/unet.py` & `ml-starter-0.1.49/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/base.py` & `ml-starter-0.1.49/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/codebook.py` & `ml-starter-0.1.49/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/embeddings.py` & `ml-starter-0.1.49/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/gan.py` & `ml-starter-0.1.49/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/init.py` & `ml-starter-0.1.49/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/kmeans.py` & `ml-starter-0.1.49/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/lora.py` & `ml-starter-0.1.49/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/modules.py` & `ml-starter-0.1.49/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/norms.py` & `ml-starter-0.1.49/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/models/parallel.py` & `ml-starter-0.1.49/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/adam.py` & `ml-starter-0.1.49/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/adan.py` & `ml-starter-0.1.49/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/base.py` & `ml-starter-0.1.49/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/common.py` & `ml-starter-0.1.49/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/gan.py` & `ml-starter-0.1.49/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/lion.py` & `ml-starter-0.1.49/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/sgd.py` & `ml-starter-0.1.49/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/optimizers/shampoo.py` & `ml-starter-0.1.49/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/scripts/cli.py` & `ml-starter-0.1.49/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/scripts/stage.py` & `ml-starter-0.1.49/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/scripts/train.py` & `ml-starter-0.1.49/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/base.py` & `ml-starter-0.1.49/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.49/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.49/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/collate.py` & `ml-starter-0.1.49/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.49/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.49/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.49/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.49/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.49/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.49/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.49/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.49/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/environments/base.py` & `ml-starter-0.1.49/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/environments/utils.py` & `ml-starter-0.1.49/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/environments/worker.py` & `ml-starter-0.1.49/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/gan/base.py` & `ml-starter-0.1.49/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/losses/audio.py` & `ml-starter-0.1.49/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/losses/image.py` & `ml-starter-0.1.49/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/losses/kl.py` & `ml-starter-0.1.49/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/losses/loss.py` & `ml-starter-0.1.49/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/rl/base.py` & `ml-starter-0.1.49/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/rl/replay.py` & `ml-starter-0.1.49/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/tasks/sl/base.py` & `ml-starter-0.1.49/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/base.py` & `ml-starter-0.1.49/ml/trainers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             OmegaConf.save(raw_config, config_path)
             logger.info("Saved config to %s", config_path)
 
 
 @dataclass
 class CheckpointConfig:
     save_every_n_steps: int | None = conf_field(None, help="Save a checkpoint every N steps")
-    save_every_n_seconds: int | None = conf_field(60 * 60, help="Save a checkpoint every N seconds")
+    save_every_n_seconds: float | None = conf_field(60.0 * 60.0, help="Save a checkpoint every N seconds")
     only_save_most_recent: bool = conf_field(False, help="Only keep the most recent checkpoint")
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
     load_strict: bool = conf_field(True, help="If set, only load weights for which have a matching key in the model")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
@@ -397,19 +397,26 @@
                         return
                     if try_load_state_dict(model, {f"{prefix}{k}": v for k, v in state_dict.items()}):
                         return
 
                 # Final call, just to throw the error if it still fails.
                 model.load_state_dict(state_dict, strict=strict_non_none)
 
-            with safetensors.safe_open(ckpt, framework="pt", device=device) as f:
-                ckpt_tensors: dict[str, Tensor] = {}
-                for k in f.keys():
-                    ckpt_tensors[k] = f.get_tensor(k)
-                metadata = f.metadata()
+            try:
+                with safetensors.safe_open(ckpt, framework="pt", device=device) as f:
+                    ckpt_tensors: dict[str, Tensor] = {}
+                    for k in f.keys():
+                        ckpt_tensors[k] = f.get_tensor(k)
+                    metadata = f.metadata()
+
+            except Exception:
+                logger.exception("Loading with safetensors failed, falling back to torch.load")
+                ckpt_dict = torch.load(ckpt, map_location=device)
+                ckpt_tensors = ckpt_dict["state"]
+                metadata = ckpt_dict.get("metadata", {})
 
             # Copies back removed pointers.
             if "removed" in metadata:
                 for removed_name, kept_name in json.loads(metadata["removed"]).items():
                     if kept_name in ckpt_tensors:
                         ckpt_tensors[removed_name] = ckpt_tensors[kept_name]
 
@@ -509,33 +516,38 @@
                         lrsd = {f"lr.{k}": v for k, v in lr_scheds.state_dict().items()}
                     add_state_dict("lr", lrsd)
 
                 if self._raw_config is not None:
                     metadata["config"] = OmegaConf.to_yaml(self._raw_config)
 
                 # Removes duplicate tensors.
-                to_removes = _remove_duplicate_names(state_dict)
-                removed: dict[str, str] = {}
-                for kept_name, to_remove_group in to_removes.items():
-                    for to_remove in to_remove_group:
-                        if to_remove not in metadata:
-                            removed[to_remove] = kept_name
-                        del state_dict[to_remove]
-                metadata["removed"] = json.dumps(removed)
-
-                self.update_state_dict(state_dict, metadata)
-
-                if last_ckpt_path.exists():
-                    if self.checkpoint_config.only_save_most_recent:
-                        base_ckpt = last_ckpt_path.resolve()
-                        if base_ckpt.is_file():
-                            base_ckpt.unlink()
-                    last_ckpt_path.unlink()
-
-                safetensors_save_file(state_dict, ckpt_path, metadata)
+                try:
+                    to_removes = _remove_duplicate_names(state_dict)
+                    removed: dict[str, str] = {}
+                    for kept_name, to_remove_group in to_removes.items():
+                        for to_remove in to_remove_group:
+                            if to_remove not in metadata:
+                                removed[to_remove] = kept_name
+                            del state_dict[to_remove]
+                    metadata["removed"] = json.dumps(removed)
+
+                    self.update_state_dict(state_dict, metadata)
+
+                    if last_ckpt_path.exists():
+                        if self.checkpoint_config.only_save_most_recent:
+                            base_ckpt = last_ckpt_path.resolve()
+                            if base_ckpt.is_file():
+                                base_ckpt.unlink()
+                        last_ckpt_path.unlink()
+
+                    safetensors_save_file(state_dict, ckpt_path, metadata)
+
+                except Exception:
+                    logger.exception("Saving with safetensors failed, falling back to torch.save")
+                    torch.save({"state": state_dict, "metadata": metadata}, ckpt_path)
 
                 try:
                     last_ckpt_path.symlink_to(ckpt_path)
                 except FileExistsError:
                     logger.exception("Exception while trying to update %s", ckpt_path)
                 self.add_lock_file("ckpt", exists_ok=True)
                 task.on_after_save_checkpoint(ckpt_path)
```

### Comparing `ml-starter-0.1.48/ml/trainers/gan.py` & `ml-starter-0.1.49/ml/trainers/gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,16 +202,15 @@
                                     optim=optim,
                                     lr_sched=lr_sched,
                                 )
 
                         except EpochDoneError:
                             break
 
-                        valid_every_n_steps = self.config.validation.valid_every_n_steps
-                        if valid_every_n_steps is not None and state.num_steps % valid_every_n_steps == 0:
+                        if self.should_validate(state):
                             self._log_prefetcher_stats(valid_pf)
 
                             with namespace_context(self._logging_key(task, state, "valid")):
                                 val_step(
                                     task_model=task_model,
                                     batch=next(valid_pf_iter),
                                     state=state,
```

### Comparing `ml-starter-0.1.48/ml/trainers/learning.py` & `ml-starter-0.1.49/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/compile.py` & `ml-starter-0.1.49/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.49/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.49/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.49/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/grad_balancer.py` & `ml-starter-0.1.49/ml/trainers/mixins/grad_balancer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.49/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.49/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.49/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.49/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.49/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/rl.py` & `ml-starter-0.1.49/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/trainers/sl.py` & `ml-starter-0.1.49/ml/trainers/sl.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ValidationConfig:
-    valid_every_n_steps: int | None = conf_field(100, help="Number of training steps to run per test step")
+    valid_every_n_steps: int | None = conf_field(None, help="Number of training steps to run per validation step")
+    valid_every_n_seconds: float | None = conf_field(60.0 * 10.0, help="Run validation every N seconds")
     num_init_valid_steps: int | None = conf_field(1, help="Number of initial validation steps")
 
 
 @dataclass
 class BatchScheduleConfig:
     num_steps: int = conf_field(MISSING, help="Number of steps to run for")
     num_batches: int = conf_field(MISSING, help="Number of minibatches for a given step")
@@ -68,14 +69,19 @@
 
 
 @register_trainer("sl", SupervisedLearningTrainerConfig)
 class SupervisedLearningTrainer(
     BaseLearningTrainer[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
     Generic[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
 ):
+    def __init__(self, config: SupervisedLearningTrainerConfigT) -> None:
+        super().__init__(config)
+
+        self.last_valid_time = 0.0
+
     @functools.lru_cache()
     def batches_per_step_schedule(self) -> list[tuple[int, int]] | None:
         schedule = self.config.batches_per_step_schedule
         if schedule is None:
             return None
         if any(s.num_steps <= 0 or s.num_batches <= 0 for s in schedule):
             raise ValueError("steps and num_batches must be non-negative")
@@ -102,14 +108,28 @@
 
     def get_batch_chunks(self, state: State) -> int:
         if (schedule := self.batch_chunks_schedule()) is None:
             return 1
         i = bisect.bisect_left(schedule, (state.num_steps, 0))
         return 1 if i == len(schedule) else schedule[i][1]
 
+    def should_validate(self, state: State) -> bool:
+        # Step-based validation.
+        valid_every_n_steps = self.config.validation.valid_every_n_steps
+        if valid_every_n_steps is not None and state.num_steps % valid_every_n_steps == 0:
+            return True
+
+        # Time-based validation.
+        valid_every_n_seconds = self.config.validation.valid_every_n_seconds
+        if valid_every_n_seconds is not None and state.elapsed_time_s - self.last_valid_time >= valid_every_n_seconds:
+            self.last_valid_time += valid_every_n_seconds
+            return True
+
+        return False
+
     def train(
         self,
         model: ModelT,
         task: SupervisedLearningTaskT,
         optimizer: BaseOptimizer,
         lr_scheduler: BaseLRScheduler,
     ) -> None:
@@ -232,16 +252,15 @@
                                 optim=optim,
                                 lr_sched=lr_sched,
                             )
 
                         except EpochDoneError:
                             break
 
-                        valid_every_n_steps = self.config.validation.valid_every_n_steps
-                        if valid_every_n_steps is not None and state.num_steps % valid_every_n_steps == 0:
+                        if self.should_validate(state):
                             self._log_prefetcher_stats(valid_pf)
 
                             val_step(
                                 task_model=task_model,
                                 batch=next(valid_pf_iter),
                                 state=state,
                                 task=task,
```

### Comparing `ml-starter-0.1.48/ml/utils/amp.py` & `ml-starter-0.1.49/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/argparse.py` & `ml-starter-0.1.49/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/atomic.py` & `ml-starter-0.1.49/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/attention.py` & `ml-starter-0.1.49/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/audio.py` & `ml-starter-0.1.49/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/augmentation.py` & `ml-starter-0.1.49/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/caching.py` & `ml-starter-0.1.49/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/checkpoint.py` & `ml-starter-0.1.49/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/cli.py` & `ml-starter-0.1.49/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/colors.py` & `ml-starter-0.1.49/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/containers.py` & `ml-starter-0.1.49/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/data.py` & `ml-starter-0.1.49/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/datetime.py` & `ml-starter-0.1.49/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/device/auto.py` & `ml-starter-0.1.49/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/device/base.py` & `ml-starter-0.1.49/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/device/cpu.py` & `ml-starter-0.1.49/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/device/gpu.py` & `ml-starter-0.1.49/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/device/metal.py` & `ml-starter-0.1.49/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/distributed.py` & `ml-starter-0.1.49/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/exceptions.py` & `ml-starter-0.1.49/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/image.py` & `ml-starter-0.1.49/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/io.py` & `ml-starter-0.1.49/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/large_models.py` & `ml-starter-0.1.49/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/logging.py` & `ml-starter-0.1.49/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/meter.py` & `ml-starter-0.1.49/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/mixed_precision.py` & `ml-starter-0.1.49/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/networking.py` & `ml-starter-0.1.49/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/numpy.py` & `ml-starter-0.1.49/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/parallel.py` & `ml-starter-0.1.49/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/spectrogram.py` & `ml-starter-0.1.49/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/staging.py` & `ml-starter-0.1.49/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/testing.py` & `ml-starter-0.1.49/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/timer.py` & `ml-starter-0.1.49/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/tokens.py` & `ml-starter-0.1.49/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/torch_distributed.py` & `ml-starter-0.1.49/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/triton/kmeans.py` & `ml-starter-0.1.49/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/triton/lion.py` & `ml-starter-0.1.49/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml/utils/video.py` & `ml-starter-0.1.49/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.49/ml_starter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.48
+Version: 0.1.49
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.48/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.49/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/pyproject.toml` & `ml-starter-0.1.49/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.48/setup.py` & `ml-starter-0.1.49/setup.py`

 * *Files identical despite different names*

