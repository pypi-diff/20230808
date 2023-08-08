# Comparing `tmp/asociita-0.3.3.tar.gz` & `tmp/asociita-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.3.3.tar", max compression
+gzip compressed data, was "asociita-0.3.4.tar", max compression
```

## Comparing `asociita-0.3.3.tar` & `asociita-0.3.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.3.3/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.3.3/asociita/__init__.py
--rw-r--r--   0        0        0     2725 2023-07-11 10:54:45.641955 asociita-0.3.3/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-07-11 10:54:39.082119 asociita-0.3.3/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0    11701 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4858 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/lsaa_evaluator.cpython-310.pyc
--rw-r--r--   0        0        0     6307 2023-06-16 21:39:14.145401 asociita-0.3.3/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc
--rw-r--r--   0        0        0    14893 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc
--rw-r--r--   0        0        0    18742 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0     5561 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/lsaa_evaluator.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.3.3/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.3.3/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0    18471 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     3999 2023-07-17 16:29:11.910865 asociita-0.3.3/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc
--rw-r--r--   0        0        0     4366 2023-07-16 13:33:46.445218 asociita-0.3.3/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     6270 2023-07-17 19:03:11.725971 asociita-0.3.3/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     5588 2023-07-13 09:26:40.219672 asociita-0.3.3/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     8999 2023-07-17 16:29:11.446877 asociita-0.3.3/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     8790 2023-07-17 19:03:05.726122 asociita-0.3.3/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     7373 2023-07-13 09:23:34.044495 asociita-0.3.3/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11545 2023-07-16 13:33:46.445218 asociita-0.3.3/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     5098 2023-07-12 15:13:21.310949 asociita-0.3.3/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc
--rw-r--r--   0        0        0     4759 2023-07-12 14:39:39.170606 asociita-0.3.3/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc
--rw-r--r--   0        0        0     1663 2023-07-12 14:39:39.170606 asociita-0.3.3/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc
--rw-r--r--   0        0        0    13715 2023-07-11 12:14:58.271395 asociita-0.3.3/asociita/components/settings/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0     6901 2023-07-12 15:13:18.167030 asociita-0.3.3/asociita/components/settings/evaluator_settings.py
--rw-r--r--   0        0        0     5835 2023-07-12 14:39:37.466652 asociita-0.3.3/asociita/components/settings/fedopt_settings.py
--rw-r--r--   0        0        0     1931 2023-07-12 14:39:31.446817 asociita-0.3.3/asociita/components/settings/init_settings.py
--rw-r--r--   0        0        0    23141 2023-07-11 12:14:58.051401 asociita-0.3.3/asociita/components/settings/settings.py
--rw-r--r--   0        0        0     2465 2023-06-07 13:17:41.861780 asociita-0.3.3/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc
--rw-r--r--   0        0        0     1997 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc
--rw-r--r--   0        0        0     2023 2023-06-07 14:35:08.314826 asociita-0.3.3/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc
--rw-r--r--   0        0        0     1420 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc
--rw-r--r--   0        0        0     4844 2023-06-12 11:32:41.024825 asociita-0.3.3/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc
--rw-r--r--   0        0        0     5554 2023-06-14 13:55:29.401627 asociita-0.3.3/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc
--rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.3.3/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.3.3/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.3.3/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.3.3/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.3.3/asociita/datasets/save_blueprint.py
--rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.3.3/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.3.3/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      798 2023-06-05 13:07:28.160901 asociita-0.3.3/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc
--rw-r--r--   0        0        0      442 2023-06-16 12:12:22.850903 asociita-0.3.3/asociita/exceptions/__pycache__/modelexception.cpython-310.pyc
--rw-r--r--   0        0        0      990 2023-06-16 09:02:36.793602 asociita-0.3.3/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.3.3/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.3.3/asociita/exceptions/modelexception.py
--rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.3.3/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0     1139 2023-05-29 09:36:33.144103 asociita-0.3.3/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc
--rw-r--r--   0        0        0    13786 2023-07-17 16:29:11.914865 asociita-0.3.3/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc
--rw-r--r--   0        0        0      557 2023-06-01 15:37:30.741582 asociita-0.3.3/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc
--rw-r--r--   0        0        0     4114 2023-06-14 08:05:54.914256 asociita-0.3.3/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    17178 2023-07-16 13:33:46.449218 asociita-0.3.3/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.3.3/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.3.3/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6202 2023-06-26 13:45:06.401533 asociita-0.3.3/asociita/utils/__pycache__/computations.cpython-310.pyc
--rw-r--r--   0        0        0     1162 2023-05-29 09:36:33.148103 asociita-0.3.3/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc
--rw-r--r--   0        0        0     1575 2023-06-22 17:32:18.144898 asociita-0.3.3/asociita/utils/__pycache__/debugger.cpython-310.pyc
--rw-r--r--   0        0        0     3695 2023-05-29 09:36:33.136103 asociita-0.3.3/asociita/utils/__pycache__/handlers.cpython-310.pyc
--rw-r--r--   0        0        0     2009 2023-06-23 10:59:17.491655 asociita-0.3.3/asociita/utils/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     1079 2023-07-17 16:29:13.102835 asociita-0.3.3/asociita/utils/__pycache__/loggers.cpython-310.pyc
--rw-r--r--   0        0        0     4876 2023-06-26 09:06:30.509538 asociita-0.3.3/asociita/utils/__pycache__/optimizers.cpython-310.pyc
--rw-r--r--   0        0        0     4859 2023-06-05 13:07:02.649795 asociita-0.3.3/asociita/utils/__pycache__/orchestrations.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2023-05-29 09:36:33.148103 asociita-0.3.3/asociita/utils/__pycache__/showcase.cpython-310.pyc
--rw-r--r--   0        0        0     5816 2023-06-26 13:44:42.626331 asociita-0.3.3/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     1388 2023-06-22 17:23:31.450734 asociita-0.3.3/asociita/utils/debugger.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/handlers.py
--rw-r--r--   0        0        0     1312 2023-06-23 10:58:27.961327 asociita-0.3.3/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1640 2023-07-16 13:33:46.449218 asociita-0.3.3/asociita/utils/loggers.py
--rw-r--r--   0        0        0     8064 2023-06-26 09:06:22.349796 asociita-0.3.3/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.3.3/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-07-18 13:18:39.613274 asociita-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.3.4/asociita/__init__.py
+-rw-r--r--   0        0        0     2725 2023-07-11 10:54:45.641955 asociita-0.3.4/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-07-11 10:54:39.082119 asociita-0.3.4/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0    11701 2023-07-19 16:09:53.710633 asociita-0.3.4/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4861 2023-08-08 11:55:37.396639 asociita-0.3.4/asociita/components/evaluator/__pycache__/lsaa_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0     6307 2023-06-16 21:39:14.145401 asociita-0.3.4/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    14893 2023-07-28 14:32:26.440241 asociita-0.3.4/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    18746 2023-07-19 16:00:11.885199 asociita-0.3.4/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0     5746 2023-08-08 11:55:31.196775 asociita-0.3.4/asociita/components/evaluator/lsaa_evaluator.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.3.4/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.3.4/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0    18471 2023-07-28 14:32:09.900591 asociita-0.3.4/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     3999 2023-07-19 17:10:28.054002 asociita-0.3.4/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4366 2023-07-19 17:01:13.903333 asociita-0.3.4/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     6293 2023-08-08 11:28:30.779903 asociita-0.3.4/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     5588 2023-07-28 15:03:51.684978 asociita-0.3.4/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8999 2023-07-19 16:31:39.886664 asociita-0.3.4/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8954 2023-08-08 11:28:28.427953 asociita-0.3.4/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     7479 2023-07-19 15:47:22.168254 asociita-0.3.4/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11626 2023-07-19 16:30:50.795815 asociita-0.3.4/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     5098 2023-07-12 15:13:21.310949 asociita-0.3.4/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     4759 2023-07-12 14:39:39.170606 asociita-0.3.4/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     1663 2023-07-12 14:39:39.170606 asociita-0.3.4/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc
+-rw-r--r--   0        0        0    13715 2023-07-11 12:14:58.271395 asociita-0.3.4/asociita/components/settings/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0     6901 2023-07-12 15:13:18.167030 asociita-0.3.4/asociita/components/settings/evaluator_settings.py
+-rw-r--r--   0        0        0     5835 2023-07-12 14:39:37.466652 asociita-0.3.4/asociita/components/settings/fedopt_settings.py
+-rw-r--r--   0        0        0     1931 2023-07-12 14:39:31.446817 asociita-0.3.4/asociita/components/settings/init_settings.py
+-rw-r--r--   0        0        0    23141 2023-07-11 12:14:58.051401 asociita-0.3.4/asociita/components/settings/settings.py
+-rw-r--r--   0        0        0     2465 2023-06-07 13:17:41.861780 asociita-0.3.4/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1997 2023-06-07 14:35:08.514819 asociita-0.3.4/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-06-07 14:35:08.514819 asociita-0.3.4/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     2023 2023-06-07 14:35:08.314826 asociita-0.3.4/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc
+-rw-r--r--   0        0        0     1420 2023-06-07 14:35:08.514819 asociita-0.3.4/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc
+-rw-r--r--   0        0        0     4880 2023-08-08 12:04:47.796793 asociita-0.3.4/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc
+-rw-r--r--   0        0        0     5554 2023-06-14 13:55:29.401627 asociita-0.3.4/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.3.4/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.3.4/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.3.4/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.3.4/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.3.4/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6963 2023-08-08 12:03:58.253862 asociita-0.3.4/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.3.4/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      798 2023-06-05 13:07:28.160901 asociita-0.3.4/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc
+-rw-r--r--   0        0        0      442 2023-06-16 12:12:22.850903 asociita-0.3.4/asociita/exceptions/__pycache__/modelexception.cpython-310.pyc
+-rw-r--r--   0        0        0      990 2023-06-16 09:02:36.793602 asociita-0.3.4/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.3.4/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.3.4/asociita/exceptions/modelexception.py
+-rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.3.4/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0     1139 2023-05-29 09:36:33.144103 asociita-0.3.4/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc
+-rw-r--r--   0        0        0    13786 2023-07-17 16:29:11.914865 asociita-0.3.4/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc
+-rw-r--r--   0        0        0      557 2023-06-01 15:37:30.741582 asociita-0.3.4/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     4114 2023-06-14 08:05:54.914256 asociita-0.3.4/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.3.4/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    17178 2023-07-16 13:33:46.449218 asociita-0.3.4/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.3.4/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.3.4/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6202 2023-06-26 13:45:06.401533 asociita-0.3.4/asociita/utils/__pycache__/computations.cpython-310.pyc
+-rw-r--r--   0        0        0     1162 2023-05-29 09:36:33.148103 asociita-0.3.4/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     1575 2023-06-22 17:32:18.144898 asociita-0.3.4/asociita/utils/__pycache__/debugger.cpython-310.pyc
+-rw-r--r--   0        0        0     3695 2023-05-29 09:36:33.136103 asociita-0.3.4/asociita/utils/__pycache__/handlers.cpython-310.pyc
+-rw-r--r--   0        0        0     2009 2023-06-23 10:59:17.491655 asociita-0.3.4/asociita/utils/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     1079 2023-07-17 16:29:13.102835 asociita-0.3.4/asociita/utils/__pycache__/loggers.cpython-310.pyc
+-rw-r--r--   0        0        0     4615 2023-07-19 16:09:53.710633 asociita-0.3.4/asociita/utils/__pycache__/optimizers.cpython-310.pyc
+-rw-r--r--   0        0        0     4859 2023-06-05 13:07:02.649795 asociita-0.3.4/asociita/utils/__pycache__/orchestrations.cpython-310.pyc
+-rw-r--r--   0        0        0     1308 2023-08-08 12:06:38.238407 asociita-0.3.4/asociita/utils/__pycache__/showcase.cpython-310.pyc
+-rw-r--r--   0        0        0     5816 2023-06-26 13:44:42.626331 asociita-0.3.4/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.3.4/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     1388 2023-06-22 17:23:31.450734 asociita-0.3.4/asociita/utils/debugger.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.3.4/asociita/utils/handlers.py
+-rw-r--r--   0        0        0     1312 2023-06-23 10:58:27.961327 asociita-0.3.4/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1640 2023-07-16 13:33:46.449218 asociita-0.3.4/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7422 2023-07-19 15:55:24.212302 asociita-0.3.4/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.3.4/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1050 2023-08-08 12:06:06.235099 asociita-0.3.4/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      678 2023-08-08 12:10:53.200883 asociita-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.3.4/PKG-INFO
```

### Comparing `asociita-0.3.3/LICENSE` & `asociita-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/README.md` & `asociita-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc` & `asociita-0.3.4/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/archiver/archive_manager.py` & `asociita-0.3.4/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc` & `asociita-0.3.4/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 19:25:33 2023 UTC, .py size: 18742 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ad95 b564 3649 0000  o..........d6I..
+00000000: 6f0d 0d0a 0000 0000 8b08 b864 3a49 0000  o..........d:I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6400 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `asociita-0.3.3/asociita/components/evaluator/__pycache__/lsaa_evaluator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/evaluator/__pycache__/lsaa_evaluator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 19:25:33 2023 UTC, .py size: 5561 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ad95 b564 b915 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 332d d264 7216 0000  o.......3-.dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 8302 5a0b 6401 5300  d.d...d...Z.d.S.
@@ -116,189 +116,189 @@
 00000730: 5f73 616d 706c 65da 096f 7074 696d 697a  _sample..optimiz
 00000740: 6572 da0d 7365 6172 6368 5f6c 656e 6774  er..search_lengt
 00000750: 68da 0969 7465 7261 7469 6f6e da0b 6669  h..iteration..fi
 00000760: 6e61 6c5f 6d6f 6465 6cda 0e70 7265 7669  nal_model..previ
 00000770: 6f75 735f 6d6f 6465 6cda 1172 6574 7572  ous_model..retur
 00000780: 6e5f 636f 616c 6974 696f 6e73 6309 0000  n_coalitionsc...
 00000790: 0000 0000 0000 0000 001a 0000 0007 0000  ................
-000007a0: 0043 0000 0073 3601 0000 6900 7d09 7c02  .C...s6...i.}.|.
-000007b0: 4400 5d8e 7d0a 6401 7d0b 7c0a 6a00 7d0c  D.].}.d.}.|.j.}.
+000007a0: 0043 0000 0073 3201 0000 6900 7d09 7c02  .C...s2...i.}.|.
+000007b0: 4400 5d8c 7d0a 6401 7d0b 7c0a 6a00 7d0c  D.].}.d.}.|.j.}.
 000007c0: 7401 a002 7c01 a101 7d0d 7c0d 7c0c 3d00  t...|...}.|.|.=.
-000007d0: 7401 a002 7c03 a101 7d0e 7401 a002 7c07  t...|...}.t...|.
-000007e0: a101 7d0f 7403 a004 7c0d a101 7d10 7c0e  ..}.t...|...}.|.
-000007f0: 6a05 7c0f a006 a100 7c10 6402 8d02 7d11  j.|.....|.d...}.
-00000800: 7c0f a007 7c11 a101 0100 7c0f a008 a100  |...|.....|.....
-00000810: 6403 1900 7d12 7c12 7c09 7409 7c0d a00a  d...}.|.|.t.|...
-00000820: a100 8301 3c00 7401 a002 7c0d a101 7d13  ....<.t...|...}.
-00000830: 740b 7c04 8301 4400 5d41 7d14 7401 a002  t.|...D.]A}.t...
-00000840: 7c03 a101 7d15 7401 a002 7c07 a101 7d16  |...}.t...|...}.
-00000850: 7401 a002 7c01 7c0c 1900 a101 7c13 7c14  t...|.|.....|.|.
-00000860: 9b00 6404 7c0c 9b00 9d03 3c00 7403 a004  ..d.|.....<.t...
-00000870: 7c13 a101 7d17 7c15 6a05 7c16 a006 a100  |...}.|.j.|.....
-00000880: 7c17 6402 8d02 7d18 7c16 a007 7c18 a101  |.d...}.|...|...
-00000890: 0100 7c16 a008 a100 6403 1900 7d19 7c0b  ..|.....d...}.|.
-000008a0: 7c19 7c12 1800 3700 7d0b 7c19 7c09 7409  |.|...7.}.|.|.t.
-000008b0: 7c13 a00a a100 8301 3c00 7147 7c0b 7c04  |.......<.qG|.|.
-000008c0: 1b00 7c00 6a0c 7c05 1900 7c0c 3c00 7104  ..|.j.|...|.<.q.
-000008d0: 7c08 6405 6b02 7299 7c09 5300 6406 5300  |.d.k.r.|.S.d.S.
-000008e0: 2907 6111 0400 004d 6574 686f 6420 7573  ).a....Method us
-000008f0: 6564 2074 6f20 7472 6163 6b5f 7265 7375  ed to track_resu
-00000900: 6c74 7320 6166 7465 7220 6561 6368 2074  lts after each t
-00000910: 7261 696e 696e 6720 726f 756e 642e 0a20  raining round.. 
-00000920: 2020 2020 2020 2047 6976 656e 2074 6865         Given the
-00000930: 2067 7261 6964 6e65 7473 2c20 6964 7320   graidnets, ids 
-00000940: 6f66 2074 6865 206e 6f64 6573 2069 6e63  of the nodes inc
-00000950: 6c75 6465 6420 696e 2073 616d 706c 652c  luded in sample,
-00000960: 0a20 2020 2020 2020 206c 6173 7420 7665  .        last ve
-00000970: 7273 696f 6e20 6f66 2074 6865 206f 7074  rsion of the opt
-00000980: 696d 697a 6572 2c20 7072 6576 696f 7573  imizer, previous
-00000990: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
-000009a0: 6d6f 6465 6c0a 2020 2020 2020 2020 616e  model.        an
-000009b0: 6420 7468 6520 7570 6461 7465 6420 7665  d the updated ve
-000009c0: 7273 696f 6e20 6f66 2074 6865 206d 6f64  rsion of the mod
-000009d0: 656c 2c20 6974 2063 616c 6375 6c61 7465  el, it calculate
-000009e0: 7320 7661 6c75 6573 206f 660a 2020 2020  s values of.    
-000009f0: 2020 2020 616c 6c20 7468 6520 6d61 7267      all the marg
-00000a00: 696e 616c 2063 6f6e 7472 6962 7574 696f  inal contributio
-00000a10: 6e73 2075 7369 6e67 204c 5341 412e 0a20  ns using LSAA.. 
-00000a20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000a30: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00000a40: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000a50: 2020 2020 2020 6772 6164 6965 6e74 733a        gradients:
-00000a60: 204f 7264 6572 6564 4469 6374 0a20 2020   OrderedDict.   
-00000a70: 2020 2020 2020 2020 2041 6e20 4f72 6465           An Orde
-00000a80: 7265 6444 6963 7420 636f 6e74 6169 6e69  redDict containi
-00000a90: 6e67 2067 7261 6469 656e 7473 206f 6620  ng gradients of 
-00000aa0: 7468 6520 7361 6d70 6c65 6420 6e6f 6465  the sampled node
-00000ab0: 732e 0a20 2020 2020 2020 206e 6f64 6573  s..        nodes
-00000ac0: 5f69 6e5f 7361 6d70 6c65 3a20 6c69 7374  _in_sample: list
-00000ad0: 0a20 2020 2020 2020 2020 2020 2041 206c  .            A l
-00000ae0: 6973 7420 636f 6e74 6169 6e69 6e67 2069  ist containing i
-00000af0: 6427 7320 6f66 2074 6865 206e 6f64 6573  d's of the nodes
-00000b00: 2074 6861 7420 7765 7265 2073 616d 706c   that were sampl
-00000b10: 6564 2e0a 2020 2020 2020 2020 6f70 7469  ed..        opti
-00000b20: 6d69 7a65 723a 204f 7074 696d 697a 6572  mizer: Optimizer
-00000b30: 730a 2020 2020 2020 2020 2020 2020 416e  s.            An
-00000b40: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-00000b50: 2061 736f 6369 6974 612e 4f70 7469 6d69   asociita.Optimi
-00000b60: 7a65 7273 2063 6c61 7373 2e0a 2020 2020  zers class..    
-00000b70: 2020 2020 7365 6172 6368 206c 656e 6774      search lengt
-00000b80: 683a 2069 6e74 2c0a 2020 2020 2020 2020  h: int,.        
-00000b90: 2020 2020 4120 6e75 6d62 6572 206f 6620      A number of 
-00000ba0: 7265 706c 6963 6173 2074 6861 7420 7368  replicas that sh
-00000bb0: 6f75 6c64 2062 6520 696e 636c 7564 6564  ould be included
-00000bc0: 2069 6e20 4c53 4120 7365 6172 6368 2e0a   in LSA search..
-00000bd0: 2020 2020 2020 2020 6974 6572 6174 696f          iteratio
-00000be0: 6e3a 2069 6e74 0a20 2020 2020 2020 2020  n: int.         
-00000bf0: 2020 2054 6865 2063 7572 7265 6e74 2069     The current i
-00000c00: 7465 7261 7469 6f6e 2e0a 2020 2020 2020  teration..      
-00000c10: 2020 7072 6576 696f 7573 5f6d 6f64 656c    previous_model
-00000c20: 3a20 4665 6465 7261 7465 644d 6f64 656c  : FederatedModel
-00000c30: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
-00000c40: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
-00000c50: 4665 6465 7261 7465 644d 6f64 656c 206f  FederatedModel o
-00000c60: 626a 6563 742e 0a20 2020 2020 2020 2075  bject..        u
-00000c70: 7064 6174 6564 5f6d 6f64 656c 3a20 4665  pdated_model: Fe
-00000c80: 6465 7261 7465 644d 6f64 656c 0a20 2020  deratedModel.   
-00000c90: 2020 2020 2020 2020 2041 6e20 696e 7374           An inst
-00000ca0: 616e 6365 206f 6620 7468 6520 4665 6465  ance of the Fede
-00000cb0: 7261 7465 644d 6f64 656c 206f 626a 6563  ratedModel objec
-00000cc0: 742e 0a20 2020 2020 2020 2052 6574 7572  t..        Retur
-00000cd0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00000ce0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00000cf0: 2020 2020 2020 2020 7201 0000 0029 02da          r....)..
-00000d00: 0777 6569 6768 7473 da05 6465 6c74 61e9  .weights..delta.
-00000d10: 0100 0000 5a0a 5f64 756d 6d79 5f6f 665f  ....Z._dummy_of_
-00000d20: 544e 290d da07 6e6f 6465 5f69 64da 0463  TN)...node_id..c
-00000d30: 6f70 79da 0864 6565 7063 6f70 7972 0400  opy..deepcopyr..
-00000d40: 0000 da0f 636f 6d70 7574 655f 6176 6572  ....compute_aver
-00000d50: 6167 65da 0c66 6564 5f6f 7074 696d 697a  age..fed_optimiz
-00000d60: 65da 0b67 6574 5f77 6569 6768 7473 da0e  e..get_weights..
-00000d70: 7570 6461 7465 5f77 6569 6768 7473 da0e  update_weights..
-00000d80: 7175 6963 6b5f 6576 616c 7561 7465 da05  quick_evaluate..
-00000d90: 7475 706c 65da 046b 6579 7372 1900 0000  tuple..keysr....
-00000da0: 721a 0000 0029 1a72 1b00 0000 721d 0000  r....).r....r...
-00000db0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00000dc0: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
-00000dd0: 2400 0000 da0f 7265 636f 7264 6564 5f76  $.....recorded_v
-00000de0: 616c 7565 7372 1100 0000 5a0a 6c73 6161  aluesr....Z.lsaa
-00000df0: 5f73 636f 7265 7228 0000 005a 126d 6172  _scorer(...Z.mar
-00000e00: 6769 6e61 6c5f 6772 6164 6965 6e74 735a  ginal_gradientsZ
-00000e10: 0e6d 6172 6769 6e61 6c5f 6f70 7469 6d5a  .marginal_optimZ
-00000e20: 0e6d 6172 6769 6e61 6c5f 6d6f 6465 6c5a  .marginal_modelZ
-00000e30: 116d 6172 6769 6e61 6c5f 6772 6164 5f61  .marginal_grad_a
-00000e40: 7667 5a10 6d61 7267 696e 616c 5f77 6569  vgZ.marginal_wei
-00000e50: 6768 7473 5a14 6d61 7267 696e 616c 5f6d  ghtsZ.marginal_m
-00000e60: 6f64 656c 5f73 636f 7265 5a12 6170 7065  odel_scoreZ.appe
-00000e70: 6e64 6564 5f67 7261 6469 656e 7473 da03  nded_gradients..
-00000e80: 7068 695a 0b63 6c65 616e 5f6f 7074 696d  phiZ.clean_optim
-00000e90: 5a0b 636c 6561 6e5f 6d6f 6465 6c5a 1161  Z.clean_modelZ.a
+000007d0: 7401 a002 7c0d a101 7d0e 7401 a002 7c07  t...|...}.t...|.
+000007e0: a101 7d0f 7401 a002 7c03 a101 7d10 7401  ..}.t...|...}.t.
+000007f0: a002 7c03 a101 7d11 7401 a002 7c07 a101  ..|...}.t...|...
+00000800: 7d12 7403 a004 7c0d a101 7d13 7c11 6a05  }.t...|...}.|.j.
+00000810: 7c12 a006 a100 7c13 6402 8d02 7d14 7c12  |.....|.d...}.|.
+00000820: a007 7c14 a101 0100 7c12 a008 a100 6403  ..|.....|.....d.
+00000830: 1900 7d15 7c15 7c09 7409 7c0d a00a a100  ..}.|.|.t.|.....
+00000840: 8301 3c00 740b 7c04 8301 4400 5d12 7d16  ..<.t.|...D.].}.
+00000850: 7401 a002 7c01 7c0c 1900 a101 7c0e 7c16  t...|.|.....|.|.
+00000860: 6403 1700 9b00 6404 7c0c 9b00 9d03 3c00  d.....d.|.....<.
+00000870: 7151 7403 a004 7c0e a101 7d17 7c10 6a05  qQt...|...}.|.j.
+00000880: 7c0f a006 a100 7c17 6402 8d02 7d18 7c0f  |.....|.d...}.|.
+00000890: a007 7c18 a101 0100 7c0f a008 a100 6403  ..|.....|.....d.
+000008a0: 1900 7d19 7c19 7c15 1800 7d0b 7c19 7c09  ..}.|.|...}.|.|.
+000008b0: 7409 7c0e a00a a100 8301 3c00 7c0b 7c00  t.|.......<.|.|.
+000008c0: 6a0c 7c05 1900 7c0c 3c00 7104 7c08 6405  j.|...|.<.q.|.d.
+000008d0: 6b02 7297 7c09 5300 6406 5300 2907 6111  k.r.|.S.d.S.).a.
+000008e0: 0400 004d 6574 686f 6420 7573 6564 2074  ...Method used t
+000008f0: 6f20 7472 6163 6b5f 7265 7375 6c74 7320  o track_results 
+00000900: 6166 7465 7220 6561 6368 2074 7261 696e  after each train
+00000910: 696e 6720 726f 756e 642e 0a20 2020 2020  ing round..     
+00000920: 2020 2047 6976 656e 2074 6865 2067 7261     Given the gra
+00000930: 6964 6e65 7473 2c20 6964 7320 6f66 2074  idnets, ids of t
+00000940: 6865 206e 6f64 6573 2069 6e63 6c75 6465  he nodes include
+00000950: 6420 696e 2073 616d 706c 652c 0a20 2020  d in sample,.   
+00000960: 2020 2020 206c 6173 7420 7665 7273 696f       last versio
+00000970: 6e20 6f66 2074 6865 206f 7074 696d 697a  n of the optimiz
+00000980: 6572 2c20 7072 6576 696f 7573 2076 6572  er, previous ver
+00000990: 7369 6f6e 206f 6620 7468 6520 6d6f 6465  sion of the mode
+000009a0: 6c0a 2020 2020 2020 2020 616e 6420 7468  l.        and th
+000009b0: 6520 7570 6461 7465 6420 7665 7273 696f  e updated versio
+000009c0: 6e20 6f66 2074 6865 206d 6f64 656c 2c20  n of the model, 
+000009d0: 6974 2063 616c 6375 6c61 7465 7320 7661  it calculates va
+000009e0: 6c75 6573 206f 660a 2020 2020 2020 2020  lues of.        
+000009f0: 616c 6c20 7468 6520 6d61 7267 696e 616c  all the marginal
+00000a00: 2063 6f6e 7472 6962 7574 696f 6e73 2075   contributions u
+00000a10: 7369 6e67 204c 5341 412e 0a20 2020 2020  sing LSAA..     
+00000a20: 2020 200a 2020 2020 2020 2020 5061 7261     .        Para
+00000a30: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00000a40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00000a50: 2020 6772 6164 6965 6e74 733a 204f 7264    gradients: Ord
+00000a60: 6572 6564 4469 6374 0a20 2020 2020 2020  eredDict.       
+00000a70: 2020 2020 2041 6e20 4f72 6465 7265 6444       An OrderedD
+00000a80: 6963 7420 636f 6e74 6169 6e69 6e67 2067  ict containing g
+00000a90: 7261 6469 656e 7473 206f 6620 7468 6520  radients of the 
+00000aa0: 7361 6d70 6c65 6420 6e6f 6465 732e 0a20  sampled nodes.. 
+00000ab0: 2020 2020 2020 206e 6f64 6573 5f69 6e5f         nodes_in_
+00000ac0: 7361 6d70 6c65 3a20 6c69 7374 0a20 2020  sample: list.   
+00000ad0: 2020 2020 2020 2020 2041 206c 6973 7420           A list 
+00000ae0: 636f 6e74 6169 6e69 6e67 2069 6427 7320  containing id's 
+00000af0: 6f66 2074 6865 206e 6f64 6573 2074 6861  of the nodes tha
+00000b00: 7420 7765 7265 2073 616d 706c 6564 2e0a  t were sampled..
+00000b10: 2020 2020 2020 2020 6f70 7469 6d69 7a65          optimize
+00000b20: 723a 204f 7074 696d 697a 6572 730a 2020  r: Optimizers.  
+00000b30: 2020 2020 2020 2020 2020 416e 2069 6e73            An ins
+00000b40: 7461 6e63 6520 6f66 2074 6865 2061 736f  tance of the aso
+00000b50: 6369 6974 612e 4f70 7469 6d69 7a65 7273  ciita.Optimizers
+00000b60: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
+00000b70: 7365 6172 6368 206c 656e 6774 683a 2069  search length: i
+00000b80: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00000b90: 4120 6e75 6d62 6572 206f 6620 7265 706c  A number of repl
+00000ba0: 6963 6173 2074 6861 7420 7368 6f75 6c64  icas that should
+00000bb0: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
+00000bc0: 4c53 4120 7365 6172 6368 2e0a 2020 2020  LSA search..    
+00000bd0: 2020 2020 6974 6572 6174 696f 6e3a 2069      iteration: i
+00000be0: 6e74 0a20 2020 2020 2020 2020 2020 2054  nt.            T
+00000bf0: 6865 2063 7572 7265 6e74 2069 7465 7261  he current itera
+00000c00: 7469 6f6e 2e0a 2020 2020 2020 2020 7072  tion..        pr
+00000c10: 6576 696f 7573 5f6d 6f64 656c 3a20 4665  evious_model: Fe
+00000c20: 6465 7261 7465 644d 6f64 656c 0a20 2020  deratedModel.   
+00000c30: 2020 2020 2020 2020 2041 6e20 696e 7374           An inst
+00000c40: 616e 6365 206f 6620 7468 6520 4665 6465  ance of the Fede
+00000c50: 7261 7465 644d 6f64 656c 206f 626a 6563  ratedModel objec
+00000c60: 742e 0a20 2020 2020 2020 2075 7064 6174  t..        updat
+00000c70: 6564 5f6d 6f64 656c 3a20 4665 6465 7261  ed_model: Federa
+00000c80: 7465 644d 6f64 656c 0a20 2020 2020 2020  tedModel.       
+00000c90: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
+00000ca0: 206f 6620 7468 6520 4665 6465 7261 7465   of the Federate
+00000cb0: 644d 6f64 656c 206f 626a 6563 742e 0a20  dModel object.. 
+00000cc0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00000cd0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00000ce0: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+00000cf0: 2020 2020 7201 0000 0029 02da 0777 6569      r....)...wei
+00000d00: 6768 7473 da05 6465 6c74 61e9 0100 0000  ghts..delta.....
+00000d10: 5a04 5f6f 665f 544e 290d da07 6e6f 6465  Z._of_TN)...node
+00000d20: 5f69 64da 0463 6f70 79da 0864 6565 7063  _id..copy..deepc
+00000d30: 6f70 7972 0400 0000 da0f 636f 6d70 7574  opyr......comput
+00000d40: 655f 6176 6572 6167 65da 0c66 6564 5f6f  e_average..fed_o
+00000d50: 7074 696d 697a 65da 0b67 6574 5f77 6569  ptimize..get_wei
+00000d60: 6768 7473 da0e 7570 6461 7465 5f77 6569  ghts..update_wei
+00000d70: 6768 7473 da0e 7175 6963 6b5f 6576 616c  ghts..quick_eval
+00000d80: 7561 7465 da05 7475 706c 65da 046b 6579  uate..tuple..key
+00000d90: 7372 1900 0000 721a 0000 0029 1a72 1b00  sr....r....).r..
+00000da0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000db0: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000dc0: 7223 0000 0072 2400 0000 da0f 7265 636f  r#...r$.....reco
+00000dd0: 7264 6564 5f76 616c 7565 7372 1100 0000  rded_valuesr....
+00000de0: 5a0a 6c73 6161 5f73 636f 7265 7228 0000  Z.lsaa_scorer(..
+00000df0: 005a 126d 6172 6769 6e61 6c5f 6772 6164  .Z.marginal_grad
+00000e00: 6965 6e74 735a 1261 7070 656e 6465 645f  ientsZ.appended_
+00000e10: 6772 6164 6965 6e74 735a 0e61 7070 656e  gradientsZ.appen
+00000e20: 6465 645f 6d6f 6465 6c5a 1261 7070 656e  ded_modelZ.appen
+00000e30: 6465 645f 6f70 7469 6d69 7a65 725a 0e6d  ded_optimizerZ.m
+00000e40: 6172 6769 6e61 6c5f 6f70 7469 6d5a 0e6d  arginal_optimZ.m
+00000e50: 6172 6769 6e61 6c5f 6d6f 6465 6c5a 116d  arginal_modelZ.m
+00000e60: 6172 6769 6e61 6c5f 6772 6164 5f61 7667  arginal_grad_avg
+00000e70: 5a10 6d61 7267 696e 616c 5f77 6569 6768  Z.marginal_weigh
+00000e80: 7473 5a14 6d61 7267 696e 616c 5f6d 6f64  tsZ.marginal_mod
+00000e90: 656c 5f73 636f 7265 da03 7068 695a 1161  el_score..phiZ.a
 00000ea0: 7070 656e 6465 645f 6772 6164 5f61 7667  ppended_grad_avg
-00000eb0: 5a10 6170 7065 6e64 6564 5f77 6965 6768  Z.appended_wiegh
-00000ec0: 7473 5a11 636c 6561 6e5f 6d6f 6465 6c5f  tsZ.clean_model_
-00000ed0: 7363 6f72 6572 1200 0000 7212 0000 0072  scorer....r....r
-00000ee0: 1300 0000 da0b 7570 6461 7465 5f6c 7361  ......update_lsa
-00000ef0: 6125 0000 0073 4000 0000 0424 0802 0401  a%...s@....$....
-00000f00: 0601 0a02 0601 0a02 0a03 0a01 0a01 0201  ................
-00000f10: 06ff 0a02 0c01 1002 0a02 0c01 0a01 0a01  ................
-00000f20: 1c02 0a01 0a01 0201 06ff 0a02 0c02 0c01  ................
-00000f30: 1202 1402 0802 0401 04ff 7a10 4c53 4141  ..........z.LSAA
-00000f40: 2e75 7064 6174 655f 6c73 6161 6301 0000  .update_lsaac...
-00000f50: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00000f60: 0043 0000 0073 4600 0000 7c00 6a00 a001  .C...sF...|.j...
-00000f70: a100 4400 5d17 7d01 7c01 a002 a100 4400  ..D.].}.|.....D.
-00000f80: 5d10 5c02 7d02 7d03 7c00 6a03 7c02 0500  ].\.}.}.|.j.|...
-00000f90: 1900 7404 a005 7c03 a101 3700 0300 3c00  ..t...|...7...<.
-00000fa0: 710b 7105 7c00 6a00 7c00 6a03 6602 5300  q.q.|.j.|.j.f.S.
-00000fb0: 2901 6104 0100 004d 6574 686f 6420 7573  ).a....Method us
-00000fc0: 6564 2074 6f20 7375 6d20 7570 2061 6c6c  ed to sum up all
-00000fd0: 2074 6865 2070 6172 7469 616c 204c 4f4f   the partial LOO
-00000fe0: 2073 636f 7265 7320 746f 206f 6274 6169   scores to obtai
-00000ff0: 6e0a 2020 2020 2020 2020 6120 6669 6e61  n.        a fina
-00001000: 6c20 4c4f 4f20 7363 6f72 6520 666f 7220  l LOO score for 
-00001010: 6561 6368 2063 6c69 656e 742e 0a20 2020  each client..   
-00001020: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-00001030: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00001040: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00001050: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00001060: 200a 2020 2020 2020 2020 5265 7475 726e   .        Return
-00001070: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00001080: 2d0a 2020 2020 2020 2020 7475 706c 655b  -.        tuple[
-00001090: 6469 6374 5b69 6e74 3a20 6469 6374 5d2c  dict[int: dict],
-000010a0: 2064 6963 745b 696e 743a 2066 6c6f 6174   dict[int: float
-000010b0: 5d5d 0a20 2020 2020 2020 2029 0672 1a00  ]].        ).r..
-000010c0: 0000 da06 7661 6c75 6573 da05 6974 656d  ....values..item
-000010d0: 7372 1800 0000 720d 0000 0072 0e00 0000  sr....r....r....
-000010e0: 2904 721b 0000 005a 1169 7465 7261 7469  ).r....Z.iterati
-000010f0: 6f6e 5f72 6573 756c 7473 7211 0000 00da  on_resultsr.....
-00001100: 0576 616c 7565 7212 0000 0072 1200 0000  .valuer....r....
-00001110: 7213 0000 00da 1463 616c 6375 6c61 7465  r......calculate
-00001120: 5f66 696e 616c 5f6c 7361 6174 0000 0073  _final_lsaat...s
-00001130: 0a00 0000 0e0d 1001 1a01 02ff 0c02 7a19  ..............z.
-00001140: 4c53 4141 2e63 616c 6375 6c61 7465 5f66  LSAA.calculate_f
-00001150: 696e 616c 5f6c 7361 6129 0154 2910 da08  inal_lsaa).T)...
-00001160: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00001170: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00001180: 5f5f da07 5f5f 646f 635f 5fda 046c 6973  __..__doc__..lis
-00001190: 74da 0369 6e74 721c 0000 0072 0500 0000  t..intr....r....
-000011a0: 7203 0000 0072 0200 0000 da04 626f 6f6c  r....r......bool
-000011b0: 7234 0000 0072 3000 0000 da04 6469 6374  r4...r0.....dict
-000011c0: da05 666c 6f61 7472 3800 0000 7212 0000  ..floatr8...r...
-000011d0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000011e0: 7206 0000 0009 0000 0073 3800 0000 0800  r........s8.....
-000011f0: 0401 0205 0201 02ff 0202 02fe 0202 0afe  ................
-00001200: 021e 04f8 0201 02ff 0202 02fe 0203 02fd  ................
-00001210: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
-00001220: 0208 0af8 2a4f 7206 0000 0029 0cda 056e  ....*Or....)...n
-00001230: 756d 7079 720d 0000 0072 2900 0000 da27  umpyr....r)....'
-00001240: 6173 6f63 6969 7461 2e6d 6f64 656c 732e  asociita.models.
-00001250: 7079 746f 7263 682e 6665 6465 7261 7465  pytorch.federate
-00001260: 645f 6d6f 6465 6c72 0200 0000 da19 6173  d_modelr......as
-00001270: 6f63 6969 7461 2e75 7469 6c73 2e6f 7074  ociita.utils.opt
-00001280: 696d 697a 6572 7372 0300 0000 da1b 6173  imizersr......as
-00001290: 6f63 6969 7461 2e75 7469 6c73 2e63 6f6d  ociita.utils.com
-000012a0: 7075 7461 7469 6f6e 7372 0400 0000 da0b  putationsr......
-000012b0: 636f 6c6c 6563 7469 6f6e 7372 0500 0000  collectionsr....
-000012c0: 7206 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000012d0: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-000012e0: 6c65 3e01 0000 0073 0e00 0000 0800 0801  le>....s........
-000012f0: 0c01 0c01 0c01 0c01 1203                 ..........
+00000eb0: 5a10 6170 7065 6e64 6564 5f77 6569 6768  Z.appended_weigh
+00000ec0: 7473 5a14 6170 7065 6e64 6564 5f6d 6f64  tsZ.appended_mod
+00000ed0: 656c 5f73 636f 7265 7212 0000 0072 1200  el_scorer....r..
+00000ee0: 0000 7213 0000 00da 0b75 7064 6174 655f  ..r......update_
+00000ef0: 6c73 6161 2500 0000 7340 0000 0004 2408  lsaa%...s@....$.
+00000f00: 0204 0106 010a 0206 010a 030a 010a 010a  ................
+00000f10: 030a 030a 010a 0102 0106 ff0a 020c 0110  ................
+00000f20: 020c 0222 010a 030a 0102 0106 ff0a 020c  ..."............
+00000f30: 0108 0110 0110 0208 0204 0104 ff7a 104c  .............z.L
+00000f40: 5341 412e 7570 6461 7465 5f6c 7361 6163  SAA.update_lsaac
+00000f50: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000f60: 0800 0000 4300 0000 7346 0000 007c 006a  ....C...sF...|.j
+00000f70: 00a0 01a1 0044 005d 177d 017c 01a0 02a1  .....D.].}.|....
+00000f80: 0044 005d 105c 027d 027d 037c 006a 037c  .D.].\.}.}.|.j.|
+00000f90: 0205 0019 0074 04a0 057c 03a1 0137 0003  .....t...|...7..
+00000fa0: 003c 0071 0b71 057c 006a 007c 006a 0366  .<.q.q.|.j.|.j.f
+00000fb0: 0253 0029 0161 0401 0000 4d65 7468 6f64  .S.).a....Method
+00000fc0: 2075 7365 6420 746f 2073 756d 2075 7020   used to sum up 
+00000fd0: 616c 6c20 7468 6520 7061 7274 6961 6c20  all the partial 
+00000fe0: 4c4f 4f20 7363 6f72 6573 2074 6f20 6f62  LOO scores to ob
+00000ff0: 7461 696e 0a20 2020 2020 2020 2061 2066  tain.        a f
+00001000: 696e 616c 204c 4f4f 2073 636f 7265 2066  inal LOO score f
+00001010: 6f72 2065 6163 6820 636c 6965 6e74 2e0a  or each client..
+00001020: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001030: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00001040: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00001050: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+00001060: 2020 2020 0a20 2020 2020 2020 2052 6574      .        Ret
+00001070: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00001080: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
+00001090: 6c65 5b64 6963 745b 696e 743a 2064 6963  le[dict[int: dic
+000010a0: 745d 2c20 6469 6374 5b69 6e74 3a20 666c  t], dict[int: fl
+000010b0: 6f61 745d 5d0a 2020 2020 2020 2020 2906  oat]].        ).
+000010c0: 721a 0000 00da 0676 616c 7565 73da 0569  r......values..i
+000010d0: 7465 6d73 7218 0000 0072 0d00 0000 720e  temsr....r....r.
+000010e0: 0000 0029 0472 1b00 0000 5a11 6974 6572  ...).r....Z.iter
+000010f0: 6174 696f 6e5f 7265 7375 6c74 7372 1100  ation_resultsr..
+00001100: 0000 da05 7661 6c75 6572 1200 0000 7212  ....valuer....r.
+00001110: 0000 0072 1300 0000 da14 6361 6c63 756c  ...r......calcul
+00001120: 6174 655f 6669 6e61 6c5f 6c73 6161 7600  ate_final_lsaav.
+00001130: 0000 730a 0000 000e 0d10 011a 0102 ff0c  ..s.............
+00001140: 027a 194c 5341 412e 6361 6c63 756c 6174  .z.LSAA.calculat
+00001150: 655f 6669 6e61 6c5f 6c73 6161 2901 5429  e_final_lsaa).T)
+00001160: 10da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00001170: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001180: 616d 655f 5fda 075f 5f64 6f63 5f5f da04  ame__..__doc__..
+00001190: 6c69 7374 da03 696e 7472 1c00 0000 7205  list..intr....r.
+000011a0: 0000 0072 0300 0000 7202 0000 00da 0462  ...r....r......b
+000011b0: 6f6f 6c72 3400 0000 7230 0000 00da 0464  oolr4...r0.....d
+000011c0: 6963 74da 0566 6c6f 6174 7238 0000 0072  ict..floatr8...r
+000011d0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+000011e0: 0000 0072 0600 0000 0900 0000 7338 0000  ...r........s8..
+000011f0: 0008 0004 0102 0502 0102 ff02 0202 fe02  ................
+00001200: 020a fe02 1e04 f802 0102 ff02 0202 fe02  ................
+00001210: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
+00001220: 0702 f902 080a f82a 5172 0600 0000 290c  .......*Qr....).
+00001230: da05 6e75 6d70 7972 0d00 0000 7229 0000  ..numpyr....r)..
+00001240: 00da 2761 736f 6369 6974 612e 6d6f 6465  ..'asociita.mode
+00001250: 6c73 2e70 7974 6f72 6368 2e66 6564 6572  ls.pytorch.feder
+00001260: 6174 6564 5f6d 6f64 656c 7202 0000 00da  ated_modelr.....
+00001270: 1961 736f 6369 6974 612e 7574 696c 732e  .asociita.utils.
+00001280: 6f70 7469 6d69 7a65 7273 7203 0000 00da  optimizersr.....
+00001290: 1b61 736f 6369 6974 612e 7574 696c 732e  .asociita.utils.
+000012a0: 636f 6d70 7574 6174 696f 6e73 7204 0000  computationsr...
+000012b0: 00da 0b63 6f6c 6c65 6374 696f 6e73 7205  ...collectionsr.
+000012c0: 0000 0072 0600 0000 7212 0000 0072 1200  ...r....r....r..
+000012d0: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
+000012e0: 6f64 756c 653e 0100 0000 730e 0000 0008  odule>....s.....
+000012f0: 0008 010c 010c 010c 010c 0112 03         .............
```

### Comparing `asociita-0.3.3/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 19:25:33 2023 UTC, .py size: 18471 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ad95 b564 2748 0000  o..........d'H..
+00000000: 6f0d 0d0a 0000 0000 69d1 c364 2748 0000  o.......i..d'H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6400 6406 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `asociita-0.3.3/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.3.4/asociita/components/evaluator/evaluation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         # Option to disable multiprocessing features
         if settings.get("disable_multiprocessing"):
             self.multip = False
         else:
             self.multip = True
             self.number_of_workers = settings['number_of_workers']
     
-
+    
     def preserve_previous_model(self,
                                 previous_model: FederatedModel):
         """Preserves the model from the previous round by copying 
         its structure and using it as an attribute's value. Should
         be called each training round before the proper training
         commences.
```

### Comparing `asociita-0.3.3/asociita/components/evaluator/lsaa_evaluator.py` & `asociita-0.3.4/asociita/components/evaluator/lsaa_evaluator.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,44 +74,46 @@
 
         for node in nodes_in_sample:
             lsaa_score = 0
             node_id = node.node_id
             # Deleting gradients of node i from the sample.
             marginal_gradients = copy.deepcopy(gradients)
             del marginal_gradients[node_id] 
+
+            # Creating copies for the appended version
+            appended_gradients = copy.deepcopy(marginal_gradients)
+            appended_model = copy.deepcopy(previous_model)
+            appended_optimizer = copy.deepcopy(optimizer)
+
             # Cloning the last optimizer
             marginal_optim = copy.deepcopy(optimizer)
 
             # Reconstrcuting the marginal model
             marginal_model = copy.deepcopy(previous_model)
             marginal_grad_avg = Aggregators.compute_average(marginal_gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
             marginal_weights = marginal_optim.fed_optimize(weights=marginal_model.get_weights(),
                                                         delta=marginal_grad_avg)
             marginal_model.update_weights(marginal_weights)
             marginal_model_score = marginal_model.quick_evaluate()[1]
 
             recorded_values[tuple(marginal_gradients.keys())] = marginal_model_score
-
-            appended_gradients = copy.deepcopy(marginal_gradients)
+            
             for phi in range(search_length):
-                clean_optim = copy.deepcopy(optimizer)
-                clean_model = copy.deepcopy(previous_model)
-
-                appended_gradients[f"{phi}_dummy_of_{node_id}"] = copy.deepcopy(gradients[node_id])
-                appended_grad_avg = Aggregators.compute_average(appended_gradients)
-                appended_wieghts = clean_optim.fed_optimize(weights=clean_model.get_weights(),
+                appended_gradients[(f"{phi + 1}_of_{node_id}")] = copy.deepcopy(gradients[node_id])
+                # TODO: Change f"{phi + 1}_dummy_of_{node_id}" after debugging
+            
+            appended_grad_avg = Aggregators.compute_average(appended_gradients)
+            appended_weights = appended_optimizer.fed_optimize(weights=appended_model.get_weights(),
                                                             delta = appended_grad_avg)
-                clean_model.update_weights(appended_wieghts)
-
-                clean_model_score = clean_model.quick_evaluate()[1]
-                lsaa_score += clean_model_score - marginal_model_score
-
-                recorded_values[tuple(appended_gradients.keys())] = clean_model_score
+            appended_model.update_weights(appended_weights)
+            appended_model_score = appended_model.quick_evaluate()[1]
+            lsaa_score = appended_model_score - marginal_model_score
+            recorded_values[tuple(appended_gradients.keys())] = appended_model_score
             
-            self.partial_lsaa[iteration][node_id] = lsaa_score / search_length
+            self.partial_lsaa[iteration][node_id] = lsaa_score # Previously: lsaa_score / search_length
        
         if return_coalitions == True:
                 return recorded_values
         
     
     def calculate_final_lsaa(self) -> tuple[dict[int: dict], dict[int: float]]:
         """Method used to sum up all the partial LOO scores to obtain
```

### Comparing `asociita-0.3.3/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.3.4/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/evaluator/or_evaluator.py` & `asociita-0.3.4/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/evaluator/sample_evaluator.py` & `asociita-0.3.4/asociita/components/evaluator/sample_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc` & `asociita-0.3.4/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 16 13:33:46 2023 UTC, .py size: 4366 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 baf1 b364 0e11 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 d916 b864 0e11 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6507  ..d.d.l.m.Z...e.
 00000060: a008 a100 5a08 4700 6405 6406 8400 6406  ....Z.G.d.d...d.
 00000070: 8302 5a09 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
```

### Comparing `asociita-0.3.3/asociita/components/nodes/federated_node.py` & `asociita-0.3.4/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 19:03:05 2023 UTC, .py size: 8790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6990 b564 5622 0000  o.......i..dV"..
+00000000: 6f0d 0d0a 0000 0000 dc26 d264 fa22 0000  o........&.d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6402 6c02 6d03 5a03  m.Z...d.d.l.m.Z.
 00000070: 6d04 5a04 6d05 5a05 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
@@ -136,27 +136,27 @@
 00000870: 6e65 6e74 732f 6f72 6368 6573 7472 6174  nents/orchestrat
 00000880: 6f72 2f65 7661 6c75 6174 6f72 5f6f 7263  or/evaluator_orc
 00000890: 6865 7374 7261 746f 722e 7079 7215 0000  hestrator.pyr...
 000008a0: 001d 0000 0073 0200 0000 1412 7a1f 4576  .....s......z.Ev
 000008b0: 616c 7561 746f 725f 4f72 6368 6573 7472  aluator_Orchestr
 000008c0: 6174 6f72 2e5f 5f69 6e69 745f 5fda 0a6e  ator.__init__..n
 000008d0: 6f64 6573 5f64 6174 6163 0200 0000 0000  odes_datac......
-000008e0: 0000 0000 0000 1900 0000 0a00 0000 0300  ................
-000008f0: 0000 7374 0200 007c 006a 006a 017d 027c  ..st...|.j.j.}.|
+000008e0: 0000 0000 0000 1a00 0000 0a00 0000 0300  ................
+000008f0: 0000 737e 0200 007c 006a 006a 017d 027c  ..s~...|.j.j.}.|
 00000900: 006a 006a 027d 037c 006a 006a 037d 0464  .j.j.}.|.j.j.}.d
 00000910: 0164 0284 0074 047c 0383 0144 0083 017d  .d...t.|...D...}
 00000920: 057c 006a 006a 057d 067c 006a 006a 0664  .|.j.j.}.|.j.j.d
 00000930: 036b 0272 2874 077c 006a 006a 087c 006a  .k.r(t.|.j.j.|.j
 00000940: 0964 048d 027d 077c 006a 006a 0a7d 0874  .d...}.|.j.j.}.t
 00000950: 0b7c 006a 0ca0 0da1 007c 0864 058d 027d  .|.j.....|.d...}
 00000960: 0974 0e7c 006a 006a 0f7c 006a 0c7c 057c  .t.|.j.j.|.j.|.|
 00000970: 0264 068d 047d 0a74 107c 057c 006a 006a  .d...}.t.|.|.j.j
 00000980: 1183 027d 0b7c 006a 127c 037c 006a 1364  ...}.|.j.|.|.j.d
 00000990: 078d 027d 0c7c 006a 147c 0b7c 0c7c 0164  ...}.|.j.|.|.|.d
-000009a0: 088d 037d 0b74 047c 0283 0144 005d cf7d  ...}.t.|...D.].}
+000009a0: 088d 037d 0b74 047c 0283 0144 005d d47d  ...}.t.|...D.].}
 000009b0: 0d7c 006a 09a0 1564 097c 0d9b 009d 02a1  .|.j...d.|......
 000009c0: 0101 0069 007d 0e7c 0a6a 167c 006a 0c64  ...i.}.|.j.|.j.d
 000009d0: 0a8d 0101 007c 0a6a 177c 0964 0b8d 0101  .....|.j.|.d....
 000009e0: 0074 187c 0b7c 067c 006a 0964 0c8d 037d  .t.|.|.|.j.d...}
 000009f0: 0f7c 006a 1972 bb74 1a6a 1b7c 0f7c 006a  .|.j.r.t.j.|.|.j
 00000a00: 1c64 0d8d 0244 005d 317d 1074 1d7c 0683  .d...D.]1}.t.|..
 00000a10: 018f 2389 0087 0066 0164 0e64 0284 087c  ..#....f.d.d...|
@@ -166,227 +166,229 @@
 00000a50: 0004 0083 0301 006e 0831 0073 b477 0101  .......n.1.s.w..
 00000a60: 0001 0001 0059 0001 0071 886e 2f74 1d7c  .....Y...q.n/t.|
 00000a70: 0683 018f 2389 0087 0066 0164 1064 0284  ....#....f.d.d..
 00000a80: 087c 0f44 0083 017d 117c 1144 005d 0f7d  .|.D...}.|.D.].}
 00000a90: 127c 12a0 1ea1 005c 027d 137d 1574 1fa0  .|.....\.}.}.t..
 00000aa0: 207c 15a1 017c 0e7c 133c 0071 cb57 0064   |...|.|.<.q.W.d
 00000ab0: 0f04 0004 0083 0301 006e 0831 0073 e577  .........n.1.s.w
-00000ac0: 0101 0001 0001 0059 0001 0074 21a0 227c  .......Y...t!."|
-00000ad0: 0ea1 017d 167c 096a 237c 006a 0ca0 0da1  ...}.|.j#|.j....
-00000ae0: 007c 1664 118d 027d 177c 0a6a 247c 006a  .|.d...}.|.j$|.j
-00000af0: 0c64 128d 0101 007c 0a6a 257c 0e7c 0f7c  .d.....|.j%|.|.|
-00000b00: 0d64 138d 0301 007c 006a 0ca0 267c 17a1  .d.....|.j..&|..
-00000b10: 0101 007c 0b44 005d 097d 187c 186a 27a0  ...|.D.].}.|.j'.
-00000b20: 267c 17a1 0101 0090 0171 107c 006a 006a  &|.......q.|.j.j
-00000b30: 0664 036b 0290 0172 2a7c 076a 287c 0d7c  .d.k...r*|.j(|.|
-00000b40: 006a 0c7c 0b64 148d 0301 0071 5b7c 0a6a  .j.|.d.....q[|.j
-00000b50: 297c 076a 2a64 158d 017d 117c 006a 09a0  )|.j*d...}.|.j..
-00000b60: 2b64 16a1 0101 0064 1753 0029 1861 b603  +d.....d.S.).a..
-00000b70: 0000 2250 6572 666f 726d 7320 6120 6675  .."Performs a fu
-00000b80: 6c6c 2066 6564 6572 6174 6564 2074 7261  ll federated tra
-00000b90: 696e 696e 6720 6163 636f 7264 696e 6720  ining according 
-00000ba0: 746f 2074 6865 2069 6e69 7469 616c 697a  to the initializ
-00000bb0: 6564 0a20 2020 2020 2020 2073 6574 7469  ed.        setti
-00000bc0: 6e67 732e 2054 6865 2074 7261 696e 5f70  ngs. The train_p
-00000bd0: 726f 746f 636f 6c20 6f66 2074 6865 206f  rotocol of the o
-00000be0: 7263 6865 7374 7261 746f 722e 6576 616c  rchestrator.eval
-00000bf0: 7561 746f 725f 6f72 6368 6573 7472 6174  uator_orchestrat
-00000c00: 6f72 0a20 2020 2020 2020 2066 6f6c 6c6f  or.        follo
-00000c10: 7773 2061 2070 6f70 756c 6172 2046 6564  ws a popular Fed
-00000c20: 4176 6720 6765 6e65 7261 6c69 7361 7469  Avg generalisati
-00000c30: 6f6e 2c20 4665 644f 7074 2e20 496e 7374  on, FedOpt. Inst
-00000c40: 6561 6420 6f66 2077 6569 6768 7473 2066  ead of weights f
-00000c50: 726f 6d20 6561 6368 0a20 2020 2020 2020  rom each.       
-00000c60: 2063 6c69 656e 7473 2c20 6974 2061 6767   clients, it agg
-00000c70: 7265 6761 7465 7320 6772 6164 6965 6e74  regates gradient
-00000c80: 7320 2875 6e64 6572 7374 6f6f 6420 6173  s (understood as
-00000c90: 2061 2064 6966 6665 7265 6e63 6520 6265   a difference be
-00000ca0: 7477 6565 6e20 7468 6520 7765 6967 6874  tween the weight
-00000cb0: 730a 2020 2020 2020 2020 6f66 2061 206d  s.        of a m
-00000cc0: 6f64 656c 2061 6674 6572 2061 6c6c 2074  odel after all t
-00000cd0: 2065 706f 6368 7320 6f66 2074 6865 206c   epochs of the l
-00000ce0: 6f63 616c 2074 7261 696e 696e 6729 2061  ocal training) a
-00000cf0: 6e64 2061 6767 7265 6761 7465 7320 6163  nd aggregates ac
-00000d00: 636f 7264 696e 6720 746f 200a 2020 2020  cording to .    
-00000d10: 2020 2020 7072 6f76 6964 6564 2072 756c      provided rul
-00000d20: 652e 2054 6865 2065 7661 6c75 6174 696f  e. The evaluatio
-00000d30: 6e20 7072 6f63 6573 7320 6973 206d 656e  n process is men
-00000d40: 6167 6564 2062 7920 7468 6520 696e 7374  aged by the inst
-00000d50: 616e 6365 206f 6620 7468 6520 4576 616c  ance of the Eval
-00000d60: 7561 7469 6f6e 0a20 2020 2020 2020 204d  uation.        M
-00000d70: 616e 6167 6572 206f 626a 6563 742c 2077  anager object, w
-00000d80: 6869 6368 2069 7320 6361 6c6c 6564 2075  hich is called u
-00000d90: 706f 6e20 6561 6368 2069 7465 7261 7469  pon each iterati
-00000da0: 6f6e 2e0a 0a20 2020 2020 2020 2050 6172  on...        Par
-00000db0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00000dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00000dd0: 2020 206e 6f64 6573 5f64 6174 613a 206c     nodes_data: l
-00000de0: 6973 745b 6461 7461 7365 7473 2e61 7272  ist[datasets.arr
-00000df0: 6f77 5f64 6174 6173 6574 2e44 6174 6173  ow_dataset.Datas
-00000e00: 6574 2c20 6461 7461 7365 7473 2e61 7272  et, datasets.arr
-00000e10: 6f77 5f64 6174 6173 6574 2e44 6174 6173  ow_dataset.Datas
-00000e20: 6574 5d3a 200a 2020 2020 2020 2020 2020  et]: .          
-00000e30: 2020 4120 6c69 7374 2063 6f6e 7461 696e    A list contain
-00000e40: 696e 6720 7472 6169 6e20 7365 7420 616e  ing train set an
-00000e50: 6420 7465 7374 2073 6574 2077 7261 7070  d test set wrapp
-00000e60: 6564 200a 2020 2020 2020 2020 2020 2020  ed .            
-00000e70: 696e 2061 2068 7567 6769 6e67 2066 6163  in a hugging fac
-00000e80: 6520 6172 726f 775f 6461 7461 7365 742e  e arrow_dataset.
-00000e90: 4461 7461 7365 7420 636f 6e74 6169 6e65  Dataset containe
-00000ea0: 7273 0a20 2020 2020 2020 200a 2020 2020  rs.        .    
-00000eb0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00000ec0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00000ed0: 2020 2020 696e 740a 2020 2020 2020 2020      int.        
-00000ee0: 2020 2020 5265 7475 726e 7320 3020 6f6e      Returns 0 on
-00000ef0: 2074 6865 2073 7563 6365 7373 6675 6c20   the successful 
-00000f00: 636f 6d70 6c65 7469 6f6e 206f 6620 7468  completion of th
-00000f10: 6520 7472 6169 6e69 6e67 2e0a 2020 2020  e training..    
-00000f20: 2020 2020 2020 2020 6301 0000 0000 0000          c.......
-00000f30: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00000f40: 0073 1000 0000 6700 7c00 5d04 7d01 7c01  .s....g.|.].}.|.
-00000f50: 9102 7102 5300 7219 0000 0072 1900 0000  ..q.S.r....r....
-00000f60: a902 da02 2e30 da04 6e6f 6465 7219 0000  .....0..noder...
-00000f70: 0072 1900 0000 721a 0000 00da 0a3c 6c69  .r....r......<li
-00000f80: 7374 636f 6d70 3e4d 0000 0073 0200 0000  stcomp>M...s....
-00000f90: 1000 7a39 4576 616c 7561 746f 725f 4f72  ..z9Evaluator_Or
-00000fa0: 6368 6573 7472 6174 6f72 2e74 7261 696e  chestrator.train
-00000fb0: 5f70 726f 746f 636f 6c2e 3c6c 6f63 616c  _protocol.<local
-00000fc0: 733e 2e3c 6c69 7374 636f 6d70 3e54 2902  s>.<listcomp>T).
-00000fd0: da0f 6172 6368 6976 655f 6d61 6e61 6765  ..archive_manage
-00000fe0: 725a 066c 6f67 6765 7229 02da 0777 6569  rZ.logger)...wei
-00000ff0: 6768 7473 7211 0000 0029 0472 1100 0000  ghtsr....).r....
-00001000: da05 6d6f 6465 6cda 056e 6f64 6573 da0a  ..model..nodes..
-00001010: 6974 6572 6174 696f 6e73 2902 da0c 6e6f  iterations)...no
-00001020: 6465 735f 6e75 6d62 6572 7222 0000 0029  des_numberr"...)
-00001030: 035a 0a6e 6f64 6573 5f6c 6973 74da 0a6d  .Z.nodes_list..m
-00001040: 6f64 656c 5f6c 6973 745a 0964 6174 615f  odel_listZ.data_
-00001050: 6c69 7374 7a0a 4974 6572 6174 696f 6e20  listz.Iteration 
-00001060: 2901 5a0e 7072 6576 696f 7573 5f6d 6f64  ).Z.previous_mod
-00001070: 656c 2901 5a12 7072 6576 696f 7573 5f6f  el).Z.previous_o
-00001080: 7074 696d 697a 6572 2902 da0b 7361 6d70  ptimizer)...samp
-00001090: 6c65 5f73 697a 65da 136f 7263 6865 7374  le_size..orchest
-000010a0: 7261 746f 725f 6c6f 6767 6572 2901 da04  rator_logger)...
-000010b0: 7369 7a65 6301 0000 0000 0000 0000 0000  sizec...........
-000010c0: 0002 0000 0007 0000 0013 0000 00f3 1c00  ................
-000010d0: 0000 6700 7c00 5d0a 7d01 8800 a000 7401  ..g.|.].}.....t.
-000010e0: 7c01 6400 6602 a102 9102 7102 5300 a901  |.d.f.....q.S...
-000010f0: da09 6772 6164 6965 6e74 73a9 025a 0b61  ..gradients..Z.a
-00001100: 7070 6c79 5f61 7379 6e63 7205 0000 0072  pply_asyncr....r
-00001110: 1c00 0000 a901 5a04 706f 6f6c 7219 0000  ......Z.poolr...
-00001120: 0072 1a00 0000 721f 0000 0079 0000 00f3  .r....r....y....
-00001130: 0200 0000 1c00 4e63 0100 0000 0000 0000  ......Nc........
-00001140: 0000 0000 0200 0000 0700 0000 1300 0000  ................
-00001150: 722a 0000 0072 2b00 0000 722d 0000 0072  r*...r+...r-...r
-00001160: 1c00 0000 722e 0000 0072 1900 0000 721a  ....r....r....r.
-00001170: 0000 0072 1f00 0000 8000 0000 722f 0000  ...r........r/..
-00001180: 0029 0272 2100 0000 5a05 6465 6c74 6129  .).r!...Z.delta)
-00001190: 015a 0d75 7064 6174 6564 5f6d 6f64 656c  .Z.updated_model
-000011a0: 2903 722c 0000 005a 0f6e 6f64 6573 5f69  ).r,...Z.nodes_i
-000011b0: 6e5f 7361 6d70 6c65 da09 6974 6572 6174  n_sample..iterat
-000011c0: 696f 6e29 0372 3000 0000 da0d 6365 6e74  ion).r0.....cent
-000011d0: 7261 6c5f 6d6f 6465 6c72 2300 0000 2901  ral_modelr#...).
-000011e0: da04 7061 7468 7a11 5472 6169 6e69 6e67  ..pathz.Training
-000011f0: 2063 6f6d 706c 6574 6572 0100 0000 292c   completer....),
-00001200: 7211 0000 0072 2400 0000 da0f 6e75 6d62  r....r$.....numb
-00001210: 6572 5f6f 665f 6e6f 6465 73da 106c 6f63  er_of_nodes..loc
-00001220: 616c 5f77 6172 6d5f 7374 6172 74da 0572  al_warm_start..r
-00001230: 616e 6765 7227 0000 00da 0f65 6e61 626c  anger'.....enabl
-00001240: 655f 6172 6368 6976 6572 720a 0000 005a  e_archiverr....Z
-00001250: 1161 7263 6869 7665 725f 7365 7474 696e  .archiver_settin
-00001260: 6773 7228 0000 00da 126f 7074 696d 697a  gsr(.....optimiz
-00001270: 6572 5f73 6574 7469 6e67 7372 0800 0000  er_settingsr....
-00001280: 7231 0000 005a 0b67 6574 5f77 6569 6768  r1...Z.get_weigh
-00001290: 7473 7209 0000 005a 1265 7661 6c75 6174  tsr....Z.evaluat
-000012a0: 6f72 5f73 6574 7469 6e67 7372 0300 0000  or_settingsr....
-000012b0: 5a0e 6e6f 6465 735f 7365 7474 696e 6773  Z.nodes_settings
-000012c0: 5a14 6d6f 6465 6c5f 696e 6974 6961 6c69  Z.model_initiali
-000012d0: 7a61 7469 6f6e 5a0b 6365 6e74 7261 6c5f  zationZ.central_
-000012e0: 6e65 745a 146e 6f64 6573 5f69 6e69 7469  netZ.nodes_initi
-000012f0: 616c 697a 6174 696f 6eda 0469 6e66 6f5a  alization..infoZ
-00001300: 1770 7265 7365 7276 655f 7072 6576 696f  .preserve_previo
-00001310: 7573 5f6d 6f64 656c 5a1b 7072 6573 6572  us_modelZ.preser
-00001320: 7665 5f70 7265 7669 6f75 735f 6f70 7469  ve_previous_opti
-00001330: 6d69 7a65 7272 0400 0000 5a09 6261 7463  mizerr....Z.batc
-00001340: 685f 6a6f 6272 0c00 0000 5a07 6368 756e  h_jobr....Z.chun
-00001350: 6b65 72da 0562 6174 6368 720d 0000 00da  ker..batchr.....
-00001360: 0367 6574 da04 636f 7079 5a08 6465 6570  .get..copyZ.deep
-00001370: 636f 7079 7206 0000 005a 0f63 6f6d 7075  copyr....Z.compu
-00001380: 7465 5f61 7665 7261 6765 5a0c 6665 645f  te_averageZ.fed_
-00001390: 6f70 7469 6d69 7a65 5a16 7072 6573 6572  optimizeZ.preser
-000013a0: 7665 5f75 7064 6174 6564 5f6d 6f64 656c  ve_updated_model
-000013b0: 5a0d 7472 6163 6b5f 7265 7375 6c74 735a  Z.track_resultsZ
-000013c0: 0e75 7064 6174 655f 7765 6967 6874 7372  .update_weightsr
-000013d0: 2200 0000 5a18 6172 6368 6976 655f 7472  "...Z.archive_tr
-000013e0: 6169 6e69 6e67 5f72 6573 756c 7473 5a11  aining_resultsZ.
-000013f0: 6669 6e61 6c69 7a65 5f74 7261 636b 696e  finalize_trackin
-00001400: 675a 106d 6574 7269 6373 5f73 6176 6570  gZ.metrics_savep
-00001410: 6174 685a 0863 7269 7469 6361 6c29 1972  athZ.critical).r
-00001420: 1600 0000 721b 0000 0072 2400 0000 7225  ....r....r$...r%
-00001430: 0000 0072 3400 0000 7223 0000 0072 2700  ...r4...r#...r'.
-00001440: 0000 7220 0000 0072 3700 0000 5a05 4f70  ..r ...r7...Z.Op
-00001450: 7469 6d5a 1265 7661 6c75 6174 696f 6e5f  timZ.evaluation_
-00001460: 6d61 6e61 6765 725a 0b6e 6f64 6573 5f67  managerZ.nodes_g
-00001470: 7265 656e 7226 0000 0072 3000 0000 722c  reenr&...r0...r,
-00001480: 0000 005a 0d73 616d 706c 6564 5f6e 6f64  ...Z.sampled_nod
-00001490: 6573 7239 0000 005a 0772 6573 756c 7473  esr9...Z.results
-000014a0: da06 7265 7375 6c74 5a07 6e6f 6465 5f69  ..resultZ.node_i
-000014b0: 645a 0d6d 6f64 656c 5f77 6569 6768 7473  dZ.model_weights
-000014c0: 5a0f 6d6f 6465 6c5f 6772 6164 6965 6e74  Z.model_gradient
-000014d0: 735a 0867 7261 645f 6176 675a 0f75 7064  sZ.grad_avgZ.upd
-000014e0: 6174 6564 5f77 6569 6768 7473 721e 0000  ated_weightsr...
-000014f0: 0072 1900 0000 722e 0000 0072 1a00 0000  .r....r....r....
-00001500: da0e 7472 6169 6e5f 7072 6f74 6f63 6f6c  ..train_protocol
-00001510: 3200 0000 739a 0000 0008 1808 0108 0112  2...s...........
-00001520: 0108 010c 0302 0106 0104 0106 fe08 050a  ................
-00001530: 0102 0106 ff08 0404 0102 0102 0106 fd04  ................
-00001540: 0606 0104 ff06 0304 0106 ff06 0302 0102  ................
-00001550: 0106 fe0c 0412 0104 010e 020c 0104 0202  ................
-00001560: 0104 0106 fe06 0314 010a 0112 0108 020c  ................
-00001570: 0110 0102 fe1c fd02 8002 ff0a 0812 0108  ................
-00001580: 020c 0110 0102 fe1c fd0a 080c 0202 0106  ................
-00001590: ff0e 0306 0302 0102 0106 fe0c 0508 0210  ................
-000015a0: 010e 0306 0104 0102 0106 fe02 800e 060c  ................
-000015b0: 0104 017a 2545 7661 6c75 6174 6f72 5f4f  ...z%Evaluator_O
-000015c0: 7263 6865 7374 7261 746f 722e 7472 6169  rchestrator.trai
-000015d0: 6e5f 7072 6f74 6f63 6f6c 290c da08 5f5f  n_protocol)...__
-000015e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000015f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00001600: da07 5f5f 646f 635f 5f72 0b00 0000 7215  ..__doc__r....r.
-00001610: 0000 00da 046c 6973 74da 0864 6174 6173  .....list..datas
-00001620: 6574 735a 0d61 7272 6f77 5f64 6174 6173  etsZ.arrow_datas
-00001630: 6574 5a07 4461 7461 7365 7472 3d00 0000  etZ.Datasetr=...
-00001640: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00001650: 1900 0000 7219 0000 0072 1700 0000 721a  ....r....r....r.
-00001660: 0000 0072 1000 0000 1400 0000 7314 0000  ...r........s...
-00001670: 0008 0004 0116 0802 1508 0106 0104 ff02  ................
-00001680: ff02 0212 fe72 1000 0000 291b 5a35 6173  .....r....).Z5as
-00001690: 6f63 6969 7461 2e63 6f6d 706f 6e65 6e74  ociita.component
-000016a0: 732e 6f72 6368 6573 7472 6174 6f72 2e67  s.orchestrator.g
-000016b0: 656e 6572 6963 5f6f 7263 6865 7374 7261  eneric_orchestra
-000016c0: 746f 7272 0200 0000 5a1d 6173 6f63 6969  torr....Z.asocii
-000016d0: 7461 2e75 7469 6c73 2e6f 7263 6865 7374  ta.utils.orchest
-000016e0: 7261 7469 6f6e 7372 0300 0000 7204 0000  rationsr....r...
-000016f0: 0072 0500 0000 5a1b 6173 6f63 6969 7461  .r....Z.asociita
-00001700: 2e75 7469 6c73 2e63 6f6d 7075 7461 7469  .utils.computati
-00001710: 6f6e 7372 0600 0000 5a16 6173 6f63 6969  onsr....Z.asocii
-00001720: 7461 2e75 7469 6c73 2e6c 6f67 6765 7273  ta.utils.loggers
-00001730: 7207 0000 005a 1961 736f 6369 6974 612e  r....Z.asociita.
-00001740: 7574 696c 732e 6f70 7469 6d69 7a65 7273  utils.optimizers
-00001750: 7208 0000 005a 3061 736f 6369 6974 612e  r....Z0asociita.
-00001760: 636f 6d70 6f6e 656e 7473 2e65 7661 6c75  components.evalu
-00001770: 6174 6f72 2e65 7661 6c75 6174 696f 6e5f  ator.evaluation_
-00001780: 6d61 6e61 6765 7272 0900 0000 5a2c 6173  managerr....Z,as
-00001790: 6f63 6969 7461 2e63 6f6d 706f 6e65 6e74  ociita.component
-000017a0: 732e 6172 6368 6976 6572 2e61 7263 6869  s.archiver.archi
-000017b0: 7665 5f6d 616e 6167 6572 720a 0000 005a  ve_managerr....Z
-000017c0: 2561 736f 6369 6974 612e 636f 6d70 6f6e  %asociita.compon
-000017d0: 656e 7473 2e73 6574 7469 6e67 732e 7365  ents.settings.se
-000017e0: 7474 696e 6773 720b 0000 005a 1661 736f  ttingsr....Z.aso
-000017f0: 6369 6974 612e 7574 696c 732e 6865 6c70  ciita.utils.help
-00001800: 6572 7372 0c00 0000 7243 0000 0072 3b00  ersr....rC...r;.
-00001810: 0000 5a0f 6d75 6c74 6970 726f 6365 7373  ..Z.multiprocess
-00001820: 696e 6772 0d00 0000 720e 0000 0072 0f00  ingr....r....r..
-00001830: 0000 7210 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00001840: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
-00001850: 6475 6c65 3e01 0000 0073 2000 0000 0c00  dule>....s .....
-00001860: 1401 0c01 0c01 1401 0c01 0c01 0c01 0c01  ................
-00001870: 0c01 0801 0801 1001 0c03 0c01 1403       ..............
+00000ac0: 0101 0001 0001 0059 0001 0074 1fa0 207c  .......Y...t.. |
+00000ad0: 0ea1 017d 1674 21a0 227c 0ea1 017d 177c  ...}.t!."|...}.|
+00000ae0: 096a 237c 006a 0ca0 0da1 007c 1764 118d  .j#|.j.....|.d..
+00000af0: 027d 187c 006a 0ca0 247c 18a1 0101 007c  .}.|.j..$|.....|
+00000b00: 0a6a 257c 006a 0c64 128d 0101 007c 0a6a  .j%|.j.d.....|.j
+00000b10: 267c 167c 0f7c 0d64 138d 0301 007c 0b44  &|.|.|.d.....|.D
+00000b20: 005d 097d 197c 196a 27a0 247c 18a1 0101  .].}.|.j'.$|....
+00000b30: 0090 0171 157c 006a 006a 0664 036b 0290  ...q.|.j.j.d.k..
+00000b40: 0172 2f7c 076a 287c 0d7c 006a 0c7c 0b64  .r/|.j(|.|.j.|.d
+00000b50: 148d 0301 0071 5b7c 0a6a 297c 076a 2a64  .....q[|.j)|.j*d
+00000b60: 158d 017d 117c 006a 09a0 2b64 16a1 0101  ...}.|.j..+d....
+00000b70: 0064 1753 0029 1861 b603 0000 2250 6572  .d.S.).a...."Per
+00000b80: 666f 726d 7320 6120 6675 6c6c 2066 6564  forms a full fed
+00000b90: 6572 6174 6564 2074 7261 696e 696e 6720  erated training 
+00000ba0: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00000bb0: 2069 6e69 7469 616c 697a 6564 0a20 2020   initialized.   
+00000bc0: 2020 2020 2073 6574 7469 6e67 732e 2054       settings. T
+00000bd0: 6865 2074 7261 696e 5f70 726f 746f 636f  he train_protoco
+00000be0: 6c20 6f66 2074 6865 206f 7263 6865 7374  l of the orchest
+00000bf0: 7261 746f 722e 6576 616c 7561 746f 725f  rator.evaluator_
+00000c00: 6f72 6368 6573 7472 6174 6f72 0a20 2020  orchestrator.   
+00000c10: 2020 2020 2066 6f6c 6c6f 7773 2061 2070       follows a p
+00000c20: 6f70 756c 6172 2046 6564 4176 6720 6765  opular FedAvg ge
+00000c30: 6e65 7261 6c69 7361 7469 6f6e 2c20 4665  neralisation, Fe
+00000c40: 644f 7074 2e20 496e 7374 6561 6420 6f66  dOpt. Instead of
+00000c50: 2077 6569 6768 7473 2066 726f 6d20 6561   weights from ea
+00000c60: 6368 0a20 2020 2020 2020 2063 6c69 656e  ch.        clien
+00000c70: 7473 2c20 6974 2061 6767 7265 6761 7465  ts, it aggregate
+00000c80: 7320 6772 6164 6965 6e74 7320 2875 6e64  s gradients (und
+00000c90: 6572 7374 6f6f 6420 6173 2061 2064 6966  erstood as a dif
+00000ca0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
+00000cb0: 7468 6520 7765 6967 6874 730a 2020 2020  the weights.    
+00000cc0: 2020 2020 6f66 2061 206d 6f64 656c 2061      of a model a
+00000cd0: 6674 6572 2061 6c6c 2074 2065 706f 6368  fter all t epoch
+00000ce0: 7320 6f66 2074 6865 206c 6f63 616c 2074  s of the local t
+00000cf0: 7261 696e 696e 6729 2061 6e64 2061 6767  raining) and agg
+00000d00: 7265 6761 7465 7320 6163 636f 7264 696e  regates accordin
+00000d10: 6720 746f 200a 2020 2020 2020 2020 7072  g to .        pr
+00000d20: 6f76 6964 6564 2072 756c 652e 2054 6865  ovided rule. The
+00000d30: 2065 7661 6c75 6174 696f 6e20 7072 6f63   evaluation proc
+00000d40: 6573 7320 6973 206d 656e 6167 6564 2062  ess is menaged b
+00000d50: 7920 7468 6520 696e 7374 616e 6365 206f  y the instance o
+00000d60: 6620 7468 6520 4576 616c 7561 7469 6f6e  f the Evaluation
+00000d70: 0a20 2020 2020 2020 204d 616e 6167 6572  .        Manager
+00000d80: 206f 626a 6563 742c 2077 6869 6368 2069   object, which i
+00000d90: 7320 6361 6c6c 6564 2075 706f 6e20 6561  s called upon ea
+00000da0: 6368 2069 7465 7261 7469 6f6e 2e0a 0a20  ch iteration... 
+00000db0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000dc0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00000dd0: 2d2d 2d2d 0a20 2020 2020 2020 206e 6f64  ----.        nod
+00000de0: 6573 5f64 6174 613a 206c 6973 745b 6461  es_data: list[da
+00000df0: 7461 7365 7473 2e61 7272 6f77 5f64 6174  tasets.arrow_dat
+00000e00: 6173 6574 2e44 6174 6173 6574 2c20 6461  aset.Dataset, da
+00000e10: 7461 7365 7473 2e61 7272 6f77 5f64 6174  tasets.arrow_dat
+00000e20: 6173 6574 2e44 6174 6173 6574 5d3a 200a  aset.Dataset]: .
+00000e30: 2020 2020 2020 2020 2020 2020 4120 6c69              A li
+00000e40: 7374 2063 6f6e 7461 696e 696e 6720 7472  st containing tr
+00000e50: 6169 6e20 7365 7420 616e 6420 7465 7374  ain set and test
+00000e60: 2073 6574 2077 7261 7070 6564 200a 2020   set wrapped .  
+00000e70: 2020 2020 2020 2020 2020 696e 2061 2068            in a h
+00000e80: 7567 6769 6e67 2066 6163 6520 6172 726f  ugging face arro
+00000e90: 775f 6461 7461 7365 742e 4461 7461 7365  w_dataset.Datase
+00000ea0: 7420 636f 6e74 6169 6e65 7273 0a20 2020  t containers.   
+00000eb0: 2020 2020 200a 2020 2020 2020 2020 5265       .        Re
+00000ec0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00000ed0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 696e  -----.        in
+00000ee0: 740a 2020 2020 2020 2020 2020 2020 5265  t.            Re
+00000ef0: 7475 726e 7320 3020 6f6e 2074 6865 2073  turns 0 on the s
+00000f00: 7563 6365 7373 6675 6c20 636f 6d70 6c65  uccessful comple
+00000f10: 7469 6f6e 206f 6620 7468 6520 7472 6169  tion of the trai
+00000f20: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
+00000f30: 2020 6301 0000 0000 0000 0000 0000 0002    c.............
+00000f40: 0000 0003 0000 0053 0000 0073 1000 0000  .......S...s....
+00000f50: 6700 7c00 5d04 7d01 7c01 9102 7102 5300  g.|.].}.|...q.S.
+00000f60: 7219 0000 0072 1900 0000 a902 da02 2e30  r....r.........0
+00000f70: da04 6e6f 6465 7219 0000 0072 1900 0000  ..noder....r....
+00000f80: 721a 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00000f90: 3e4d 0000 0073 0200 0000 1000 7a39 4576  >M...s......z9Ev
+00000fa0: 616c 7561 746f 725f 4f72 6368 6573 7472  aluator_Orchestr
+00000fb0: 6174 6f72 2e74 7261 696e 5f70 726f 746f  ator.train_proto
+00000fc0: 636f 6c2e 3c6c 6f63 616c 733e 2e3c 6c69  col.<locals>.<li
+00000fd0: 7374 636f 6d70 3e54 2902 da0f 6172 6368  stcomp>T)...arch
+00000fe0: 6976 655f 6d61 6e61 6765 725a 066c 6f67  ive_managerZ.log
+00000ff0: 6765 7229 02da 0777 6569 6768 7473 7211  ger)...weightsr.
+00001000: 0000 0029 0472 1100 0000 da05 6d6f 6465  ...).r......mode
+00001010: 6cda 056e 6f64 6573 da0a 6974 6572 6174  l..nodes..iterat
+00001020: 696f 6e73 2902 da0c 6e6f 6465 735f 6e75  ions)...nodes_nu
+00001030: 6d62 6572 7222 0000 0029 035a 0a6e 6f64  mberr"...).Z.nod
+00001040: 6573 5f6c 6973 74da 0a6d 6f64 656c 5f6c  es_list..model_l
+00001050: 6973 745a 0964 6174 615f 6c69 7374 7a0a  istZ.data_listz.
+00001060: 4974 6572 6174 696f 6e20 2901 5a0e 7072  Iteration ).Z.pr
+00001070: 6576 696f 7573 5f6d 6f64 656c 2901 5a12  evious_model).Z.
+00001080: 7072 6576 696f 7573 5f6f 7074 696d 697a  previous_optimiz
+00001090: 6572 2902 da0b 7361 6d70 6c65 5f73 697a  er)...sample_siz
+000010a0: 65da 136f 7263 6865 7374 7261 746f 725f  e..orchestrator_
+000010b0: 6c6f 6767 6572 2901 da04 7369 7a65 6301  logger)...sizec.
+000010c0: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+000010d0: 0000 0013 0000 00f3 1c00 0000 6700 7c00  ............g.|.
+000010e0: 5d0a 7d01 8800 a000 7401 7c01 6400 6602  ].}.....t.|.d.f.
+000010f0: a102 9102 7102 5300 a901 da09 6772 6164  ....q.S.....grad
+00001100: 6965 6e74 73a9 025a 0b61 7070 6c79 5f61  ients..Z.apply_a
+00001110: 7379 6e63 7205 0000 0072 1c00 0000 a901  syncr....r......
+00001120: 5a04 706f 6f6c 7219 0000 0072 1a00 0000  Z.poolr....r....
+00001130: 721f 0000 0079 0000 00f3 0200 0000 1c00  r....y..........
+00001140: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00001150: 0000 0700 0000 1300 0000 722a 0000 0072  ..........r*...r
+00001160: 2b00 0000 722d 0000 0072 1c00 0000 722e  +...r-...r....r.
+00001170: 0000 0072 1900 0000 721a 0000 0072 1f00  ...r....r....r..
+00001180: 0000 8000 0000 722f 0000 0029 0272 2100  ......r/...).r!.
+00001190: 0000 5a05 6465 6c74 6129 015a 0d75 7064  ..Z.delta).Z.upd
+000011a0: 6174 6564 5f6d 6f64 656c 2903 722c 0000  ated_model).r,..
+000011b0: 005a 0f6e 6f64 6573 5f69 6e5f 7361 6d70  .Z.nodes_in_samp
+000011c0: 6c65 da09 6974 6572 6174 696f 6e29 0372  le..iteration).r
+000011d0: 3000 0000 da0d 6365 6e74 7261 6c5f 6d6f  0.....central_mo
+000011e0: 6465 6c72 2300 0000 2901 da04 7061 7468  delr#...)...path
+000011f0: 7a11 5472 6169 6e69 6e67 2063 6f6d 706c  z.Training compl
+00001200: 6574 6572 0100 0000 292c 7211 0000 0072  eter....),r....r
+00001210: 2400 0000 da0f 6e75 6d62 6572 5f6f 665f  $.....number_of_
+00001220: 6e6f 6465 73da 106c 6f63 616c 5f77 6172  nodes..local_war
+00001230: 6d5f 7374 6172 74da 0572 616e 6765 7227  m_start..ranger'
+00001240: 0000 00da 0f65 6e61 626c 655f 6172 6368  .....enable_arch
+00001250: 6976 6572 720a 0000 005a 1161 7263 6869  iverr....Z.archi
+00001260: 7665 725f 7365 7474 696e 6773 7228 0000  ver_settingsr(..
+00001270: 00da 126f 7074 696d 697a 6572 5f73 6574  ...optimizer_set
+00001280: 7469 6e67 7372 0800 0000 7231 0000 005a  tingsr....r1...Z
+00001290: 0b67 6574 5f77 6569 6768 7473 7209 0000  .get_weightsr...
+000012a0: 005a 1265 7661 6c75 6174 6f72 5f73 6574  .Z.evaluator_set
+000012b0: 7469 6e67 7372 0300 0000 5a0e 6e6f 6465  tingsr....Z.node
+000012c0: 735f 7365 7474 696e 6773 5a14 6d6f 6465  s_settingsZ.mode
+000012d0: 6c5f 696e 6974 6961 6c69 7a61 7469 6f6e  l_initialization
+000012e0: 5a0b 6365 6e74 7261 6c5f 6e65 745a 146e  Z.central_netZ.n
+000012f0: 6f64 6573 5f69 6e69 7469 616c 697a 6174  odes_initializat
+00001300: 696f 6eda 0469 6e66 6f5a 1770 7265 7365  ion..infoZ.prese
+00001310: 7276 655f 7072 6576 696f 7573 5f6d 6f64  rve_previous_mod
+00001320: 656c 5a1b 7072 6573 6572 7665 5f70 7265  elZ.preserve_pre
+00001330: 7669 6f75 735f 6f70 7469 6d69 7a65 7272  vious_optimizerr
+00001340: 0400 0000 5a09 6261 7463 685f 6a6f 6272  ....Z.batch_jobr
+00001350: 0c00 0000 5a07 6368 756e 6b65 72da 0562  ....Z.chunker..b
+00001360: 6174 6368 720d 0000 00da 0367 6574 da04  atchr......get..
+00001370: 636f 7079 5a08 6465 6570 636f 7079 7206  copyZ.deepcopyr.
+00001380: 0000 005a 0f63 6f6d 7075 7465 5f61 7665  ...Z.compute_ave
+00001390: 7261 6765 5a0c 6665 645f 6f70 7469 6d69  rageZ.fed_optimi
+000013a0: 7a65 5a0e 7570 6461 7465 5f77 6569 6768  zeZ.update_weigh
+000013b0: 7473 5a16 7072 6573 6572 7665 5f75 7064  tsZ.preserve_upd
+000013c0: 6174 6564 5f6d 6f64 656c 5a0d 7472 6163  ated_modelZ.trac
+000013d0: 6b5f 7265 7375 6c74 7372 2200 0000 5a18  k_resultsr"...Z.
+000013e0: 6172 6368 6976 655f 7472 6169 6e69 6e67  archive_training
+000013f0: 5f72 6573 756c 7473 5a11 6669 6e61 6c69  _resultsZ.finali
+00001400: 7a65 5f74 7261 636b 696e 675a 106d 6574  ze_trackingZ.met
+00001410: 7269 6373 5f73 6176 6570 6174 685a 0863  rics_savepathZ.c
+00001420: 7269 7469 6361 6c29 1a72 1600 0000 721b  ritical).r....r.
+00001430: 0000 0072 2400 0000 7225 0000 0072 3400  ...r$...r%...r4.
+00001440: 0000 7223 0000 0072 2700 0000 7220 0000  ..r#...r'...r ..
+00001450: 0072 3700 0000 5a05 4f70 7469 6d5a 1265  .r7...Z.OptimZ.e
+00001460: 7661 6c75 6174 696f 6e5f 6d61 6e61 6765  valuation_manage
+00001470: 725a 0b6e 6f64 6573 5f67 7265 656e 7226  rZ.nodes_greenr&
+00001480: 0000 0072 3000 0000 722c 0000 005a 0d73  ...r0...r,...Z.s
+00001490: 616d 706c 6564 5f6e 6f64 6573 7239 0000  ampled_nodesr9..
+000014a0: 005a 0772 6573 756c 7473 da06 7265 7375  .Z.results..resu
+000014b0: 6c74 5a07 6e6f 6465 5f69 645a 0d6d 6f64  ltZ.node_idZ.mod
+000014c0: 656c 5f77 6569 6768 7473 5a0f 6d6f 6465  el_weightsZ.mode
+000014d0: 6c5f 6772 6164 6965 6e74 735a 0967 7261  l_gradientsZ.gra
+000014e0: 645f 636f 7079 5a08 6772 6164 5f61 7667  d_copyZ.grad_avg
+000014f0: 5a0f 7570 6461 7465 645f 7765 6967 6874  Z.updated_weight
+00001500: 7372 1e00 0000 7219 0000 0072 2e00 0000  sr....r....r....
+00001510: 721a 0000 00da 0e74 7261 696e 5f70 726f  r......train_pro
+00001520: 746f 636f 6c32 0000 0073 9c00 0000 0818  tocol2...s......
+00001530: 0801 0801 1201 0801 0c03 0201 0601 0401  ................
+00001540: 06fe 0805 0a01 0201 06ff 0804 0401 0201  ................
+00001550: 0201 06fd 0406 0601 04ff 0603 0401 06ff  ................
+00001560: 0603 0201 0201 06fe 0c04 1201 0401 0e02  ................
+00001570: 0c01 0402 0201 0401 06fe 0603 1401 0a01  ................
+00001580: 1201 0802 0c01 1001 02fe 1cfd 0280 02ff  ................
+00001590: 0a08 1201 0802 0c01 1001 02fe 1cfd 0a07  ................
+000015a0: 0a02 0c02 0201 06ff 0c03 0e02 0602 0201  ................
+000015b0: 0201 06fe 0804 1001 0e03 0601 0401 0201  ................
+000015c0: 06fe 0280 0e06 0c01 0401 7a25 4576 616c  ..........z%Eval
+000015d0: 7561 746f 725f 4f72 6368 6573 7472 6174  uator_Orchestrat
+000015e0: 6f72 2e74 7261 696e 5f70 726f 746f 636f  or.train_protoco
+000015f0: 6c29 0cda 085f 5f6e 616d 655f 5fda 0a5f  l)...__name__.._
+00001600: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001610: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00001620: 720b 0000 0072 1500 0000 da04 6c69 7374  r....r......list
+00001630: da08 6461 7461 7365 7473 5a0d 6172 726f  ..datasetsZ.arro
+00001640: 775f 6461 7461 7365 745a 0744 6174 6173  w_datasetZ.Datas
+00001650: 6574 723d 0000 00da 0d5f 5f63 6c61 7373  etr=.....__class
+00001660: 6365 6c6c 5f5f 7219 0000 0072 1900 0000  cell__r....r....
+00001670: 7217 0000 0072 1a00 0000 7210 0000 0014  r....r....r.....
+00001680: 0000 0073 1400 0000 0800 0401 1608 0215  ...s............
+00001690: 0801 0601 04ff 02ff 0202 12fe 7210 0000  ............r...
+000016a0: 0029 1b5a 3561 736f 6369 6974 612e 636f  .).Z5asociita.co
+000016b0: 6d70 6f6e 656e 7473 2e6f 7263 6865 7374  mponents.orchest
+000016c0: 7261 746f 722e 6765 6e65 7269 635f 6f72  rator.generic_or
+000016d0: 6368 6573 7472 6174 6f72 7202 0000 005a  chestratorr....Z
+000016e0: 1d61 736f 6369 6974 612e 7574 696c 732e  .asociita.utils.
+000016f0: 6f72 6368 6573 7472 6174 696f 6e73 7203  orchestrationsr.
+00001700: 0000 0072 0400 0000 7205 0000 005a 1b61  ...r....r....Z.a
+00001710: 736f 6369 6974 612e 7574 696c 732e 636f  sociita.utils.co
+00001720: 6d70 7574 6174 696f 6e73 7206 0000 005a  mputationsr....Z
+00001730: 1661 736f 6369 6974 612e 7574 696c 732e  .asociita.utils.
+00001740: 6c6f 6767 6572 7372 0700 0000 5a19 6173  loggersr....Z.as
+00001750: 6f63 6969 7461 2e75 7469 6c73 2e6f 7074  ociita.utils.opt
+00001760: 696d 697a 6572 7372 0800 0000 5a30 6173  imizersr....Z0as
+00001770: 6f63 6969 7461 2e63 6f6d 706f 6e65 6e74  ociita.component
+00001780: 732e 6576 616c 7561 746f 722e 6576 616c  s.evaluator.eval
+00001790: 7561 7469 6f6e 5f6d 616e 6167 6572 7209  uation_managerr.
+000017a0: 0000 005a 2c61 736f 6369 6974 612e 636f  ...Z,asociita.co
+000017b0: 6d70 6f6e 656e 7473 2e61 7263 6869 7665  mponents.archive
+000017c0: 722e 6172 6368 6976 655f 6d61 6e61 6765  r.archive_manage
+000017d0: 7272 0a00 0000 5a25 6173 6f63 6969 7461  rr....Z%asociita
+000017e0: 2e63 6f6d 706f 6e65 6e74 732e 7365 7474  .components.sett
+000017f0: 696e 6773 2e73 6574 7469 6e67 7372 0b00  ings.settingsr..
+00001800: 0000 5a16 6173 6f63 6969 7461 2e75 7469  ..Z.asociita.uti
+00001810: 6c73 2e68 656c 7065 7273 720c 0000 0072  ls.helpersr....r
+00001820: 4300 0000 723b 0000 005a 0f6d 756c 7469  C...r;...Z.multi
+00001830: 7072 6f63 6573 7369 6e67 720d 0000 0072  processingr....r
+00001840: 0e00 0000 720f 0000 0072 1000 0000 7219  ....r....r....r.
+00001850: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00001860: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001870: 7320 0000 000c 0014 010c 010c 0114 010c  s ..............
+00001880: 010c 010c 010c 010c 0108 0108 0110 010c  ................
+00001890: 030c 0114 03                             .....
```

### Comparing `asociita-0.3.3/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 13 09:23:34 2023 UTC, .py size: 7373 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 96c2 af64 cd1c 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 8a05 b864 371d 0000  o..........d7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `asociita-0.3.3/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc` & `asociita-0.3.4/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 16 13:33:46 2023 UTC, .py size: 11545 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 baf1 b364 192d 0000  o..........d.-..
+00000000: 6f0d 0d0a 0000 0000 ba0f b864 6a2d 0000  o..........dj-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
@@ -462,19 +462,19 @@
 00001cd0: 697a 6563 0100 0000 0000 0000 0000 0000  izec............
 00001ce0: 0200 0000 0600 0000 1300 0000 f31a 0000  ................
 00001cf0: 0067 007c 005d 097d 0188 00a0 0074 017c  .g.|.].}.....t.|
 00001d00: 0166 01a1 0291 0271 0253 0072 1f00 0000  .f.....q.S.r....
 00001d10: a902 da0b 6170 706c 795f 6173 796e 6372  ....apply_asyncr
 00001d20: 0a00 0000 723e 0000 00a9 01da 0470 6f6f  ....r>.......poo
 00001d30: 6c72 1f00 0000 7220 0000 0072 2f00 0000  lr....r ...r/...
-00001d40: e300 0000 f302 0000 001a 004e 6301 0000  ...........Nc...
+00001d40: e200 0000 f302 0000 001a 004e 6301 0000  ...........Nc...
 00001d50: 0000 0000 0000 0000 0002 0000 0006 0000  ................
 00001d60: 0013 0000 0072 4300 0000 721f 0000 0072  .....rC...r....r
 00001d70: 4400 0000 723e 0000 0072 4600 0000 721f  D...r>...rF...r.
-00001d80: 0000 0072 2000 0000 722f 0000 00ea 0000  ...r ...r/......
+00001d80: 0000 0072 2000 0000 722f 0000 00e9 0000  ...r ...r/......
 00001d90: 0072 4800 0000 2903 da09 6974 6572 6174  .rH...)...iterat
 00001da0: 696f 6e72 2600 0000 da05 6e6f 6465 7329  ionr&.....nodes)
 00001db0: 0172 4900 0000 7a11 5472 6169 6e69 6e67  .rI...z.Training
 00001dc0: 2063 6f6d 706c 6574 6572 0100 0000 2920   completer....) 
 00001dd0: 7215 0000 00da 0a69 7465 7261 7469 6f6e  r......iteration
 00001de0: 73da 0f6e 756d 6265 725f 6f66 5f6e 6f64  s..number_of_nod
 00001df0: 6573 7229 0000 0072 3100 0000 7241 0000  esr)...r1...rA..
@@ -500,15 +500,15 @@
 00001f30: 1900 0000 7238 0000 0072 3b00 0000 da07  ....r8...r;.....
 00001f40: 6e6f 6465 5f69 64da 0d6d 6f64 656c 5f77  node_id..model_w
 00001f50: 6569 6768 7473 5a03 6176 6772 3900 0000  eightsZ.avgr9...
 00001f60: 721f 0000 0072 4600 0000 7220 0000 00da  r....rF...r ....
 00001f70: 0e74 7261 696e 5f70 726f 746f 636f 6ca8  .train_protocol.
 00001f80: 0000 0073 7600 0000 0815 0801 0801 1201  ...sv...........
 00001f90: 0801 0c03 0201 0601 0401 06fe 0405 0601  ................
-00001fa0: 04ff 0605 0401 06ff 0604 0201 0201 06fe  ................
+00001fa0: 04ff 0604 0401 06ff 0604 0201 0201 06fe  ................
 00001fb0: 0c06 1201 0401 0402 0201 0401 06fe 0603  ................
 00001fc0: 1401 0a01 1201 0802 0c01 0a01 02fe 1cfd  ................
 00001fd0: 0280 02ff 0a08 1201 0802 0c01 0a01 02fe  ................
 00001fe0: 1cfd 0a07 0802 0e01 0c02 0c03 0601 0401  ................
 00001ff0: 0201 06fe 0a03 0a01 0280 0c02 0401 7a1b  ..............z.
 00002000: 4f72 6368 6573 7472 6174 6f72 2e74 7261  Orchestrator.tra
 00002010: 696e 5f70 726f 746f 636f 6c29 0146 2914  in_protocol).F).
```

### Comparing `asociita-0.3.3/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.3.4/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
         Returns
         -------
         int
             Returns 0 on the successful completion of the training.
             """
         
         # Initializing all the attributes using an instance of the Settings object.
-        iterations = self.settings.iterations
-        nodes_number = self.settings.number_of_nodes
+        iterations = self.settings.iterations # Int, number of iterations
+        nodes_number = self.settings.number_of_nodes # Int, number of nodes
         local_warm_start = self.settings.local_warm_start
-        nodes = [node for node in range(nodes_number)]
-        sample_size = self.settings.sample_size
+        nodes = [node for node in range(nodes_number)] # List of ints, list of nodes ids
+        sample_size = self.settings.sample_size # Int, size of the sample
         
         # Initializing an instance of the Archiver class if enabled in the settings.
         if self.settings.enable_archiver == True:
             archive_manager = Archive_Manager(
                 archive_manager = self.settings.archiver_settings,
                 logger = self.orchestrator_logger)
         
@@ -127,29 +127,28 @@
                 with Pool(sample_size) as pool:
                     results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_gradients = result.get()
                         gradients[node_id] = copy.deepcopy(model_gradients)
             
+            grad_copy = copy.deepcopy(gradients) #TODO DEBUG DEBUG
             # Computing the average
             grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
             # Upadting the weights using gradients and momentum
             updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
                                                     delta=grad_avg)
+            # Updating the orchestrator
+            self.central_model.update_weights(updated_weights)
             # Evaluation step: preserving the updated central model
             evaluation_manager.preserve_updated_model(updated_model = self.central_model)
-
             # Evaluation step: calculating all the marginal contributions
-            evaluation_manager.track_results(gradients = gradients,
+            evaluation_manager.track_results(gradients = grad_copy,
                                              nodes_in_sample = sampled_nodes,
                                              iteration = iteration)
-            
-            # Updating the orchestrator
-            self.central_model.update_weights(updated_weights)
             # Updating the nodes
             for node in nodes_green:
                 node.model.update_weights(updated_weights)         
                    
             # Passing results to the archiver -> only if so enabled in the settings.
             if self.settings.enable_archiver == True:
                 archive_manager.archive_training_results(iteration = iteration,
```

### Comparing `asociita-0.3.3/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.3.4/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,19 @@
         
         Returns
         -------
         int
             Returns 0 on the successful completion of the training.
         """
         # Initializing all the attributes using an instance of the Settings object.
-        iterations = self.settings.iterations
-        nodes_number = self.settings.number_of_nodes
+        iterations = self.settings.iterations # Int, number of iteraions
+        nodes_number = self.settings.number_of_nodes # Int, number of nodes
         local_warm_start = self.settings.local_warm_start # Note: not implemented yet.
-        nodes = [node for node in range(nodes_number)]
-        sample_size = self.settings.sample_size
+        nodes = [node for node in range(nodes_number)] # list of int, individual ids
+        sample_size = self.settings.sample_size # int, size of the sample
         
         # Initializing an instance of the Archiver class if enabled in the settings.
         if self.settings.enable_archiver == True:
             archive_manager = Archive_Manager(
                 archive_manager = self.settings.archiver_settings,
                 logger = self.orchestrator_logger)
```

### Comparing `asociita-0.3.3/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.3.4/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,31 +182,30 @@
             wrapped in a hugging face arrow_dataset.Dataset containers.
         -------------
         Returns:
         Int
             Returns 0 on the successful completion of the training."""
         
         # Initializing all the attributes using an instance of the Settings object.
-        iterations = self.settings.iterations
-        nodes_number = self.settings.number_of_nodes
+        iterations = self.settings.iterations # Iterations: int
+        nodes_number = self.settings.number_of_nodes # Number of nodes: int
         local_warm_start = self.settings.local_warm_start # Note: not implemeneted yet.
-        nodes = [node for node in range(nodes_number)]
-        sample_size = self.settings.sample_size
+        nodes = [node for node in range(nodes_number)] # List containing int
+        sample_size = self.settings.sample_size # Sample size: int
         
         # Initializing an instance of the Archiver class if enabled in the settings.
         if self.settings.enable_archiver == True:
             archive_manager = Archive_Manager(
                 archive_manager = self.settings.archiver_settings,
                 logger = self.orchestrator_logger)
 
         # Creating (empty) federated nodes.
         nodes_green = create_nodes(nodes, 
                                    self.settings.nodes_settings)
 
-
         # Creating a list of models for the nodes.
         model_list = self.model_initialization(nodes_number=nodes_number,
                                                model=self.central_net) # return deep copies of nets.
         
         # Initializing nodes -> loading the data and models onto empty nodes.
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
```

### Comparing `asociita-0.3.3/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc` & `asociita-0.3.4/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc` & `asociita-0.3.4/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc` & `asociita-0.3.4/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/__pycache__/settings.cpython-310.pyc` & `asociita-0.3.4/asociita/components/settings/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/evaluator_settings.py` & `asociita-0.3.4/asociita/components/settings/evaluator_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/fedopt_settings.py` & `asociita-0.3.4/asociita/components/settings/fedopt_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/init_settings.py` & `asociita-0.3.4/asociita/components/settings/init_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/components/settings/settings.py` & `asociita-0.3.4/asociita/components/settings/settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 14:54:11 2023 UTC, .py size: 6838 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 133d 8364 b61a 0000  o........=.d....
+00000000: 6f0d 0d0a 0000 0000 2e2f d264 331b 0000  o......../.d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6401 6c08 5a08 6400  m.Z...d.d.l.Z.d.
 00000070: 6401 6c09 5a0a 6406 6407 8400 5a0b 4700  d.l.Z.d.d...Z.G.
@@ -50,254 +50,256 @@
 00000310: 5a0d 640e 5300 290f da0c 5368 6172 645f  Z.d.S.)...Shard_
 00000320: 5370 6c69 7473 7a3c 6120 636f 6d6d 6f6e  Splitsz<a common
 00000330: 2063 6c61 7373 2066 6f72 2063 7265 6174   class for creat
 00000340: 696e 6720 7661 7269 6f75 7320 7370 6c69  ing various spli
 00000350: 7473 2061 6d6f 6e67 2074 6865 2063 6c69  ts among the cli
 00000360: 656e 7473 da07 6461 7461 7365 74da 0873  ents..dataset..s
 00000370: 6574 7469 6e67 7363 0200 0000 0000 0000  ettingsc........
-00000380: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
-00000390: 73b2 0000 0067 007d 0274 007c 0164 0119  s....g.}.t.|.d..
-000003a0: 0083 0144 005d 4e7d 037c 006a 017c 0164  ...D.]N}.|.j.|.d
+00000380: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
+00000390: 73bc 0000 0067 007d 0274 007c 0164 0119  s....g.}.t.|.d..
+000003a0: 0083 0144 005d 537d 037c 006a 017c 0164  ...D.]S}.|.j.|.d
 000003b0: 0119 007c 0364 028d 027d 047c 037c 0164  ...|.d...}.|.|.d
-000003c0: 0319 00a0 02a1 0076 0072 437c 0164 0419  .......v.rC|.d..
+000003c0: 0319 00a0 02a1 0076 0072 487c 0164 0419  .......v.rH|.d..
 000003d0: 0072 2674 03a0 047c 0464 0519 00a1 017d  .r&t...|.d.....}
 000003e0: 0574 056a 067c 047c 0164 0319 007c 0319  .t.j.|.|.d...|..
-000003f0: 0064 068d 027d 047c 0164 0419 0072 4374  .d...}.|.d...rCt
+000003f0: 0064 068d 027d 047c 0164 0419 0072 4874  .d...}.|.d...rHt
 00000400: 077c 057c 0464 0519 007c 0164 0319 007c  .|.|.d...|.d...|
-00000410: 0319 0064 0719 0083 0301 007c 046a 087c  ...d.......|.j.|
-00000420: 0164 0819 0064 098d 017d 047c 02a0 097c  .d...d...}.|...|
-00000430: 0464 0a19 007c 0464 0b19 0067 02a1 0101  .d...|.d...g....
-00000440: 0071 087c 0253 0029 0c4e da06 7368 6172  .q.|.S.).N..shar
-00000450: 6473 a902 da0a 6e75 6d5f 7368 6172 6473  ds....num_shards
-00000460: da05 696e 6465 78da 0f74 7261 6e73 666f  ..index..transfo
-00000470: 726d 6174 696f 6e73 5a14 7361 7665 5f74  rmationsZ.save_t
-00000480: 7261 6e73 666f 726d 6174 696f 6e73 da05  ransformations..
-00000490: 696d 6167 6529 01da 0b70 7265 6665 7265  image)...prefere
-000004a0: 6e63 6573 da13 7472 616e 7366 6f72 6d61  nces..transforma
-000004b0: 7469 6f6e 5f74 7970 65da 0f6c 6f63 616c  tion_type..local
-000004c0: 5f74 6573 745f 7369 7a65 a901 da09 7465  _test_size....te
-000004d0: 7374 5f73 697a 65da 0574 7261 696e da04  st_size..train..
-000004e0: 7465 7374 290a 720c 0000 00da 0573 6861  test).r......sha
-000004f0: 7264 da04 6b65 7973 da04 636f 7079 da08  rd..keys..copy..
-00000500: 6465 6570 636f 7079 7203 0000 00da 0974  deepcopyr......t
-00000510: 7261 6e73 666f 726d 7205 0000 00da 1074  ransformr......t
-00000520: 7261 696e 5f74 6573 745f 7370 6c69 74da  rain_test_split.
-00000530: 0661 7070 656e 6429 0672 1700 0000 7218  .append).r....r.
-00000540: 0000 00da 0a6e 6f64 6573 5f64 6174 6172  .....nodes_datar
-00000550: 2600 0000 da0a 6167 656e 745f 6461 7461  &.....agent_data
-00000560: 5a0d 6f72 6967 696e 616c 5f69 6d67 7372  Z.original_imgsr
-00000570: 1300 0000 7213 0000 0072 1400 0000 da0b  ....r....r......
-00000580: 686f 6d6f 6765 6e65 6f75 7316 0000 0073  homogeneous....s
-00000590: 1800 0000 0403 1001 1201 1003 0801 0e01  ................
-000005a0: 1601 0801 1c01 1003 1801 0401 7a18 5368  ............z.Sh
-000005b0: 6172 645f 5370 6c69 7473 2e68 6f6d 6f67  ard_Splits.homog
-000005c0: 656e 656f 7573 6302 0000 0000 0000 0000  eneousc.........
-000005d0: 0000 000b 0000 0006 0000 0043 0000 0073  ...........C...s
-000005e0: b200 0000 6700 7d02 7c01 6401 1900 7d03  ....g.}.|.d...}.
-000005f0: 7400 7c00 8301 7c03 1b00 7d04 7401 6a02  t.|...|...}.t.j.
-00000600: a003 6402 a101 7d05 7c05 6a04 7c04 7c03  ..d...}.|.j.|.|.
-00000610: 6403 8d02 7d06 7405 7c06 7400 7c00 8301  d...}.t.|.t.|...
-00000620: 6404 8d02 7d06 7406 7c06 8301 0100 7c00  d...}.t.|.....|.
-00000630: 6a07 6402 6405 8d01 7d00 6406 7d07 7408  j.d.d...}.d.}.t.
-00000640: 7c03 8301 4400 5d25 7d08 7c07 7c06 7c08  |...D.]%}.|.|.|.
-00000650: 1900 1700 7d09 7c00 a009 7408 7c07 7c09  ....}.|...t.|.|.
-00000660: 8302 a101 7d0a 7c09 7d07 7c0a 6a0a 7c01  ....}.|.}.|.j.|.
-00000670: 6407 1900 6408 8d01 7d0a 7c02 a00b 7c0a  d...d...}.|...|.
-00000680: 6409 1900 7c0a 640a 1900 6702 a101 0100  d...|.d...g.....
-00000690: 7131 7c02 5300 290b 4eda 0661 6765 6e74  q1|.S.).N..agent
-000006a0: 73e9 2a00 0000 2902 da05 7363 616c 65da  s.*...)...scale.
-000006b0: 0473 697a 6529 0272 0e00 0000 720f 0000  .size).r....r...
-000006c0: 0029 01da 0473 6565 6472 0100 0000 7221  .)...seedr....r!
-000006d0: 0000 0072 2200 0000 7224 0000 0072 2500  ...r"...r$...r%.
-000006e0: 0000 290c da03 6c65 6e72 0a00 0000 da06  ..)...lenr......
-000006f0: 7261 6e64 6f6d da0b 6465 6661 756c 745f  random..default_
-00000700: 726e 67da 0b65 7870 6f6e 656e 7469 616c  rng..exponential
-00000710: 7215 0000 00da 0570 7269 6e74 da07 7368  r......print..sh
-00000720: 7566 666c 6572 0c00 0000 da06 7365 6c65  uffler......sele
-00000730: 6374 722b 0000 0072 2c00 0000 290b 7217  ctr+...r,...).r.
-00000740: 0000 0072 1800 0000 722d 0000 005a 0763  ...r....r-...Z.c
-00000750: 6c69 656e 7473 da04 6265 7461 da03 726e  lients..beta..rn
-00000760: 675a 0c73 6861 7264 735f 7369 7a65 735a  gZ.shards_sizesZ
-00000770: 0a6d 6f76 696e 675f 6964 78da 0561 6765  .moving_idx..age
-00000780: 6e74 5a06 6167 5f69 6478 722e 0000 0072  ntZ.ag_idxr....r
-00000790: 1300 0000 7213 0000 0072 1400 0000 da12  ....r....r......
-000007a0: 6865 7465 726f 6765 6e65 6f75 735f 7369  heterogeneous_si
-000007b0: 7a65 2a00 0000 7320 0000 0004 0308 010c  ze*...s ........
-000007c0: 010c 010e 0310 0108 010c 0204 010c 010c  ................
-000007d0: 0110 0104 0110 0118 0104 017a 1f53 6861  ...........z.Sha
-000007e0: 7264 5f53 706c 6974 732e 6865 7465 726f  rd_Splits.hetero
-000007f0: 6765 6e65 6f75 735f 7369 7a65 6302 0000  geneous_sizec...
-00000800: 0000 0000 0000 0000 000a 0000 0006 0000  ................
-00000810: 0003 0000 0073 ba01 0000 6700 7d02 7c01  .....s....g.}.|.
-00000820: 6401 1900 7d03 7c01 6402 1900 8901 6403  d...}.|.d.....d.
-00000830: 6404 8400 7400 7c03 8301 4400 8301 7d04  d...t.|...D...}.
-00000840: 7c00 a001 a100 6a02 6405 6406 6407 8d02  |.....j.d.d.d...
-00000850: 7d05 7403 7c05 6a04 a005 a100 8301 8902  }.t.|.j.........
-00000860: 7c01 a006 6408 a101 722d 7c01 6408 1900  |...d...r-|.d...
-00000870: 7d06 6e08 7407 7408 7c00 8301 7c03 1b00  }.n.t.t.|...|...
-00000880: 8301 7d06 7c04 4400 5d66 8900 8800 8801  ..}.|.D.]f......
-00000890: 7600 7298 8700 8701 8702 6603 6409 640a  v.r.......f.d.d.
-000008a0: 8408 8802 4400 8301 8904 8801 8800 1900  ....D...........
-000008b0: 6406 1900 8804 8801 8800 1900 640b 1900  d...........d...
-000008c0: 3c00 7c05 640c 1900 a009 8704 6601 640d  <.|.d.......f.d.
-000008d0: 640e 8408 a101 7c05 640f 3c00 7c05 6a0a  d.....|.d.<.|.j.
-000008e0: 7c06 640f 6410 6411 8d03 8903 8803 640c  |.d.d.d.......d.
-000008f0: 1900 a00b a100 a00c a100 7d07 7c00 6a0d  ..........}.|.j.
-00000900: 8703 6601 6412 640e 8408 6413 6414 8d02  ..f.d.d...d.d...
-00000910: 7d08 7c08 6a0e 7c01 6415 1900 6416 8d01  }.|.j.|.d...d...
-00000920: 7d09 7c02 a00f 7c09 6417 1900 7c09 6418  }.|...|.d...|.d.
-00000930: 1900 6702 a101 0100 7c05 6a02 8803 6a10  ..g.....|.j...j.
-00000940: 6413 6419 8d02 0100 7137 7c02 a00f 6700  d.d.....q7|...g.
-00000950: a101 0100 7137 7c04 4400 5d3a 8900 8800  ....q7|.D.]:....
-00000960: 8801 7601 72da 7c05 6a0a 7c06 6410 641a  ..v.r.|.j.|.d.d.
-00000970: 8d02 8903 8803 640c 1900 a00b a100 a00c  ......d.........
-00000980: a100 7d07 7c00 6a0d 8703 6601 641b 640e  ..}.|.j...f.d.d.
-00000990: 8408 6413 6414 8d02 7d08 7c08 6a0e 7c01  ..d.d...}.|.j.|.
-000009a0: 6415 1900 6416 8d01 7d09 7c09 6417 1900  d...d...}.|.d...
-000009b0: 7c09 6418 1900 6702 7c02 8800 3c00 7c05  |.d...g.|...<.|.
-000009c0: 6a02 8803 6a10 6413 6419 8d02 0100 71a0  j...j.d.d.....q.
-000009d0: 7c02 5300 291c 4e72 3000 0000 5a12 696d  |.S.).Nr0...Z.im
-000009e0: 6261 6c61 6e63 6564 5f63 6c69 656e 7473  balanced_clients
-000009f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000a00: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
-00000a10: 7c00 5d04 7d01 7c01 9102 7102 5300 7213  |.].}.|...q.S.r.
-00000a20: 0000 0072 1300 0000 2902 da02 2e30 723e  ...r....)....0r>
-00000a30: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000a40: 0000 da0a 3c6c 6973 7463 6f6d 703e 4700  ....<listcomp>G.
-00000a50: 0000 7302 0000 0010 007a 3253 6861 7264  ..s......z2Shard
-00000a60: 5f53 706c 6974 732e 646f 6d69 6e61 6e74  _Splits.dominant
-00000a70: 5f73 616d 706c 696e 672e 3c6c 6f63 616c  _sampling.<local
-00000a80: 733e 2e3c 6c69 7374 636f 6d70 3e72 1e00  s>.<listcomp>r..
-00000a90: 0000 7206 0000 0029 01da 0461 7869 735a  ..r....)...axisZ
-00000aa0: 1263 7573 746f 6d5f 7361 6d70 6c65 5f73  .custom_sample_s
-00000ab0: 697a 6563 0100 0000 0000 0000 0000 0000  izec............
-00000ac0: 0200 0000 0600 0000 1300 0000 732a 0000  ............s*..
-00000ad0: 0069 007c 005d 117d 017c 0164 0088 0188  .i.|.].}.|.d....
-00000ae0: 0019 0064 0019 0018 0074 0088 0283 0164  ...d.....t.....d
-00000af0: 0018 001b 0093 0271 0253 0029 0172 0600  .......q.S.).r..
-00000b00: 0000 2901 7235 0000 0029 0272 4000 0000  ..).r5...).r@...
-00000b10: da03 6b65 7929 0372 3e00 0000 da11 696d  ..key).r>.....im
-00000b20: 6261 6c61 6e63 6564 5f61 6765 6e74 73da  balanced_agents.
-00000b30: 066c 6162 656c 7372 1300 0000 7214 0000  .labelsr....r...
-00000b40: 00da 0a3c 6469 6374 636f 6d70 3e53 0000  ...<dictcomp>S..
-00000b50: 0073 0200 0000 2a00 7a32 5368 6172 645f  .s....*.z2Shard_
-00000b60: 5370 6c69 7473 2e64 6f6d 696e 616e 745f  Splits.dominant_
-00000b70: 7361 6d70 6c69 6e67 2e3c 6c6f 6361 6c73  sampling.<locals
-00000b80: 3e2e 3c64 6963 7463 6f6d 703e 7201 0000  >.<dictcomp>r...
-00000b90: 00da 056c 6162 656c 6301 0000 0000 0000  ...labelc.......
-00000ba0: 0000 0000 0001 0000 0002 0000 0013 0000  ................
-00000bb0: 0073 0800 0000 8800 7c00 1900 5300 a901  .s......|...S...
-00000bc0: 4e72 1300 0000 2901 da01 7829 01da 1073  Nr....)...x)...s
-00000bd0: 616d 706c 696e 675f 7765 6967 6874 7372  ampling_weightsr
-00000be0: 1300 0000 7214 0000 00da 083c 6c61 6d62  ....r......<lamb
-00000bf0: 6461 3e5b 0000 0073 0200 0000 0800 7a30  da>[...s......z0
-00000c00: 5368 6172 645f 5370 6c69 7473 2e64 6f6d  Shard_Splits.dom
-00000c10: 696e 616e 745f 7361 6d70 6c69 6e67 2e3c  inant_sampling.<
-00000c20: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00000c30: da07 7765 6967 6874 7372 3100 0000 2903  ..weightsr1...).
-00000c40: da01 6e72 4c00 0000 da0c 7261 6e64 6f6d  ..nrL.....random
-00000c50: 5f73 7461 7465 6302 0000 0000 0000 0000  _statec.........
-00000c60: 0000 0002 0000 0003 0000 0013 0000 00f3  ................
-00000c70: 0e00 0000 7c01 7400 8800 6a01 8301 7600  ....|.t...j...v.
-00000c80: 5300 7248 0000 00a9 02da 046c 6973 7472  S.rH.......listr
-00000c90: 1c00 0000 a902 da06 6669 6c74 6572 da03  ........filter..
-00000ca0: 6964 78a9 01da 0673 616d 706c 6572 1300  idx....sampler..
-00000cb0: 0000 7214 0000 0072 4b00 0000 6000 0000  ..r....rK...`...
-00000cc0: f302 0000 000e 0054 2901 da0c 7769 7468  .......T)...with
-00000cd0: 5f69 6e64 6963 6573 7221 0000 0072 2200  _indicesr!...r".
-00000ce0: 0000 7224 0000 0072 2500 0000 2901 da07  ..r$...r%...)...
-00000cf0: 696e 706c 6163 6529 0272 4d00 0000 724e  inplace).rM...rN
-00000d00: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000d10: 0200 0000 0300 0000 1300 0000 724f 0000  ............rO..
-00000d20: 0072 4800 0000 7250 0000 0072 5200 0000  .rH...rP...rR...
-00000d30: 7255 0000 0072 1300 0000 7214 0000 0072  rU...r....r....r
-00000d40: 4b00 0000 7100 0000 7257 0000 0029 1172  K...q...rW...).r
-00000d50: 0c00 0000 da09 746f 5f70 616e 6461 73da  ......to_pandas.
-00000d60: 0464 726f 70da 0673 6f72 7465 6472 4700  .drop..sortedrG.
-00000d70: 0000 da06 756e 6971 7565 da03 6765 7472  ....unique..getr
-00000d80: 0900 0000 7235 0000 00da 0561 7070 6c79  ....r5.....apply
-00000d90: 7256 0000 00da 0c76 616c 7565 5f63 6f75  rV.....value_cou
-00000da0: 6e74 73da 0a73 6f72 745f 696e 6465 7872  nts..sort_indexr
-00000db0: 5300 0000 722b 0000 0072 2c00 0000 721c  S...r+...r,...r.
-00000dc0: 0000 0029 0a72 1700 0000 7218 0000 0072  ...).r....r....r
-00000dd0: 2d00 0000 5a09 6e6f 5f61 6765 6e74 7372  -...Z.no_agentsr
-00000de0: 3000 0000 da09 7061 6e64 6173 5f64 66da  0.....pandas_df.
-00000df0: 0b73 616d 706c 655f 7369 7a65 da06 636f  .sample_size..co
-00000e00: 756e 7473 5a0c 7361 6d70 6c65 645f 6461  untsZ.sampled_da
-00000e10: 7461 722e 0000 0072 1300 0000 2905 723e  tar....r....).r>
-00000e20: 0000 0072 4400 0000 7245 0000 0072 5600  ...rD...rE...rV.
-00000e30: 0000 724a 0000 0072 1400 0000 da11 646f  ..rJ...r......do
-00000e40: 6d69 6e61 6e74 5f73 616d 706c 696e 6741  minant_samplingA
-00000e50: 0000 0073 3e00 0000 0403 0801 0801 1201  ...s>...........
-00000e60: 1201 0e01 0a01 0a01 1002 0803 0801 1602  ................
-00000e70: 1801 1a07 1001 1002 1602 1001 1601 1203  ................
-00000e80: 0c02 0804 0801 0e02 1001 1602 1001 1401  ................
-00000e90: 1002 0280 0401 7a1e 5368 6172 645f 5370  ......z.Shard_Sp
-00000ea0: 6c69 7473 2e64 6f6d 696e 616e 745f 7361  lits.dominant_sa
-00000eb0: 6d70 6c69 6e67 6302 0000 0000 0000 0000  mplingc.........
-00000ec0: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00000ed0: 5a00 0000 6700 7d02 7c00 6a00 6401 6402  Z...g.}.|.j.d.d.
-00000ee0: 6403 8d02 7d03 7c03 6a01 7c01 6404 1900  d...}.|.j.|.d...
-00000ef0: 6405 8d01 7d03 7402 7c01 6406 1900 8301  d...}.t.|.d.....
-00000f00: 4400 5d13 7d04 7c02 a003 7404 a005 7c03  D.].}.|...t...|.
-00000f10: 6407 1900 a101 7404 a005 7c03 6408 1900  d.....t...|.d...
-00000f20: a101 6702 a101 0100 7117 7c02 5300 2909  ..g.....q.|.S.).
-00000f30: 4e72 0600 0000 7201 0000 0072 1a00 0000  Nr....r....r....
-00000f40: 7221 0000 0072 2200 0000 7230 0000 0072  r!...r"...r0...r
-00000f50: 2400 0000 7225 0000 0029 0672 2600 0000  $...r%...).r&...
-00000f60: 722b 0000 0072 0c00 0000 722c 0000 0072  r+...r....r,...r
-00000f70: 2800 0000 7229 0000 0029 0572 1700 0000  (...r)...).r....
-00000f80: 7218 0000 0072 2d00 0000 722e 0000 0072  r....r-...r....r
-00000f90: 1200 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00000fa0: 0000 00da 1672 6570 6c69 6361 7465 5f73  .....replicate_s
-00000fb0: 616d 655f 6461 7461 7365 7478 0000 0073  ame_datasetx...s
-00000fc0: 0c00 0000 0403 0e01 1001 1001 2401 0402  ............$...
-00000fd0: 7a23 5368 6172 645f 5370 6c69 7473 2e72  z#Shard_Splits.r
-00000fe0: 6570 6c69 6361 7465 5f73 616d 655f 6461  eplicate_same_da
-00000ff0: 7461 7365 7463 0200 0000 0000 0000 0000  tasetc..........
-00001000: 0000 0600 0000 0900 0000 4300 0000 737c  ..........C...s|
-00001010: 0000 0067 007d 0274 007c 0164 0119 0083  ...g.}.t.|.d....
-00001020: 0144 005d 337d 037c 006a 017c 0164 0119  .D.]3}.|.j.|.d..
-00001030: 007c 0364 028d 027d 047c 046a 027c 0164  .|.d...}.|.j.|.d
-00001040: 0319 0064 048d 017d 0474 0074 037c 0164  ...d...}.t.t.|.d
-00001050: 0519 007c 0164 0119 001b 0083 0183 0144  ...|.d.........D
-00001060: 005d 137d 057c 02a0 0474 05a0 067c 0464  .].}.|...t...|.d
-00001070: 0619 00a1 0174 05a0 067c 0464 0719 00a1  .....t...|.d....
-00001080: 0167 02a1 0101 0071 2771 087c 0253 0029  .g.....q'q.|.S.)
-00001090: 084e 7219 0000 0072 1a00 0000 7221 0000  .Nr....r....r!..
-000010a0: 0072 2200 0000 7230 0000 0072 2400 0000  .r"...r0...r$...
-000010b0: 7225 0000 0029 0772 0c00 0000 7226 0000  r%...).r....r&..
-000010c0: 0072 2b00 0000 7209 0000 0072 2c00 0000  .r+...r....r,...
-000010d0: 7228 0000 0072 2900 0000 2906 7217 0000  r(...r)...).r...
-000010e0: 0072 1800 0000 722d 0000 0072 2600 0000  .r....r-...r&...
-000010f0: 722e 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001100: 1300 0000 7214 0000 00da 0f73 706c 6974  ....r......split
-00001110: 5f69 6e5f 626c 6f63 6b73 8400 0000 7310  _in_blocks....s.
-00001120: 0000 0004 0310 0112 0110 011c 0124 0102  .............$..
-00001130: ff04 027a 1c53 6861 7264 5f53 706c 6974  ...z.Shard_Split
-00001140: 732e 7370 6c69 745f 696e 5f62 6c6f 636b  s.split_in_block
-00001150: 734e 290e da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
-00001160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001170: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00001180: 5fda 0c73 7461 7469 636d 6574 686f 64da  _..staticmethod.
-00001190: 0864 6174 6173 6574 73da 0d61 7272 6f77  .datasets..arrow
-000011a0: 5f64 6174 6173 6574 da07 4461 7461 7365  _dataset..Datase
-000011b0: 74da 0464 6963 7472 2f00 0000 723f 0000  t..dictr/...r?..
-000011c0: 0072 6500 0000 7266 0000 0072 6700 0000  .re...rf...rg...
-000011d0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-000011e0: 1400 0000 7216 0000 0013 0000 0073 2c00  ....r........s,.
-000011f0: 0000 0800 0401 0202 0a01 0201 0cff 0213  ................
-00001200: 0a01 0201 0cff 0216 0a01 0201 0cff 0236  ...............6
-00001210: 0a01 0201 0cff 020b 0a01 0201 10ff 7216  ..............r.
-00001220: 0000 0029 0d72 6d00 0000 7202 0000 00da  ...).rm...r.....
-00001230: 2661 736f 6369 6974 612e 6461 7461 7365  &asociita.datase
-00001240: 7473 2e73 6861 7264 5f74 7261 6e73 666f  ts.shard_transfo
-00001250: 726d 6174 696f 6e72 0300 0000 da17 6173  rmationr......as
-00001260: 6f63 6969 7461 2e75 7469 6c73 2e68 616e  ociita.utils.han
-00001270: 646c 6572 7372 0400 0000 da17 6173 6f63  dlersr......asoc
-00001280: 6969 7461 2e75 7469 6c73 2e73 686f 7763  iita.utils.showc
-00001290: 6173 6572 0500 0000 7228 0000 00da 056e  aser....r(.....n
-000012a0: 756d 7079 720a 0000 0072 1500 0000 7216  umpyr....r....r.
-000012b0: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-000012c0: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000012d0: 3e01 0000 0073 1200 0000 0800 0c01 0c01  >....s..........
-000012e0: 0c01 0c01 0801 0801 0802 120a            ............
+00000410: 0319 0064 0719 0064 087c 039b 009d 0264  ...d...d.|.....d
+00000420: 098d 0401 007c 046a 087c 0164 0a19 0064  .....|.j.|.d...d
+00000430: 0b8d 017d 047c 02a0 097c 0464 0c19 007c  ...}.|...|.d...|
+00000440: 0464 0d19 0067 02a1 0101 0071 087c 0253  .d...g.....q.|.S
+00000450: 0029 0e4e da06 7368 6172 6473 a902 da0a  .).N..shards....
+00000460: 6e75 6d5f 7368 6172 6473 da05 696e 6465  num_shards..inde
+00000470: 78da 0f74 7261 6e73 666f 726d 6174 696f  x..transformatio
+00000480: 6e73 5a14 7361 7665 5f74 7261 6e73 666f  nsZ.save_transfo
+00000490: 726d 6174 696f 6e73 da05 696d 6167 6529  rmations..image)
+000004a0: 01da 0b70 7265 6665 7265 6e63 6573 da13  ...preferences..
+000004b0: 7472 616e 7366 6f72 6d61 7469 6f6e 5f74  transformation_t
+000004c0: 7970 655a 086f 665f 6e6f 6465 5f29 01da  ypeZ.of_node_)..
+000004d0: 046e 616d 65da 0f6c 6f63 616c 5f74 6573  .name..local_tes
+000004e0: 745f 7369 7a65 a901 da09 7465 7374 5f73  t_size....test_s
+000004f0: 697a 65da 0574 7261 696e da04 7465 7374  ize..train..test
+00000500: 290a 720c 0000 00da 0573 6861 7264 da04  ).r......shard..
+00000510: 6b65 7973 da04 636f 7079 da08 6465 6570  keys..copy..deep
+00000520: 636f 7079 7203 0000 00da 0974 7261 6e73  copyr......trans
+00000530: 666f 726d 7205 0000 00da 1074 7261 696e  formr......train
+00000540: 5f74 6573 745f 7370 6c69 74da 0661 7070  _test_split..app
+00000550: 656e 6429 0672 1700 0000 7218 0000 00da  end).r....r.....
+00000560: 0a6e 6f64 6573 5f64 6174 6172 2700 0000  .nodes_datar'...
+00000570: da0a 6167 656e 745f 6461 7461 5a0d 6f72  ..agent_dataZ.or
+00000580: 6967 696e 616c 5f69 6d67 7372 1300 0000  iginal_imgsr....
+00000590: 7213 0000 0072 1400 0000 da0b 686f 6d6f  r....r......homo
+000005a0: 6765 6e65 6f75 7316 0000 0073 2000 0000  geneous....s ...
+000005b0: 0403 1001 1201 1003 0801 0e01 1601 0801  ................
+000005c0: 0401 0601 0e01 0801 06fd 1006 1801 0401  ................
+000005d0: 7a18 5368 6172 645f 5370 6c69 7473 2e68  z.Shard_Splits.h
+000005e0: 6f6d 6f67 656e 656f 7573 6302 0000 0000  omogeneousc.....
+000005f0: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
+00000600: 0000 0073 b200 0000 6700 7d02 7c01 6401  ...s....g.}.|.d.
+00000610: 1900 7d03 7400 7c00 8301 7c03 1b00 7d04  ..}.t.|...|...}.
+00000620: 7401 6a02 a003 6402 a101 7d05 7c05 6a04  t.j...d...}.|.j.
+00000630: 7c04 7c03 6403 8d02 7d06 7405 7c06 7400  |.|.d...}.t.|.t.
+00000640: 7c00 8301 6404 8d02 7d06 7406 7c06 8301  |...d...}.t.|...
+00000650: 0100 7c00 6a07 6402 6405 8d01 7d00 6406  ..|.j.d.d...}.d.
+00000660: 7d07 7408 7c03 8301 4400 5d25 7d08 7c07  }.t.|...D.]%}.|.
+00000670: 7c06 7c08 1900 1700 7d09 7c00 a009 7408  |.|.....}.|...t.
+00000680: 7c07 7c09 8302 a101 7d0a 7c09 7d07 7c0a  |.|.....}.|.}.|.
+00000690: 6a0a 7c01 6407 1900 6408 8d01 7d0a 7c02  j.|.d...d...}.|.
+000006a0: a00b 7c0a 6409 1900 7c0a 640a 1900 6702  ..|.d...|.d...g.
+000006b0: a101 0100 7131 7c02 5300 290b 4eda 0661  ....q1|.S.).N..a
+000006c0: 6765 6e74 73e9 2a00 0000 2902 da05 7363  gents.*...)...sc
+000006d0: 616c 65da 0473 697a 6529 0272 0e00 0000  ale..size).r....
+000006e0: 720f 0000 0029 01da 0473 6565 6472 0100  r....)...seedr..
+000006f0: 0000 7222 0000 0072 2300 0000 7225 0000  ..r"...r#...r%..
+00000700: 0072 2600 0000 290c da03 6c65 6e72 0a00  .r&...)...lenr..
+00000710: 0000 da06 7261 6e64 6f6d da0b 6465 6661  ....random..defa
+00000720: 756c 745f 726e 67da 0b65 7870 6f6e 656e  ult_rng..exponen
+00000730: 7469 616c 7215 0000 00da 0570 7269 6e74  tialr......print
+00000740: da07 7368 7566 666c 6572 0c00 0000 da06  ..shuffler......
+00000750: 7365 6c65 6374 722c 0000 0072 2d00 0000  selectr,...r-...
+00000760: 290b 7217 0000 0072 1800 0000 722e 0000  ).r....r....r...
+00000770: 005a 0763 6c69 656e 7473 da04 6265 7461  .Z.clients..beta
+00000780: da03 726e 675a 0c73 6861 7264 735f 7369  ..rngZ.shards_si
+00000790: 7a65 735a 0a6d 6f76 696e 675f 6964 78da  zesZ.moving_idx.
+000007a0: 0561 6765 6e74 5a06 6167 5f69 6478 722f  .agentZ.ag_idxr/
+000007b0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+000007c0: 0000 da12 6865 7465 726f 6765 6e65 6f75  ....heterogeneou
+000007d0: 735f 7369 7a65 2d00 0000 7320 0000 0004  s_size-...s ....
+000007e0: 0308 010c 010c 010e 0310 0108 010c 0204  ................
+000007f0: 010c 010c 0110 0104 0110 0118 0104 017a  ...............z
+00000800: 1f53 6861 7264 5f53 706c 6974 732e 6865  .Shard_Splits.he
+00000810: 7465 726f 6765 6e65 6f75 735f 7369 7a65  terogeneous_size
+00000820: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
+00000830: 0006 0000 0003 0000 0073 ba01 0000 6700  .........s....g.
+00000840: 7d02 7c01 6401 1900 7d03 7c01 6402 1900  }.|.d...}.|.d...
+00000850: 8901 6403 6404 8400 7400 7c03 8301 4400  ..d.d...t.|...D.
+00000860: 8301 7d04 7c00 a001 a100 6a02 6405 6406  ..}.|.....j.d.d.
+00000870: 6407 8d02 7d05 7403 7c05 6a04 a005 a100  d...}.t.|.j.....
+00000880: 8301 8902 7c01 a006 6408 a101 722d 7c01  ....|...d...r-|.
+00000890: 6408 1900 7d06 6e08 7407 7408 7c00 8301  d...}.n.t.t.|...
+000008a0: 7c03 1b00 8301 7d06 7c04 4400 5d66 8900  |.....}.|.D.]f..
+000008b0: 8800 8801 7600 7298 8700 8701 8702 6603  ....v.r.......f.
+000008c0: 6409 640a 8408 8802 4400 8301 8904 8801  d.d.....D.......
+000008d0: 8800 1900 6406 1900 8804 8801 8800 1900  ....d...........
+000008e0: 640b 1900 3c00 7c05 640c 1900 a009 8704  d...<.|.d.......
+000008f0: 6601 640d 640e 8408 a101 7c05 640f 3c00  f.d.d.....|.d.<.
+00000900: 7c05 6a0a 7c06 640f 6410 6411 8d03 8903  |.j.|.d.d.d.....
+00000910: 8803 640c 1900 a00b a100 a00c a100 7d07  ..d...........}.
+00000920: 7c00 6a0d 8703 6601 6412 640e 8408 6413  |.j...f.d.d...d.
+00000930: 6414 8d02 7d08 7c08 6a0e 7c01 6415 1900  d...}.|.j.|.d...
+00000940: 6416 8d01 7d09 7c02 a00f 7c09 6417 1900  d...}.|...|.d...
+00000950: 7c09 6418 1900 6702 a101 0100 7c05 6a02  |.d...g.....|.j.
+00000960: 8803 6a10 6413 6419 8d02 0100 7137 7c02  ..j.d.d.....q7|.
+00000970: a00f 6700 a101 0100 7137 7c04 4400 5d3a  ..g.....q7|.D.]:
+00000980: 8900 8800 8801 7601 72da 7c05 6a0a 7c06  ......v.r.|.j.|.
+00000990: 6410 641a 8d02 8903 8803 640c 1900 a00b  d.d.......d.....
+000009a0: a100 a00c a100 7d07 7c00 6a0d 8703 6601  ......}.|.j...f.
+000009b0: 641b 640e 8408 6413 6414 8d02 7d08 7c08  d.d...d.d...}.|.
+000009c0: 6a0e 7c01 6415 1900 6416 8d01 7d09 7c09  j.|.d...d...}.|.
+000009d0: 6417 1900 7c09 6418 1900 6702 7c02 8800  d...|.d...g.|...
+000009e0: 3c00 7c05 6a02 8803 6a10 6413 6419 8d02  <.|.j...j.d.d...
+000009f0: 0100 71a0 7c02 5300 291c 4e72 3100 0000  ..q.|.S.).Nr1...
+00000a00: da12 696d 6261 6c61 6e63 6564 5f63 6c69  ..imbalanced_cli
+00000a10: 656e 7473 6301 0000 0000 0000 0000 0000  entsc...........
+00000a20: 0002 0000 0003 0000 0053 0000 0073 1000  .........S...s..
+00000a30: 0000 6700 7c00 5d04 7d01 7c01 9102 7102  ..g.|.].}.|...q.
+00000a40: 5300 7213 0000 0072 1300 0000 2902 da02  S.r....r....)...
+00000a50: 2e30 723f 0000 0072 1300 0000 7213 0000  .0r?...r....r...
+00000a60: 0072 1400 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000a70: 703e 4a00 0000 7302 0000 0010 007a 3253  p>J...s......z2S
+00000a80: 6861 7264 5f53 706c 6974 732e 646f 6d69  hard_Splits.domi
+00000a90: 6e61 6e74 5f73 616d 706c 696e 672e 3c6c  nant_sampling.<l
+00000aa0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000ab0: 3e72 1e00 0000 7206 0000 0029 01da 0461  >r....r....)...a
+00000ac0: 7869 735a 1263 7573 746f 6d5f 7361 6d70  xisZ.custom_samp
+00000ad0: 6c65 5f73 697a 6563 0100 0000 0000 0000  le_sizec........
+00000ae0: 0000 0000 0200 0000 0600 0000 1300 0000  ................
+00000af0: 732a 0000 0069 007c 005d 117d 017c 0164  s*...i.|.].}.|.d
+00000b00: 0088 0188 0019 0064 0019 0018 0074 0088  .......d.....t..
+00000b10: 0283 0164 0018 001b 0093 0271 0253 0029  ...d.......q.S.)
+00000b20: 0172 0600 0000 2901 7236 0000 0029 0272  .r....).r6...).r
+00000b30: 4200 0000 da03 6b65 7929 0372 3f00 0000  B.....key).r?...
+00000b40: da11 696d 6261 6c61 6e63 6564 5f61 6765  ..imbalanced_age
+00000b50: 6e74 73da 066c 6162 656c 7372 1300 0000  nts..labelsr....
+00000b60: 7214 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
+00000b70: 3e56 0000 0073 0200 0000 2a00 7a32 5368  >V...s....*.z2Sh
+00000b80: 6172 645f 5370 6c69 7473 2e64 6f6d 696e  ard_Splits.domin
+00000b90: 616e 745f 7361 6d70 6c69 6e67 2e3c 6c6f  ant_sampling.<lo
+00000ba0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00000bb0: 7201 0000 00da 056c 6162 656c 6301 0000  r......labelc...
+00000bc0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000bd0: 0013 0000 0073 0800 0000 8800 7c00 1900  .....s......|...
+00000be0: 5300 a901 4e72 1300 0000 2901 da01 7829  S...Nr....)...x)
+00000bf0: 01da 1073 616d 706c 696e 675f 7765 6967  ...sampling_weig
+00000c00: 6874 7372 1300 0000 7214 0000 00da 083c  htsr....r......<
+00000c10: 6c61 6d62 6461 3e5e 0000 0073 0200 0000  lambda>^...s....
+00000c20: 0800 7a30 5368 6172 645f 5370 6c69 7473  ..z0Shard_Splits
+00000c30: 2e64 6f6d 696e 616e 745f 7361 6d70 6c69  .dominant_sampli
+00000c40: 6e67 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ng.<locals>.<lam
+00000c50: 6264 613e da07 7765 6967 6874 7372 3200  bda>..weightsr2.
+00000c60: 0000 2903 da01 6e72 4e00 0000 da0c 7261  ..)...nrN.....ra
+00000c70: 6e64 6f6d 5f73 7461 7465 6302 0000 0000  ndom_statec.....
+00000c80: 0000 0000 0000 0002 0000 0003 0000 0013  ................
+00000c90: 0000 00f3 0e00 0000 7c01 7400 8800 6a01  ........|.t...j.
+00000ca0: 8301 7600 5300 724a 0000 00a9 02da 046c  ..v.S.rJ.......l
+00000cb0: 6973 7472 1c00 0000 a902 da06 6669 6c74  istr........filt
+00000cc0: 6572 da03 6964 78a9 01da 0673 616d 706c  er..idx....sampl
+00000cd0: 6572 1300 0000 7214 0000 0072 4d00 0000  er....r....rM...
+00000ce0: 6300 0000 f302 0000 000e 0054 2901 da0c  c..........T)...
+00000cf0: 7769 7468 5f69 6e64 6963 6573 7222 0000  with_indicesr"..
+00000d00: 0072 2300 0000 7225 0000 0072 2600 0000  .r#...r%...r&...
+00000d10: 2901 da07 696e 706c 6163 6529 0272 4f00  )...inplace).rO.
+00000d20: 0000 7250 0000 0063 0200 0000 0000 0000  ..rP...c........
+00000d30: 0000 0000 0200 0000 0300 0000 1300 0000  ................
+00000d40: 7251 0000 0072 4a00 0000 7252 0000 0072  rQ...rJ...rR...r
+00000d50: 5400 0000 7257 0000 0072 1300 0000 7214  T...rW...r....r.
+00000d60: 0000 0072 4d00 0000 7400 0000 7259 0000  ...rM...t...rY..
+00000d70: 0029 1172 0c00 0000 da09 746f 5f70 616e  .).r......to_pan
+00000d80: 6461 73da 0464 726f 70da 0673 6f72 7465  das..drop..sorte
+00000d90: 6472 4900 0000 da06 756e 6971 7565 da03  drI.....unique..
+00000da0: 6765 7472 0900 0000 7236 0000 00da 0561  getr....r6.....a
+00000db0: 7070 6c79 7258 0000 00da 0c76 616c 7565  pplyrX.....value
+00000dc0: 5f63 6f75 6e74 73da 0a73 6f72 745f 696e  _counts..sort_in
+00000dd0: 6465 7872 5500 0000 722c 0000 0072 2d00  dexrU...r,...r-.
+00000de0: 0000 721c 0000 0029 0a72 1700 0000 7218  ..r....).r....r.
+00000df0: 0000 0072 2e00 0000 5a09 6e6f 5f61 6765  ...r....Z.no_age
+00000e00: 6e74 7372 3100 0000 da09 7061 6e64 6173  ntsr1.....pandas
+00000e10: 5f64 66da 0b73 616d 706c 655f 7369 7a65  _df..sample_size
+00000e20: da06 636f 756e 7473 5a0c 7361 6d70 6c65  ..countsZ.sample
+00000e30: 645f 6461 7461 722f 0000 0072 1300 0000  d_datar/...r....
+00000e40: 2905 723f 0000 0072 4600 0000 7247 0000  ).r?...rF...rG..
+00000e50: 0072 5800 0000 724c 0000 0072 1400 0000  .rX...rL...r....
+00000e60: da11 646f 6d69 6e61 6e74 5f73 616d 706c  ..dominant_sampl
+00000e70: 696e 6744 0000 0073 3e00 0000 0403 0801  ingD...s>.......
+00000e80: 0801 1201 1201 0e01 0a01 0a01 1002 0803  ................
+00000e90: 0801 1602 1801 1a07 1001 1002 1602 1001  ................
+00000ea0: 1601 1203 0c02 0804 0801 0e02 1001 1602  ................
+00000eb0: 1001 1401 1002 0280 0401 7a1e 5368 6172  ..........z.Shar
+00000ec0: 645f 5370 6c69 7473 2e64 6f6d 696e 616e  d_Splits.dominan
+00000ed0: 745f 7361 6d70 6c69 6e67 6302 0000 0000  t_samplingc.....
+00000ee0: 0000 0000 0000 0005 0000 0008 0000 0043  ...............C
+00000ef0: 0000 0073 5a00 0000 6700 7d02 7c00 6a00  ...sZ...g.}.|.j.
+00000f00: 6401 6402 6403 8d02 7d03 7c03 6a01 7c01  d.d.d...}.|.j.|.
+00000f10: 6404 1900 6405 8d01 7d03 7402 7c01 6406  d...d...}.t.|.d.
+00000f20: 1900 8301 4400 5d13 7d04 7c02 a003 7404  ....D.].}.|...t.
+00000f30: a005 7c03 6407 1900 a101 7404 a005 7c03  ..|.d.....t...|.
+00000f40: 6408 1900 a101 6702 a101 0100 7117 7c02  d.....g.....q.|.
+00000f50: 5300 2909 4e72 0600 0000 7201 0000 0072  S.).Nr....r....r
+00000f60: 1a00 0000 7222 0000 0072 2300 0000 7231  ....r"...r#...r1
+00000f70: 0000 0072 2500 0000 7226 0000 0029 0672  ...r%...r&...).r
+00000f80: 2700 0000 722c 0000 0072 0c00 0000 722d  '...r,...r....r-
+00000f90: 0000 0072 2900 0000 722a 0000 0029 0572  ...r)...r*...).r
+00000fa0: 1700 0000 7218 0000 0072 2e00 0000 722f  ....r....r....r/
+00000fb0: 0000 0072 1200 0000 7213 0000 0072 1300  ...r....r....r..
+00000fc0: 0000 7214 0000 00da 1672 6570 6c69 6361  ..r......replica
+00000fd0: 7465 5f73 616d 655f 6461 7461 7365 747b  te_same_dataset{
+00000fe0: 0000 0073 0c00 0000 0403 0e01 1001 1001  ...s............
+00000ff0: 2401 0402 7a23 5368 6172 645f 5370 6c69  $...z#Shard_Spli
+00001000: 7473 2e72 6570 6c69 6361 7465 5f73 616d  ts.replicate_sam
+00001010: 655f 6461 7461 7365 7463 0200 0000 0000  e_datasetc......
+00001020: 0000 0000 0000 0600 0000 0900 0000 4300  ..............C.
+00001030: 0000 737c 0000 0067 007d 0274 007c 0164  ..s|...g.}.t.|.d
+00001040: 0119 0083 0144 005d 337d 037c 006a 017c  .....D.]3}.|.j.|
+00001050: 0164 0119 007c 0364 028d 027d 047c 046a  .d...|.d...}.|.j
+00001060: 027c 0164 0319 0064 048d 017d 0474 0074  .|.d...d...}.t.t
+00001070: 037c 0164 0519 007c 0164 0119 001b 0083  .|.d...|.d......
+00001080: 0183 0144 005d 137d 057c 02a0 0474 05a0  ...D.].}.|...t..
+00001090: 067c 0464 0619 00a1 0174 05a0 067c 0464  .|.d.....t...|.d
+000010a0: 0719 00a1 0167 02a1 0101 0071 2771 087c  .....g.....q'q.|
+000010b0: 0253 0029 084e 7219 0000 0072 1a00 0000  .S.).Nr....r....
+000010c0: 7222 0000 0072 2300 0000 7231 0000 0072  r"...r#...r1...r
+000010d0: 2500 0000 7226 0000 0029 0772 0c00 0000  %...r&...).r....
+000010e0: 7227 0000 0072 2c00 0000 7209 0000 0072  r'...r,...r....r
+000010f0: 2d00 0000 7229 0000 0072 2a00 0000 2906  -...r)...r*...).
+00001100: 7217 0000 0072 1800 0000 722e 0000 0072  r....r....r....r
+00001110: 2700 0000 722f 0000 0072 1200 0000 7213  '...r/...r....r.
+00001120: 0000 0072 1300 0000 7214 0000 00da 0f73  ...r....r......s
+00001130: 706c 6974 5f69 6e5f 626c 6f63 6b73 8700  plit_in_blocks..
+00001140: 0000 7310 0000 0004 0310 0112 0110 011c  ..s.............
+00001150: 0124 0102 ff04 027a 1c53 6861 7264 5f53  .$.....z.Shard_S
+00001160: 706c 6974 732e 7370 6c69 745f 696e 5f62  plits.split_in_b
+00001170: 6c6f 636b 734e 290e da08 5f5f 6e61 6d65  locksN)...__name
+00001180: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001190: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+000011a0: 646f 635f 5fda 0c73 7461 7469 636d 6574  doc__..staticmet
+000011b0: 686f 64da 0864 6174 6173 6574 73da 0d61  hod..datasets..a
+000011c0: 7272 6f77 5f64 6174 6173 6574 da07 4461  rrow_dataset..Da
+000011d0: 7461 7365 74da 0464 6963 7472 3000 0000  taset..dictr0...
+000011e0: 7240 0000 0072 6700 0000 7268 0000 0072  r@...rg...rh...r
+000011f0: 6900 0000 7213 0000 0072 1300 0000 7213  i...r....r....r.
+00001200: 0000 0072 1400 0000 7216 0000 0013 0000  ...r....r.......
+00001210: 0073 2c00 0000 0800 0401 0202 0a01 0201  .s,.............
+00001220: 0cff 0216 0a01 0201 0cff 0216 0a01 0201  ................
+00001230: 0cff 0236 0a01 0201 0cff 020b 0a01 0201  ...6............
+00001240: 10ff 7216 0000 0029 0d72 6f00 0000 7202  ..r....).ro...r.
+00001250: 0000 00da 2661 736f 6369 6974 612e 6461  ....&asociita.da
+00001260: 7461 7365 7473 2e73 6861 7264 5f74 7261  tasets.shard_tra
+00001270: 6e73 666f 726d 6174 696f 6e72 0300 0000  nsformationr....
+00001280: da17 6173 6f63 6969 7461 2e75 7469 6c73  ..asociita.utils
+00001290: 2e68 616e 646c 6572 7372 0400 0000 da17  .handlersr......
+000012a0: 6173 6f63 6969 7461 2e75 7469 6c73 2e73  asociita.utils.s
+000012b0: 686f 7763 6173 6572 0500 0000 7229 0000  howcaser....r)..
+000012c0: 00da 056e 756d 7079 720a 0000 0072 1500  ...numpyr....r..
+000012d0: 0000 7216 0000 0072 1300 0000 7213 0000  ..r....r....r...
+000012e0: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
+000012f0: 6475 6c65 3e01 0000 0073 1200 0000 0800  dule>....s......
+00001300: 0c01 0c01 0c01 0c01 0801 0801 0802 120a  ................
```

### Comparing `asociita-0.3.3/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc` & `asociita-0.3.4/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/fetch_data.py` & `asociita-0.3.4/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/load_cifar.py` & `asociita-0.3.4/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/load_fmnist.py` & `asociita-0.3.4/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/load_mnist.py` & `asociita-0.3.4/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/save_blueprint.py` & `asociita-0.3.4/asociita/datasets/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/datasets/shard_splits.py` & `asociita-0.3.4/asociita/datasets/shard_splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
             
             # Shard transformation
             if shard in settings['transformations'].keys():
                 if settings['save_transformations']:
                     original_imgs = copy.deepcopy(agent_data['image'])
                 agent_data = Shard_Transformation.transform(agent_data, preferences=settings['transformations'][shard]) # CALL SHARD_TRANSFORMATION CLASS
                 if settings['save_transformations']:
-                    save_random(original_imgs, agent_data['image'], settings['transformations'][shard]["transformation_type"])
+                    save_random(original_imgs, 
+                                agent_data['image'], 
+                                settings['transformations'][shard]["transformation_type"],
+                                name = f"of_node_{shard}")
 
             # In-shard split between test and train data.
             agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
             nodes_data.append([agent_data['train'], agent_data['test']])
         return nodes_data
     
     @staticmethod
```

### Comparing `asociita-0.3.3/asociita/datasets/shard_transformation.py` & `asociita-0.3.4/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc` & `asociita-0.3.4/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc` & `asociita-0.3.4/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc` & `asociita-0.3.4/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc` & `asociita-0.3.4/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc` & `asociita-0.3.4/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc` & `asociita-0.3.4/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/cifar10.py` & `asociita-0.3.4/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/federated_model.py` & `asociita-0.3.4/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/models/pytorch/mnist.py` & `asociita-0.3.4/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/computations.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/computations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/debugger.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/debugger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/handlers.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/handlers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/helpers.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/loggers.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/loggers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/orchestrations.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/orchestrations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/__pycache__/showcase.cpython-310.pyc` & `asociita-0.3.4/asociita/utils/__pycache__/showcase.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 29 08:30:33 2023 UTC, .py size: 1026 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,82 @@
-00000000: 6f0d 0d0a 0000 0000 a962 7464 0204 0000  o........btd....
+00000000: 6f0d 0d0a 0000 0000 ae2f d264 1a04 0000  o......../.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
+00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 5a04 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6401 6c07 5a07 6403 6404 8400 5a08 6405  d.l.Z.d.d...Z.d.
-00000060: 6406 8400 5a09 6407 650a 6602 6408 6409  d...Z.d.e.f.d.d.
-00000070: 8404 5a0b 6401 5300 290a e900 0000 004e  ..Z.d.S.)......N
-00000080: 2901 da05 496d 6167 6563 0100 0000 0000  )...Imagec......
-00000090: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000000a0: 0000 7318 0000 0074 00a0 017c 00a1 017d  ..s....t...|...}
-000000b0: 0074 02a0 037c 00a1 0101 0064 0053 0029  .t...|.....d.S.)
-000000c0: 014e 2904 da02 6e70 da07 6173 6172 7261  .N)...np..asarra
-000000d0: 79da 0370 6c74 da06 696d 7368 6f77 2901  y..plt..imshow).
-000000e0: da03 696d 67a9 0072 0800 0000 fa66 2f68  ..img..r.....f/h
-000000f0: 6f6d 652f 6d7a 757a 6961 6b2f 736e 6170  ome/mzuziak/snap
-00000100: 2f73 6e61 7064 2d64 6573 6b74 6f70 2d69  /snapd-desktop-i
-00000110: 6e74 6567 7261 7469 6f6e 2f38 332f 446f  ntegration/83/Do
-00000120: 6375 6d65 6e74 732f 4173 6f63 6969 7461  cuments/Asociita
-00000130: 2f61 736f 6369 6974 612f 6173 6f63 6969  /asociita/asocii
-00000140: 7461 2f75 7469 6c73 2f73 686f 7763 6173  ta/utils/showcas
-00000150: 652e 7079 da0a 7368 6f77 5f69 6d61 6765  e.py..show_image
-00000160: 0700 0000 7304 0000 000a 010e 0172 0a00  ....s........r..
-00000170: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
-00000180: 0000 0006 0000 0043 0000 0073 7e00 0000  .......C...s~...
-00000190: 7400 a001 6401 6402 a102 5c02 7d02 7d03  t...d.d...\.}.}.
-000001a0: 7402 6402 8301 4400 5d2c 7d04 7403 a004  t.d...D.],}.t...
-000001b0: 6403 7405 7c00 8301 6404 1800 a102 7d05  d.t.|...d.....}.
-000001c0: 7406 a007 7c00 7c05 1900 a101 7d06 7406  t...|.|.....}.t.
-000001d0: a007 7c01 7c05 1900 a101 7d07 7c03 6403  ..|.|.....}.|.d.
-000001e0: 1900 7c04 1900 a008 7c06 a101 0100 7c03  ..|.....|.....|.
-000001f0: 6404 1900 7c04 1900 a008 7c07 a101 0100  d...|.....|.....
-00000200: 710c 7400 a009 a100 0100 6400 5300 2905  q.t.......d.S.).
-00000210: 4ee9 0200 0000 e905 0000 0072 0100 0000  N..........r....
-00000220: e901 0000 0029 0a72 0500 0000 da08 7375  .....).r......su
-00000230: 6270 6c6f 7473 da05 7261 6e67 65da 0672  bplots..range..r
-00000240: 616e 646f 6dda 0772 616e 6469 6e74 da03  andom..randint..
-00000250: 6c65 6e72 0300 0000 7204 0000 0072 0600  lenr....r....r..
-00000260: 0000 da04 7368 6f77 2908 da09 696d 6773  ....show)...imgs
-00000270: 5f6f 7269 67da 1069 6d67 735f 7472 616e  _orig..imgs_tran
-00000280: 7366 6f72 6d65 64da 0366 6967 da02 6178  sformed..fig..ax
-00000290: da08 706f 7369 7469 6f6e da0a 7261 6e64  ..position..rand
-000002a0: 6f6d 5f70 6f73 da0c 6f72 6967 696e 616c  om_pos..original
-000002b0: 5f69 6d67 da0f 7472 616e 7366 6f72 6d65  _img..transforme
-000002c0: 645f 696d 6772 0800 0000 7208 0000 0072  d_imgr....r....r
-000002d0: 0900 0000 da0b 7368 6f77 5f72 616e 646f  ......show_rando
-000002e0: 6d0c 0000 0073 1000 0000 1001 0c01 1401  m....s..........
-000002f0: 0e01 0e01 1201 1401 0c01 721c 0000 00da  ..........r.....
-00000300: 0e74 7261 6e73 666f 726d 6174 696f 6e63  .transformationc
-00000310: 0300 0000 0000 0000 0000 0000 0a00 0000  ................
-00000320: 0600 0000 4300 0000 7388 0000 0074 00a0  ....C...s....t..
-00000330: 0164 0164 02a1 025c 027d 037d 0474 0264  .d.d...\.}.}.t.d
-00000340: 0283 0144 005d 2c7d 0574 03a0 0464 0374  ...D.],}.t...d.t
-00000350: 057c 0083 0164 0418 00a1 027d 0674 06a0  .|...d.....}.t..
-00000360: 077c 007c 0619 00a1 017d 0774 06a0 077c  .|.|.....}.t...|
-00000370: 017c 0619 00a1 017d 087c 0464 0319 007c  .|.....}.|.d...|
-00000380: 0519 00a0 087c 07a1 0101 007c 0464 0419  .....|.....|.d..
-00000390: 007c 0519 00a0 087c 08a1 0101 0071 0c7c  .|.....|.....q.|
-000003a0: 0264 0517 007d 0974 00a0 097c 09a1 0101  .d...}.t...|....
-000003b0: 0064 0053 0029 064e 720b 0000 0072 0c00  .d.S.).Nr....r..
-000003c0: 0000 7201 0000 0072 0d00 0000 7a04 2e70  ..r....r....z..p
-000003d0: 6466 290a 7205 0000 0072 0e00 0000 720f  df).r....r....r.
-000003e0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-000003f0: 0000 7203 0000 0072 0400 0000 7206 0000  ..r....r....r...
-00000400: 005a 0773 6176 6566 6967 290a 7214 0000  .Z.savefig).r...
-00000410: 0072 1500 0000 721d 0000 0072 1600 0000  .r....r....r....
-00000420: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000430: 1a00 0000 721b 0000 00da 0574 6974 6c65  ....r......title
-00000440: 7208 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
-00000450: 0b73 6176 655f 7261 6e64 6f6d 1700 0000  .save_random....
-00000460: 7312 0000 0010 010c 0114 010e 010e 0112  s...............
-00000470: 0114 0108 010e 0172 1f00 0000 290c da11  .......r....)...
-00000480: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-00000490: 74da 0670 7970 6c6f 7472 0500 0000 da05  t..pyplotr......
-000004a0: 6e75 6d70 7972 0300 0000 da03 5049 4c72  numpyr......PILr
-000004b0: 0200 0000 7210 0000 0072 0a00 0000 721c  ....r....r....r.
-000004c0: 0000 00da 0373 7472 721f 0000 0072 0800  .....strr....r..
-000004d0: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
-000004e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000004f0: 0e00 0000 0c00 0801 0c01 0801 0803 0805  ................
-00000500: 120b                                     ..
+00000060: 6406 8400 5a09 6407 650a 6408 650a 6604  d...Z.d.e.d.e.f.
+00000070: 6409 640a 8404 5a0b 6401 5300 290b e900  d.d...Z.d.S.)...
+00000080: 0000 004e 2901 da05 496d 6167 6563 0100  ...N)...Imagec..
+00000090: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000000a0: 0000 4300 0000 7318 0000 0074 00a0 017c  ..C...s....t...|
+000000b0: 00a1 017d 0074 02a0 037c 00a1 0101 0064  ...}.t...|.....d
+000000c0: 0053 0029 014e 2904 da02 6e70 da07 6173  .S.).N)...np..as
+000000d0: 6172 7261 79da 0370 6c74 da06 696d 7368  array..plt..imsh
+000000e0: 6f77 2901 da03 696d 67a9 0072 0800 0000  ow)...img..r....
+000000f0: fa66 2f68 6f6d 652f 6d7a 757a 6961 6b2f  .f/home/mzuziak/
+00000100: 736e 6170 2f73 6e61 7064 2d64 6573 6b74  snap/snapd-deskt
+00000110: 6f70 2d69 6e74 6567 7261 7469 6f6e 2f38  op-integration/8
+00000120: 332f 446f 6375 6d65 6e74 732f 4173 6f63  3/Documents/Asoc
+00000130: 6969 7461 2f61 736f 6369 6974 612f 6173  iita/asociita/as
+00000140: 6f63 6969 7461 2f75 7469 6c73 2f73 686f  ociita/utils/sho
+00000150: 7763 6173 652e 7079 da0a 7368 6f77 5f69  wcase.py..show_i
+00000160: 6d61 6765 0700 0000 7304 0000 000a 010e  mage....s.......
+00000170: 0172 0a00 0000 6302 0000 0000 0000 0000  .r....c.........
+00000180: 0000 0008 0000 0006 0000 0043 0000 0073  ...........C...s
+00000190: 7e00 0000 7400 a001 6401 6402 a102 5c02  ~...t...d.d...\.
+000001a0: 7d02 7d03 7402 6402 8301 4400 5d2c 7d04  }.}.t.d...D.],}.
+000001b0: 7403 a004 6403 7405 7c00 8301 6404 1800  t...d.t.|...d...
+000001c0: a102 7d05 7406 a007 7c00 7c05 1900 a101  ..}.t...|.|.....
+000001d0: 7d06 7406 a007 7c01 7c05 1900 a101 7d07  }.t...|.|.....}.
+000001e0: 7c03 6403 1900 7c04 1900 a008 7c06 a101  |.d...|.....|...
+000001f0: 0100 7c03 6404 1900 7c04 1900 a008 7c07  ..|.d...|.....|.
+00000200: a101 0100 710c 7400 a009 a100 0100 6400  ....q.t.......d.
+00000210: 5300 2905 4ee9 0200 0000 e905 0000 0072  S.).N..........r
+00000220: 0100 0000 e901 0000 0029 0a72 0500 0000  .........).r....
+00000230: da08 7375 6270 6c6f 7473 da05 7261 6e67  ..subplots..rang
+00000240: 65da 0672 616e 646f 6dda 0772 616e 6469  e..random..randi
+00000250: 6e74 da03 6c65 6e72 0300 0000 7204 0000  nt..lenr....r...
+00000260: 0072 0600 0000 da04 7368 6f77 2908 da09  .r......show)...
+00000270: 696d 6773 5f6f 7269 67da 1069 6d67 735f  imgs_orig..imgs_
+00000280: 7472 616e 7366 6f72 6d65 64da 0366 6967  transformed..fig
+00000290: da02 6178 da08 706f 7369 7469 6f6e da0a  ..ax..position..
+000002a0: 7261 6e64 6f6d 5f70 6f73 da0c 6f72 6967  random_pos..orig
+000002b0: 696e 616c 5f69 6d67 da0f 7472 616e 7366  inal_img..transf
+000002c0: 6f72 6d65 645f 696d 6772 0800 0000 7208  ormed_imgr....r.
+000002d0: 0000 0072 0900 0000 da0b 7368 6f77 5f72  ...r......show_r
+000002e0: 616e 646f 6d0c 0000 0073 1000 0000 1001  andom....s......
+000002f0: 0c01 1401 0e01 0e01 1201 1401 0c01 721c  ..............r.
+00000300: 0000 00da 0e74 7261 6e73 666f 726d 6174  .....transformat
+00000310: 696f 6eda 046e 616d 6563 0400 0000 0000  ion..namec......
+00000320: 0000 0000 0000 0b00 0000 0600 0000 4300  ..............C.
+00000330: 0000 7390 0000 0074 00a0 0164 0164 02a1  ..s....t...d.d..
+00000340: 025c 027d 047d 0574 0264 0283 0144 005d  .\.}.}.t.d...D.]
+00000350: 2c7d 0674 03a0 0464 0374 057c 0083 0164  ,}.t...d.t.|...d
+00000360: 0418 00a1 027d 0774 06a0 077c 007c 0719  .....}.t...|.|..
+00000370: 00a1 017d 0874 06a0 077c 017c 0719 00a1  ...}.t...|.|....
+00000380: 017d 097c 0564 0319 007c 0619 00a0 087c  .}.|.d...|.....|
+00000390: 08a1 0101 007c 0564 0419 007c 0619 00a0  .....|.d...|....
+000003a0: 087c 09a1 0101 0071 0c7c 0264 0517 007c  .|.....q.|.d...|
+000003b0: 0317 0064 0617 007d 0a74 00a0 097c 0aa1  ...d...}.t...|..
+000003c0: 0101 0064 0053 0029 074e 720b 0000 0072  ...d.S.).Nr....r
+000003d0: 0c00 0000 7201 0000 0072 0d00 0000 da01  ....r....r......
+000003e0: 5f7a 042e 7064 6629 0a72 0500 0000 720e  _z..pdf).r....r.
+000003f0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00000400: 0000 7212 0000 0072 0300 0000 7204 0000  ..r....r....r...
+00000410: 0072 0600 0000 da07 7361 7665 6669 6729  .r......savefig)
+00000420: 0b72 1400 0000 7215 0000 0072 1d00 0000  .r....r....r....
+00000430: 721e 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000440: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+00000450: 0000 00da 0574 6974 6c65 7208 0000 0072  .....titler....r
+00000460: 0800 0000 7209 0000 00da 0b73 6176 655f  ....r......save_
+00000470: 7261 6e64 6f6d 1700 0000 7312 0000 0010  random....s.....
+00000480: 010c 0114 010e 010e 0112 0114 0110 010e  ................
+00000490: 0172 2200 0000 290c da11 6d61 7470 6c6f  .r"...)...matplo
+000004a0: 746c 6962 2e70 7970 6c6f 74da 0670 7970  tlib.pyplot..pyp
+000004b0: 6c6f 7472 0500 0000 da05 6e75 6d70 7972  lotr......numpyr
+000004c0: 0300 0000 da03 5049 4c72 0200 0000 7210  ......PILr....r.
+000004d0: 0000 0072 0a00 0000 721c 0000 00da 0373  ...r....r......s
+000004e0: 7472 7222 0000 0072 0800 0000 7208 0000  trr"...r....r...
+000004f0: 0072 0800 0000 7209 0000 00da 083c 6d6f  .r....r......<mo
+00000500: 6475 6c65 3e01 0000 0073 0e00 0000 0c00  dule>....s......
+00000510: 0801 0c01 0801 0803 0805 160b            ............
```

### Comparing `asociita-0.3.3/asociita/utils/computations.py` & `asociita-0.3.4/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/custom_transformations.py` & `asociita-0.3.4/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/debugger.py` & `asociita-0.3.4/asociita/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/handlers.py` & `asociita-0.3.4/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/helpers.py` & `asociita-0.3.4/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/loggers.py` & `asociita-0.3.4/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/optimizers.py` & `asociita-0.3.4/asociita/utils/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 
 class Optimizers():
     def __init__(self,
                  weights: OrderedDict,
                  settings: dict) -> None:
         # Seting up a device for the Optimizer. Please note, that the device must be the same as this
         # that the nets were placed on. Otherwise, PyTorch will raise an exception trying to combine
-        # data placec on CPU and GPU.
-        self.device = torch.device("cpu")
-        self.previous_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        self.previous_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        # data placed on CPU and GPU.
+        self.previous_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        self.previous_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
         self.optimizer = settings['name']
         self.learning_rate = torch.tensor(settings['learning_rate'])
 
         # Selecting a proper centralised optimizer and placing all the tensors on the same device.
         if self.optimizer == 'Simple':
-            self.learning_rate = self.learning_rate.to(self.device)
+            pass
         elif self.optimizer == "FedAdagard":
             self.b1 = torch.tensor(settings['b1'])
             self.tau = torch.tensor(settings['tau'])
-            self.b1, self.tau, self.learning_rate = self.b1.to(self.device), self.tau.to(self.device), self.learning_rate.to(self.device)
         elif self.optimizer == "FedYogi" or self.optimizer == "FedAdam":
             self.b1 = torch.tensor(settings['b1'])
             self.b2 = torch.tensor(settings['b2'])
             self.tau = torch.tensor(settings['tau'])
-            self.b1, self.b2, self.tau, self.learning_rate = self.b1.to(self.device), self.b2.to(self.device), self.tau.to(self.device), self.learning_rate.to(self.device)
         else:
             "Wrong optimizer's name was provided. Unable to retrieve parameters!"
 
 
     def fed_optimize(self,
                      weights: OrderedDict,
                      delta: OrderedDict) -> OrderedDict:
@@ -80,27 +77,26 @@
     def FedAdagard(self,
                    weights: OrderedDict,
                    delta: OrderedDict,
                    b1: float, 
                    tau: float,
                    learning_rate: float) -> OrderedDict:
         # Defining the current delta.
-        current_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        current_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        updated_weights = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-
+        current_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        current_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        updated_weights = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
 
         for row_key in current_delta.keys():
             current_delta[row_key] = b1 * self.previous_delta[row_key] + (1 - b1) * delta[row_key]
         
         for row_key in current_momentum.keys():
             current_momentum[row_key] = self.previous_momentum[row_key] + (current_delta[row_key] ** 2)
 
         for row_key in updated_weights.keys():
-            updated_weights[row_key] = (weights[row_key].to(self.device)) + (learning_rate * (current_delta[row_key] / (torch.sqrt(current_momentum[row_key]) + tau)))
+            updated_weights[row_key] = weights[row_key] + (learning_rate * (current_delta[row_key] / (torch.sqrt(current_momentum[row_key]) + tau)))
         
         self.previous_delta = current_delta
         self.previous_momentum = current_momentum
 
         return updated_weights
 
 
@@ -108,17 +104,17 @@
                 weights: OrderedDict,
                 delta: OrderedDict,
                 b1: float,
                 b2: float,
                 tau: float,
                 learning_rate: float):
         # Defining the current delta.
-        current_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        current_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        updated_weights = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        current_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        current_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        updated_weights = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
 
         for row_key in current_delta.keys():
             current_delta[row_key] = b1 * self.previous_delta[row_key] + (1 - b1) * delta[row_key]
         
         for row_key in current_momentum.keys():
             current_momentum[row_key] = self.previous_momentum[row_key] - ((1 - b2) * (current_delta[row_key] ** 2) * torch.sign((self.previous_momentum[row_key] - (current_delta[row_key] ** 2))))
 
@@ -135,17 +131,17 @@
                 weights: OrderedDict,
                 delta: OrderedDict,
                 b1: float,
                 b2: float,
                 tau: float,
                 learning_rate: float):
         # Defining the current delta.
-        current_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        current_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
-        updated_weights = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        current_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        current_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        updated_weights = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
 
         for row_key in current_delta.keys():
             current_delta[row_key] = b1 * self.previous_delta[row_key] + (1 - b1) * delta[row_key]
         
         for row_key in current_momentum.keys():
             current_momentum[row_key] = (b2 * self.previous_momentum[row_key]) + ((1 - b2) * (current_delta[row_key] ** 2))
```

### Comparing `asociita-0.3.3/asociita/utils/orchestrations.py` & `asociita-0.3.4/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.3/asociita/utils/showcase.py` & `asociita-0.3.4/asociita/utils/showcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         original_img = np.asarray(imgs_orig[random_pos])
         transformed_img = np.asarray(imgs_transformed[random_pos])
         ax[0][position].imshow(original_img)
         ax[1][position].imshow(transformed_img)
     plt.show()
 
 
-def save_random(imgs_orig, imgs_transformed, transformation: str):
+def save_random(imgs_orig, imgs_transformed, transformation: str, name: str):
     fig, ax = plt.subplots(2, 5)
     for position in range(5):
         random_pos = random.randint(0, len(imgs_orig) - 1)
         original_img = np.asarray(imgs_orig[random_pos])
         transformed_img = np.asarray(imgs_transformed[random_pos])
         ax[0][position].imshow(original_img)
         ax[1][position].imshow(transformed_img)
-    title = transformation + '.pdf'
+    title = transformation + '_' + name + '.pdf'
     plt.savefig(title)
```

### Comparing `asociita-0.3.3/pyproject.toml` & `asociita-0.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.3.3"
+version = "0.3.4"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.3.3/PKG-INFO` & `asociita-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.3.3
+Version: 0.3.4
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

