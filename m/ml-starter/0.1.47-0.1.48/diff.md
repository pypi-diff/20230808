# Comparing `tmp/ml-starter-0.1.47.tar.gz` & `tmp/ml-starter-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.47.tar", last modified: Fri Aug  4 21:42:29 2023, max compression
+gzip compressed data, was "ml-starter-0.1.48.tar", last modified: Mon Aug  7 23:13:45 2023, max compression
```

## Comparing `ml-starter-0.1.47.tar` & `ml-starter-0.1.48.tar`

### file list

```diff
@@ -1,190 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.032661 ml-starter-0.1.47/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 21:42:15.000000 ml-starter-0.1.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-04 21:42:15.000000 ml-starter-0.1.47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 21:42:29.032661 ml-starter-0.1.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-04 21:42:15.000000 ml-starter-0.1.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:28.992660 ml-starter-0.1.47/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:28.996660 ml-starter-0.1.47/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:28.996660 ml-starter-0.1.47/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:28.996660 ml-starter-0.1.47/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.000660 ml-starter-0.1.47/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.000660 ml-starter-0.1.47/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.004660 ml-starter-0.1.47/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.004660 ml-starter-0.1.47/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.004660 ml-starter-0.1.47/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.008660 ml-starter-0.1.47/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.008660 ml-starter-0.1.47/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.008660 ml-starter-0.1.47/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.012660 ml-starter-0.1.47/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.012660 ml-starter-0.1.47/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.012660 ml-starter-0.1.47/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.012660 ml-starter-0.1.47/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.016660 ml-starter-0.1.47/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.016660 ml-starter-0.1.47/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.016660 ml-starter-0.1.47/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.020660 ml-starter-0.1.47/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.028660 ml-starter-0.1.47/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.028660 ml-starter-0.1.47/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.028660 ml-starter-0.1.47/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-04 21:42:15.000000 ml-starter-0.1.47/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:29.032661 ml-starter-0.1.47/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 21:42:28.000000 ml-starter-0.1.47/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-04 21:42:28.000000 ml-starter-0.1.47/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:42:28.000000 ml-starter-0.1.47/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-04 21:42:28.000000 ml-starter-0.1.47/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-04 21:42:28.000000 ml-starter-0.1.47/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-04 21:42:15.000000 ml-starter-0.1.47/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 21:42:29.032661 ml-starter-0.1.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-04 21:42:15.000000 ml-starter-0.1.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 23:13:28.000000 ml-starter-0.1.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 23:13:28.000000 ml-starter-0.1.48/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 23:13:45.926980 ml-starter-0.1.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-07 23:13:28.000000 ml-starter-0.1.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.890980 ml-starter-0.1.48/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.894980 ml-starter-0.1.48/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.894980 ml-starter-0.1.48/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.898980 ml-starter-0.1.48/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.902980 ml-starter-0.1.48/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.906980 ml-starter-0.1.48/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.910980 ml-starter-0.1.48/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.914980 ml-starter-0.1.48/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.914980 ml-starter-0.1.48/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/grad_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.922980 ml-starter-0.1.48/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-07 23:13:28.000000 ml-starter-0.1.48/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:13:45.926980 ml-starter-0.1.48/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-07 23:13:45.000000 ml-starter-0.1.48/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-07 23:13:28.000000 ml-starter-0.1.48/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 23:13:45.926980 ml-starter-0.1.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-07 23:13:28.000000 ml-starter-0.1.48/setup.py
```

### Comparing `ml-starter-0.1.47/LICENSE` & `ml-starter-0.1.48/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/PKG-INFO` & `ml-starter-0.1.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.47
+Version: 0.1.48
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.47/README.md` & `ml-starter-0.1.48/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/api.py` & `ml-starter-0.1.48/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "BiFPN",
     "cached_object",
     "cast_activation_type",
     "cast_beta_schedule",
     "cast_embedding_kind",
     "cast_init_type",
     "cast_norm_type",
+    "cast_parametrize_norm_type",
     "check_md5",
     "check_sha256",
     "ChunkSampler",
     "Clamp",
     "ClippifyDataset",
     "collate_non_null",
     "collate",
@@ -98,14 +99,15 @@
     "get_master_addr",
     "get_master_port",
     "get_model_dir",
     "get_norm_1d",
     "get_norm_2d",
     "get_norm_3d",
     "get_norm_linear",
+    "get_parametrization_norm",
     "get_positional_embeddings",
     "get_random_port",
     "get_rank_optional",
     "get_rank",
     "get_run_dir",
     "get_state_dict_prefix",
     "get_type_from_string",
@@ -155,14 +157,15 @@
     "open_atomic",
     "Output",
     "pad_all",
     "pad_sequence",
     "parallel_group_info",
     "ParallelEmbedding",
     "parallelism_is_initialized",
+    "ParametrizationNormType",
     "parse_cli",
     "Phase",
     "Prefetcher",
     "project_dir_paths",
     "read_audio_random_order",
     "read_audio",
     "read_gif",
@@ -276,15 +279,25 @@
     freeze_non_lora_,
     lora,
     maybe_lora,
     maybe_lora_weight_norm,
     reset_lora_weights_,
 )
 from ml.models.modules import combine_grads, invert_grad, scale_grad, swap_grads
-from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
+from ml.models.norms import (
+    NormType,
+    ParametrizationNormType,
+    cast_norm_type,
+    cast_parametrize_norm_type,
+    get_norm_1d,
+    get_norm_2d,
+    get_norm_3d,
+    get_norm_linear,
+    get_parametrization_norm,
+)
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
 from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
```

### Comparing `ml-starter-0.1.47/ml/core/common_types.py` & `ml-starter-0.1.48/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/core/config.py` & `ml-starter-0.1.48/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/core/env.py` & `ml-starter-0.1.48/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/core/registry.py` & `ml-starter-0.1.48/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/core/state.py` & `ml-starter-0.1.48/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/launchers/base.py` & `ml-starter-0.1.48/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/launchers/mp.py` & `ml-starter-0.1.48/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/launchers/sagemaker.py` & `ml-starter-0.1.48/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/launchers/slurm.py` & `ml-starter-0.1.48/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/launchers/torchrun.py` & `ml-starter-0.1.48/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/loggers/base.py` & `ml-starter-0.1.48/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/loggers/meter.py` & `ml-starter-0.1.48/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/loggers/multi.py` & `ml-starter-0.1.48/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/loggers/stdout.py` & `ml-starter-0.1.48/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/loggers/tensorboard.py` & `ml-starter-0.1.48/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/base.py` & `ml-starter-0.1.48/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/constant.py` & `ml-starter-0.1.48/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.48/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.48/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/gan.py` & `ml-starter-0.1.48/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/linear.py` & `ml-starter-0.1.48/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.48/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.48/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/activations.py` & `ml-starter-0.1.48/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/architectures/bifpn.py` & `ml-starter-0.1.48/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/architectures/unet.py` & `ml-starter-0.1.48/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/base.py` & `ml-starter-0.1.48/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/codebook.py` & `ml-starter-0.1.48/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/embeddings.py` & `ml-starter-0.1.48/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/gan.py` & `ml-starter-0.1.48/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/init.py` & `ml-starter-0.1.48/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/kmeans.py` & `ml-starter-0.1.48/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/lora.py` & `ml-starter-0.1.48/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/modules.py` & `ml-starter-0.1.48/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/models/norms.py` & `ml-starter-0.1.48/ml/models/norms.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,38 +20,52 @@
 - ``"instance"`` or ``"instance_affine"``: Instance normalization
 - ``"group"`` or ``"group_affine"``: Group normalization
 - ``"layer"`` or ``"layer_affine"``: Layer normalization
 
 Note that instance norm and group norm are not available for linear layers.
 """
 
-from typing import Literal, cast, get_args
+from typing import Literal, TypeVar, cast, get_args
 
 import torch
 from torch import Tensor, nn
 
+T_module = TypeVar("T_module", bound=nn.Module)
+
 NormType = Literal[
     "no_norm",
     "batch",
     "batch_affine",
     "instance",
     "instance_affine",
     "group",
     "group_affine",
     "layer",
     "layer_affine",
 ]
 
+ParametrizationNormType = Literal[
+    "no_norm",
+    "weight",
+    "spectral",
+]
+
 
 def cast_norm_type(s: str) -> NormType:
     args = get_args(NormType)
     assert s in args, f"Invalid norm type: '{s}' Valid options are {args}"
     return cast(NormType, s)
 
 
+def cast_parametrize_norm_type(s: str) -> ParametrizationNormType:
+    args = get_args(ParametrizationNormType)
+    assert s in args, f"Invalid parametrization norm type: '{s}' Valid options are {args}"
+    return cast(ParametrizationNormType, s)
+
+
 class LastBatchNorm(nn.Module):
     """Applies batch norm along final dimension without transposing the tensor.
 
     The normalization is pretty simple, it basically just tracks the running
     mean and variance for each channel, then normalizes each channel to have
     a unit normal distribution.
 
@@ -328,7 +342,57 @@
             assert dim is not None, "`dim` is required for batch norm"
             return LastBatchNorm(dim, affine=norm == "batch_affine", device=device, dtype=dtype)
         case "layer" | "layer_affine":
             assert dim is not None, "`dim` is required for layer norm"
             return nn.LayerNorm(dim, elementwise_affine=norm == "layer_affine", device=device, dtype=dtype)
         case _:
             raise NotImplementedError(f"Invalid linear norm type: {norm}")
+
+
+def get_parametrization_norm(
+    module: T_module,
+    norm: ParametrizationNormType,
+    *,
+    name: str = "weight",
+    n_power_iterations: int = 1,
+    eps: float = 1e-12,
+    weight_dim: int = 0,
+    spectral_dim: int | None = None,
+) -> T_module:
+    """Returns a parametrized version of the module.
+
+    Args:
+        module: The module to parametrize
+        norm: The parametrization norm type to use
+        name: The name of the parameter to use for the parametrization; this
+            should reference the name on the module (for instance, ``weight``
+            for a ``nn.Linear`` module)
+        n_power_iterations: The number of power iterations to use for spectral
+            normalization
+        eps: The epsilon value to use for spectral normalization
+        weight_dim: The dimension of the weight parameter to normalize when
+            using weight normalization
+        spectral_dim: The dimension of the weight parameter to normalize when
+            using spectral normalization
+
+    Returns:
+        The parametrized module
+    """
+    match norm:
+        case "no_norm":
+            return module
+        case "weight":
+            return nn.utils.weight_norm(
+                module,
+                name=name,
+                dim=weight_dim,
+            )
+        case "spectral":
+            return nn.utils.spectral_norm(
+                module,
+                name=name,
+                n_power_iterations=n_power_iterations,
+                eps=eps,
+                dim=spectral_dim,
+            )
+        case _:
+            raise NotImplementedError(f"Invalid parametrization norm type: {norm}")
```

### Comparing `ml-starter-0.1.47/ml/models/parallel.py` & `ml-starter-0.1.48/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/adam.py` & `ml-starter-0.1.48/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/adan.py` & `ml-starter-0.1.48/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/base.py` & `ml-starter-0.1.48/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/common.py` & `ml-starter-0.1.48/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/gan.py` & `ml-starter-0.1.48/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/lion.py` & `ml-starter-0.1.48/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/sgd.py` & `ml-starter-0.1.48/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/optimizers/shampoo.py` & `ml-starter-0.1.48/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/scripts/cli.py` & `ml-starter-0.1.48/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/scripts/stage.py` & `ml-starter-0.1.48/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/scripts/train.py` & `ml-starter-0.1.48/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/base.py` & `ml-starter-0.1.48/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.48/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.48/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/collate.py` & `ml-starter-0.1.48/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.48/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.48/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.48/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.48/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.48/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.48/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.48/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.48/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/environments/base.py` & `ml-starter-0.1.48/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/environments/utils.py` & `ml-starter-0.1.48/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/environments/worker.py` & `ml-starter-0.1.48/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/gan/base.py` & `ml-starter-0.1.48/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/losses/audio.py` & `ml-starter-0.1.48/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/losses/image.py` & `ml-starter-0.1.48/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/losses/kl.py` & `ml-starter-0.1.48/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/losses/loss.py` & `ml-starter-0.1.48/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/rl/base.py` & `ml-starter-0.1.48/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/rl/replay.py` & `ml-starter-0.1.48/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/tasks/sl/base.py` & `ml-starter-0.1.48/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/base.py` & `ml-starter-0.1.48/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/gan.py` & `ml-starter-0.1.48/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/learning.py` & `ml-starter-0.1.48/ml/trainers/learning.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 if bsz is not None:
                     total_bsz = bsz if total_bsz is None else total_bsz + bsz
                 with self.step_context("forward"):
                     loss = task_model(batch, state)
                 with self.step_context("get_single_loss"):
                     single_loss, loss_names = task.get_single_loss(loss)
                 with self.step_context("backward"):
-                    self.backward_grads(task_model, single_loss)
+                    self.backward_grads(task_model, single_loss, loss_names)
                 with self.step_context("log_losses"):
                     self.log_mp_scale()
                     single_loss_detached = single_loss.detach()
                     for i, name in enumerate(loss_names):
                         new_loss = single_loss_detached[i]
                         if name in losses:
                             old_loss, count = losses[name]
```

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/compile.py` & `ml-starter-0.1.48/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.48/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.48/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.48/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.48/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.48/ml/trainers/mixins/mixed_precision.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,38 @@
 import torch
 from torch import Tensor, nn
 from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel as FSDP
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig, ModelT, TaskT
+from ml.trainers.mixins.grad_balancer import GradBalancer
 from ml.utils.exceptions import MinGradScaleError, NaNError
 from ml.utils.mixed_precision import clip_grad_norm_, get_weight_norm
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class MixedPrecisionConfig:
     enabled: bool = conf_field(True, help="If set, should FP16 training be enabled")
     init_scale: float = conf_field(2.0**16, help="Initial scaling factor")
     growth_factor: float = conf_field(2.0, help="Factor by which the scale is multiplied if no gradient NaNs occur")
     backoff_factor: float = conf_field(0.5, help="Factor by which the scale is multiplied if gradient NaNs occur")
     growth_interval: int = conf_field(2000, help="How often to grow the scale")
     min_grad_scale: float = conf_field(1e-4, help="Minimum allowable gradient scale")
+    foreach: bool | None = conf_field(None, help="If set, use foreach implementation")
 
 
 @dataclass
 class MixedPrecisionTrainerConfig(BaseTrainerConfig):
     mixed_precision: MixedPrecisionConfig = conf_field(MixedPrecisionConfig(), help="Mixed precision configuration")
     clip_grad_norm: float = conf_field(10.0, help="What to clip the gradient norm to")
     clip_grad_norm_type: Any = conf_field(2, help="Type of norm to use")
+    balance_grad_norms: bool = conf_field(False, help="If set, balance gradient norms")
 
 
 MixedPrecisionConfigT = TypeVar("MixedPrecisionConfigT", bound=MixedPrecisionTrainerConfig)
 
 
 class MixedPrecisionTrainerMixin(BaseTrainer[MixedPrecisionConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for doing FP16 scaling."""
@@ -61,24 +64,37 @@
                 enabled=True,
             )
         else:
             self.grad_scaler = None
 
         self.autocast_context = self._device.autocast_context(enabled=self.config.mixed_precision.enabled)
 
+        self.balancer = (
+            GradBalancer(
+                logger=self.logger,
+                total_norm=self.config.clip_grad_norm,
+                norm_type=self.config.clip_grad_norm_type,
+                foreach=self.config.mixed_precision.foreach,
+            )
+            if self.config.balance_grad_norms
+            else None
+        )
+
     def scale_mixed_precision(self, tensor: Tensor) -> Tensor:
         if self.grad_scaler is not None:
             return self.grad_scaler.scale(tensor)
         return tensor
 
-    def backward_grads(self, model: nn.Module, loss: Tensor) -> None:
-        if loss.numel() > 1:
-            loss = loss.sum()
+    def backward_grads(self, model: nn.Module, loss: Tensor, loss_names: list[str]) -> None:
         if self.grad_scaler is not None:
             loss = self.grad_scaler.scale(loss)
+        if self.balancer is not None:
+            loss = self.balancer.balance(model, loss, loss_names)
+        if loss.numel() > 1:
+            loss = loss.sum()
         isnan = not bool(torch.isfinite(loss))
         if isnan:
             loss.backward(torch.zeros_like(loss))
         else:
             loss.backward()
 
         if isnan:
@@ -93,14 +109,16 @@
                     self.grad_scaler.update(new_scale)
 
     @torch.no_grad()
     def step_optimizer(self, model: nn.Module, optim: Optimizer, num_steps: int = 1) -> None:
         clip_norm = self.config.clip_grad_norm
         norm_type = self.config.clip_grad_norm_type
 
+        # When accumulating multiple steps of gradients per backward pass, we
+        # need to divide the gradients by the number of steps.
         if num_steps > 1:
             for p in model.parameters():
                 if p.grad is not None:
                     p.grad /= num_steps
 
         # Unscale gradients.
         if self.grad_scaler is not None:
@@ -111,15 +129,15 @@
             total_norm = model.clip_grad_norm_(clip_norm, norm_type)
             was_clipped = bool(torch.isfinite(total_norm))
         else:
             total_norm, was_clipped = clip_grad_norm_(
                 model.parameters(),
                 max_norm=clip_norm,
                 norm_type=norm_type,
-                foreach=True,
+                foreach=self.config.mixed_precision.foreach,
             )
 
         # Logs weight and gradient norms.
         self.logger.log_scalar("weight_norm", lambda: get_weight_norm(model.parameters()), namespace="📉 optim")
         self.logger.log_scalar("grad_norm", total_norm, namespace="📉 optim")
 
         # Steps the optimizer.
```

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.48/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.48/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.48/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/rl.py` & `ml-starter-0.1.48/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/trainers/sl.py` & `ml-starter-0.1.48/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/amp.py` & `ml-starter-0.1.48/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/argparse.py` & `ml-starter-0.1.48/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/atomic.py` & `ml-starter-0.1.48/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/attention.py` & `ml-starter-0.1.48/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/audio.py` & `ml-starter-0.1.48/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/augmentation.py` & `ml-starter-0.1.48/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/caching.py` & `ml-starter-0.1.48/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/checkpoint.py` & `ml-starter-0.1.48/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/cli.py` & `ml-starter-0.1.48/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/colors.py` & `ml-starter-0.1.48/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/containers.py` & `ml-starter-0.1.48/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/data.py` & `ml-starter-0.1.48/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/datetime.py` & `ml-starter-0.1.48/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/device/auto.py` & `ml-starter-0.1.48/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/device/base.py` & `ml-starter-0.1.48/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/device/cpu.py` & `ml-starter-0.1.48/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/device/gpu.py` & `ml-starter-0.1.48/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/device/metal.py` & `ml-starter-0.1.48/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/distributed.py` & `ml-starter-0.1.48/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/exceptions.py` & `ml-starter-0.1.48/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/image.py` & `ml-starter-0.1.48/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/io.py` & `ml-starter-0.1.48/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/large_models.py` & `ml-starter-0.1.48/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/logging.py` & `ml-starter-0.1.48/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/meter.py` & `ml-starter-0.1.48/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/mixed_precision.py` & `ml-starter-0.1.48/ml/utils/mixed_precision.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,42 @@
                 norms.extend([torch.norm(g, norm_type) for g in param])
         total_norm = torch.norm(torch.stack([norm.to(first_device) for norm in norms]), norm_type)
 
     return total_norm
 
 
 @torch.no_grad()
+def get_grad_norm(
+    parameters: Iterable[nn.Parameter],
+    norm_type: float = 2.0,
+    foreach: bool | None = None,
+) -> tuple[Tensor, GradDict]:
+    grads = [p.grad for p in parameters if p.grad is not None]
+    if len(grads) == 0:
+        return torch.tensor([0.0]), {}
+
+    first_device = grads[0].device
+    grouped_grads = cast(GradDict, _group_tensors_by_device_and_dtype([[g.detach() for g in grads]]))
+
+    if norm_type == inf:
+        norms = [g.detach().abs().max().to(first_device) for g in grads]
+        total_norm = norms[0] if len(norms) == 1 else torch.max(torch.stack(norms))
+    else:
+        norms = []
+        for (device, _), [grads] in grouped_grads.items():
+            if (foreach is None or foreach) and _has_foreach_support(grads, device=device):
+                norms.extend(torch._foreach_norm(grads, norm_type))
+            else:
+                norms.extend([torch.norm(g, norm_type) for g in grads])
+        total_norm = torch.norm(torch.stack([norm.to(first_device) for norm in norms]), norm_type)
+
+    return total_norm, grouped_grads
+
+
+@torch.no_grad()
 def clip_grad_norm_(
     parameters: Iterable[nn.Parameter],
     max_norm: float,
     norm_type: float = 2.0,
     foreach: bool | None = None,
 ) -> tuple[Tensor, bool]:
     """Clips gradient norm of an iterable of parameters.
@@ -73,32 +101,15 @@
             implementation, respectively, and raise an error if the chosen
             implementation is not available.
 
     Returns:
         The total norm of the parameters (viewed as a single vector) and
         whether the parameters were successfully clipped.
     """
-    grads = [p.grad for p in parameters if p.grad is not None]
-    if len(grads) == 0:
-        return torch.tensor([0.0]), True
-
-    first_device = grads[0].device
-    grouped_grads = cast(GradDict, _group_tensors_by_device_and_dtype([[g.detach() for g in grads]]))
-
-    if norm_type == inf:
-        norms = [g.detach().abs().max().to(first_device) for g in grads]
-        total_norm = norms[0] if len(norms) == 1 else torch.max(torch.stack(norms))
-    else:
-        norms = []
-        for (device, _), [grads] in grouped_grads.items():
-            if (foreach is None or foreach) and _has_foreach_support(grads, device=device):
-                norms.extend(torch._foreach_norm(grads, norm_type))
-            else:
-                norms.extend([torch.norm(g, norm_type) for g in grads])
-        total_norm = torch.norm(torch.stack([norm.to(first_device) for norm in norms]), norm_type)
+    total_norm, grouped_grads = get_grad_norm(parameters, norm_type, foreach)
 
     if not torch.isfinite(total_norm):
         return total_norm, False
 
     clip_coef = max_norm / (total_norm + 1e-6)
     clip_coef_clamped = torch.clamp(clip_coef, max=1.0)
     for (device, _), [grads] in grouped_grads.items():
```

### Comparing `ml-starter-0.1.47/ml/utils/networking.py` & `ml-starter-0.1.48/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/numpy.py` & `ml-starter-0.1.48/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/parallel.py` & `ml-starter-0.1.48/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/spectrogram.py` & `ml-starter-0.1.48/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/staging.py` & `ml-starter-0.1.48/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/testing.py` & `ml-starter-0.1.48/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/timer.py` & `ml-starter-0.1.48/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/tokens.py` & `ml-starter-0.1.48/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/torch_distributed.py` & `ml-starter-0.1.48/ml/utils/torch_distributed.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         RuntimeError: If the function fails in any subprocess.
     """
     MultiprocessConfig.resolve(cfg)
 
     if cfg.world_size <= 1:
         logger.warning("Multi-process trainer expects more than one device; running single-process")
         cfg.rank = 0
-        init_and_run(func, cfg)
+        init_and_run(func, cfg, *args, **kwargs)
         return
 
     logger.info("Launching %d training workers", cfg.world_size)
     ctx = mp.get_context(cfg.launch_method)
     error_queues: list["mp.SimpleQueue[str | None]"] = []
     procs = []
     for rank in range(cfg.world_size):
```

### Comparing `ml-starter-0.1.47/ml/utils/triton/kmeans.py` & `ml-starter-0.1.48/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/triton/lion.py` & `ml-starter-0.1.48/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml/utils/video.py` & `ml-starter-0.1.48/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.48/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.47
+Version: 0.1.48
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.47/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.48/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 ml/trainers/rl.py
 ml/trainers/sl.py
 ml/trainers/mixins/__init__.py
 ml/trainers/mixins/compile.py
 ml/trainers/mixins/cpu_stats.py
 ml/trainers/mixins/data_parallel.py
 ml/trainers/mixins/gpu_stats.py
+ml/trainers/mixins/grad_balancer.py
 ml/trainers/mixins/heartbeat.py
 ml/trainers/mixins/mixed_precision.py
 ml/trainers/mixins/monitor_process.py
 ml/trainers/mixins/profiler.py
 ml/trainers/mixins/step_wrapper.py
 ml/utils/__init__.py
 ml/utils/amp.py
```

### Comparing `ml-starter-0.1.47/pyproject.toml` & `ml-starter-0.1.48/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.47/setup.py` & `ml-starter-0.1.48/setup.py`

 * *Files identical despite different names*

