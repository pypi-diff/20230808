# Comparing `tmp/keras-core-0.1.3.tar.gz` & `tmp/keras-core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-core-0.1.3.tar", last modified: Wed Jul 26 20:30:10 2023, max compression
+gzip compressed data, was "keras-core-0.1.4.tar", last modified: Tue Aug  8 19:08:53 2023, max compression
```

## Comparing `keras-core-0.1.3.tar` & `keras-core-0.1.4.tar`

### file list

```diff
@@ -1,619 +1,628 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.494075 keras-core-0.1.3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3822 2023-07-26 20:30:10.493832 keras-core-0.1.3/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2972 2023-07-26 20:30:01.000000 keras-core-0.1.3/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.396905 keras-core-0.1.3/keras_core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1641 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.397858 keras-core-0.1.3/keras_core/_tf_keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1759 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398076 keras-core-0.1.3/keras_core/_tf_keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398282 keras-core-0.1.3/keras_core/_tf_keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398457 keras-core-0.1.3/keras_core/_tf_keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398630 keras-core-0.1.3/keras_core/_tf_keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398798 keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.398979 keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399148 keras-core-0.1.3/keras_core/_tf_keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399320 keras-core-0.1.3/keras_core/_tf_keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399482 keras-core-0.1.3/keras_core/_tf_keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399639 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399803 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.399945 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400087 keras-core-0.1.3/keras_core/_tf_keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400245 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400400 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400533 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400692 keras-core-0.1.3/keras_core/_tf_keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.400860 keras-core-0.1.3/keras_core/_tf_keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401027 keras-core-0.1.3/keras_core/_tf_keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401172 keras-core-0.1.3/keras_core/_tf_keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7283 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401331 keras-core-0.1.3/keras_core/_tf_keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401533 keras-core-0.1.3/keras_core/_tf_keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401729 keras-core-0.1.3/keras_core/_tf_keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      858 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.401884 keras-core-0.1.3/keras_core/_tf_keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402042 keras-core-0.1.3/keras_core/_tf_keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402202 keras-core-0.1.3/keras_core/_tf_keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402376 keras-core-0.1.3/keras_core/_tf_keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402529 keras-core-0.1.3/keras_core/_tf_keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402678 keras-core-0.1.3/keras_core/_tf_keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402831 keras-core-0.1.3/keras_core/_tf_keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.402982 keras-core-0.1.3/keras_core/_tf_keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.403159 keras-core-0.1.3/keras_core/_tf_keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2926 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.403317 keras-core-0.1.3/keras_core/_tf_keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10318 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.403475 keras-core-0.1.3/keras_core/_tf_keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      160 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.403615 keras-core-0.1.3/keras_core/_tf_keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.403838 keras-core-0.1.3/keras_core/_tf_keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3358 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404134 keras-core-0.1.3/keras_core/_tf_keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5556 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404331 keras-core-0.1.3/keras_core/_tf_keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      591 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404487 keras-core-0.1.3/keras_core/_tf_keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404628 keras-core-0.1.3/keras_core/_tf_keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7979 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404772 keras-core-0.1.3/keras_core/_tf_keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      274 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.404926 keras-core-0.1.3/keras_core/_tf_keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1331 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405068 keras-core-0.1.3/keras_core/_tf_keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5770 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405207 keras-core-0.1.3/keras_core/_tf_keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      881 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405349 keras-core-0.1.3/keras_core/_tf_keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405497 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      745 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405639 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1397 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405775 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      530 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.405912 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/text/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      462 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406043 keras-core-0.1.3/keras_core/_tf_keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      492 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406175 keras-core-0.1.3/keras_core/_tf_keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      871 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406312 keras-core-0.1.3/keras_core/_tf_keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406446 keras-core-0.1.3/keras_core/_tf_keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2696 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406686 keras-core-0.1.3/keras_core/_tf_keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/_tf_keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406844 keras-core-0.1.3/keras_core/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.406991 keras-core-0.1.3/keras_core/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407136 keras-core-0.1.3/keras_core/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407288 keras-core-0.1.3/keras_core/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407427 keras-core-0.1.3/keras_core/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407569 keras-core-0.1.3/keras_core/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407727 keras-core-0.1.3/keras_core/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.407880 keras-core-0.1.3/keras_core/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408017 keras-core-0.1.3/keras_core/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408154 keras-core-0.1.3/keras_core/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408307 keras-core-0.1.3/keras_core/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408439 keras-core-0.1.3/keras_core/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408574 keras-core-0.1.3/keras_core/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408715 keras-core-0.1.3/keras_core/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.408870 keras-core-0.1.3/keras_core/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409016 keras-core-0.1.3/keras_core/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409158 keras-core-0.1.3/keras_core/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409296 keras-core-0.1.3/keras_core/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409441 keras-core-0.1.3/keras_core/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409597 keras-core-0.1.3/keras_core/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      743 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409731 keras-core-0.1.3/keras_core/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.409886 keras-core-0.1.3/keras_core/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410036 keras-core-0.1.3/keras_core/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      858 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410181 keras-core-0.1.3/keras_core/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410323 keras-core-0.1.3/keras_core/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410469 keras-core-0.1.3/keras_core/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410608 keras-core-0.1.3/keras_core/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410765 keras-core-0.1.3/keras_core/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.410912 keras-core-0.1.3/keras_core/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411048 keras-core-0.1.3/keras_core/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411186 keras-core-0.1.3/keras_core/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411330 keras-core-0.1.3/keras_core/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2926 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411481 keras-core-0.1.3/keras_core/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9976 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411665 keras-core-0.1.3/keras_core/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      160 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.411868 keras-core-0.1.3/keras_core/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412039 keras-core-0.1.3/keras_core/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412206 keras-core-0.1.3/keras_core/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412354 keras-core-0.1.3/keras_core/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      591 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412504 keras-core-0.1.3/keras_core/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412643 keras-core-0.1.3/keras_core/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7979 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412780 keras-core-0.1.3/keras_core/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      274 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.412925 keras-core-0.1.3/keras_core/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1331 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413054 keras-core-0.1.3/keras_core/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5770 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413181 keras-core-0.1.3/keras_core/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      881 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413309 keras-core-0.1.3/keras_core/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413439 keras-core-0.1.3/keras_core/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413580 keras-core-0.1.3/keras_core/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      347 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413715 keras-core-0.1.3/keras_core/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      185 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413846 keras-core-0.1.3/keras_core/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      492 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.413978 keras-core-0.1.3/keras_core/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      871 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.414120 keras-core-0.1.3/keras_core/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.414573 keras-core-0.1.3/keras_core/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      744 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.414857 keras-core-0.1.3/keras_core/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3483 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11945 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.417692 keras-core-0.1.3/keras_core/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24800 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16679 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25463 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40581 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16018 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14607 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15601 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17253 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18015 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23532 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30652 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19116 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6454 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9197 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9520 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12784 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.418441 keras-core-0.1.3/keras_core/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2274 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.419341 keras-core-0.1.3/keras_core/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      573 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4777 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3153 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9214 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2525 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15831 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7075 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/device_placement.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      643 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.421108 keras-core-0.1.3/keras_core/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1189 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9383 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5064 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      119 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2909 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12720 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10304 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2408 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7377 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25925 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.423013 keras-core-0.1.3/keras_core/src/backend/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1121 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6138 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5144 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       59 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2869 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14371 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10704 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3088 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7683 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      663 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/numpy/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.425043 keras-core-0.1.3/keras_core/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1408 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5000 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3716 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2539 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2612 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19966 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11352 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4920 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2554 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34993 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32643 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.426605 keras-core-0.1.3/keras_core/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1967 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11256 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8599 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      837 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4157 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19426 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24797 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/numpy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.428206 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       84 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1688 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1905 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1499 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      161 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      428 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2069 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1186 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5129 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13627 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/torch_module_wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18935 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.430732 keras-core-0.1.3/keras_core/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      856 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9866 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5277 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3237 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7605 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3467 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2972 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17330 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3140 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5373 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2756 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27243 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      700 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.431052 keras-core-0.1.3/keras_core/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1835 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/constraints/constraints.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.433037 keras-core-0.1.3/keras_core/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      424 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      472 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3314 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3122 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2950 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2955 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7130 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2419 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7255 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.433812 keras-core-0.1.3/keras_core/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4095 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4742 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2587 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23680 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/initializers/random_initializers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.434290 keras-core-0.1.3/keras_core/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8973 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.435464 keras-core-0.1.3/keras_core/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      298 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      838 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3504 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2299 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/activations/softmax.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.436124 keras-core-0.1.3/keras_core/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4359 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11501 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26275 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.439064 keras-core-0.1.3/keras_core/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11882 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10751 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11658 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12685 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5617 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5697 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5721 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5920 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5927 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6024 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6084 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6481 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6533 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.440403 keras-core-0.1.3/keras_core/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5516 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4750 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      512 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4354 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9070 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2680 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1566 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9851 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    56764 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.441906 keras-core-0.1.3/keras_core/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2242 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2306 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8910 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6555 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12921 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2345 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2343 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2298 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2771 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.442780 keras-core-0.1.3/keras_core/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11595 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8915 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9266 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4266 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.445008 keras-core-0.1.3/keras_core/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3396 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4213 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3293 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1533 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2456 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3177 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2510 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2398 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2492 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2626 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3395 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4177 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3272 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.448154 keras-core-0.1.3/keras_core/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6156 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5234 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8807 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28583 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5534 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7922 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21565 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14065 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6466 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3803 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3622 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3365 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5173 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10504 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10662 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4650 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21063 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18964 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2155 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.449513 keras-core-0.1.3/keras_core/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1229 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3010 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2010 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2056 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7361 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.452008 keras-core-0.1.3/keras_core/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2802 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8710 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11123 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1853 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1381 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5701 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4968 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2153 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4698 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5112 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.454878 keras-core-0.1.3/keras_core/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13008 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27285 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8320 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8405 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8313 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26680 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25526 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17379 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17630 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4908 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4848 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.455850 keras-core-0.1.3/keras_core/src/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    71452 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/backend.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8478 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/layers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      544 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.456988 keras-core-0.1.3/keras_core/src/legacy/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    65688 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/preprocessing/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11230 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11177 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.458314 keras-core-0.1.3/keras_core/src/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7312 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/json_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22666 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      491 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/saving_options.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6570 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/saving_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21412 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/legacy/saving/serialization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.459050 keras-core-0.1.3/keras_core/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5787 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5914 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61931 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/losses/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.461117 keras-core-0.1.3/keras_core/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7381 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14709 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61800 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11725 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3084 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26966 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26235 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10449 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6729 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19339 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/metrics/regression_metrics.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.461475 keras-core-0.1.3/keras_core/src/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      769 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/mixed_precision/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6675 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/mixed_precision/dtype_policy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.462700 keras-core-0.1.3/keras_core/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      159 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10792 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26385 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21945 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11700 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/models/sequential.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.464834 keras-core-0.1.3/keras_core/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      666 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18262 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14329 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14950 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13219 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    42223 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5575 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   122621 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9505 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9713 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1686 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.466879 keras-core-0.1.3/keras_core/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2905 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4262 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7231 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3637 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5448 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4684 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3582 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27718 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8554 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5408 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      753 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5422 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/rmsprop.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.467427 keras-core-0.1.3/keras_core/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      577 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34551 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4057 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/optimizers/sgd.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.468262 keras-core-0.1.3/keras_core/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2730 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/random/seed_generator.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.468769 keras-core-0.1.3/keras_core/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1851 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11862 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/regularizers/regularizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.469764 keras-core-0.1.3/keras_core/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      660 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7429 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8364 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20986 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27351 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/saving/serialization_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.470269 keras-core-0.1.3/keras_core/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15426 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1196 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/testing/test_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.470855 keras-core-0.1.3/keras_core/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25404 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/compile_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.472065 keras-core-0.1.3/keras_core/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12464 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7028 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2292 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19550 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3278 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2612 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/data_adapters/torch_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8838 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34980 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/trainers/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.493168 keras-core-0.1.3/keras_core/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1507 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2282 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1750 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23647 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1246 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15848 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/file_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16042 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3545 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15136 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1028 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/module_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1802 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3656 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/nest.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10306 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3823 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4760 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      722 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/shape_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13813 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9093 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4906 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/utils/tracking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       72 2023-07-26 20:30:01.000000 keras-core-0.1.3/keras_core/src/version.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.493350 keras-core-0.1.3/keras_core/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2696 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.493528 keras-core-0.1.3/keras_core/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-07-26 20:30:05.000000 keras-core-0.1.3/keras_core/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-26 20:30:10.397696 keras-core-0.1.3/keras_core.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3822 2023-07-26 20:30:10.000000 keras-core-0.1.3/keras_core.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19960 2023-07-26 20:30:10.000000 keras-core-0.1.3/keras_core.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-26 20:30:10.000000 keras-core-0.1.3/keras_core.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-07-26 20:30:10.000000 keras-core-0.1.3/keras_core.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       11 2023-07-26 20:30:10.000000 keras-core-0.1.3/keras_core.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-07-26 20:30:10.494132 keras-core-0.1.3/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1915 2023-07-26 20:30:01.000000 keras-core-0.1.3/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.646768 keras-core-0.1.4/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3822 2023-08-08 19:08:53.646574 keras-core-0.1.4/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2972 2023-08-08 19:08:40.000000 keras-core-0.1.4/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.524447 keras-core-0.1.4/keras_core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1641 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.525454 keras-core-0.1.4/keras_core/_tf_keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1759 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.525598 keras-core-0.1.4/keras_core/_tf_keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.525755 keras-core-0.1.4/keras_core/_tf_keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.525912 keras-core-0.1.4/keras_core/_tf_keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.526065 keras-core-0.1.4/keras_core/_tf_keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.526215 keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.526360 keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.526518 keras-core-0.1.4/keras_core/_tf_keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.526767 keras-core-0.1.4/keras_core/_tf_keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.527044 keras-core-0.1.4/keras_core/_tf_keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.527270 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.527459 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.527630 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.527792 keras-core-0.1.4/keras_core/_tf_keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.528005 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.528280 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.528473 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.528653 keras-core-0.1.4/keras_core/_tf_keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.528828 keras-core-0.1.4/keras_core/_tf_keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529004 keras-core-0.1.4/keras_core/_tf_keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529183 keras-core-0.1.4/keras_core/_tf_keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7283 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529359 keras-core-0.1.4/keras_core/_tf_keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529530 keras-core-0.1.4/keras_core/_tf_keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529703 keras-core-0.1.4/keras_core/_tf_keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      858 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.529891 keras-core-0.1.4/keras_core/_tf_keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530075 keras-core-0.1.4/keras_core/_tf_keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530244 keras-core-0.1.4/keras_core/_tf_keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530420 keras-core-0.1.4/keras_core/_tf_keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530589 keras-core-0.1.4/keras_core/_tf_keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530754 keras-core-0.1.4/keras_core/_tf_keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.530924 keras-core-0.1.4/keras_core/_tf_keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531083 keras-core-0.1.4/keras_core/_tf_keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531246 keras-core-0.1.4/keras_core/_tf_keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2926 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531403 keras-core-0.1.4/keras_core/_tf_keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10318 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531555 keras-core-0.1.4/keras_core/_tf_keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      160 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531717 keras-core-0.1.4/keras_core/_tf_keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.531894 keras-core-0.1.4/keras_core/_tf_keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3358 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532057 keras-core-0.1.4/keras_core/_tf_keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5556 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532212 keras-core-0.1.4/keras_core/_tf_keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      591 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532374 keras-core-0.1.4/keras_core/_tf_keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532531 keras-core-0.1.4/keras_core/_tf_keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8250 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532698 keras-core-0.1.4/keras_core/_tf_keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      274 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532840 keras-core-0.1.4/keras_core/_tf_keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1292 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.532976 keras-core-0.1.4/keras_core/_tf_keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6032 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533110 keras-core-0.1.4/keras_core/_tf_keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      929 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533247 keras-core-0.1.4/keras_core/_tf_keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533420 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      767 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533631 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1397 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533800 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      530 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.533967 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/text/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      462 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534122 keras-core-0.1.4/keras_core/_tf_keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      558 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534268 keras-core-0.1.4/keras_core/_tf_keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      871 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534404 keras-core-0.1.4/keras_core/_tf_keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534554 keras-core-0.1.4/keras_core/_tf_keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2724 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534709 keras-core-0.1.4/keras_core/_tf_keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/_tf_keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534855 keras-core-0.1.4/keras_core/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.534993 keras-core-0.1.4/keras_core/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535144 keras-core-0.1.4/keras_core/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535287 keras-core-0.1.4/keras_core/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535422 keras-core-0.1.4/keras_core/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535561 keras-core-0.1.4/keras_core/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535696 keras-core-0.1.4/keras_core/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535834 keras-core-0.1.4/keras_core/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.535976 keras-core-0.1.4/keras_core/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536122 keras-core-0.1.4/keras_core/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536271 keras-core-0.1.4/keras_core/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536411 keras-core-0.1.4/keras_core/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536551 keras-core-0.1.4/keras_core/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536696 keras-core-0.1.4/keras_core/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.536854 keras-core-0.1.4/keras_core/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537037 keras-core-0.1.4/keras_core/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537220 keras-core-0.1.4/keras_core/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537394 keras-core-0.1.4/keras_core/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537553 keras-core-0.1.4/keras_core/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537695 keras-core-0.1.4/keras_core/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      743 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.537850 keras-core-0.1.4/keras_core/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.538003 keras-core-0.1.4/keras_core/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.538179 keras-core-0.1.4/keras_core/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      858 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.538350 keras-core-0.1.4/keras_core/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.538518 keras-core-0.1.4/keras_core/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.538689 keras-core-0.1.4/keras_core/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.539061 keras-core-0.1.4/keras_core/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.539316 keras-core-0.1.4/keras_core/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.539544 keras-core-0.1.4/keras_core/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.539763 keras-core-0.1.4/keras_core/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.539967 keras-core-0.1.4/keras_core/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.540178 keras-core-0.1.4/keras_core/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2926 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.540387 keras-core-0.1.4/keras_core/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9976 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.540589 keras-core-0.1.4/keras_core/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      160 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.540783 keras-core-0.1.4/keras_core/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.540974 keras-core-0.1.4/keras_core/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.541159 keras-core-0.1.4/keras_core/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.541340 keras-core-0.1.4/keras_core/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      591 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.541521 keras-core-0.1.4/keras_core/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.541710 keras-core-0.1.4/keras_core/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8250 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.541902 keras-core-0.1.4/keras_core/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      274 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542091 keras-core-0.1.4/keras_core/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1292 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542283 keras-core-0.1.4/keras_core/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6032 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542469 keras-core-0.1.4/keras_core/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      929 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542639 keras-core-0.1.4/keras_core/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542798 keras-core-0.1.4/keras_core/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      462 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.542948 keras-core-0.1.4/keras_core/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      347 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.543090 keras-core-0.1.4/keras_core/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      185 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.543231 keras-core-0.1.4/keras_core/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      558 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.543372 keras-core-0.1.4/keras_core/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      871 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.543653 keras-core-0.1.4/keras_core/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.544492 keras-core-0.1.4/keras_core/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      744 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.545037 keras-core-0.1.4/keras_core/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3483 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11944 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.547943 keras-core-0.1.4/keras_core/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24800 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16679 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25463 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40581 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16018 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14607 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15601 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17253 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18015 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23532 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30652 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19116 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6454 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9197 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9520 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12786 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.548503 keras-core-0.1.4/keras_core/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2274 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.549457 keras-core-0.1.4/keras_core/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      573 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4777 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2786 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9214 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      909 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/name_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2525 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16094 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7075 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/device_placement.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      643 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.550851 keras-core-0.1.4/keras_core/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1189 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9383 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5064 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      119 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3271 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13213 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10672 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2556 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7377 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25925 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.552267 keras-core-0.1.4/keras_core/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1121 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6138 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5144 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       59 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3779 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14371 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11001 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3088 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7683 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10521 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.554882 keras-core-0.1.4/keras_core/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1408 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5000 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3716 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2539 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2990 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19966 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11738 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4920 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2586 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34993 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32833 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.556987 keras-core-0.1.4/keras_core/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1967 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11277 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8599 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      837 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5470 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19426 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25381 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.559002 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       84 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1688 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1905 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1499 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      161 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1794 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      428 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2069 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1186 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5227 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13627 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/torch_module_wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18935 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.563476 keras-core-0.1.4/keras_core/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      856 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9866 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5277 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3237 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7605 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3467 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3021 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17330 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3140 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5373 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2756 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27243 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      700 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.564142 keras-core-0.1.4/keras_core/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1835 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/constraints/constraints.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.565991 keras-core-0.1.4/keras_core/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      424 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      472 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3314 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3122 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2950 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2955 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7130 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2419 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7255 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.566840 keras-core-0.1.4/keras_core/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4095 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4742 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2587 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23680 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/initializers/random_initializers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.567705 keras-core-0.1.4/keras_core/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8973 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.570341 keras-core-0.1.4/keras_core/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      298 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      838 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3504 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2299 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/activations/softmax.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.571273 keras-core-0.1.4/keras_core/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4359 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11501 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26429 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.574785 keras-core-0.1.4/keras_core/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11882 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10751 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11658 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12685 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5617 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5697 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5721 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5920 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5927 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6024 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6084 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6481 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6533 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.576741 keras-core-0.1.4/keras_core/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5572 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4750 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      512 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4354 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9070 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2680 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1566 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9851 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    56877 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.579009 keras-core-0.1.4/keras_core/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2242 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2306 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8918 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6585 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12921 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2345 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2343 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2298 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2771 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.580219 keras-core-0.1.4/keras_core/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11595 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8993 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9266 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4266 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.584217 keras-core-0.1.4/keras_core/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3396 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4213 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3293 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1533 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2456 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3177 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2510 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2398 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2492 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2626 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3395 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4177 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3272 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.590068 keras-core-0.1.4/keras_core/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6156 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5234 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8807 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28583 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5534 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11009 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21565 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14065 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6466 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3803 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6309 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3729 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9595 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10504 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10662 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4650 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21063 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18964 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2155 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.597498 keras-core-0.1.4/keras_core/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1229 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3010 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2010 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2056 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7361 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.604589 keras-core-0.1.4/keras_core/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2802 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8710 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11123 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1853 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1381 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5701 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4968 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2153 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4698 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5112 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.611550 keras-core-0.1.4/keras_core/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13008 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27285 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8320 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8405 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8313 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26680 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25526 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17379 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17630 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4908 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4848 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.614124 keras-core-0.1.4/keras_core/src/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    71452 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/backend.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8478 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/layers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      544 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.617475 keras-core-0.1.4/keras_core/src/legacy/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    65688 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/preprocessing/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11230 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11177 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.621130 keras-core-0.1.4/keras_core/src/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7312 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/json_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22666 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      491 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/saving_options.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6570 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21412 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/legacy/saving/serialization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.622177 keras-core-0.1.4/keras_core/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5787 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5914 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61931 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/losses/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.627418 keras-core-0.1.4/keras_core/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7381 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14709 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61800 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11725 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3084 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26966 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26235 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10449 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6882 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19339 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/metrics/regression_metrics.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.628179 keras-core-0.1.4/keras_core/src/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      769 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/mixed_precision/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6679 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/mixed_precision/dtype_policy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.629937 keras-core-0.1.4/keras_core/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      159 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10792 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26385 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22208 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11700 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/sequential.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/models/variable_mapping.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.632503 keras-core-0.1.4/keras_core/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      666 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18262 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14329 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15066 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15050 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    46575 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5575 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   128350 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9505 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9713 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1686 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.635478 keras-core-0.1.4/keras_core/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2963 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4262 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7231 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3637 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5448 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4684 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3582 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27718 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8554 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4494 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5408 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      753 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5422 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/rmsprop.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.635863 keras-core-0.1.4/keras_core/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      577 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34551 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4057 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/optimizers/sgd.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.636668 keras-core-0.1.4/keras_core/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4944 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/random/seed_generator.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.637086 keras-core-0.1.4/keras_core/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1851 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11862 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/regularizers/regularizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.638118 keras-core-0.1.4/keras_core/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      660 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7429 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8607 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21529 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27381 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/saving/serialization_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.638697 keras-core-0.1.4/keras_core/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15581 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1196 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/testing/test_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.639346 keras-core-0.1.4/keras_core/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25404 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/compile_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.641255 keras-core-0.1.4/keras_core/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12464 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7028 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2292 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19550 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3278 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2612 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/data_adapters/torch_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8838 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34980 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/trainers/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.645936 keras-core-0.1.4/keras_core/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1544 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2282 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14006 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1750 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27748 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1246 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15848 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/file_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14962 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/image_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16635 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3551 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15136 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1167 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1802 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3656 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/nest.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10306 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3823 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4760 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      722 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/shape_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13813 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10376 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/text_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3484 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/tf_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9873 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4906 2023-08-08 19:08:41.000000 keras-core-0.1.4/keras_core/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       72 2023-08-08 19:08:40.000000 keras-core-0.1.4/keras_core/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.646101 keras-core-0.1.4/keras_core/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2724 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.646290 keras-core-0.1.4/keras_core/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2023-08-08 19:08:51.000000 keras-core-0.1.4/keras_core/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-08-08 19:08:53.525307 keras-core-0.1.4/keras_core.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3822 2023-08-08 19:08:53.000000 keras-core-0.1.4/keras_core.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20347 2023-08-08 19:08:53.000000 keras-core-0.1.4/keras_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-08-08 19:08:53.000000 keras-core-0.1.4/keras_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-08-08 19:08:53.000000 keras-core-0.1.4/keras_core.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       11 2023-08-08 19:08:53.000000 keras-core-0.1.4/keras_core.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-08-08 19:08:53.646818 keras-core-0.1.4/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1915 2023-08-08 19:08:40.000000 keras-core-0.1.4/setup.py
```

### Comparing `keras-core-0.1.3/PKG-INFO` & `keras-core-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras-core
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-core-0.1.3/README.md` & `keras-core-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/__init__.py` & `keras-core-0.1.4/keras_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 from keras_core.src.models.sequential import Sequential
 from keras_core.src.ops.function import Function
 from keras_core.src.ops.operation import Operation
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.regularizers.regularizers import Regularizer
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/activations/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/applications/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/applications/convnext/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/applications/efficientnet_v2/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/backend/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/callbacks/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/config/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/constraints/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/initializers/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/layers/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/losses/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/metrics/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/mixed_precision/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/ops/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/ops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras_core.src.ops.core import unstack
 from keras_core.src.ops.core import while_loop
 from keras_core.src.ops.math import fft
 from keras_core.src.ops.math import fft2
 from keras_core.src.ops.math import in_top_k
 from keras_core.src.ops.math import logsumexp
 from keras_core.src.ops.math import qr
+from keras_core.src.ops.math import segment_max
 from keras_core.src.ops.math import segment_sum
 from keras_core.src.ops.math import top_k
 from keras_core.src.ops.nn import average_pool
 from keras_core.src.ops.nn import binary_crossentropy
 from keras_core.src.ops.nn import categorical_crossentropy
 from keras_core.src.ops.nn import conv
 from keras_core.src.ops.nn import conv_transpose
@@ -50,48 +51,51 @@
 from keras_core.src.ops.nn import sigmoid
 from keras_core.src.ops.nn import silu
 from keras_core.src.ops.nn import softmax
 from keras_core.src.ops.nn import softplus
 from keras_core.src.ops.nn import softsign
 from keras_core.src.ops.nn import sparse_categorical_crossentropy
 from keras_core.src.ops.nn import swish
-from keras_core.src.ops.nn import tanh
 from keras_core.src.ops.numpy import abs
 from keras_core.src.ops.numpy import absolute
 from keras_core.src.ops.numpy import add
 from keras_core.src.ops.numpy import all
 from keras_core.src.ops.numpy import amax
 from keras_core.src.ops.numpy import amin
 from keras_core.src.ops.numpy import any
 from keras_core.src.ops.numpy import append
 from keras_core.src.ops.numpy import arange
 from keras_core.src.ops.numpy import arccos
 from keras_core.src.ops.numpy import arcsin
+from keras_core.src.ops.numpy import arcsinh
 from keras_core.src.ops.numpy import arctan
 from keras_core.src.ops.numpy import arctan2
+from keras_core.src.ops.numpy import arctanh
 from keras_core.src.ops.numpy import argmax
 from keras_core.src.ops.numpy import argmin
 from keras_core.src.ops.numpy import argsort
 from keras_core.src.ops.numpy import array
 from keras_core.src.ops.numpy import average
 from keras_core.src.ops.numpy import bincount
 from keras_core.src.ops.numpy import broadcast_to
 from keras_core.src.ops.numpy import ceil
 from keras_core.src.ops.numpy import clip
 from keras_core.src.ops.numpy import concatenate
 from keras_core.src.ops.numpy import conj
 from keras_core.src.ops.numpy import conjugate
 from keras_core.src.ops.numpy import copy
 from keras_core.src.ops.numpy import cos
+from keras_core.src.ops.numpy import cosh
 from keras_core.src.ops.numpy import count_nonzero
 from keras_core.src.ops.numpy import cross
 from keras_core.src.ops.numpy import cumprod
 from keras_core.src.ops.numpy import cumsum
 from keras_core.src.ops.numpy import diag
 from keras_core.src.ops.numpy import diagonal
+from keras_core.src.ops.numpy import digitize
 from keras_core.src.ops.numpy import divide
 from keras_core.src.ops.numpy import dot
 from keras_core.src.ops.numpy import einsum
 from keras_core.src.ops.numpy import empty
 from keras_core.src.ops.numpy import equal
 from keras_core.src.ops.numpy import exp
 from keras_core.src.ops.numpy import expand_dims
@@ -151,28 +155,30 @@
 from keras_core.src.ops.numpy import reciprocal
 from keras_core.src.ops.numpy import repeat
 from keras_core.src.ops.numpy import reshape
 from keras_core.src.ops.numpy import roll
 from keras_core.src.ops.numpy import round
 from keras_core.src.ops.numpy import sign
 from keras_core.src.ops.numpy import sin
+from keras_core.src.ops.numpy import sinh
 from keras_core.src.ops.numpy import size
 from keras_core.src.ops.numpy import sort
 from keras_core.src.ops.numpy import split
 from keras_core.src.ops.numpy import sqrt
 from keras_core.src.ops.numpy import square
 from keras_core.src.ops.numpy import squeeze
 from keras_core.src.ops.numpy import stack
 from keras_core.src.ops.numpy import std
 from keras_core.src.ops.numpy import subtract
 from keras_core.src.ops.numpy import sum
 from keras_core.src.ops.numpy import swapaxes
 from keras_core.src.ops.numpy import take
 from keras_core.src.ops.numpy import take_along_axis
 from keras_core.src.ops.numpy import tan
+from keras_core.src.ops.numpy import tanh
 from keras_core.src.ops.numpy import tensordot
 from keras_core.src.ops.numpy import tile
 from keras_core.src.ops.numpy import trace
 from keras_core.src.ops.numpy import transpose
 from keras_core.src.ops.numpy import tri
 from keras_core.src.ops.numpy import tril
 from keras_core.src.ops.numpy import triu
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/ops/nn/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/ops/nn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,8 +27,7 @@
 from keras_core.src.ops.nn import sigmoid
 from keras_core.src.ops.nn import silu
 from keras_core.src.ops.nn import softmax
 from keras_core.src.ops.nn import softplus
 from keras_core.src.ops.nn import softsign
 from keras_core.src.ops.nn import sparse_categorical_crossentropy
 from keras_core.src.ops.nn import swish
-from keras_core.src.ops.nn import tanh
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/ops/numpy/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 from keras_core.src.ops.numpy import amax
 from keras_core.src.ops.numpy import amin
 from keras_core.src.ops.numpy import any
 from keras_core.src.ops.numpy import append
 from keras_core.src.ops.numpy import arange
 from keras_core.src.ops.numpy import arccos
 from keras_core.src.ops.numpy import arcsin
+from keras_core.src.ops.numpy import arcsinh
 from keras_core.src.ops.numpy import arctan
 from keras_core.src.ops.numpy import arctan2
+from keras_core.src.ops.numpy import arctanh
 from keras_core.src.ops.numpy import argmax
 from keras_core.src.ops.numpy import argmin
 from keras_core.src.ops.numpy import argsort
 from keras_core.src.ops.numpy import array
 from keras_core.src.ops.numpy import average
 from keras_core.src.ops.numpy import bincount
 from keras_core.src.ops.numpy import broadcast_to
 from keras_core.src.ops.numpy import ceil
 from keras_core.src.ops.numpy import clip
 from keras_core.src.ops.numpy import concatenate
 from keras_core.src.ops.numpy import conj
 from keras_core.src.ops.numpy import conjugate
 from keras_core.src.ops.numpy import copy
 from keras_core.src.ops.numpy import cos
+from keras_core.src.ops.numpy import cosh
 from keras_core.src.ops.numpy import count_nonzero
 from keras_core.src.ops.numpy import cross
 from keras_core.src.ops.numpy import cumprod
 from keras_core.src.ops.numpy import cumsum
 from keras_core.src.ops.numpy import diag
 from keras_core.src.ops.numpy import diagonal
+from keras_core.src.ops.numpy import digitize
 from keras_core.src.ops.numpy import divide
 from keras_core.src.ops.numpy import dot
 from keras_core.src.ops.numpy import einsum
 from keras_core.src.ops.numpy import empty
 from keras_core.src.ops.numpy import equal
 from keras_core.src.ops.numpy import exp
 from keras_core.src.ops.numpy import expand_dims
@@ -101,28 +105,30 @@
 from keras_core.src.ops.numpy import reciprocal
 from keras_core.src.ops.numpy import repeat
 from keras_core.src.ops.numpy import reshape
 from keras_core.src.ops.numpy import roll
 from keras_core.src.ops.numpy import round
 from keras_core.src.ops.numpy import sign
 from keras_core.src.ops.numpy import sin
+from keras_core.src.ops.numpy import sinh
 from keras_core.src.ops.numpy import size
 from keras_core.src.ops.numpy import sort
 from keras_core.src.ops.numpy import split
 from keras_core.src.ops.numpy import sqrt
 from keras_core.src.ops.numpy import square
 from keras_core.src.ops.numpy import squeeze
 from keras_core.src.ops.numpy import stack
 from keras_core.src.ops.numpy import std
 from keras_core.src.ops.numpy import subtract
 from keras_core.src.ops.numpy import sum
 from keras_core.src.ops.numpy import swapaxes
 from keras_core.src.ops.numpy import take
 from keras_core.src.ops.numpy import take_along_axis
 from keras_core.src.ops.numpy import tan
+from keras_core.src.ops.numpy import tanh
 from keras_core.src.ops.numpy import tensordot
 from keras_core.src.ops.numpy import tile
 from keras_core.src.ops.numpy import trace
 from keras_core.src.ops.numpy import transpose
 from keras_core.src.ops.numpy import tri
 from keras_core.src.ops.numpy import tril
 from keras_core.src.ops.numpy import triu
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/optimizers/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/optimizers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 from keras_core.src.optimizers.adadelta import Adadelta
 from keras_core.src.optimizers.adafactor import Adafactor
 from keras_core.src.optimizers.adagrad import Adagrad
 from keras_core.src.optimizers.adam import Adam
 from keras_core.src.optimizers.adamax import Adamax
 from keras_core.src.optimizers.adamw import AdamW
 from keras_core.src.optimizers.ftrl import Ftrl
+from keras_core.src.optimizers.lion import Lion
 from keras_core.src.optimizers.nadam import Nadam
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.optimizers.rmsprop import RMSprop
 from keras_core.src.optimizers.sgd import SGD
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/optimizers/schedules/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/preprocessing/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/preprocessing/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
 
 from keras_core._tf_keras.preprocessing import image
 from keras_core._tf_keras.preprocessing import sequence
-from keras_core.src.utils.dataset_utils import image_dataset_from_directory
-from keras_core.src.utils.dataset_utils import text_dataset_from_directory
-from keras_core.src.utils.dataset_utils import timeseries_dataset_from_array
+from keras_core.src.utils.image_dataset_utils import image_dataset_from_directory
+from keras_core.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras_core.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
 
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
```

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/preprocessing/image/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/preprocessing/sequence/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/preprocessing/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/regularizers/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/saving/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/_tf_keras/utils/__init__.py` & `keras-core-0.1.4/keras_core/_tf_keras/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 from keras_core.src.saving.object_registration import register_keras_serializable
 from keras_core.src.saving.serialization_lib import deserialize_keras_object
 from keras_core.src.saving.serialization_lib import serialize_keras_object
 from keras_core.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
 from keras_core.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
 from keras_core.src.trainers.data_adapters.py_dataset_adapter import PyDataset
 from keras_core.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
-from keras_core.src.utils.dataset_utils import audio_dataset_from_directory
-from keras_core.src.utils.dataset_utils import image_dataset_from_directory
+from keras_core.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras_core.src.utils.dataset_utils import split_dataset
-from keras_core.src.utils.dataset_utils import text_dataset_from_directory
-from keras_core.src.utils.dataset_utils import timeseries_dataset_from_array
 from keras_core.src.utils.file_utils import get_file
+from keras_core.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras_core.src.utils.image_utils import array_to_img
 from keras_core.src.utils.image_utils import img_to_array
 from keras_core.src.utils.image_utils import load_img
 from keras_core.src.utils.image_utils import save_img
 from keras_core.src.utils.io_utils import disable_interactive_logging
 from keras_core.src.utils.io_utils import enable_interactive_logging
 from keras_core.src.utils.io_utils import is_interactive_logging_enabled
 from keras_core.src.utils.model_visualization import model_to_dot
 from keras_core.src.utils.model_visualization import plot_model
 from keras_core.src.utils.numerical_utils import normalize
 from keras_core.src.utils.numerical_utils import to_categorical
 from keras_core.src.utils.progbar import Progbar
 from keras_core.src.utils.rng_utils import set_random_seed
 from keras_core.src.utils.sequence_utils import pad_sequences
+from keras_core.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras_core.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
 from keras_core.utils import legacy
```

### Comparing `keras-core-0.1.3/keras_core/activations/__init__.py` & `keras-core-0.1.4/keras_core/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/applications/__init__.py` & `keras-core-0.1.4/keras_core/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/applications/convnext/__init__.py` & `keras-core-0.1.4/keras_core/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/applications/efficientnet/__init__.py` & `keras-core-0.1.4/keras_core/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/applications/efficientnet_v2/__init__.py` & `keras-core-0.1.4/keras_core/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/backend/__init__.py` & `keras-core-0.1.4/keras_core/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/callbacks/__init__.py` & `keras-core-0.1.4/keras_core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/config/__init__.py` & `keras-core-0.1.4/keras_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/constraints/__init__.py` & `keras-core-0.1.4/keras_core/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/initializers/__init__.py` & `keras-core-0.1.4/keras_core/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/layers/__init__.py` & `keras-core-0.1.4/keras_core/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/losses/__init__.py` & `keras-core-0.1.4/keras_core/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/metrics/__init__.py` & `keras-core-0.1.4/keras_core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/mixed_precision/__init__.py` & `keras-core-0.1.4/keras_core/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/ops/__init__.py` & `keras-core-0.1.4/keras_core/ops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras_core.src.ops.core import unstack
 from keras_core.src.ops.core import while_loop
 from keras_core.src.ops.math import fft
 from keras_core.src.ops.math import fft2
 from keras_core.src.ops.math import in_top_k
 from keras_core.src.ops.math import logsumexp
 from keras_core.src.ops.math import qr
+from keras_core.src.ops.math import segment_max
 from keras_core.src.ops.math import segment_sum
 from keras_core.src.ops.math import top_k
 from keras_core.src.ops.nn import average_pool
 from keras_core.src.ops.nn import binary_crossentropy
 from keras_core.src.ops.nn import categorical_crossentropy
 from keras_core.src.ops.nn import conv
 from keras_core.src.ops.nn import conv_transpose
@@ -50,48 +51,51 @@
 from keras_core.src.ops.nn import sigmoid
 from keras_core.src.ops.nn import silu
 from keras_core.src.ops.nn import softmax
 from keras_core.src.ops.nn import softplus
 from keras_core.src.ops.nn import softsign
 from keras_core.src.ops.nn import sparse_categorical_crossentropy
 from keras_core.src.ops.nn import swish
-from keras_core.src.ops.nn import tanh
 from keras_core.src.ops.numpy import abs
 from keras_core.src.ops.numpy import absolute
 from keras_core.src.ops.numpy import add
 from keras_core.src.ops.numpy import all
 from keras_core.src.ops.numpy import amax
 from keras_core.src.ops.numpy import amin
 from keras_core.src.ops.numpy import any
 from keras_core.src.ops.numpy import append
 from keras_core.src.ops.numpy import arange
 from keras_core.src.ops.numpy import arccos
 from keras_core.src.ops.numpy import arcsin
+from keras_core.src.ops.numpy import arcsinh
 from keras_core.src.ops.numpy import arctan
 from keras_core.src.ops.numpy import arctan2
+from keras_core.src.ops.numpy import arctanh
 from keras_core.src.ops.numpy import argmax
 from keras_core.src.ops.numpy import argmin
 from keras_core.src.ops.numpy import argsort
 from keras_core.src.ops.numpy import array
 from keras_core.src.ops.numpy import average
 from keras_core.src.ops.numpy import bincount
 from keras_core.src.ops.numpy import broadcast_to
 from keras_core.src.ops.numpy import ceil
 from keras_core.src.ops.numpy import clip
 from keras_core.src.ops.numpy import concatenate
 from keras_core.src.ops.numpy import conj
 from keras_core.src.ops.numpy import conjugate
 from keras_core.src.ops.numpy import copy
 from keras_core.src.ops.numpy import cos
+from keras_core.src.ops.numpy import cosh
 from keras_core.src.ops.numpy import count_nonzero
 from keras_core.src.ops.numpy import cross
 from keras_core.src.ops.numpy import cumprod
 from keras_core.src.ops.numpy import cumsum
 from keras_core.src.ops.numpy import diag
 from keras_core.src.ops.numpy import diagonal
+from keras_core.src.ops.numpy import digitize
 from keras_core.src.ops.numpy import divide
 from keras_core.src.ops.numpy import dot
 from keras_core.src.ops.numpy import einsum
 from keras_core.src.ops.numpy import empty
 from keras_core.src.ops.numpy import equal
 from keras_core.src.ops.numpy import exp
 from keras_core.src.ops.numpy import expand_dims
@@ -151,28 +155,30 @@
 from keras_core.src.ops.numpy import reciprocal
 from keras_core.src.ops.numpy import repeat
 from keras_core.src.ops.numpy import reshape
 from keras_core.src.ops.numpy import roll
 from keras_core.src.ops.numpy import round
 from keras_core.src.ops.numpy import sign
 from keras_core.src.ops.numpy import sin
+from keras_core.src.ops.numpy import sinh
 from keras_core.src.ops.numpy import size
 from keras_core.src.ops.numpy import sort
 from keras_core.src.ops.numpy import split
 from keras_core.src.ops.numpy import sqrt
 from keras_core.src.ops.numpy import square
 from keras_core.src.ops.numpy import squeeze
 from keras_core.src.ops.numpy import stack
 from keras_core.src.ops.numpy import std
 from keras_core.src.ops.numpy import subtract
 from keras_core.src.ops.numpy import sum
 from keras_core.src.ops.numpy import swapaxes
 from keras_core.src.ops.numpy import take
 from keras_core.src.ops.numpy import take_along_axis
 from keras_core.src.ops.numpy import tan
+from keras_core.src.ops.numpy import tanh
 from keras_core.src.ops.numpy import tensordot
 from keras_core.src.ops.numpy import tile
 from keras_core.src.ops.numpy import trace
 from keras_core.src.ops.numpy import transpose
 from keras_core.src.ops.numpy import tri
 from keras_core.src.ops.numpy import tril
 from keras_core.src.ops.numpy import triu
```

### Comparing `keras-core-0.1.3/keras_core/ops/nn/__init__.py` & `keras-core-0.1.4/keras_core/ops/nn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,8 +27,7 @@
 from keras_core.src.ops.nn import sigmoid
 from keras_core.src.ops.nn import silu
 from keras_core.src.ops.nn import softmax
 from keras_core.src.ops.nn import softplus
 from keras_core.src.ops.nn import softsign
 from keras_core.src.ops.nn import sparse_categorical_crossentropy
 from keras_core.src.ops.nn import swish
-from keras_core.src.ops.nn import tanh
```

### Comparing `keras-core-0.1.3/keras_core/ops/numpy/__init__.py` & `keras-core-0.1.4/keras_core/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 from keras_core.src.ops.numpy import amax
 from keras_core.src.ops.numpy import amin
 from keras_core.src.ops.numpy import any
 from keras_core.src.ops.numpy import append
 from keras_core.src.ops.numpy import arange
 from keras_core.src.ops.numpy import arccos
 from keras_core.src.ops.numpy import arcsin
+from keras_core.src.ops.numpy import arcsinh
 from keras_core.src.ops.numpy import arctan
 from keras_core.src.ops.numpy import arctan2
+from keras_core.src.ops.numpy import arctanh
 from keras_core.src.ops.numpy import argmax
 from keras_core.src.ops.numpy import argmin
 from keras_core.src.ops.numpy import argsort
 from keras_core.src.ops.numpy import array
 from keras_core.src.ops.numpy import average
 from keras_core.src.ops.numpy import bincount
 from keras_core.src.ops.numpy import broadcast_to
 from keras_core.src.ops.numpy import ceil
 from keras_core.src.ops.numpy import clip
 from keras_core.src.ops.numpy import concatenate
 from keras_core.src.ops.numpy import conj
 from keras_core.src.ops.numpy import conjugate
 from keras_core.src.ops.numpy import copy
 from keras_core.src.ops.numpy import cos
+from keras_core.src.ops.numpy import cosh
 from keras_core.src.ops.numpy import count_nonzero
 from keras_core.src.ops.numpy import cross
 from keras_core.src.ops.numpy import cumprod
 from keras_core.src.ops.numpy import cumsum
 from keras_core.src.ops.numpy import diag
 from keras_core.src.ops.numpy import diagonal
+from keras_core.src.ops.numpy import digitize
 from keras_core.src.ops.numpy import divide
 from keras_core.src.ops.numpy import dot
 from keras_core.src.ops.numpy import einsum
 from keras_core.src.ops.numpy import empty
 from keras_core.src.ops.numpy import equal
 from keras_core.src.ops.numpy import exp
 from keras_core.src.ops.numpy import expand_dims
@@ -101,28 +105,30 @@
 from keras_core.src.ops.numpy import reciprocal
 from keras_core.src.ops.numpy import repeat
 from keras_core.src.ops.numpy import reshape
 from keras_core.src.ops.numpy import roll
 from keras_core.src.ops.numpy import round
 from keras_core.src.ops.numpy import sign
 from keras_core.src.ops.numpy import sin
+from keras_core.src.ops.numpy import sinh
 from keras_core.src.ops.numpy import size
 from keras_core.src.ops.numpy import sort
 from keras_core.src.ops.numpy import split
 from keras_core.src.ops.numpy import sqrt
 from keras_core.src.ops.numpy import square
 from keras_core.src.ops.numpy import squeeze
 from keras_core.src.ops.numpy import stack
 from keras_core.src.ops.numpy import std
 from keras_core.src.ops.numpy import subtract
 from keras_core.src.ops.numpy import sum
 from keras_core.src.ops.numpy import swapaxes
 from keras_core.src.ops.numpy import take
 from keras_core.src.ops.numpy import take_along_axis
 from keras_core.src.ops.numpy import tan
+from keras_core.src.ops.numpy import tanh
 from keras_core.src.ops.numpy import tensordot
 from keras_core.src.ops.numpy import tile
 from keras_core.src.ops.numpy import trace
 from keras_core.src.ops.numpy import transpose
 from keras_core.src.ops.numpy import tri
 from keras_core.src.ops.numpy import tril
 from keras_core.src.ops.numpy import triu
```

### Comparing `keras-core-0.1.3/keras_core/optimizers/__init__.py` & `keras-core-0.1.4/keras_core/optimizers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 from keras_core.src.optimizers.adadelta import Adadelta
 from keras_core.src.optimizers.adafactor import Adafactor
 from keras_core.src.optimizers.adagrad import Adagrad
 from keras_core.src.optimizers.adam import Adam
 from keras_core.src.optimizers.adamax import Adamax
 from keras_core.src.optimizers.adamw import AdamW
 from keras_core.src.optimizers.ftrl import Ftrl
+from keras_core.src.optimizers.lion import Lion
 from keras_core.src.optimizers.nadam import Nadam
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.optimizers.rmsprop import RMSprop
 from keras_core.src.optimizers.sgd import SGD
```

### Comparing `keras-core-0.1.3/keras_core/optimizers/schedules/__init__.py` & `keras-core-0.1.4/keras_core/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/regularizers/__init__.py` & `keras-core-0.1.4/keras_core/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/saving/__init__.py` & `keras-core-0.1.4/keras_core/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/__init__.py` & `keras-core-0.1.4/keras_core/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/activations/__init__.py` & `keras-core-0.1.4/keras_core/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/activations/activations.py` & `keras-core-0.1.4/keras_core/src/activations/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,12 +425,12 @@
     """Log-Softmax activation function.
 
     Each input vector is handled independently.
     The `axis` argument sets which axis of the input the function
     is applied along.
 
     Args:
-        x : Input tensor.
+        x: Input tensor.
         axis: Integer, axis along which the softmax is applied.
     """
     return ops.log_softmax(x, axis=axis)
```

### Comparing `keras-core-0.1.3/keras_core/src/api_export.py` & `keras-core-0.1.4/keras_core/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/convnext.py` & `keras-core-0.1.4/keras_core/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/densenet.py` & `keras-core-0.1.4/keras_core/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/efficientnet.py` & `keras-core-0.1.4/keras_core/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/efficientnet_v2.py` & `keras-core-0.1.4/keras_core/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/imagenet_utils.py` & `keras-core-0.1.4/keras_core/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/inception_resnet_v2.py` & `keras-core-0.1.4/keras_core/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/inception_v3.py` & `keras-core-0.1.4/keras_core/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/mobilenet.py` & `keras-core-0.1.4/keras_core/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/mobilenet_v2.py` & `keras-core-0.1.4/keras_core/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/mobilenet_v3.py` & `keras-core-0.1.4/keras_core/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/nasnet.py` & `keras-core-0.1.4/keras_core/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/resnet.py` & `keras-core-0.1.4/keras_core/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/resnet_v2.py` & `keras-core-0.1.4/keras_core/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/vgg16.py` & `keras-core-0.1.4/keras_core/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/vgg19.py` & `keras-core-0.1.4/keras_core/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/applications/xception.py` & `keras-core-0.1.4/keras_core/src/applications/xception.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     For transfer learning use cases, make sure to read the
     [guide to transfer learning & fine-tuning](
       https://keras.io/guides/transfer_learning/).
 
     The default input image size for this model is 299x299.
 
     Note: each Keras Application expects a specific kind of input preprocessing.
-    For Xception, call `tf.keras.applications.xception.preprocess_input` on your
-    inputs before passing them to the model.
+    For Xception, call `keras_core.applications.xception.preprocess_input`
+    on your inputs before passing them to the model.
     `xception.preprocess_input` will scale input pixels between -1 and 1.
 
     Args:
         include_top: whether to include the 3 fully-connected
             layers at the top of the network.
         weights: one of `None` (random initialization),
             `"imagenet"` (pre-training on ImageNet),
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/backend_utils.py` & `keras-core-0.1.4/keras_core/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/global_state.py` & `keras-core-0.1.4/keras_core/src/backend/common/global_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,27 +16,14 @@
     if attr is None and default is not None:
         attr = default
         if set_to_default:
             set_global_attribute(name, attr)
     return attr
 
 
-def set_global_setting(name, value):
-    setattr(GLOBAL_SETTINGS_TRACKER, name, value)
-
-
-def get_global_setting(name, default=None, set_to_default=False):
-    attr = getattr(GLOBAL_SETTINGS_TRACKER, name, None)
-    if attr is None and default is not None:
-        attr = default
-        if set_to_default:
-            set_global_setting(name, attr)
-    return attr
-
-
 @keras_core_export(
     ["keras_core.utils.clear_session", "keras_core.backend.clear_session"]
 )
 def clear_session():
     """Resets all state generated by Keras.
 
     Keras manages a global state, which it uses to implement the Functional
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/keras_tensor.py` & `keras-core-0.1.4/keras_core/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/stateless_scope.py` & `keras-core-0.1.4/keras_core/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/common/variables.py` & `keras-core-0.1.4/keras_core/src/backend/common/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from keras_core.src.utils.naming import auto_name
 
 
 class KerasVariable:
     def __init__(
         self, initializer, shape=None, dtype=None, trainable=True, name=None
     ):
-        self.name = name or auto_name(self.__class__.__name__)
+        name = name or auto_name(self.__class__.__name__)
+        if not isinstance(name, str) or "/" in name:
+            raise ValueError(
+                "Argument `name` must be a string and "
+                "cannot contain character `/`. "
+                f"Received: name={name}"
+            )
+        self.name = name
         dtype = standardize_dtype(dtype)
         self._dtype = dtype
         self._shape = None
         self._initializer = None
         self.trainable = trainable
         if callable(initializer):
             if shape is None:
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/config.py` & `keras-core-0.1.4/keras_core/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/exports.py` & `keras-core-0.1.4/keras_core/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/core.py` & `keras-core-0.1.4/keras_core/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/image.py` & `keras-core-0.1.4/keras_core/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/math.py` & `keras-core-0.1.4/keras_core/src/backend/jax/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,25 @@
             "Received: num_segments=None"
         )
     return jax.ops.segment_sum(
         data, segment_ids, num_segments, indices_are_sorted=sorted
     )
 
 
+def segment_max(data, segment_ids, num_segments=None, sorted=False):
+    if num_segments is None:
+        raise ValueError(
+            "Argument `num_segments` must be set when using the JAX backend. "
+            "Received: num_segments=None"
+        )
+    return jax.ops.segment_max(
+        data, segment_ids, num_segments, indices_are_sorted=sorted
+    )
+
+
 def top_k(x, k, sorted=True):
     # Jax does not supported `sorted`, but in the case where `sorted=False`,
     # order is not guaranteed, so OK to return sorted output.
     return jax.lax.top_k(x, k)
 
 
 def in_top_k(targets, predictions, k):
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/nn.py` & `keras-core-0.1.4/keras_core/src/backend/jax/nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,74 +10,90 @@
 )
 from keras_core.src.backend.config import epsilon
 from keras_core.src.backend.jax.core import cast
 from keras_core.src.backend.jax.core import convert_to_tensor
 
 
 def relu(x):
+    x = convert_to_tensor(x)
     return jnn.relu(x)
 
 
 def relu6(x):
+    x = convert_to_tensor(x)
     return jnn.relu6(x)
 
 
 def sigmoid(x):
+    x = convert_to_tensor(x)
     return jnn.sigmoid(x)
 
 
 def tanh(x):
+    x = convert_to_tensor(x)
     return jnn.tanh(x)
 
 
 def softplus(x):
+    x = convert_to_tensor(x)
     return jnn.softplus(x)
 
 
 def softsign(x):
+    x = convert_to_tensor(x)
     return jnn.soft_sign(x)
 
 
 def silu(x):
+    x = convert_to_tensor(x)
     return jnn.silu(x)
 
 
 def swish(x):
+    x = convert_to_tensor(x)
     return jnn.swish(x)
 
 
 def log_sigmoid(x):
+    x = convert_to_tensor(x)
     return jnn.log_sigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
+    x = convert_to_tensor(x)
     return jnn.leaky_relu(x, negative_slope=negative_slope)
 
 
 def hard_sigmoid(x):
+    x = convert_to_tensor(x)
     return jnn.hard_sigmoid(x)
 
 
 def elu(x, alpha=1.0):
+    x = convert_to_tensor(x)
     return jnn.elu(x, alpha=alpha)
 
 
 def selu(x):
+    x = convert_to_tensor(x)
     return jnn.selu(x)
 
 
 def gelu(x, approximate=True):
+    x = convert_to_tensor(x)
     return jnn.gelu(x, approximate)
 
 
 def softmax(x, axis=None):
+    x = convert_to_tensor(x)
     return jnn.softmax(x, axis=axis)
 
 
 def log_softmax(x, axis=-1):
+    x = convert_to_tensor(x)
     return jnn.log_softmax(x, axis=axis)
 
 
 def _convert_to_spatial_operand(
     x,
     num_spatial_dims,
     data_format="channels_last",
@@ -385,14 +401,15 @@
         rhs_dilation=dilation_rate,
         dimension_numbers=dimension_numbers,
         transpose_kernel=True,
     )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32"):
+    x = convert_to_tensor(x)
     return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32"):
     reduction_axis = 1 if len(x.shape) > 1 else 0
     outputs = jnp.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/numpy.py` & `keras-core-0.1.4/keras_core/src/backend/jax/numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,26 +103,38 @@
     return jnp.arange(start, stop, step=step, dtype=dtype)
 
 
 def arccos(x):
     return jnp.arccos(x)
 
 
+def arccosh(x):
+    return jnp.arccosh(x)
+
+
 def arcsin(x):
     return jnp.arcsin(x)
 
 
+def arcsinh(x):
+    return jnp.arcsinh(x)
+
+
 def arctan(x):
     return jnp.arctan(x)
 
 
 def arctan2(x1, x2):
     return jnp.arctan2(x1, x2)
 
 
+def arctanh(x):
+    return jnp.arctanh(x)
+
+
 def argmax(x, axis=None):
     return jnp.argmax(x, axis=axis)
 
 
 def argmin(x, axis=None):
     return jnp.argmin(x, axis=axis)
 
@@ -167,14 +179,18 @@
     return jnp.copy(x)
 
 
 def cos(x):
     return jnp.cos(x)
 
 
+def cosh(x):
+    return jnp.cosh(x)
+
+
 def count_nonzero(x, axis=None):
     return jnp.count_nonzero(x, axis=axis)
 
 
 def cross(x1, x2, axisa=-1, axisb=-1, axisc=-1, axis=None):
     return jnp.cross(
         x1,
@@ -203,14 +219,20 @@
         x,
         offset=offset,
         axis1=axis1,
         axis2=axis2,
     )
 
 
+def digitize(x, bins):
+    x = convert_to_tensor(x)
+    bins = convert_to_tensor(bins)
+    return jnp.digitize(x, bins)
+
+
 def dot(x, y):
     return jnp.dot(x, y)
 
 
 def empty(shape, dtype="float32"):
     return jnp.empty(shape, dtype=dtype)
 
@@ -437,14 +459,18 @@
     return jnp.sign(x)
 
 
 def sin(x):
     return jnp.sin(x)
 
 
+def sinh(x):
+    return jnp.sinh(x)
+
+
 def size(x):
     return jnp.size(x)
 
 
 def sort(x, axis=-1):
     return jnp.sort(x, axis=axis)
 
@@ -475,14 +501,18 @@
     return jnp.take_along_axis(x, indices, axis=axis)
 
 
 def tan(x):
     return jnp.tan(x)
 
 
+def tanh(x):
+    return jnp.tanh(x)
+
+
 def tensordot(x1, x2, axes=2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.tensordot(x1, x2, axes=axes)
 
 
 def round(x, decimals=0):
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/random.py` & `keras-core-0.1.4/keras_core/src/backend/jax/random.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,50 +2,57 @@
 
 from keras_core.src.backend.config import floatx
 from keras_core.src.random.seed_generator import SeedGenerator
 from keras_core.src.random.seed_generator import draw_seed
 from keras_core.src.random.seed_generator import make_default_seed
 
 
+def jax_draw_seed(seed):
+    if isinstance(seed, jax.Array):
+        return seed
+    else:
+        return draw_seed(seed)
+
+
 def normal(shape, mean=0.0, stddev=1.0, dtype=None, seed=None):
     dtype = dtype or floatx()
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     sample = jax.random.normal(seed, shape=shape, dtype=dtype)
     return sample * stddev + mean
 
 
 def uniform(shape, minval=0.0, maxval=1.0, dtype=None, seed=None):
     dtype = dtype or floatx()
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     return jax.random.uniform(
         seed, shape=shape, dtype=dtype, minval=minval, maxval=maxval
     )
 
 
 def categorical(logits, num_samples, dtype="int32", seed=None):
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     output_shape = list(logits.shape)
     output_shape[1] = num_samples
     output_shape = tuple(output_shape)
     output = jax.random.categorical(
         seed, logits[..., None], shape=output_shape, axis=1
     )
     return output.astype(dtype)
 
 
 def randint(shape, minval, maxval, dtype="int32", seed=None):
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     return jax.random.randint(
         seed, shape=shape, dtype=dtype, minval=minval, maxval=maxval
     )
 
 
 def truncated_normal(shape, mean=0.0, stddev=1.0, dtype=None, seed=None):
     dtype = dtype or floatx()
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     sample = jax.random.truncated_normal(
         seed, shape=shape, lower=-2.0, upper=2.0, dtype=dtype
     )
     return sample * stddev + mean
 
 
 def _get_concrete_noise_shape(inputs, noise_shape):
@@ -58,15 +65,15 @@
         concrete_noise_shape.append(
             concrete_inputs_shape[i] if value is None else value
         )
     return concrete_noise_shape
 
 
 def dropout(inputs, rate, noise_shape=None, seed=None):
-    seed = draw_seed(seed)
+    seed = jax_draw_seed(seed)
     keep_prob = 1.0 - rate
     # The `noise_shape` may contain `None` so we need to convert it
     # into a concrete shape before passing it on to jax.
     noise_shape = _get_concrete_noise_shape(inputs, noise_shape)
     mask = jax.random.bernoulli(seed, p=keep_prob, shape=noise_shape)
     mask = jax.numpy.broadcast_to(mask, inputs.shape)
     return jax.lax.select(
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/rnn.py` & `keras-core-0.1.4/keras_core/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/jax/trainer.py` & `keras-core-0.1.4/keras_core/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/core.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/image.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/nn.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/numpy.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,26 +80,38 @@
     return np.arange(start, stop, step=step, dtype=dtype)
 
 
 def arccos(x):
     return np.arccos(x)
 
 
+def arccosh(x):
+    return np.arccosh(x)
+
+
 def arcsin(x):
     return np.arcsin(x)
 
 
+def arcsinh(x):
+    return np.arcsinh(x)
+
+
 def arctan(x):
     return np.arctan(x)
 
 
 def arctan2(x1, x2):
     return np.arctan2(x1, x2)
 
 
+def arctanh(x):
+    return np.arctanh(x)
+
+
 def argmax(x, axis=None):
     axis = tuple(axis) if isinstance(axis, list) else axis
     return np.argmax(x, axis=axis)
 
 
 def argmin(x, axis=None):
     axis = tuple(axis) if isinstance(axis, list) else axis
@@ -153,14 +165,18 @@
     return np.copy(x)
 
 
 def cos(x):
     return np.cos(x)
 
 
+def cosh(x):
+    return np.cosh(x)
+
+
 def count_nonzero(x, axis=None):
     axis = tuple(axis) if isinstance(axis, list) else axis
     return np.count_nonzero(x, axis=axis)
 
 
 def cross(x1, x2, axisa=-1, axisb=-1, axisc=-1, axis=None):
     axis = tuple(axis) if isinstance(axis, list) else axis
@@ -195,14 +211,18 @@
         x,
         offset=offset,
         axis1=axis1,
         axis2=axis2,
     )
 
 
+def digitize(x, bins):
+    return np.digitize(x, bins)
+
+
 def dot(x, y):
     return np.dot(x, y)
 
 
 def empty(shape, dtype="float32"):
     return np.empty(shape, dtype=dtype)
 
@@ -434,14 +454,18 @@
     return np.sign(x)
 
 
 def sin(x):
     return np.sin(x)
 
 
+def sinh(x):
+    return np.sinh(x)
+
+
 def size(x):
     return np.size(x)
 
 
 def sort(x, axis=-1):
     axis = tuple(axis) if isinstance(axis, list) else axis
     return np.sort(x, axis=axis)
@@ -476,14 +500,18 @@
     return np.take_along_axis(x, indices, axis=axis)
 
 
 def tan(x):
     return np.tan(x)
 
 
+def tanh(x):
+    return np.tanh(x)
+
+
 def tensordot(x1, x2, axes=2):
     axes = tuple(axes) if isinstance(axes, list) else axes
     return np.tensordot(x1, x2, axes=axes)
 
 
 def round(x, decimals=0):
     return np.round(x, decimals=decimals)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/random.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/numpy/rnn.py` & `keras-core-0.1.4/keras_core/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/core.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/image.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/layer.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/math.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/math.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,24 @@
     else:
         if num_segments is None:
             unique_segment_ids, _ = tf.unique(segment_ids)
             num_segments = tf.shape(unique_segment_ids)[0]
         return tf.math.unsorted_segment_sum(data, segment_ids, num_segments)
 
 
+def segment_max(data, segment_ids, num_segments=None, sorted=False):
+    if sorted:
+        return tf.math.segment_max(data, segment_ids)
+    else:
+        if num_segments is None:
+            unique_segment_ids, _ = tf.unique(segment_ids)
+            num_segments = tf.shape(unique_segment_ids)[0]
+        return tf.math.unsorted_segment_max(data, segment_ids, num_segments)
+
+
 def top_k(x, k, sorted=True):
     return tf.math.top_k(x, k, sorted=sorted)
 
 
 def in_top_k(targets, predictions, k):
     return tf.math.in_top_k(targets, predictions, k)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/nn.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/numpy.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,26 +101,38 @@
     return tf.range(start, stop, delta=step, dtype=dtype)
 
 
 def arccos(x):
     return tfnp.arccos(x)
 
 
+def arccosh(x):
+    return tfnp.arccosh(x)
+
+
 def arcsin(x):
     return tfnp.arcsin(x)
 
 
+def arcsinh(x):
+    return tfnp.arcsinh(x)
+
+
 def arctan(x):
     return tfnp.arctan(x)
 
 
 def arctan2(x1, x2):
     return tfnp.arctan2(x1, x2)
 
 
+def arctanh(x):
+    return tfnp.arctanh(x)
+
+
 def argmax(x, axis=None):
     return tfnp.argmax(x, axis=axis)
 
 
 def argmin(x, axis=None):
     return tfnp.argmin(x, axis=axis)
 
@@ -170,14 +182,18 @@
     return tfnp.copy(x)
 
 
 def cos(x):
     return tfnp.cos(x)
 
 
+def cosh(x):
+    return tfnp.cosh(x)
+
+
 def count_nonzero(x, axis=None):
     return tfnp.count_nonzero(x, axis=axis)
 
 
 def cross(x1, x2, axisa=-1, axisb=-1, axisc=-1, axis=None):
     return tfnp.cross(
         x1,
@@ -206,14 +222,20 @@
         x,
         offset=offset,
         axis1=axis1,
         axis2=axis2,
     )
 
 
+def digitize(x, bins):
+    x = convert_to_tensor(x)
+    bins = list(bins)
+    return tf.raw_ops.Bucketize(input=x, boundaries=bins)
+
+
 def dot(x, y):
     return tfnp.dot(x, y)
 
 
 def empty(shape, dtype="float32"):
     return tfnp.empty(shape, dtype=dtype)
 
@@ -468,14 +490,18 @@
     return tfnp.sign(x)
 
 
 def sin(x):
     return tfnp.sin(x)
 
 
+def sinh(x):
+    return tfnp.sinh(x)
+
+
 def size(x):
     return tfnp.size(x)
 
 
 def sort(x, axis=-1):
     return tfnp.sort(x, axis=axis)
 
@@ -504,14 +530,18 @@
     return tfnp.take_along_axis(x, indices, axis=axis)
 
 
 def tan(x):
     return tfnp.tan(x)
 
 
+def tanh(x):
+    return tfnp.tanh(x)
+
+
 def tensordot(x1, x2, axes=2):
     return tfnp.tensordot(x1, x2, axes=axes)
 
 
 def round(x, decimals=0):
     return tfnp.round(x, decimals=decimals)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/optimizer.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/random.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/random.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 
 def uniform(shape, minval=0.0, maxval=1.0, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
     return tf.random.stateless_uniform(
         shape=shape,
-        minval=minval,
-        maxval=maxval,
+        minval=tf.cast(minval, dtype),
+        maxval=tf.cast(maxval, dtype),
         dtype=dtype,
         seed=seed,
     )
 
 
 def categorical(logits, num_samples, dtype="int64", seed=None):
     seed = tf_draw_seed(seed)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/rnn.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/tensorflow/trainer.py` & `keras-core-0.1.4/keras_core/src/backend/tensorflow/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,15 @@
                 if getattr(self, "_eval_epoch_iterator", None) is None:
                     self._eval_epoch_iterator = TFEpochIterator(
                         x=val_x,
                         y=val_y,
                         sample_weight=val_sample_weight,
                         batch_size=validation_batch_size or batch_size,
                         distribute_strategy=self.distribute_strategy,
+                        steps_per_execution=self.steps_per_execution,
                     )
                 val_logs = self.evaluate(
                     x=val_x,
                     y=val_y,
                     sample_weight=val_sample_weight,
                     batch_size=validation_batch_size or batch_size,
                     steps=validation_steps,
@@ -397,14 +398,15 @@
                 x=x,
                 y=y,
                 sample_weight=sample_weight,
                 batch_size=batch_size,
                 steps_per_epoch=steps,
                 shuffle=False,
                 distribute_strategy=self.distribute_strategy,
+                steps_per_execution=self.steps_per_execution,
             )
 
         # Container that configures and calls callbacks.
         if not isinstance(callbacks, callbacks_module.CallbackList):
             callbacks = callbacks_module.CallbackList(
                 callbacks,
                 add_history=True,
@@ -438,14 +440,15 @@
         # Create an iterator that yields batches of input data.
         epoch_iterator = TFEpochIterator(
             x=x,
             batch_size=batch_size,
             steps_per_epoch=steps,
             shuffle=False,
             distribute_strategy=self.distribute_strategy,
+            steps_per_execution=self.steps_per_execution,
         )
 
         # Container that configures and calls callbacks.
         if not isinstance(callbacks, callbacks_module.CallbackList):
             callbacks = callbacks_module.CallbackList(
                 callbacks,
                 add_history=True,
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/__init__.py` & `keras-core-0.1.4/keras_core/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/core.py` & `keras-core-0.1.4/keras_core/src/backend/torch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,18 @@
     device = global_state.get_global_attribute("torch_device", None)
     if device is None:
         return DEFAULT_DEVICE
     return device
 
 
 def to_torch_dtype(dtype):
-    dtype = standardize_dtype(dtype)
-    dtype = TORCH_DTYPES.get(dtype, None)
-    if dtype is None:
+    standardized_dtype = TORCH_DTYPES.get(standardize_dtype(dtype), None)
+    if standardized_dtype is None:
         raise ValueError(f"Unsupported dtype for PyTorch: {dtype}")
-    return dtype
+    return standardized_dtype
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         self._value = torch.nn.Parameter(
             convert_to_tensor(value, dtype=self._dtype),
             requires_grad=self.trainable,
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/image.py` & `keras-core-0.1.4/keras_core/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/layer.py` & `keras-core-0.1.4/keras_core/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/math.py` & `keras-core-0.1.4/keras_core/src/backend/torch/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,52 @@
 
     # Removing the extra dimension.
     result = result[:-1, ...]
 
     return result.type(data.dtype)
 
 
+def segment_max(data, segment_ids, num_segments=None, **kwargs):
+    data = convert_to_tensor(data)
+    segment_ids = convert_to_tensor(segment_ids)
+    num_repeats = torch.prod(
+        torch.tensor(data.shape[1:], device=get_device())
+    ).long()
+    # To use `scatter_reduce` in torch, we need to replicate `segment_ids` into
+    # the shape of `data`.
+    segment_ids = (
+        segment_ids.repeat_interleave(num_repeats)
+        .view(*data.shape)
+        .type(torch.int64)
+    )
+    num_segments = num_segments or len(torch.unique(segment_ids))
+
+    # .scatter_reduce does not support -1 in the indices.
+    # Add all out-of-bound indices value to an extra dimension after
+    # num_segments, which is removed before returning the result.
+
+    # Replacing the out-of-bound indices.
+    segment_ids = torch.where(segment_ids >= 0, segment_ids, num_segments)
+    segment_ids = torch.where(
+        segment_ids < num_segments, segment_ids, num_segments
+    )
+
+    # Add one more dimension to the result shape with the "+1".
+    shape = (num_segments + 1,) + tuple(data.shape[1:])
+
+    result = torch.zeros(*shape, device=get_device()).scatter_reduce(
+        0, segment_ids, data.float(), "amax"
+    )
+
+    # Removing the extra dimension.
+    result = result[:-1, ...]
+
+    return result.type(data.dtype)
+
+
 def top_k(x, k, sorted=True):
     x = convert_to_tensor(x)
     return torch.topk(x, k, sorted=sorted)
 
 
 def in_top_k(targets, predictions, k):
     targets = convert_to_tensor(targets).type(torch.int64)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/nn.py` & `keras-core-0.1.4/keras_core/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/numpy.py` & `keras-core-0.1.4/keras_core/src/backend/torch/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,29 +169,44 @@
 
 
 def arccos(x):
     x = convert_to_tensor(x)
     return torch.arccos(x)
 
 
+def arccosh(x):
+    x = convert_to_tensor(x)
+    return torch.arccosh(x)
+
+
 def arcsin(x):
     x = convert_to_tensor(x)
     return torch.arcsin(x)
 
 
+def arcsinh(x):
+    x = convert_to_tensor(x)
+    return torch.arcsinh(x)
+
+
 def arctan(x):
     x = convert_to_tensor(x)
     return torch.arctan(x)
 
 
 def arctan2(x1, x2):
     x1, x2 = convert_to_tensor(x1), convert_to_tensor(x2)
     return torch.arctan2(x1, x2)
 
 
+def arctanh(x):
+    x = convert_to_tensor(x)
+    return torch.arctanh(x)
+
+
 def argmax(x, axis=None):
     x = convert_to_tensor(x)
     return torch.argmax(x, dim=axis)
 
 
 def argmin(x, axis=None):
     x = convert_to_tensor(x)
@@ -273,14 +288,19 @@
 
 
 def cos(x):
     x = convert_to_tensor(x)
     return torch.cos(x)
 
 
+def cosh(x):
+    x = convert_to_tensor(x)
+    return torch.cosh(x)
+
+
 def count_nonzero(x, axis=None):
     x = convert_to_tensor(x)
     if axis == () or axis == []:
         # Torch handles the empty axis case differently from numpy.
         return cast(torch.ne(x, 0), "int32")
     return torch.count_nonzero(x, dim=axis).T
 
@@ -323,14 +343,20 @@
         x,
         offset=offset,
         dim1=axis1,
         dim2=axis2,
     )
 
 
+def digitize(x, bins):
+    x = convert_to_tensor(x)
+    bins = convert_to_tensor(bins)
+    return cast(torch.bucketize(x, bins, right=True), "int32")
+
+
 def dot(x, y):
     x, y = convert_to_tensor(x), convert_to_tensor(y)
     if x.ndim == 0 or y.ndim == 0:
         return torch.multiply(x, y)
     return torch.matmul(x, y)
 
 
@@ -725,14 +751,19 @@
 
 
 def sin(x):
     x = convert_to_tensor(x)
     return torch.sin(x)
 
 
+def sinh(x):
+    x = convert_to_tensor(x)
+    return torch.sinh(x)
+
+
 def size(x):
     x_shape = convert_to_tensor(tuple(x.shape))
     return torch.prod(x_shape)
 
 
 def sort(x, axis=-1):
     x = convert_to_tensor(x)
@@ -802,14 +833,19 @@
 
 
 def tan(x):
     x = convert_to_tensor(x)
     return torch.tan(x)
 
 
+def tanh(x):
+    x = convert_to_tensor(x)
+    return torch.tanh(x)
+
+
 def tensordot(x1, x2, axes=2):
     x1, x2 = convert_to_tensor(x1), convert_to_tensor(x2)
     # Conversion to long necessary for `torch.tensordot`
     x1 = cast(x1, "int64") if x1.dtype in TORCH_INT_TYPES else x1
     x2 = cast(x2, "int64") if x2.dtype in TORCH_INT_TYPES else x2
     return torch.tensordot(x1, x2, dims=axes)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adadelta.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adagrad.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adam.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_adamax.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_nadam.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_optimizer.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,26 @@
     def __new__(cls, *args, **kwargs):
         # Import locally to avoid circular imports.
         from keras_core.src.backend.torch.optimizers import torch_adadelta
         from keras_core.src.backend.torch.optimizers import torch_adagrad
         from keras_core.src.backend.torch.optimizers import torch_adam
         from keras_core.src.backend.torch.optimizers import torch_adamax
         from keras_core.src.backend.torch.optimizers import torch_adamw
+        from keras_core.src.backend.torch.optimizers import torch_lion
         from keras_core.src.backend.torch.optimizers import torch_nadam
         from keras_core.src.backend.torch.optimizers import torch_rmsprop
         from keras_core.src.backend.torch.optimizers import torch_sgd
 
         OPTIMIZERS = {
             optimizers.Adadelta: torch_adadelta.Adadelta,
             optimizers.Adagrad: torch_adagrad.Adagrad,
             optimizers.Adam: torch_adam.Adam,
             optimizers.Adamax: torch_adamax.Adamax,
             optimizers.AdamW: torch_adamw.AdamW,
+            optimizers.Lion: torch_lion.Lion,
             optimizers.Nadam: torch_nadam.Nadam,
             optimizers.RMSprop: torch_rmsprop.RMSprop,
             optimizers.SGD: torch_sgd.SGD,
         }
 
         if cls in OPTIMIZERS:
             return OPTIMIZERS[cls](*args, **kwargs)
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/optimizers/torch_sgd.py` & `keras-core-0.1.4/keras_core/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/random.py` & `keras-core-0.1.4/keras_core/src/backend/torch/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,30 @@
         generator=generator,
     ).type(dtype)
 
 
 def uniform(shape, minval=0.0, maxval=1.0, dtype=None, seed=None):
     dtype = dtype or floatx()
     dtype = to_torch_dtype(dtype)
-    if len(shape) == 0:
+    requested_shape = shape
+    if len(requested_shape) == 0:
         shape = (1,)
     # Do not use generator during symbolic execution.
     if get_device() == "meta":
         rand_tensor = torch.rand(size=shape, dtype=dtype, device=get_device())
     else:
         generator = torch_seed_generator(seed)
         rand_tensor = torch.rand(
             size=shape, generator=generator, dtype=dtype, device=get_device()
         )
 
     output = (maxval - minval) * rand_tensor + minval
+
+    if len(requested_shape) == 0:
+        return output[0]
     return output
 
 
 def randint(shape, minval, maxval, dtype="int32", seed=None):
     dtype = to_torch_dtype(dtype)
     # Do not use generator during symbolic execution.
     if get_device() == "meta":
```

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/rnn.py` & `keras-core-0.1.4/keras_core/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/torch_module_wrapper.py` & `keras-core-0.1.4/keras_core/src/backend/torch/torch_module_wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/backend/torch/trainer.py` & `keras-core-0.1.4/keras_core/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/__init__.py` & `keras-core-0.1.4/keras_core/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/callback.py` & `keras-core-0.1.4/keras_core/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/callback_list.py` & `keras-core-0.1.4/keras_core/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/csv_logger.py` & `keras-core-0.1.4/keras_core/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/early_stopping.py` & `keras-core-0.1.4/keras_core/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/history.py` & `keras-core-0.1.4/keras_core/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/lambda_callback.py` & `keras-core-0.1.4/keras_core/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/learning_rate_scheduler.py` & `keras-core-0.1.4/keras_core/src/callbacks/learning_rate_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,9 +72,11 @@
             io_utils.print_msg(
                 f"\nEpoch {epoch + 1}: LearningRateScheduler setting learning "
                 f"rate to {learning_rate}."
             )
 
     def on_epoch_end(self, epoch, logs=None):
         logs = logs or {}
-        logs["learning_rate"] = self.model.optimizer.learning_rate.value
+        logs["learning_rate"] = float(
+            backend.convert_to_numpy(self.model.optimizer.learning_rate)
+        )
```

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/model_checkpoint.py` & `keras-core-0.1.4/keras_core/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/progbar_logger.py` & `keras-core-0.1.4/keras_core/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/reduce_lr_on_plateau.py` & `keras-core-0.1.4/keras_core/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/remote_monitor.py` & `keras-core-0.1.4/keras_core/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/tensorboard.py` & `keras-core-0.1.4/keras_core/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/callbacks/terminate_on_nan.py` & `keras-core-0.1.4/keras_core/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/constraints/__init__.py` & `keras-core-0.1.4/keras_core/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/constraints/constraints.py` & `keras-core-0.1.4/keras_core/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/california_housing.py` & `keras-core-0.1.4/keras_core/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/cifar.py` & `keras-core-0.1.4/keras_core/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/cifar10.py` & `keras-core-0.1.4/keras_core/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/cifar100.py` & `keras-core-0.1.4/keras_core/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/fashion_mnist.py` & `keras-core-0.1.4/keras_core/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/imdb.py` & `keras-core-0.1.4/keras_core/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/mnist.py` & `keras-core-0.1.4/keras_core/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/datasets/reuters.py` & `keras-core-0.1.4/keras_core/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/initializers/__init__.py` & `keras-core-0.1.4/keras_core/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/initializers/constant_initializers.py` & `keras-core-0.1.4/keras_core/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/initializers/initializer.py` & `keras-core-0.1.4/keras_core/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/initializers/random_initializers.py` & `keras-core-0.1.4/keras_core/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/__init__.py` & `keras-core-0.1.4/keras_core/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/activation.py` & `keras-core-0.1.4/keras_core/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/elu.py` & `keras-core-0.1.4/keras_core/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/leaky_relu.py` & `keras-core-0.1.4/keras_core/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/prelu.py` & `keras-core-0.1.4/keras_core/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/relu.py` & `keras-core-0.1.4/keras_core/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/activations/softmax.py` & `keras-core-0.1.4/keras_core/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/attention/additive_attention.py` & `keras-core-0.1.4/keras_core/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/attention/attention.py` & `keras-core-0.1.4/keras_core/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/attention/multi_head_attention.py` & `keras-core-0.1.4/keras_core/src/layers/attention/multi_head_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
         bias_constraint=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.supports_masking = True
         self._num_heads = num_heads
         self._key_dim = key_dim
+        # Cache 1.0 / math.sqrt(self._key_dim).
+        self._inverse_sqrt_key_dim = None
         self._value_dim = value_dim if value_dim else key_dim
         self._dropout = dropout
         self._use_bias = use_bias
         self._output_shape = output_shape
         self._kernel_initializer = initializers.get(kernel_initializer)
         self._bias_initializer = initializers.get(bias_initializer)
         self._kernel_regularizer = regularizers.get(kernel_regularizer)
@@ -307,14 +309,15 @@
         norm_axes = tuple(
             range(
                 attn_scores_rank - len(self._attention_axes), attn_scores_rank
             )
         )
         self._softmax = Softmax(axis=norm_axes)
         self._dropout_layer = Dropout(rate=self._dropout)
+        self._inverse_sqrt_key_dim = 1.0 / math.sqrt(float(self._key_dim))
 
     def _masked_softmax(self, attention_scores, attention_mask=None):
         # Normalize the attention scores to probabilities.
         # attention_scores = [B, N, T, S]
         if attention_mask is not None:
             # The expand dim happens starting from the `num_heads` dimension,
             # (<batch_dims>, num_heads, <query_attention_dims,
@@ -351,15 +354,15 @@
         Returns:
           attention_output: Multi-headed outputs of attention computation.
           attention_scores: Multi-headed attention weights.
         """
         # Note: Applying scalar multiply at the smaller end of einsum improves
         # XLA performance, but may introduce slight numeric differences in
         # the Transformer attention head.
-        query = ops.multiply(query, 1.0 / math.sqrt(float(self._key_dim)))
+        query = ops.multiply(query, self._inverse_sqrt_key_dim)
 
         # Take the dot product between "query" and "key" to get the raw
         # attention scores.
         attention_scores = ops.einsum(self._dot_product_equation, key, query)
 
         attention_scores = self._masked_softmax(
             attention_scores, attention_mask
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/base_conv.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/base_conv_transpose.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/base_depthwise_conv.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/base_separable_conv.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv1d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv1d_transpose.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv2d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv2d_transpose.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv3d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/conv3d_transpose.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/depthwise_conv1d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/depthwise_conv2d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/separable_conv1d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/convolutional/separable_conv2d.py` & `keras-core-0.1.4/keras_core/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/dense.py` & `keras-core-0.1.4/keras_core/src/layers/core/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,20 +83,22 @@
 
         self.input_spec = InputSpec(min_ndim=2)
         self.supports_masking = True
 
     def build(self, input_shape):
         input_dim = input_shape[-1]
         self.kernel = self.add_weight(
+            name="kernel",
             shape=(input_dim, self.units),
             initializer=self.kernel_initializer,
             regularizer=self.kernel_regularizer,
         )
         if self.use_bias:
             self.bias = self.add_weight(
+                name="bias",
                 shape=(self.units,),
                 initializer=self.bias_initializer,
                 regularizer=self.bias_regularizer,
             )
         self.input_spec = InputSpec(min_ndim=2, axes={-1: input_dim})
         self.built = True
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/einsum_dense.py` & `keras-core-0.1.4/keras_core/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/embedding.py` & `keras-core-0.1.4/keras_core/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/identity.py` & `keras-core-0.1.4/keras_core/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/input_layer.py` & `keras-core-0.1.4/keras_core/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/lambda_layer.py` & `keras-core-0.1.4/keras_core/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/masking.py` & `keras-core-0.1.4/keras_core/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/core/wrapper.py` & `keras-core-0.1.4/keras_core/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/input_spec.py` & `keras-core-0.1.4/keras_core/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/layer.py` & `keras-core-0.1.4/keras_core/src/layers/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,17 +620,14 @@
     def __call__(self, *args, **kwargs):
         self._check_super_called()
 
         #####################################
         # 1. Convert any array arguments to tensors of correct dtype.
         def maybe_convert(x):
             if backend.is_tensor(x):
-                # Handle Torch device placement.
-                if backend.backend() == "torch":
-                    x = backend.convert_to_tensor(x)
                 if (
                     self.autocast
                     and backend.is_float_dtype(x.dtype)
                     and x.dtype != self.compute_dtype
                 ):
                     x = backend.cast(x, dtype=self.compute_dtype)
                 return x
@@ -642,15 +639,21 @@
                 ):
                     x.dtype = self.compute_dtype
                 return x
             elif hasattr(x, "__array__"):
                 return backend.convert_to_tensor(x, dtype=self.compute_dtype)
             return x
 
-        if self._convert_input_args:
+        # Used to avoid expensive `tree` operations in the most common case.
+        if (
+            kwargs
+            or len(args) != 1
+            or not backend.is_tensor(args[0])
+            or backend.standardize_dtype(args[0].dtype) != self.compute_dtype
+        ) and self._convert_input_args:
             args = tree.map_structure(maybe_convert, args)
             kwargs = tree.map_structure(maybe_convert, kwargs)
 
         ##########################################################
         # 2. Enforce that only tensors can be passed positionally.
         if not self._allow_non_tensor_positional_args:
             for arg in tree.flatten(args):
@@ -1346,15 +1349,15 @@
     ```
     >>> get_shapes_dict(call_spec)
     {"input_a_shape": (2, 3)}
     ```
     """
     shapes_dict = {}
     for k, v in call_spec.tensor_arguments_dict.items():
-        if k == "mask" or k.startswith("mask_"):
+        if k == "mask" or k.endswith("_mask"):
             # Do not include mask tensors in shapes dict
             continue
         if k == "kwargs" or k == "args":
             # Do not include catch-alls in shapes dict
             continue
         if k in call_spec.nested_tensor_argument_names:
             shapes_dict[f"{k}_shape"] = tree.map_structure(
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/add.py` & `keras-core-0.1.4/keras_core/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/average.py` & `keras-core-0.1.4/keras_core/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/base_merge.py` & `keras-core-0.1.4/keras_core/src/layers/merging/base_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                         f"Received shapes {shape1} and {shape2}"
                     )
                 output_shape.append(i)
         return tuple(output_shape)
 
     def build(self, input_shape):
         # Used purely for shape validation.
-        if not isinstance(input_shape[0], tuple):
+        if not isinstance(input_shape[0], (tuple, list)):
             raise ValueError(
                 "A merge layer should be called on a list of inputs. "
                 f"Received: input_shape={input_shape} (not a list of shapes)"
             )
         if len(input_shape) < 1:
             raise ValueError(
                 "A merge layer should be called "
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/concatenate.py` & `keras-core-0.1.4/keras_core/src/layers/merging/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         super().__init__(**kwargs)
         self.axis = axis
         self.supports_masking = True
         self._reshape_required = False
 
     def build(self, input_shape):
         # Used purely for shape validation.
-        if len(input_shape) < 1 or not isinstance(input_shape[0], tuple):
+        if len(input_shape) < 1 or not isinstance(
+            input_shape[0], (tuple, list)
+        ):
             raise ValueError(
                 "A `Concatenate` layer should be called on a list of "
                 f"at least 1 input. Received: input_shape={input_shape}"
             )
         if all(shape is None for shape in input_shape):
             return
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/dot.py` & `keras-core-0.1.4/keras_core/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/maximum.py` & `keras-core-0.1.4/keras_core/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/minimum.py` & `keras-core-0.1.4/keras_core/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/multiply.py` & `keras-core-0.1.4/keras_core/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/merging/subtract.py` & `keras-core-0.1.4/keras_core/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/normalization/batch_normalization.py` & `keras-core-0.1.4/keras_core/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/normalization/group_normalization.py` & `keras-core-0.1.4/keras_core/src/layers/normalization/group_normalization.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,48 +173,47 @@
 
         mean = ops.mean(
             reshaped_inputs, axis=group_reduction_axes, keepdims=True
         )
         variance = ops.var(
             reshaped_inputs, axis=group_reduction_axes, keepdims=True
         )
-
         gamma, beta = self._get_reshaped_weights(input_shape)
 
         # Compute the batch normalization.
         inv = 1 / ops.sqrt(variance + self.epsilon)
+
         if gamma is not None:
-            inv *= gamma
+            inv = ops.multiply(inv, gamma)
+
+        if beta is not None:
+            x = beta - ops.multiply(mean, inv)
+        else:
+            x = -ops.multiply(mean, inv)
 
-        x = beta - mean * inv if beta is not None else -mean * inv
         normalized_inputs = reshaped_inputs * ops.cast(
             inv, reshaped_inputs.dtype
         ) + ops.cast(x, reshaped_inputs.dtype)
-
         normalized_inputs = ops.cast(normalized_inputs, reshaped_inputs.dtype)
-
         return normalized_inputs
 
     def _get_reshaped_weights(self, input_shape):
         broadcast_shape = self._create_broadcast_shape(input_shape)
         gamma = None
         beta = None
         if self.scale:
             gamma = ops.reshape(self.gamma, broadcast_shape)
-
         if self.center:
             beta = ops.reshape(self.beta, broadcast_shape)
         return gamma, beta
 
     def _create_broadcast_shape(self, input_shape):
         broadcast_shape = [1] * len(input_shape)
-
         broadcast_shape[self.axis] = input_shape[self.axis] // self.groups
         broadcast_shape.insert(self.axis, self.groups)
-
         return broadcast_shape
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = {
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/normalization/layer_normalization.py` & `keras-core-0.1.4/keras_core/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/normalization/spectral_normalization.py` & `keras-core-0.1.4/keras_core/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/normalization/unit_normalization.py` & `keras-core-0.1.4/keras_core/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling1d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling2d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/average_pooling3d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/base_global_pooling.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/base_pooling.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling1d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling2d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_average_pooling3d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling1d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling2d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/global_max_pooling3d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling1d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling2d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/pooling/max_pooling3d.py` & `keras-core-0.1.4/keras_core/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/category_encoding.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/center_crop.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/discretization.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/feature_space.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/hashed_crossing.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/hashing.py` & `keras-core-0.1.4/keras_core/src/layers/regularization/spatial_dropout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,193 @@
-import numpy as np
-
 from keras_core.src import backend
+from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
-from keras_core.src.layers.layer import Layer
-from keras_core.src.utils import backend_utils
-from keras_core.src.utils.module_utils import tensorflow as tf
-
-
-@keras_core_export("keras_core.layers.Hashing")
-class Hashing(Layer):
-    """A preprocessing layer which hashes and bins categorical features.
-
-    This layer transforms categorical inputs to hashed output. It element-wise
-    converts a ints or strings to ints in a fixed range. The stable hash
-    function uses `tensorflow::ops::Fingerprint` to produce the same output
-    consistently across all platforms.
-
-    This layer uses [FarmHash64](https://github.com/google/farmhash) by default,
-    which provides a consistent hashed output across different platforms and is
-    stable across invocations, regardless of device and context, by mixing the
-    input bits thoroughly.
-
-    If you want to obfuscate the hashed output, you can also pass a random
-    `salt` argument in the constructor. In that case, the layer will use the
-    [SipHash64](https://github.com/google/highwayhash) hash function, with
-    the `salt` value serving as additional input to the hash function.
-
-    **Note:** This layer wraps `tf.keras.layers.Hashing`. It cannot
-    be used as part of the compiled computation graph of a model with
-    any backend other than TensorFlow.
-    It can however be used with any backend when running eagerly.
-    It can also always be used as part of an input preprocessing pipeline
-    with any backend (outside the model itself), which is how we recommend
-    to use this layer.
-
-    **Note:** This layer is safe to use inside a `tf.data` pipeline
-    (independently of which backend you're using).
-
-    **Example (FarmHash64)**
-
-    >>> layer = keras_core.layers.Hashing(num_bins=3)
-    >>> inp = [['A'], ['B'], ['C'], ['D'], ['E']]
-    >>> layer(inp)
-    array([[1],
-            [0],
-            [1],
-            [1],
-            [2]])>
-
-    **Example (FarmHash64) with a mask value**
-
-    >>> layer = keras_core.layers.Hashing(num_bins=3, mask_value='')
-    >>> inp = [['A'], ['B'], [''], ['C'], ['D']]
-    >>> layer(inp)
-    array([[1],
-            [1],
-            [0],
-            [2],
-            [2]])
-
-    **Example (SipHash64)**
-
-    >>> layer = keras_core.layers.Hashing(num_bins=3, salt=[133, 137])
-    >>> inp = [['A'], ['B'], ['C'], ['D'], ['E']]
-    >>> layer(inp)
-    array([[1],
-            [2],
-            [1],
-            [0],
-            [2]])
-
-    **Example (Siphash64 with a single integer, same as `salt=[133, 133]`)**
-
-    >>> layer = keras_core.layers.Hashing(num_bins=3, salt=133)
-    >>> inp = [['A'], ['B'], ['C'], ['D'], ['E']]
-    >>> layer(inp)
-    array([[0],
-            [0],
-            [2],
-            [1],
-            [0]])
+from keras_core.src.layers.input_spec import InputSpec
+from keras_core.src.layers.regularization.dropout import Dropout
+
+
+class BaseSpatialDropout(Dropout):
+    def __init__(self, rate, seed=None, name=None, dtype=None):
+        super().__init__(rate, seed=seed, name=name, dtype=dtype)
+
+    def call(self, inputs, training=False):
+        if training and self.rate > 0:
+            return backend.random.dropout(
+                inputs,
+                self.rate,
+                noise_shape=self._get_noise_shape(inputs),
+                seed=self.seed_generator,
+            )
+        return inputs
+
+    def get_config(self):
+        return {
+            "rate": self.rate,
+            "seed": self.seed,
+            "name": self.name,
+            "dtype": self.dtype,
+        }
+
+
+@keras_core_export("keras_core.layers.SpatialDropout1D")
+class SpatialDropout1D(BaseSpatialDropout):
+    """Spatial 1D version of Dropout.
+
+    This layer performs the same function as Dropout, however, it drops
+    entire 1D feature maps instead of individual elements. If adjacent frames
+    within feature maps are strongly correlated (as is normally the case in
+    early convolution layers) then regular dropout will not regularize the
+    activations and will otherwise just result in an effective learning rate
+    decrease. In this case, `SpatialDropout1D` will help promote independence
+    between feature maps and should be used instead.
+
+    Args:
+        rate: Float between 0 and 1. Fraction of the input units to drop.
+
+    Call arguments:
+        inputs: A 3D tensor.
+        training: Python boolean indicating whether the layer
+            should behave in training mode (applying dropout)
+            or in inference mode (pass-through).
+
+    Input shape:
+        3D tensor with shape: `(samples, timesteps, channels)`
+
+    Output shape: Same as input.
+
+    Reference:
+
+    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
+    """
+
+    def __init__(self, rate, seed=None, name=None, dtype=None):
+        super().__init__(rate, seed=seed, name=name, dtype=dtype)
+        self.input_spec = InputSpec(ndim=3)
+
+    def _get_noise_shape(self, inputs):
+        input_shape = ops.shape(inputs)
+        return (input_shape[0], 1, input_shape[2])
+
+
+@keras_core_export("keras_core.layers.SpatialDropout2D")
+class SpatialDropout2D(BaseSpatialDropout):
+    """Spatial 2D version of Dropout.
+
+    This version performs the same function as Dropout, however, it drops
+    entire 2D feature maps instead of individual elements. If adjacent pixels
+    within feature maps are strongly correlated (as is normally the case in
+    early convolution layers) then regular dropout will not regularize the
+    activations and will otherwise just result in an effective learning rate
+    decrease. In this case, `SpatialDropout2D` will help promote independence
+    between feature maps and should be used instead.
 
     Args:
-        num_bins: Number of hash bins. Note that this includes the `mask_value`
-            bin, so the effective number of bins is `(num_bins - 1)`
-            if `mask_value` is set.
-        mask_value: A value that represents masked inputs, which are mapped to
-            index 0. `None` means no mask term will be added and the
-            hashing will start at index 0. Defaults to `None`.
-        salt: A single unsigned integer or None.
-            If passed, the hash function used will be SipHash64,
-            with these values used as an additional input
-            (known as a "salt" in cryptography).
-            These should be non-zero. If `None`, uses the FarmHash64 hash
-            function. It also supports tuple/list of 2 unsigned
-            integer numbers, see reference paper for details.
-            Defaults to `None`.
-        output_mode: Specification for the output of the layer. Values can be
-            `"int"`, `"one_hot"`, `"multi_hot"`, or
-            `"count"` configuring the layer as follows:
-            - `"int"`: Return the integer bin indices directly.
-            - `"one_hot"`: Encodes each individual element in the input into an
-                array the same size as `num_bins`, containing a 1
-                at the input's bin index. If the last dimension is size 1,
-                will encode on that dimension.
-                If the last dimension is not size 1, will append a new
-                dimension for the encoded output.
-            - `"multi_hot"`: Encodes each sample in the input into a
-                single array the same size as `num_bins`,
-                containing a 1 for each bin index
-                index present in the sample. Treats the last dimension
-                as the sample dimension, if input shape is
-                `(..., sample_length)`, output shape will be
-                `(..., num_tokens)`.
-            - `"count"`: As `"multi_hot"`, but the int array contains a count of
-                the number of times the bin index appeared in the sample.
-            Defaults to `"int"`.
-        sparse: Boolean. Only applicable to `"one_hot"`, `"multi_hot"`,
-            and `"count"` output modes. Only supported with TensorFlow
-            backend. If `True`, returns a `SparseTensor` instead of
-            a dense `Tensor`. Defaults to `False`.
-        **kwargs: Keyword arguments to construct a layer.
+        rate: Float between 0 and 1. Fraction of the input units to drop.
+        data_format: `"channels_first"` or `"channels_last"`.
+            In `"channels_first"` mode, the channels dimension (the depth)
+            is at index 1, in `"channels_last"` mode is it at index 3.
+            It defaults to the `image_data_format` value found in your
+            Keras config file at `~/.keras/keras.json`.
+            If you never set it, then it will be `"channels_last"`.
+
+    Call arguments:
+        inputs: A 4D tensor.
+        training: Python boolean indicating whether the layer
+            should behave in training mode (applying dropout)
+            or in inference mode (pass-through).
 
     Input shape:
-        A single string, a list of strings, or an `int32` or `int64` tensor
-        of shape `(batch_size, ...,)`.
+        4D tensor with shape: `(samples, channels, rows, cols)` if
+            data_format='channels_first'
+        or 4D tensor with shape: `(samples, rows, cols, channels)` if
+            data_format='channels_last'.
 
-    Output shape:
-        An `int32` tensor of shape `(batch_size, ...)`.
+    Output shape: Same as input.
 
     Reference:
 
-    - [SipHash with salt](https://www.131002.net/siphash/siphash.pdf)
+    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
     """
 
     def __init__(
-        self,
-        num_bins,
-        mask_value=None,
-        salt=None,
-        output_mode="int",
-        sparse=False,
-        name=None,
-        **kwargs,
+        self, rate, data_format=None, seed=None, name=None, dtype=None
     ):
-        if not tf.available:
-            raise ImportError(
-                "Layer Hashing requires TensorFlow. "
-                "Install it via `pip install tensorflow`."
-            )
+        super().__init__(rate, seed=seed, name=name, dtype=dtype)
+        self.data_format = backend.standardize_data_format(data_format)
+        self.input_spec = InputSpec(ndim=4)
+
+    def _get_noise_shape(self, inputs):
+        input_shape = ops.shape(inputs)
+        if self.data_format == "channels_first":
+            return (input_shape[0], input_shape[1], 1, 1)
+        elif self.data_format == "channels_last":
+            return (input_shape[0], 1, 1, input_shape[3])
+
+    def get_config(self):
+        base_config = super().get_config()
+        config = {
+            "data_format": self.data_format,
+        }
+        return {**base_config, **config}
+
+
+@keras_core_export("keras_core.layers.SpatialDropout3D")
+class SpatialDropout3D(BaseSpatialDropout):
+    """Spatial 3D version of Dropout.
+
+    This version performs the same function as Dropout, however, it drops
+    entire 3D feature maps instead of individual elements. If adjacent voxels
+    within feature maps are strongly correlated (as is normally the case in
+    early convolution layers) then regular dropout will not regularize the
+    activations and will otherwise just result in an effective learning rate
+    decrease. In this case, SpatialDropout3D will help promote independence
+    between feature maps and should be used instead.
+
+    Args:
+        rate: Float between 0 and 1. Fraction of the input units to drop.
+        data_format: `"channels_first"` or `"channels_last"`.
+            In `"channels_first"` mode, the channels dimension (the depth)
+            is at index 1, in `"channels_last"` mode is it at index 4.
+            It defaults to the `image_data_format` value found in your
+            Keras config file at `~/.keras/keras.json`.
+            If you never set it, then it will be `"channels_last"`.
+
+    Call arguments:
+        inputs: A 5D tensor.
+        training: Python boolean indicating whether the layer
+                should behave in training mode (applying dropout)
+                or in inference mode (pass-through).
 
-        super().__init__(name=name)
-        self.layer = tf.keras.layers.Hashing(
-            num_bins=num_bins,
-            mask_value=mask_value,
-            salt=salt,
-            output_mode=output_mode,
-            sparse=sparse,
-            name=name,
-            **kwargs,
-        )
-        self.num_bins = num_bins
-        self.mask_value = mask_value
-        self.strong_hash = True if salt is not None else False
-        self.output_mode = output_mode
-        self.sparse = sparse
-        self.salt = None
-        if salt is not None:
-            if isinstance(salt, (tuple, list)) and len(salt) == 2:
-                self.salt = salt
-            elif isinstance(salt, int):
-                self.salt = [salt, salt]
-            else:
-                raise ValueError(
-                    "The `salt` argument for `Hashing` can only be a tuple "
-                    "of 2 integers, or a single integer. "
-                    f"Received: salt={salt}."
-                )
-        self._convert_input_args = False
-        self._allow_non_tensor_positional_args = True
-        self.supports_jit = False
-
-    def call(self, inputs):
-        if not isinstance(inputs, (tf.Tensor, np.ndarray, list, tuple)):
-            inputs = tf.convert_to_tensor(np.array(inputs))
-        outputs = self.layer.call(inputs)
-        if (
-            backend.backend() != "tensorflow"
-            and not backend_utils.in_tf_graph()
-        ):
-            outputs = backend.convert_to_tensor(outputs)
-        return outputs
+    Input shape:
+        5D tensor with shape: `(samples, channels, dim1, dim2, dim3)` if
+            data_format='channels_first'
+        or 5D tensor with shape: `(samples, dim1, dim2, dim3, channels)` if
+            data_format='channels_last'.
 
-    def compute_output_spec(self, inputs):
-        return backend.KerasTensor(shape=inputs.shape, dtype="int32")
+    Output shape: Same as input.
+
+    Reference:
+
+    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
+    """
+
+    def __init__(
+        self, rate, data_format=None, seed=None, name=None, dtype=None
+    ):
+        super().__init__(rate, seed=seed, name=name, dtype=dtype)
+        self.data_format = backend.standardize_data_format(data_format)
+        self.input_spec = InputSpec(ndim=5)
+
+    def _get_noise_shape(self, inputs):
+        input_shape = ops.shape(inputs)
+        if self.data_format == "channels_first":
+            return (input_shape[0], input_shape[1], 1, 1, 1)
+        elif self.data_format == "channels_last":
+            return (input_shape[0], 1, 1, 1, input_shape[4])
 
     def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "num_bins": self.num_bins,
-                "salt": self.salt,
-                "mask_value": self.mask_value,
-                "output_mode": self.output_mode,
-                "sparse": self.sparse,
-            }
-        )
-        return config
+        base_config = super().get_config()
+        config = {
+            "data_format": self.data_format,
+        }
+        return {**base_config, **config}
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/integer_lookup.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/normalization.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_brightness.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_contrast.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_crop.py` & `keras-core-0.1.4/keras_core/src/layers/regularization/dropout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,77 @@
-import numpy as np
-
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
-from keras_core.src.utils import backend_utils
-from keras_core.src.utils.module_utils import tensorflow as tf
 
 
-@keras_core_export("keras_core.layers.RandomCrop")
-class RandomCrop(Layer):
-    """A preprocessing layer which randomly crops images during training.
-
-    During training, this layer will randomly choose a location to crop images
-    down to a target size. The layer will crop all the images in the same batch
-    to the same cropping location.
-
-    At inference time, and during training if an input image is smaller than the
-    target size, the input will be resized and cropped so as to return the
-    largest possible window in the image that matches the target aspect ratio.
-    If you need to apply random cropping at inference time, set `training` to
-    True when calling the layer.
-
-    Input pixel values can be of any range (e.g. `[0., 1.)` or `[0, 255]`) and
-    of integer or floating point dtype. By default, the layer will output
-    floats.
-
-    **Note:** This layer wraps `tf.keras.layers.RandomCrop`. It cannot
-    be used as part of the compiled computation graph of a model with
-    any backend other than TensorFlow.
-    It can however be used with any backend when running eagerly.
-    It can also always be used as part of an input preprocessing pipeline
-    with any backend (outside the model itself), which is how we recommend
-    to use this layer.
-
-    **Note:** This layer is safe to use inside a `tf.data` pipeline
-    (independently of which backend you're using).
-
-    Input shape:
-        3D (unbatched) or 4D (batched) tensor with shape:
-        `(..., height, width, channels)`, in `"channels_last"` format.
-
-    Output shape:
-        3D (unbatched) or 4D (batched) tensor with shape:
-        `(..., target_height, target_width, channels)`.
+@keras_core_export("keras_core.layers.Dropout")
+class Dropout(Layer):
+    """Applies dropout to the input.
+
+    The `Dropout` layer randomly sets input units to 0 with a frequency of
+    `rate` at each step during training time, which helps prevent overfitting.
+    Inputs not set to 0 are scaled up by `1 / (1 - rate)` such that the sum over
+    all inputs is unchanged.
+
+    Note that the `Dropout` layer only applies when `training` is set to `True`
+    in `call()`, such that no values are dropped during inference.
+    When using `model.fit`, `training` will be appropriately set to `True`
+    automatically. In other contexts, you can set the argument explicitly
+    to `True` when calling the layer.
+
+    (This is in contrast to setting `trainable=False` for a `Dropout` layer.
+    `trainable` does not affect the layer's behavior, as `Dropout` does
+    not have any variables/weights that can be frozen during training.)
 
     Args:
-        height: Integer, the height of the output shape.
-        width: Integer, the width of the output shape.
-        seed: Integer. Used to create a random seed.
-        **kwargs: Base layer keyword arguments, such as
-            `name` and `dtype`.
+        rate: Float between 0 and 1. Fraction of the input units to drop.
+        noise_shape: 1D integer tensor representing the shape of the
+            binary dropout mask that will be multiplied with the input.
+            For instance, if your inputs have shape
+            `(batch_size, timesteps, features)` and
+            you want the dropout mask to be the same for all timesteps,
+            you can use `noise_shape=(batch_size, 1, features)`.
+        seed: A Python integer to use as random seed.
+
+    Call arguments:
+        inputs: Input tensor (of any rank).
+        training: Python boolean indicating whether the layer should behave in
+            training mode (adding dropout) or in inference mode (doing nothing).
     """
 
-    def __init__(self, height, width, seed=None, name=None, **kwargs):
-        if not tf.available:
-            raise ImportError(
-                "Layer RandomCrop requires TensorFlow. "
-                "Install it via `pip install tensorflow`."
+    def __init__(self, rate, noise_shape=None, seed=None, **kwargs):
+        super().__init__(**kwargs)
+        if not 0 <= rate <= 1:
+            raise ValueError(
+                f"Invalid value received for argument "
+                "`rate`. Expected a float value between 0 and 1. "
+                f"Received: rate={rate}"
             )
-
-        super().__init__(name=name, **kwargs)
-        self.seed = seed or backend.random.make_default_seed()
-        self.layer = tf.keras.layers.RandomCrop(
-            height=height,
-            width=width,
-            seed=self.seed,
-            name=name,
-        )
-        self.supports_masking = False
-        self.supports_jit = False
-        self._convert_input_args = False
-        self._allow_non_tensor_positional_args = True
-
-    def call(self, inputs, training=True):
-        if not isinstance(inputs, (tf.Tensor, np.ndarray, list, tuple)):
-            inputs = tf.convert_to_tensor(backend.convert_to_numpy(inputs))
-        outputs = self.layer.call(inputs, training=training)
-        if (
-            backend.backend() != "tensorflow"
-            and not backend_utils.in_tf_graph()
-        ):
-            outputs = backend.convert_to_tensor(outputs)
-        return outputs
+        self.rate = rate
+        self.seed = seed
+        self.noise_shape = noise_shape
+        self.seed_generator = backend.random.SeedGenerator(seed)
+        self.supports_masking = True
+        self.built = True
+
+    def call(self, inputs, training=False):
+        if training and self.rate > 0:
+            return backend.random.dropout(
+                inputs,
+                self.rate,
+                noise_shape=self.noise_shape,
+                seed=self.seed_generator,
+            )
+        return inputs
 
     def compute_output_shape(self, input_shape):
-        return tuple(self.layer.compute_output_shape(input_shape))
+        return input_shape
 
     def get_config(self):
-        config = self.layer.get_config()
-        config.update({"seed": self.seed})
-        return config
+        base_config = super().get_config()
+        config = {
+            "rate": self.rate,
+            "seed": self.seed,
+            "noise_shape": self.noise_shape,
+        }
+        return {**base_config, **config}
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_flip.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/random_flip.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,34 +40,45 @@
     """
 
     def __init__(self, mode=HORIZONTAL_AND_VERTICAL, seed=None, **kwargs):
         super().__init__(**kwargs)
         self.seed = seed
         self.generator = SeedGenerator(seed)
         self.mode = mode
-        self.supports_jit = False
         self._convert_input_args = False
         self._allow_non_tensor_positional_args = True
 
     def _randomly_flip_inputs(self, inputs):
+        unbatched = len(inputs.shape) == 3
+        if unbatched:
+            inputs = self.backend.numpy.expand_dims(inputs, axis=0)
+        batch_size = self.backend.shape(inputs)[0]
         flipped_outputs = inputs
         seed_generator = self._get_seed_generator(self.backend._backend)
         if self.mode == HORIZONTAL or self.mode == HORIZONTAL_AND_VERTICAL:
-            flipped_outputs = self.backend.cond(
-                self.backend.random.uniform(shape=(), seed=seed_generator)
+            flipped_outputs = self.backend.numpy.where(
+                self.backend.random.uniform(
+                    shape=(batch_size,), seed=seed_generator
+                )
                 <= 0.5,
-                lambda: self.backend.numpy.flip(flipped_outputs, axis=-2),
-                lambda: flipped_outputs,
+                self.backend.numpy.flip(flipped_outputs, axis=-2),
+                flipped_outputs,
             )
         if self.mode == VERTICAL or self.mode == HORIZONTAL_AND_VERTICAL:
-            flipped_outputs = self.backend.cond(
-                self.backend.random.uniform(shape=(), seed=seed_generator)
+            flipped_outputs = self.backend.numpy.where(
+                self.backend.random.uniform(
+                    shape=(batch_size,), seed=seed_generator
+                )
                 <= 0.5,
-                lambda: self.backend.numpy.flip(flipped_outputs, axis=-3),
-                lambda: flipped_outputs,
+                self.backend.numpy.flip(flipped_outputs, axis=-3),
+                flipped_outputs,
+            )
+        if unbatched:
+            flipped_outputs = self.backend.numpy.squeeze(
+                flipped_outputs, axis=0
             )
         return flipped_outputs
 
     def call(self, inputs, training=True):
         inputs = self.backend.cast(inputs, self.compute_dtype)
         if training:
             return self._randomly_flip_inputs(inputs)
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_translation.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/random_zoom.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/rescaling.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/resizing.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/string_lookup.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/text_vectorization.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/preprocessing/tf_data_layer.py` & `keras-core-0.1.4/keras_core/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/regularization/activity_regularization.py` & `keras-core-0.1.4/keras_core/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/regularization/dropout.py` & `keras-core-0.1.4/keras_core/src/layers/regularization/gaussian_dropout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,61 @@
+import math
+
 from keras_core.src import backend
+from keras_core.src import layers
+from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
-from keras_core.src.layers.layer import Layer
 
 
-@keras_core_export("keras_core.layers.Dropout")
-class Dropout(Layer):
-    """Applies dropout to the input.
-
-    The `Dropout` layer randomly sets input units to 0 with a frequency of
-    `rate` at each step during training time, which helps prevent overfitting.
-    Inputs not set to 0 are scaled up by `1 / (1 - rate)` such that the sum over
-    all inputs is unchanged.
-
-    Note that the `Dropout` layer only applies when `training` is set to `True`
-    in `call()`, such that no values are dropped during inference.
-    When using `model.fit`, `training` will be appropriately set to `True`
-    automatically. In other contexts, you can set the argument explicitly
-    to `True` when calling the layer.
-
-    (This is in contrast to setting `trainable=False` for a `Dropout` layer.
-    `trainable` does not affect the layer's behavior, as `Dropout` does
-    not have any variables/weights that can be frozen during training.)
+@keras_core_export("keras_core.layers.GaussianDropout")
+class GaussianDropout(layers.Layer):
+    """Apply multiplicative 1-centered Gaussian noise.
+
+    As it is a regularization layer, it is only active at training time.
 
     Args:
-        rate: Float between 0 and 1. Fraction of the input units to drop.
-        noise_shape: 1D integer tensor representing the shape of the
-            binary dropout mask that will be multiplied with the input.
-            For instance, if your inputs have shape
-            `(batch_size, timesteps, features)` and
-            you want the dropout mask to be the same for all timesteps,
-            you can use `noise_shape=(batch_size, 1, features)`.
-        seed: A Python integer to use as random seed.
+        rate: Float, drop probability (as with `Dropout`).
+            The multiplicative noise will have
+            standard deviation `sqrt(rate / (1 - rate))`.
+        seed: Integer, optional random seed to enable deterministic behavior.
 
     Call arguments:
         inputs: Input tensor (of any rank).
         training: Python boolean indicating whether the layer should behave in
             training mode (adding dropout) or in inference mode (doing nothing).
     """
 
-    def __init__(self, rate, noise_shape=None, seed=None, **kwargs):
+    def __init__(self, rate, seed=None, **kwargs):
         super().__init__(**kwargs)
         if not 0 <= rate <= 1:
             raise ValueError(
                 f"Invalid value received for argument "
                 "`rate`. Expected a float value between 0 and 1. "
                 f"Received: rate={rate}"
             )
         self.rate = rate
         self.seed = seed
-        self.noise_shape = noise_shape
         self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
-        self.built = True
 
     def call(self, inputs, training=False):
         if training and self.rate > 0:
-            return backend.random.dropout(
-                inputs,
-                self.rate,
-                noise_shape=self.noise_shape,
+            stddev = math.sqrt(self.rate / (1.0 - self.rate))
+            return inputs * backend.random.normal(
+                shape=ops.shape(inputs),
+                mean=1.0,
+                stddev=stddev,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
-            "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/regularization/gaussian_noise.py` & `keras-core-0.1.4/keras_core/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/regularization/spatial_dropout.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,218 @@
-from keras_core.src import backend
-from keras_core.src import ops
-from keras_core.src.api_export import keras_core_export
-from keras_core.src.layers.input_spec import InputSpec
-from keras_core.src.layers.regularization.dropout import Dropout
+import math
 
+import numpy as np
+import tree
 
-class BaseSpatialDropout(Dropout):
-    def __init__(self, rate, seed=None, name=None, dtype=None):
-        super().__init__(rate, seed=seed, name=name, dtype=dtype)
-
-    def call(self, inputs, training=False):
-        if training and self.rate > 0:
-            return backend.random.dropout(
-                inputs,
-                self.rate,
-                noise_shape=self._get_noise_shape(inputs),
-                seed=self.seed_generator,
-            )
-        return inputs
+from keras_core.src import backend
+from keras_core.src.api_export import keras_core_export
 
-    def get_config(self):
-        return {
-            "rate": self.rate,
-            "seed": self.seed,
-            "name": self.name,
-            "dtype": self.dtype,
-        }
-
-
-@keras_core_export("keras_core.layers.SpatialDropout1D")
-class SpatialDropout1D(BaseSpatialDropout):
-    """Spatial 1D version of Dropout.
-
-    This layer performs the same function as Dropout, however, it drops
-    entire 1D feature maps instead of individual elements. If adjacent frames
-    within feature maps are strongly correlated (as is normally the case in
-    early convolution layers) then regular dropout will not regularize the
-    activations and will otherwise just result in an effective learning rate
-    decrease. In this case, `SpatialDropout1D` will help promote independence
-    between feature maps and should be used instead.
+try:
+    import pandas
+except ImportError:
+    pandas = None
+
+
+# Leave jax, tf, and torch arrays off this list. Instead we will use
+# `__array__` to detect these types. Doing so allows us to avoid importing a
+# backend framework we are not currently using just to do type-checking.
+ARRAY_TYPES = (np.ndarray,)
+if backend.backend() == "tensorflow":
+    from keras_core.src.utils.module_utils import tensorflow as tf
+
+    ARRAY_TYPES = ARRAY_TYPES + (np.ndarray, tf.RaggedTensor)
+if pandas:
+    ARRAY_TYPES = ARRAY_TYPES + (pandas.Series, pandas.DataFrame)
+
+
+@keras_core_export("keras_core.utils.unpack_x_y_sample_weight")
+def unpack_x_y_sample_weight(data):
+    """Unpacks user-provided data tuple.
+
+    This is a convenience utility to be used when overriding
+    `Model.train_step`, `Model.test_step`, or `Model.predict_step`.
+    This utility makes it easy to support data of the form `(x,)`,
+    `(x, y)`, or `(x, y, sample_weight)`.
+
+    Standalone usage:
+
+    >>> features_batch = ops.ones((10, 5))
+    >>> labels_batch = ops.zeros((10, 5))
+    >>> data = (features_batch, labels_batch)
+    >>> # `y` and `sample_weight` will default to `None` if not provided.
+    >>> x, y, sample_weight = unpack_x_y_sample_weight(data)
+    >>> sample_weight is None
+    True
 
     Args:
-        rate: Float between 0 and 1. Fraction of the input units to drop.
-
-    Call arguments:
-        inputs: A 3D tensor.
-        training: Python boolean indicating whether the layer
-            should behave in training mode (applying dropout)
-            or in inference mode (pass-through).
-
-    Input shape:
-        3D tensor with shape: `(samples, timesteps, channels)`
-
-    Output shape: Same as input.
+        data: A tuple of the form `(x,)`, `(x, y)`, or `(x, y, sample_weight)`.
 
-    Reference:
-
-    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
+    Returns:
+        The unpacked tuple, with `None`s for `y` and `sample_weight` if they are
+        not provided.
     """
-
-    def __init__(self, rate, seed=None, name=None, dtype=None):
-        super().__init__(rate, seed=seed, name=name, dtype=dtype)
-        self.input_spec = InputSpec(ndim=3)
-
-    def _get_noise_shape(self, inputs):
-        input_shape = ops.shape(inputs)
-        return (input_shape[0], 1, input_shape[2])
-
-
-@keras_core_export("keras_core.layers.SpatialDropout2D")
-class SpatialDropout2D(BaseSpatialDropout):
-    """Spatial 2D version of Dropout.
-
-    This version performs the same function as Dropout, however, it drops
-    entire 2D feature maps instead of individual elements. If adjacent pixels
-    within feature maps are strongly correlated (as is normally the case in
-    early convolution layers) then regular dropout will not regularize the
-    activations and will otherwise just result in an effective learning rate
-    decrease. In this case, `SpatialDropout2D` will help promote independence
-    between feature maps and should be used instead.
+    if isinstance(data, list):
+        data = tuple(data)
+    if not isinstance(data, tuple):
+        return (data, None, None)
+    elif len(data) == 1:
+        return (data[0], None, None)
+    elif len(data) == 2:
+        return (data[0], data[1], None)
+    elif len(data) == 3:
+        return (data[0], data[1], data[2])
+    error_msg = (
+        "Data is expected to be in format `x`, `(x,)`, `(x, y)`, "
+        f"or `(x, y, sample_weight)`, found: {data}"
+    )
+    raise ValueError(error_msg)
+
+
+@keras_core_export("keras_core.utils.pack_x_y_sample_weight")
+def pack_x_y_sample_weight(x, y=None, sample_weight=None):
+    """Packs user-provided data into a tuple.
+
+    This is a convenience utility for packing data into the tuple formats
+    that `Model.fit()` uses.
+
+    Standalone usage:
+
+    >>> x = ops.ones((10, 1))
+    >>> data = pack_x_y_sample_weight(x)
+    >>> isinstance(data, ops.Tensor)
+    True
+    >>> y = ops.ones((10, 1))
+    >>> data = pack_x_y_sample_weight(x, y)
+    >>> isinstance(data, tuple)
+    True
+    >>> x, y = data
 
     Args:
-        rate: Float between 0 and 1. Fraction of the input units to drop.
-        data_format: `"channels_first"` or `"channels_last"`.
-            In `"channels_first"` mode, the channels dimension (the depth)
-            is at index 1, in `"channels_last"` mode is it at index 3.
-            It defaults to the `image_data_format` value found in your
-            Keras config file at `~/.keras/keras.json`.
-            If you never set it, then it will be `"channels_last"`.
-
-    Call arguments:
-        inputs: A 4D tensor.
-        training: Python boolean indicating whether the layer
-            should behave in training mode (applying dropout)
-            or in inference mode (pass-through).
-
-    Input shape:
-        4D tensor with shape: `(samples, channels, rows, cols)` if
-            data_format='channels_first'
-        or 4D tensor with shape: `(samples, rows, cols, channels)` if
-            data_format='channels_last'.
+        x: Features to pass to `Model`.
+        y: Ground-truth targets to pass to `Model`.
+        sample_weight: Sample weight for each element.
 
-    Output shape: Same as input.
+    Returns:
+        Tuple in the format used in `Model.fit()`.
+    """
+    if y is None:
+        # For single x-input, we do no tuple wrapping since in this case
+        # there is no ambiguity. This also makes NumPy and Dataset
+        # consistent in that the user does not have to wrap their Dataset
+        # data in an unnecessary tuple.
+        if not isinstance(x, tuple or list):
+            return x
+        else:
+            return (x,)
+    elif sample_weight is None:
+        return (x, y)
+    else:
+        return (x, y, sample_weight)
+
+
+def list_to_tuple(maybe_list):
+    """Datasets will stack any list of tensors, so we convert them to tuples."""
+    if isinstance(maybe_list, list):
+        return tuple(maybe_list)
+    return maybe_list
+
+
+def check_data_cardinality(data):
+    num_samples = set(int(i.shape[0]) for i in tree.flatten(data))
+    if len(num_samples) > 1:
+        msg = (
+            "Data cardinality is ambiguous. "
+            "Make sure all arrays contain the same number of samples."
+        )
+        for label, single_data in zip(["x", "y", "sample_weight"], data):
+            sizes = ", ".join(
+                str(i.shape[0]) for i in tree.flatten(single_data)
+            )
+            msg += f"'{label}' sizes: {sizes}\n"
+        raise ValueError(msg)
 
-    Reference:
 
-    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
-    """
+def sync_shuffle(data, num_samples=None):
+    if num_samples is None:
+        num_samples_set = set(int(i.shape[0]) for i in tree.flatten(data))
+        assert len(num_samples_set) == 1
+        num_samples = num_samples_set.pop()
+    p = np.random.permutation(num_samples)
+    return tree.map_structure(lambda x: x[p], data)
 
-    def __init__(
-        self, rate, data_format=None, seed=None, name=None, dtype=None
-    ):
-        super().__init__(rate, seed=seed, name=name, dtype=dtype)
-        self.data_format = backend.standardize_data_format(data_format)
-        self.input_spec = InputSpec(ndim=4)
-
-    def _get_noise_shape(self, inputs):
-        input_shape = ops.shape(inputs)
-        if self.data_format == "channels_first":
-            return (input_shape[0], input_shape[1], 1, 1)
-        elif self.data_format == "channels_last":
-            return (input_shape[0], 1, 1, input_shape[3])
-
-    def get_config(self):
-        base_config = super().get_config()
-        config = {
-            "data_format": self.data_format,
-        }
-        return {**base_config, **config}
-
-
-@keras_core_export("keras_core.layers.SpatialDropout3D")
-class SpatialDropout3D(BaseSpatialDropout):
-    """Spatial 3D version of Dropout.
-
-    This version performs the same function as Dropout, however, it drops
-    entire 3D feature maps instead of individual elements. If adjacent voxels
-    within feature maps are strongly correlated (as is normally the case in
-    early convolution layers) then regular dropout will not regularize the
-    activations and will otherwise just result in an effective learning rate
-    decrease. In this case, SpatialDropout3D will help promote independence
-    between feature maps and should be used instead.
 
-    Args:
-        rate: Float between 0 and 1. Fraction of the input units to drop.
-        data_format: `"channels_first"` or `"channels_last"`.
-            In `"channels_first"` mode, the channels dimension (the depth)
-            is at index 1, in `"channels_last"` mode is it at index 4.
-            It defaults to the `image_data_format` value found in your
-            Keras config file at `~/.keras/keras.json`.
-            If you never set it, then it will be `"channels_last"`.
-
-    Call arguments:
-        inputs: A 5D tensor.
-        training: Python boolean indicating whether the layer
-                should behave in training mode (applying dropout)
-                or in inference mode (pass-through).
-
-    Input shape:
-        5D tensor with shape: `(samples, channels, dim1, dim2, dim3)` if
-            data_format='channels_first'
-        or 5D tensor with shape: `(samples, dim1, dim2, dim3, channels)` if
-            data_format='channels_last'.
+def train_validation_split(arrays, validation_split):
+    """Split arrays into train and validation subsets in deterministic order.
 
-    Output shape: Same as input.
+    The last part of data will become validation data.
 
-    Reference:
+    Args:
+        arrays: Tensors to split. Allowed inputs are arbitrarily nested
+            structures of Tensors and NumPy arrays.
+        validation_split: Float between 0 and 1. The proportion of the dataset
+            to include in the validation split. The rest of the dataset will be
+            included in the training split.
 
-    - [Tompson et al., 2014](https://arxiv.org/abs/1411.4280)
+    Returns:
+        `(train_arrays, validation_arrays)`
     """
 
-    def __init__(
-        self, rate, data_format=None, seed=None, name=None, dtype=None
-    ):
-        super().__init__(rate, seed=seed, name=name, dtype=dtype)
-        self.data_format = backend.standardize_data_format(data_format)
-        self.input_spec = InputSpec(ndim=5)
-
-    def _get_noise_shape(self, inputs):
-        input_shape = ops.shape(inputs)
-        if self.data_format == "channels_first":
-            return (input_shape[0], input_shape[1], 1, 1, 1)
-        elif self.data_format == "channels_last":
-            return (input_shape[0], 1, 1, 1, input_shape[4])
-
-    def get_config(self):
-        base_config = super().get_config()
-        config = {
-            "data_format": self.data_format,
-        }
-        return {**base_config, **config}
+    def _can_split(t):
+        return isinstance(t, ARRAY_TYPES) or t is None
+
+    flat_arrays = tree.flatten(arrays)
+    unsplitable = [type(t) for t in flat_arrays if not _can_split(t)]
+    if unsplitable:
+        raise ValueError(
+            "Argument `validation_split` is only supported "
+            "for tensors or NumPy "
+            "arrays. Found incompatible type in the input: {unsplitable}"
+        )
+
+    if all(t is None for t in flat_arrays):
+        return arrays, arrays
+
+    first_non_none = None
+    for t in flat_arrays:
+        if t is not None:
+            first_non_none = t
+            break
+
+    # Assumes all arrays have the same batch shape or are `None`.
+    batch_dim = int(first_non_none.shape[0])
+    split_at = int(math.floor(batch_dim * (1.0 - validation_split)))
+
+    if split_at == 0 or split_at == batch_dim:
+        raise ValueError(
+            f"Training data contains {batch_dim} samples, which is not "
+            "sufficient to split it into a validation and training set as "
+            f"specified by `validation_split={validation_split}`. Either "
+            "provide more data, or a different value for the "
+            "`validation_split` argument."
+        )
+
+    def _split(t, start, end):
+        if t is None:
+            return t
+        return t[start:end]
+
+    train_arrays = tree.map_structure(
+        lambda x: _split(x, start=0, end=split_at), arrays
+    )
+    val_arrays = tree.map_structure(
+        lambda x: _split(x, start=split_at, end=batch_dim), arrays
+    )
+    return train_arrays, val_arrays
+
+
+def class_weight_to_sample_weights(y, class_weight):
+    sample_weight = np.ones(shape=(y.shape[0],), dtype=y.dtype)
+    if len(y.shape) > 1:
+        if y.shape[-1] != 1:
+            y = np.argmax(y, axis=-1)
+        else:
+            y = np.squeeze(y, axis=-1)
+    y = np.round(y).astype("int32")
+    for i in range(y.shape[0]):
+        sample_weight[i] = class_weight.get(int(y[i]), 1.0)
+    return sample_weight
```

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/cropping1d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/cropping2d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/cropping3d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/flatten.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/permute.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/repeat_vector.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/reshape.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling1d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling2d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/up_sampling3d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding1d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding2d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/reshaping/zero_padding3d.py` & `keras-core-0.1.4/keras_core/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/bidirectional.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm1d.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm2d.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/conv_lstm3d.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/dropout_rnn_cell.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/gru.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/lstm.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/rnn.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/simple_rnn.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/stacked_rnn_cells.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/layers/rnn/time_distributed.py` & `keras-core-0.1.4/keras_core/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/backend.py` & `keras-core-0.1.4/keras_core/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/layers.py` & `keras-core-0.1.4/keras_core/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/losses.py` & `keras-core-0.1.4/keras_core/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/preprocessing/image.py` & `keras-core-0.1.4/keras_core/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/preprocessing/sequence.py` & `keras-core-0.1.4/keras_core/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/preprocessing/text.py` & `keras-core-0.1.4/keras_core/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/saving/json_utils.py` & `keras-core-0.1.4/keras_core/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/saving/legacy_h5_format.py` & `keras-core-0.1.4/keras_core/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/saving/saving_utils.py` & `keras-core-0.1.4/keras_core/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/legacy/saving/serialization.py` & `keras-core-0.1.4/keras_core/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/losses/__init__.py` & `keras-core-0.1.4/keras_core/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/losses/loss.py` & `keras-core-0.1.4/keras_core/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/losses/losses.py` & `keras-core-0.1.4/keras_core/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/__init__.py` & `keras-core-0.1.4/keras_core/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/accuracy_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/confusion_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/f_score_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/hinge_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/iou_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/metric.py` & `keras-core-0.1.4/keras_core/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/metrics_utils.py` & `keras-core-0.1.4/keras_core/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/probabilistic_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/metrics/reduction_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/reduction_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,18 @@
     >>> m.result()
     4.0
     """
 
     def __init__(self, name="sum", dtype=None):
         super().__init__(name=name, dtype=dtype)
         self.total = self.add_variable(
-            shape=(), initializer=initializers.Zeros(), dtype=self.dtype
+            shape=(),
+            initializer=initializers.Zeros(),
+            dtype=self.dtype,
+            name="total",
         )
 
     def update_state(self, values, sample_weight=None):
         values, _ = reduce_to_samplewise_values(
             values, sample_weight, reduce_fn=ops.sum, dtype=self.dtype
         )
         self.total.assign(self.total + ops.sum(values))
@@ -111,18 +114,24 @@
     2.0
     ```
     """
 
     def __init__(self, name="mean", dtype=None):
         super().__init__(name=name, dtype=dtype)
         self.total = self.add_variable(
-            shape=(), initializer=initializers.Zeros(), dtype=self.dtype
+            shape=(),
+            initializer=initializers.Zeros(),
+            dtype=self.dtype,
+            name="total",
         )
         self.count = self.add_variable(
-            shape=(), initializer=initializers.Zeros(), dtype=self.dtype
+            shape=(),
+            initializer=initializers.Zeros(),
+            dtype=self.dtype,
+            name="count",
         )
 
     def update_state(self, values, sample_weight=None):
         values, sample_weight = reduce_to_samplewise_values(
             values, sample_weight, reduce_fn=ops.mean, dtype=self.dtype
         )
         self.total.assign(self.total + ops.sum(values))
```

### Comparing `keras-core-0.1.3/keras_core/src/metrics/regression_metrics.py` & `keras-core-0.1.4/keras_core/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/mixed_precision/__init__.py` & `keras-core-0.1.4/keras_core/src/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/mixed_precision/dtype_policy.py` & `keras-core-0.1.4/keras_core/src/mixed_precision/dtype_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,24 +160,24 @@
             raise ValueError(
                 "Invalid `policy` argument. "
                 "Expected the string name of a policy "
                 "(such as 'mixed_float16') or a `DTypePolicy` "
                 f"instance. Received: policy={policy} "
                 f"(of type {type(policy)})"
             )
-    global_state.set_global_setting("dtype_policy", policy)
+    global_state.set_global_attribute("dtype_policy", policy)
 
 
 @keras_core_export(
     [
         "keras_core.mixed_precision.dtype_policy",
         "keras_core.mixed_precision.global_policy",
     ]
 )
 def dtype_policy():
     """Returns the current default dtype policy object."""
-    policy = global_state.get_global_setting("dtype_policy", None)
+    policy = global_state.get_global_attribute("dtype_policy", None)
     if policy is None:
         policy = DTypePolicy(backend.floatx())
         set_dtype_policy(policy)
     return policy
```

### Comparing `keras-core-0.1.3/keras_core/src/models/cloning.py` & `keras-core-0.1.4/keras_core/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/models/functional.py` & `keras-core-0.1.4/keras_core/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/models/model.py` & `keras-core-0.1.4/keras_core/src/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import warnings
 
 from keras_core.src import backend
 from keras_core.src import utils
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
+from keras_core.src.models.variable_mapping import map_trackable_variables
 from keras_core.src.saving import saving_api
 from keras_core.src.saving import saving_lib
 from keras_core.src.trainers import trainer as base_trainer
 from keras_core.src.utils import io_utils
 from keras_core.src.utils import summary_utils
 from keras_core.src.utils import traceback_utils
 
@@ -503,14 +504,21 @@
                 "`from_config(cls, config)` class method to specify "
                 "how to create an "
                 f"instance of {cls.__name__} from its config.\n\n"
                 f"Received config={config}\n\n"
                 f"Error encountered during deserialization: {e}"
             )
 
+    def _get_variable_map(self):
+        store = {}
+        map_trackable_variables(
+            self, store=store, inner_path="", visited_trackables=set()
+        )
+        return store
+
 
 @keras_core_export("keras_core.models.model_from_json")
 def model_from_json(json_string, custom_objects=None):
     """Parses a JSON model configuration string and returns a model instance.
 
     Usage:
```

### Comparing `keras-core-0.1.3/keras_core/src/models/sequential.py` & `keras-core-0.1.4/keras_core/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/__init__.py` & `keras-core-0.1.4/keras_core/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/core.py` & `keras-core-0.1.4/keras_core/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/function.py` & `keras-core-0.1.4/keras_core/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/image.py` & `keras-core-0.1.4/keras_core/src/ops/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,16 @@
         size,
         strides=None,
         dilation_rate=1,
         padding="valid",
         data_format="channels_last",
     ):
         super().__init__()
+        if isinstance(size, int):
+            size = (size, size)
         self.size = size
         self.strides = strides
         self.dilation_rate = dilation_rate
         self.padding = padding
         self.data_format = data_format
 
     def call(self, image):
@@ -344,22 +346,24 @@
             `"channels_last"`.
 
     Returns:
         Extracted patches 3D (if not batched) or 4D (if batched)
 
     Examples:
 
-    >>> image = np.random.random((1, 20, 20, 3)) # batch of 2 RGB images
+    >>> image = np.random.random(
+    ...     (2, 20, 20, 3)
+    ... ).astype("float32") # batch of 2 RGB images
     >>> patches = keras_core.ops.image.extract_patches(image, (5, 5))
     >>> patches.shape
-    (1, 4, 4, 75)
-    >>> image = np.random.random((20, 20, 3)) # batch of 2 RGB images
+    (2, 4, 4, 75)
+    >>> image = np.random.random((20, 20, 3)).astype("float32") # 1 RGB image
     >>> patches = keras_core.ops.image.extract_patches(image, (3, 3), (1, 1))
     >>> patches.shape
-    (4, 4, 75)
+    (18, 18, 27)
     """
     if any_symbolic_tensors((image,)):
         return ExtractPatches(
             size=size,
             strides=strides,
             dilation_rate=dilation_rate,
             padding=padding,
```

### Comparing `keras-core-0.1.3/keras_core/src/ops/math.py` & `keras-core-0.1.4/keras_core/src/ops/math.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,66 @@
     if any_symbolic_tensors((data,)):
         return SegmentSum(num_segments, sorted).symbolic_call(data, segment_ids)
     return backend.math.segment_sum(
         data, segment_ids, num_segments=num_segments, sorted=sorted
     )
 
 
+class SegmentMax(Operation):
+    def __init__(self, num_segments=None, sorted=False):
+        super().__init__()
+        self.num_segments = num_segments
+        self.sorted = sorted
+
+    def compute_output_spec(self, data, segment_ids):
+        num_segments = self.num_segments
+        output_shape = (num_segments,) + tuple(data.shape[1:])
+        return KerasTensor(shape=output_shape, dtype=data.dtype)
+
+    def call(self, data, segment_ids):
+        return backend.math.segment_max(
+            data,
+            segment_ids,
+            num_segments=self.num_segments,
+            sorted=self.sorted,
+        )
+
+
+@keras_core_export("keras_core.ops.segment_max")
+def segment_max(data, segment_ids, num_segments=None, sorted=False):
+    """Computes the max of segments in a tensor.
+
+    Args:
+        data: Input tensor.
+        segment_ids: A 1-D tensor containing segment indices for each
+            element in `data`.
+        num_segments: An integer representing the total number of
+            segments. If not specified, it is inferred from the maximum
+            value in `segment_ids`.
+        sorted: A boolean indicating whether `segment_ids` is sorted.
+            Default is `False`.
+
+    Returns:
+        A tensor containing the max of segments, where each element
+        represents the max of the corresponding segment in `data`.
+
+    Example:
+
+    >>> data = keras_core.ops.convert_to_tensor([1, 2, 3, 4, 5, 6])
+    >>> segment_ids = keras_core.ops.convert_to_tensor([0, 1, 0, 1, 0, 1])
+    >>> segment_max(data, segment_ids)
+    array([9 12], shape=(2,), dtype=int32)
+    """
+    if any_symbolic_tensors((data,)):
+        return SegmentSum(num_segments, sorted).symbolic_call(data, segment_ids)
+    return backend.math.segment_max(
+        data, segment_ids, num_segments=num_segments, sorted=sorted
+    )
+
+
 class TopK(Operation):
     def __init__(self, k, sorted=False):
         super().__init__()
         self.k = k
         self.sorted = sorted
 
     def compute_output_spec(self, x):
```

### Comparing `keras-core-0.1.3/keras_core/src/ops/nn.py` & `keras-core-0.1.4/keras_core/src/ops/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,32 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.relu", "keras_core.ops.nn.relu"])
 def relu(x):
+    """Rectified linear unit activation function.
+
+    It is defined as `f(x) = max(0, x)`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_relu = keras_core.ops.relu(x)
+    >>> print(x_relu)
+    array([0., 0., 1.], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Relu().symbolic_call(x)
     return backend.nn.relu(x)
 
 
 class Relu6(Operation):
     def call(self, x):
@@ -33,14 +51,32 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.relu6", "keras_core.ops.nn.relu6"])
 def relu6(x):
+    """Rectified linear unit activation function with upper bound of 6.
+
+    It is defined as `f(x) = np.clip(x, 0, 6)`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1., 6., 7.])
+    >>> x_relu6 = keras_core.ops.relu6(x)
+    >>> print(x_relu6)
+    array([0., 0., 1., 6., 6.], shape=(5,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Relu6().symbolic_call(x)
     return backend.nn.relu6(x)
 
 
 class Sigmoid(Operation):
     def call(self, x):
@@ -48,44 +84,66 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.sigmoid", "keras_core.ops.nn.sigmoid"])
 def sigmoid(x):
-    if any_symbolic_tensors((x,)):
-        return Sigmoid().symbolic_call(x)
-    return backend.nn.sigmoid(x)
+    """Sigmoid activation function.
 
+    It is defined as `f(x) = 1 / (1 + exp(-x))`.
 
-class Tanh(Operation):
-    def call(self, x):
-        return backend.nn.tanh(x)
+    Args:
+        x: Input tensor.
 
-    def compute_output_spec(self, x):
-        return KerasTensor(x.shape, dtype=x.dtype)
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
 
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_sigmoid = keras_core.ops.sigmoid(x)
+    >>> print(x_sigmoid)
+    array([0.26894143, 0.5, 0.7310586 ], dtype=float64)
 
-@keras_core_export(["keras_core.ops.tanh", "keras_core.ops.nn.tanh"])
-def tanh(x):
+    """
     if any_symbolic_tensors((x,)):
-        return Tanh().symbolic_call(x)
-    return backend.nn.tanh(x)
+        return Sigmoid().symbolic_call(x)
+    return backend.nn.sigmoid(x)
 
 
 class Softplus(Operation):
     def call(self, x):
         return backend.nn.softplus(x)
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.softplus", "keras_core.ops.nn.softplus"])
 def softplus(x):
+    """Softplus activation function.
+
+    It is defined as `f(x) = log(exp(x) + 1)`, where `log` is the natural
+    logarithm and `exp` is the exponential function.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_softplus = keras_core.ops.softplus(x)
+    >>> print(x_softplus)
+    array([0.31326166, 0.6931472 , 1.3132616 ], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Softplus().symbolic_call(x)
     return backend.nn.softplus(x)
 
 
 class Softsign(Operation):
     def call(self, x):
@@ -93,14 +151,32 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.softsign", "keras_core.ops.nn.softsign"])
 def softsign(x):
+    """Softsign activation function.
+
+    It is defined as `f(x) = x / (abs(x) + 1)`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_softsign = keras_core.ops.softsign(x)
+    >>> print(x_softsign)
+    array([-0.5, 0., 0.5], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Softsign().symbolic_call(x)
     return backend.nn.softsign(x)
 
 
 class Silu(Operation):
     def call(self, x):
@@ -108,14 +184,32 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.silu", "keras_core.ops.nn.silu"])
 def silu(x):
+    """Sigmoid-weighted linear unit activation function.
+
+    It is defined as `f(x) = x * sigmoid(x)`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_silu = keras_core.ops.silu(x)
+    >>> print(x_silu)
+    array([-0.26894143, 0., 0.7310586], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Silu().symbolic_call(x)
     return backend.nn.silu(x)
 
 
 class Swish(Operation):
     def call(self, x):
@@ -143,14 +237,32 @@
 @keras_core_export(
     [
         "keras_core.ops.log_sigmoid",
         "keras_core.ops.nn.log_sigmoid",
     ]
 )
 def log_sigmoid(x):
+    """Logarithm of the sigmoid activation function.
+
+    It is defined as `f(x) = log(1 / (1 + exp(-x)))`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_log_sigmoid = keras_core.ops.log_sigmoid(x)
+    >>> print(x_log_sigmoid)
+    array([-1.3132616, -0.6931472, -0.3132616], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return LogSigmoid().symbolic_call(x)
     return backend.nn.log_sigmoid(x)
 
 
 class LeakyRelu(Operation):
     def __init__(self, negative_slope=0.2):
@@ -164,14 +276,36 @@
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(
     ["keras_core.ops.leaky_relu", "keras_core.ops.nn.leaky_relu"]
 )
 def leaky_relu(x, negative_slope=0.2):
+    """Leaky version of a Rectified Linear Unit.
+
+    It allows a small gradient when the unit is not active, it is defined as:
+
+    `f(x) = alpha * x for x < 0` or `f(x) = x for x >= 0`.
+
+    Args:
+        x: Input tensor.
+        negative_slope: Slope of the activation function at x < 0.
+            Defaults to `0.2`.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_leaky_relu = keras_core.ops.leaky_relu(x)
+    >>> print(x_leaky_relu)
+    array([-0.2,  0. ,  1. ], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return LeakyRelu(negative_slope).symbolic_call(x)
     return backend.nn.leaky_relu(x, negative_slope=negative_slope)
 
 
 class HardSigmoid(Operation):
     def call(self, x):
@@ -184,14 +318,34 @@
 @keras_core_export(
     [
         "keras_core.ops.hard_sigmoid",
         "keras_core.ops.nn.hard_sigmoid",
     ]
 )
 def hard_sigmoid(x):
+    """Hard sigmoid activation function.
+
+    It is defined as:
+
+    `0 if x < -2.5`, `1 if x > 2.5`, `(0.2 * x) + 0.5 if -2.5 <= x <= 2.5`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_hard_sigmoid = keras_core.ops.hard_sigmoid(x)
+    >>> print(x_hard_sigmoid)
+    array([0.3, 0.5, 0.7], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return HardSigmoid().symbolic_call(x)
     return backend.nn.hard_sigmoid(x)
 
 
 class Elu(Operation):
     def __init__(self, alpha=1.0):
@@ -203,14 +357,35 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.elu", "keras_core.ops.nn.elu"])
 def elu(x, alpha=1.0):
+    """Exponential Linear Unit.
+
+    It is defined as:
+
+    `f(x) =  alpha * (exp(x) - 1.) for x < 0`, `f(x) = x for x >= 0`.
+
+    Args:
+        x: Input tensor.
+        alpha: A scalar, slope of positive section. Defaults to `1.0`.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_elu = keras_core.ops.elu(x)
+    >>> print(x_elu)
+    array([-0.63212055, 0., 1.], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Elu(alpha).symbolic_call(x)
     return backend.nn.elu(x, alpha=alpha)
 
 
 class Selu(Operation):
     def call(self, x):
@@ -218,14 +393,35 @@
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.selu", "keras_core.ops.nn.selu"])
 def selu(x):
+    """Scaled Exponential Linear Unit (SELU).
+
+    It is defined as:
+
+    `f(x) =  scale * alpha * (exp(x) - 1.) for x < 0`,
+    `f(x) = scale * x for x >= 0`.
+
+    Args:
+        x: Input tensor.
+
+    Returns:
+        A tensor with the same shape as `x`.
+
+    Example:
+
+    >>> x = np.array([-1., 0., 1.])
+    >>> x_selu = keras_core.ops.selu(x)
+    >>> print(x_selu)
+    array([-1.11133055, 0., 1.05070098], shape=(3,), dtype=float64)
+
+    """
     if any_symbolic_tensors((x,)):
         return Selu().symbolic_call(x)
     return backend.nn.selu(x)
 
 
 class Gelu(Operation):
     def __init__(self, approximate=True):
```

### Comparing `keras-core-0.1.3/keras_core/src/ops/node.py` & `keras-core-0.1.4/keras_core/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/numpy.py` & `keras-core-0.1.4/keras_core/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,38 +6,43 @@
 add
 all
 amax
 amin
 append
 arange
 arccos
+arccosh
 arcsin
+arcsinh
 arctan
 arctan2
+arctanh
 argmax
 argmin
 argsort
 array
 average
 bincount
 broadcast_to
 ceil
 clip
 concatenate
 conj
 conjugate
 copy
 cos
+cosh
 count_nonzero
 cross
 cumprod
 cumsum
 diag
 diagonal
 diff
+digitize
 divide
 dot
 dtype
 einsum
 empty
 equal
 exp
@@ -98,28 +103,30 @@
 reciprocal
 repeat
 reshape
 roll
 round
 sign
 sin
+sinh
 size
 sort
 split
 sqrt
 square
 squeeze
 stack
 std
 subtract
 sum
 swapaxes
 take
 take_along_axis
 tan
+tanh
 tensordot
 tile
 trace
 transpose
 tri
 tril
 triu
@@ -709,14 +716,36 @@
     array([0., 3.1415927], dtype=float32)
     """
     if any_symbolic_tensors((x,)):
         return Arccos().symbolic_call(x)
     return backend.numpy.arccos(x)
 
 
+class Arccosh(Operation):
+    def call(self, x):
+        return backend.numpy.arccosh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+def arccosh(x):
+    """Inverse hyperbolic cosine, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Arccosh().symbolic_call(x)
+    return backend.numpy.arccosh(x)
+
+
 class Arcsin(Operation):
     def call(self, x):
         return backend.numpy.arcsin(x)
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
@@ -738,14 +767,37 @@
     array([ 1.5707964, -1.5707964,  0.], dtype=float32)
     """
     if any_symbolic_tensors((x,)):
         return Arcsin().symbolic_call(x)
     return backend.numpy.arcsin(x)
 
 
+class Arcsinh(Operation):
+    def call(self, x):
+        return backend.numpy.arcsinh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+@keras_core_export(["keras_core.ops.arcsinh", "keras_core.ops.numpy.arcsinh"])
+def arcsinh(x):
+    """Inverse hyperbolic sine, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Arcsinh().symbolic_call(x)
+    return backend.numpy.arcsinh(x)
+
+
 class Arctan(Operation):
     def call(self, x):
         return backend.numpy.arctan(x)
 
     def compute_output_spec(self, x):
         return KerasTensor(x.shape, dtype=x.dtype)
 
@@ -822,14 +874,37 @@
     array([0., 3.1415925, 0.7853982], dtype=float32)
     """
     if any_symbolic_tensors((x1, x2)):
         return Arctan2().symbolic_call(x1, x2)
     return backend.numpy.arctan2(x1, x2)
 
 
+class Arctanh(Operation):
+    def call(self, x):
+        return backend.numpy.arctanh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+@keras_core_export(["keras_core.ops.arctanh", "keras_core.ops.numpy.arctanh"])
+def arctanh(x):
+    """Inverse hyperbolic tangent, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Arctanh().symbolic_call(x)
+    return backend.numpy.arctanh(x)
+
+
 class Argmax(Operation):
     def __init__(self, axis=None):
         super().__init__()
         self.axis = axis
 
     def call(self, x):
         return backend.numpy.argmax(x, axis=self.axis)
@@ -1050,15 +1125,15 @@
 @keras_core_export(["keras_core.ops.average", "keras_core.ops.numpy.average"])
 def average(x, axis=None, weights=None):
     """Compute the weighted average along the specified axis.
 
     Args:
         x: Input tensor.
         axis: Integer along which to average `x`. The default, `axis=None`,
-            will average over all of the elements of the input tendor. If axis
+            will average over all of the elements of the input tensor. If axis
             is negative it counts from the last to the first axis.
         weights: Tensor of wieghts associated with the values in `x`. Each
             value in `x` contributes to the average according to its
             associated weight. The weights array can either be 1-D (in which
             case its length must be the size of a along the given axis) or of
             the same shape as `x`. If `weights=None` (default), then all data
             in `x` are assumed to have a weight equal to one.
@@ -1119,14 +1194,48 @@
     def compute_output_spec(self, x):
         out_shape = backend.numpy.amax(x) + 1
         return KerasTensor(out_shape, dtype=x.dtype)
 
 
 @keras_core_export(["keras_core.ops.bincount", "keras_core.ops.numpy.bincount"])
 def bincount(x, weights=None, minlength=0):
+    """Count the number of occurrences of each value in a tensor of integers.
+
+    Args:
+        x: Input tensor.
+            It must be of dimension 1, and it must only contain non-negative
+            integer(s).
+        weights: Weight tensor.
+            It must have the same length as `x`. The default value is `None`.
+            If specified, `x` is weighted by it, i.e. if `n = x[i]`,
+            `out[n] += weight[i]` instead of the default behavior `out[n] += 1`.
+        minlength: An integer.
+            The default value is 0. If specified, there will be at least
+            this number of bins in the output tensor. If greater than
+            `max(x) + 1`, each value of the output at an index higher than
+            `max(x)` is set to 0.
+
+    Returns:
+        1D tensor where each element gives the number of occurrence(s) of its
+        index value in x. Its length is the maximum between `max(x) + 1` and
+        minlength.
+
+    Examples:
+    >>> x = keras_core.ops.array([1, 2, 2, 3], dtype="uint8")
+    >>> keras_core.ops.bincount(x)
+    array([0, 1, 2, 1], dtype=int32)
+    >>> weights = x / 2
+    >>> weights
+    array([0.5, 1., 1., 1.5], dtype=float64)
+    >>> keras_core.ops.bincount(x, weights=weights)
+    array([0., 0.5, 2., 1.5], dtype=float64)
+    >>> minlength = (keras_core.ops.max(x).numpy() + 1) + 2 # 6
+    >>> keras_core.ops.bincount(x, minlength=minlength)
+    array([0, 1, 2, 1, 0, 0], dtype=int32)
+    """
     if any_symbolic_tensors((x,)):
         return Bincount(weights=weights, minlength=minlength).symbolic_call(x)
     return backend.numpy.bincount(x, weights=weights, minlength=minlength)
 
 
 class BroadcastTo(Operation):
     def __init__(self, shape):
@@ -1285,14 +1394,37 @@
 @keras_core_export(["keras_core.ops.cos", "keras_core.ops.numpy.cos"])
 def cos(x):
     if any_symbolic_tensors((x,)):
         return Cos().symbolic_call(x)
     return backend.numpy.cos(x)
 
 
+class Cosh(Operation):
+    def call(self, x):
+        return backend.numpy.cosh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+@keras_core_export(["keras_core.ops.cosh", "keras_core.ops.numpy.cosh"])
+def cosh(x):
+    """Hyperbolic cosine, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Cosh().symbolic_call(x)
+    return backend.numpy.cosh(x)
+
+
 class CountNonzero(Operation):
     def __init__(self, axis=None):
         super().__init__()
         if isinstance(axis, int):
             self.axis = (axis,)
         else:
             self.axis = axis
@@ -1530,14 +1662,52 @@
         x,
         offset=offset,
         axis1=axis1,
         axis2=axis2,
     )
 
 
+class Digitize(Operation):
+    def call(self, x, bins):
+        return backend.numpy.digitize(x, bins)
+
+    def compute_output_spec(self, x, bins):
+        bins_shape = bins.shape
+        if len(bins_shape) > 1:
+            raise ValueError(
+                f"`bins` must be a 1D array. Received: bins={bins} "
+                f"with shape bins.shape={bins_shape}"
+            )
+        return KerasTensor(x.shape, dtype="int32")
+
+
+@keras_core_export(["keras_core.ops.digitize", "keras_core.ops.numpy.digitize"])
+def digitize(x, bins):
+    """Returns the indices of the bins to which each value in `x` belongs.
+
+    Args:
+        x: Input array to be binned.
+        bins: Array of bins. It has to be one-dimensional and monotonically
+            increasing.
+
+    Returns:
+        Output array of indices, of same shape as x.
+
+    Example:
+
+    >>> x = np.array([0.0, 1.0, 3.0, 1.6])
+    >>> bins = np.array([0.0, 3.0, 4.5, 7.0])
+    >>> keras_core.ops.digitize(x, bins)
+    array([1, 1, 2, 1])
+    """
+    if any_symbolic_tensors((x, bins)):
+        return Digitize().symbolic_call(x, bins)
+    return backend.numpy.digitize(x, bins)
+
+
 class Dot(Operation):
     def call(self, x1, x2):
         return backend.numpy.dot(x1, x2)
 
     def compute_output_spec(self, x1, x2):
         x1_shape = list(getattr(x1, "shape", []))
         x2_shape = list(getattr(x2, "shape", []))
@@ -3111,14 +3281,37 @@
 @keras_core_export(["keras_core.ops.sin", "keras_core.ops.numpy.sin"])
 def sin(x):
     if any_symbolic_tensors((x,)):
         return Sin().symbolic_call(x)
     return backend.numpy.sin(x)
 
 
+class Sinh(Operation):
+    def call(self, x):
+        return backend.numpy.sinh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+@keras_core_export(["keras_core.ops.sinh", "keras_core.ops.numpy.sinh"])
+def sinh(x):
+    """Hyperbolic sine, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Sinh().symbolic_call(x)
+    return backend.numpy.sinh(x)
+
+
 class Size(Operation):
     def call(self, x):
         return backend.numpy.size(x)
 
     def compute_output_spec(self, x):
         return KerasTensor([], dtype="int32")
 
@@ -3372,14 +3565,37 @@
 @keras_core_export(["keras_core.ops.tan", "keras_core.ops.numpy.tan"])
 def tan(x):
     if any_symbolic_tensors((x,)):
         return Tan().symbolic_call(x)
     return backend.numpy.tan(x)
 
 
+class Tanh(Operation):
+    def call(self, x):
+        return backend.numpy.tanh(x)
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
+
+
+@keras_core_export(["keras_core.ops.tanh", "keras_core.ops.numpy.tanh"])
+def tanh(x):
+    """Hyperbolic tangent, element-wise.
+
+    Arguments:
+        x: Input tensor.
+
+    Returns:
+        Output tensor of same shape as x.
+    """
+    if any_symbolic_tensors((x,)):
+        return Tanh().symbolic_call(x)
+    return backend.numpy.tanh(x)
+
+
 class Tensordot(Operation):
     def __init__(self, axes=2):
         super().__init__()
         self.axes = axes
 
     def call(self, x1, x2):
         return backend.numpy.tensordot(x1, x2, axes=self.axes)
```

### Comparing `keras-core-0.1.3/keras_core/src/ops/operation.py` & `keras-core-0.1.4/keras_core/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/operation_utils.py` & `keras-core-0.1.4/keras_core/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/ops/symbolic_arguments.py` & `keras-core-0.1.4/keras_core/src/ops/symbolic_arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class SymbolicArguments:
     def __init__(self, *args, **kwargs):
         self.args = tree.map_structure(lambda x: x, args)
         self.kwargs = tree.map_structure(lambda x: x, kwargs)
         self._flat_arguments = tree.flatten((self.args, self.kwargs))
 
-        # Used to avoid expensive `nest` operations in the most common case.
+        # Used to avoid expensive `tree` operations in the most common case.
         if (
             not self.kwargs
             and len(self.args) == 1
             and isinstance(self.args[0], KerasTensor)
         ):
             self._single_positional_tensor = self.args[0]
         else:
```

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/__init__.py` & `keras-core-0.1.4/keras_core/src/optimizers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from keras_core.src.optimizers.adadelta import Adadelta
 from keras_core.src.optimizers.adafactor import Adafactor
 from keras_core.src.optimizers.adagrad import Adagrad
 from keras_core.src.optimizers.adam import Adam
 from keras_core.src.optimizers.adamax import Adamax
 from keras_core.src.optimizers.adamw import AdamW
 from keras_core.src.optimizers.ftrl import Ftrl
+from keras_core.src.optimizers.lion import Lion
 from keras_core.src.optimizers.nadam import Nadam
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.optimizers.rmsprop import RMSprop
 from keras_core.src.optimizers.sgd import SGD
 from keras_core.src.saving import serialization_lib
 
 ALL_OBJECTS = {
@@ -20,14 +21,15 @@
     Adadelta,
     AdamW,
     Adagrad,
     Adamax,
     Adafactor,
     Nadam,
     Ftrl,
+    Lion,
 }
 ALL_OBJECTS_DICT = {cls.__name__.lower(): cls for cls in ALL_OBJECTS}
 
 
 @keras_core_export("keras_core.optimizers.serialize")
 def serialize(optimizer):
     """Returns the optimizer configuration as a Python dict.
```

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adadelta.py` & `keras-core-0.1.4/keras_core/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adafactor.py` & `keras-core-0.1.4/keras_core/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adagrad.py` & `keras-core-0.1.4/keras_core/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adam.py` & `keras-core-0.1.4/keras_core/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adamax.py` & `keras-core-0.1.4/keras_core/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/adamw.py` & `keras-core-0.1.4/keras_core/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/base_optimizer.py` & `keras-core-0.1.4/keras_core/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/ftrl.py` & `keras-core-0.1.4/keras_core/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/nadam.py` & `keras-core-0.1.4/keras_core/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/optimizer.py` & `keras-core-0.1.4/keras_core/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/rmsprop.py` & `keras-core-0.1.4/keras_core/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/schedules/__init__.py` & `keras-core-0.1.4/keras_core/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/schedules/learning_rate_schedule.py` & `keras-core-0.1.4/keras_core/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/optimizers/sgd.py` & `keras-core-0.1.4/keras_core/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/random/random.py` & `keras-core-0.1.4/keras_core/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/regularizers/__init__.py` & `keras-core-0.1.4/keras_core/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/regularizers/regularizers.py` & `keras-core-0.1.4/keras_core/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/saving/__init__.py` & `keras-core-0.1.4/keras_core/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/saving/object_registration.py` & `keras-core-0.1.4/keras_core/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/saving/saving_api.py` & `keras-core-0.1.4/keras_core/src/saving/saving_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except ImportError:
     h5py = None
 
 
 @keras_core_export(
     ["keras_core.saving.save_model", "keras_core.models.save_model"]
 )
-def save_model(model, filepath, overwrite=True, save_format=None, **kwargs):
+def save_model(model, filepath, overwrite=True, **kwargs):
     """Saves a model as a `.keras` file.
 
     Args:
         model: Keras model instance to be saved.
         filepath: `str` or `pathlib.Path` object. Path where to save the model.
         overwrite: Whether we should overwrite any existing model at the target
             location, or instead ask the user via an interactive prompt.
@@ -48,52 +48,70 @@
 
     - The model's configuration (architecture)
     - The model's weights
     - The model's optimizer's state (if any)
 
     Thus models can be reinstantiated in the exact same state.
     """
-    save_format = get_save_format(filepath, save_format)
     include_optimizer = kwargs.pop("include_optimizer", True)
+    save_format = kwargs.pop("save_format", False)
+    if save_format:
+        if str(filepath).endswith((".h5", ".hdf5")) or str(filepath).endswith(
+            ".keras"
+        ):
+            logging.warning(
+                "The `save_format` argument is deprecated in Keras Core. "
+                "We recommend removing this argument as it can be inferred "
+                "from the file path. "
+                f"Received: save_format={save_format}"
+            )
+        else:
+            raise ValueError(
+                "The `save_format` argument is deprecated in Keras Core. "
+                "Please remove this argument and pass a file path with "
+                "either `.keras` or `.h5` extension."
+                f"Received: save_format={save_format}"
+            )
     if kwargs:
         raise ValueError(
             "The following argument(s) are not supported: "
             f"{list(kwargs.keys())}"
         )
 
     # Deprecation warnings
-    if save_format == "h5":
+    if str(filepath).endswith((".h5", ".hdf5")):
         logging.warning(
             "You are saving your model as an HDF5 file via `model.save()`. "
             "This file format is considered legacy. "
             "We recommend using instead the native Keras format, "
             "e.g. `model.save('my_model.keras')`."
         )
 
-    if save_format == "keras":
+    if str(filepath).endswith(".keras"):
         # If file exists and should not be overwritten.
         try:
             exists = os.path.exists(filepath)
         except TypeError:
             exists = False
         if exists and not overwrite:
             proceed = io_utils.ask_to_proceed_with_overwrite(filepath)
             if not proceed:
                 return
         saving_lib.save_model(model, filepath)
-    elif save_format == "h5":
+    elif str(filepath).endswith((".h5", ".hdf5")):
         legacy_h5_format.save_model_to_hdf5(
             model, filepath, overwrite, include_optimizer
         )
     else:
-        # TODO(nkovela): Replace code route when SavedModel format is supported
         raise ValueError(
             "Invalid filepath extension for saving. "
             "Please add either a `.keras` extension for the native Keras "
             f"format (recommended) or a `.h5` extension. "
+            "Use `tf.saved_model.save()` if you want to export a SavedModel "
+            "for use with TFLite/TFServing/etc. "
             f"Received: filepath = {filepath}."
         )
 
 
 @keras_core_export(
     ["keras_core.saving.load_model", "keras_core.models.load_model"]
 )
@@ -129,16 +147,14 @@
     ```
 
     Note that the model variables may have different name values
     (`var.name` property, e.g. `"dense_1/kernel:0"`) after being reloaded.
     It is recommended that you use layer attributes to
     access specific variables, e.g. `model.get_layer("dense_1").kernel`.
     """
-    save_format = get_save_format(filepath, save_format=None)
-
     is_keras_zip = str(filepath).endswith(".keras") and zipfile.is_zipfile(
         filepath
     )
 
     # Support for remote zip files
     if (
         file_utils.is_remote_path(filepath)
@@ -160,20 +176,29 @@
     if is_keras_zip:
         return saving_lib.load_model(
             filepath,
             custom_objects=custom_objects,
             compile=compile,
             safe_mode=safe_mode,
         )
-    if save_format == "h5":
+    if str(filepath).endswith((".h5", ".hdf5")):
         return legacy_h5_format.load_model_from_hdf5(filepath)
+    elif str(filepath).endswith(".keras"):
+        raise ValueError(
+            f"File not found: filepath={filepath}. "
+            "Please ensure the file is an accessible `.keras` "
+            "zip file."
+        )
     else:
-        # TODO(nkovela): Replace code route when SavedModel format is supported
-        raise NotImplementedError(
-            "The SavedModel format is not currently supported."
+        raise ValueError(
+            f"File format not supported: filepath={filepath}. "
+            "Keras Core only supports V3 `.keras` files and "
+            "legacy H5 format files (`.h5` extension). "
+            "Note that the legacy SavedModel format is not "
+            "supported in Keras Core."
         )
 
 
 def load_weights(model, filepath, skip_mismatch=False, **kwargs):
     if str(filepath).endswith(".keras"):
         if kwargs:
             raise ValueError(f"Invalid keyword arguments: {kwargs}")
@@ -206,42 +231,7 @@
     else:
         raise ValueError(
             f"File format not supported: filepath={filepath}. "
             "Keras Core only supports V3 `.keras` and `.weights.h5` "
             "files."
         )
 
-
-def get_save_format(filepath, save_format):
-    if save_format:
-        if save_format == "keras_v3":
-            return "keras"
-        if save_format == "keras":
-            return "keras"
-        else:
-            return "h5"
-        if save_format in ("h5", "hdf5"):
-            return "h5"
-        if save_format in ("tf", "tensorflow"):
-            return "tf"
-
-        raise ValueError(
-            "Unknown `save_format` argument. Expected one of "
-            "'keras', 'tf', or 'h5'. "
-            f"Received: save_format{save_format}"
-        )
-
-    # No save format specified: infer from filepath.
-
-    if str(filepath).endswith(".keras"):
-        return "keras"
-    else:
-        return "h5"
-
-    if str(filepath).endswith((".h5", ".hdf5")):
-        return "h5"
-
-    if h5py is not None and isinstance(filepath, h5py.File):
-        return "h5"
-
-    return "tf"
-
```

### Comparing `keras-core-0.1.3/keras_core/src/saving/saving_lib.py` & `keras-core-0.1.4/keras_core/src/saving/saving_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Python-based idempotent model-saving functionality."""
 
 import datetime
 import io
 import json
-import os
 import tempfile
 import warnings
 import zipfile
 
 import numpy as np
 
 from keras_core.src.backend.common import global_state
 from keras_core.src.layers.layer import Layer
 from keras_core.src.losses.loss import Loss
 from keras_core.src.metrics.metric import Metric
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.saving.serialization_lib import ObjectSharingScope
 from keras_core.src.saving.serialization_lib import deserialize_keras_object
 from keras_core.src.saving.serialization_lib import serialize_keras_object
+from keras_core.src.trainers.compile_utils import CompileMetrics
 from keras_core.src.utils import file_utils
 from keras_core.src.utils import naming
 from keras_core.src.version import __version__ as keras_version
 
 try:
     import h5py
 except ImportError:
@@ -81,16 +81,16 @@
     metadata_json = json.dumps(
         {
             "keras_version": keras_version,
             "date_saved": datetime.datetime.now().strftime("%Y-%m-%d@%H:%M:%S"),
         }
     )
     if file_utils.is_remote_path(filepath):
-        # Remote path. Zip to local drive and copy to remote
-        zip_filepath = os.path.join(get_temp_dir(), "tmp_model.keras")
+        # Remote path. Zip to local memory byte io and copy to remote
+        zip_filepath = io.BytesIO()
     else:
         zip_filepath = filepath
 
     with zipfile.ZipFile(zip_filepath, "w") as zf:
         with zf.open(_METADATA_FILENAME, "w") as f:
             f.write(metadata_json.encode())
         with zf.open(_CONFIG_FILENAME, "w") as f:
@@ -118,18 +118,16 @@
             inner_path="",
             visited_trackables=set(),
         )
         weights_store.close()
         asset_store.close()
 
     if file_utils.is_remote_path(filepath):
-        # Using gfile context manager doesn't close zip file when
-        # writing to GCS. Hence writing to local and copying to filepath.
-        file_utils.copy(zip_filepath, filepath, overwrite=True)
-        os.remove(zip_filepath)
+        with file_utils.File(filepath, "wb") as f:
+            f.write(zip_filepath.getvalue())
 
 
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
     """Load a zip archive representing a Keras model."""
 
     filepath = str(filepath)
     if not filepath.endswith(".keras"):
@@ -251,39 +249,50 @@
             zip_file_path = file_utils.join(zip_path, file_name)
             _write_to_zip_recursively(
                 zipfile_to_save, system_file_path, zip_file_path
             )
 
 
 def _walk_trackable(trackable):
-    if isinstance(trackable, Layer):
+    from keras_core.src.models import Functional
+    from keras_core.src.models import Sequential
+
+    if isinstance(trackable, Sequential):
+        obj_type = "Sequential"
+    elif isinstance(trackable, Functional):
+        obj_type = "Functional"
+    elif isinstance(trackable, Layer):
         obj_type = "Layer"
     elif isinstance(trackable, Optimizer):
         obj_type = "Optimizer"
     elif isinstance(trackable, Metric):
         obj_type = "Metric"
     elif isinstance(trackable, Loss):
         obj_type = "Loss"
     else:
         raise ValueError(f"Invalid obj_type: {obj_type}")
     attr_skiplist = get_attr_skiplist(obj_type)
 
-    for child_attr in dir(trackable):
+    for child_attr in sorted(dir(trackable)):
         if child_attr.startswith("__") or child_attr in attr_skiplist:
             continue
         try:
             child_obj = getattr(trackable, child_attr)
         except Exception:
             # Avoid raising the exception when visiting the attributes.
             continue
         yield child_attr, child_obj
 
 
 def _save_state(
-    trackable, weights_store, assets_store, inner_path, visited_trackables
+    trackable,
+    weights_store,
+    assets_store,
+    inner_path,
+    visited_trackables,
 ):
     # If the trackable has already been saved, skip it.
     if id(trackable) in visited_trackables:
         return
 
     if hasattr(trackable, "save_own_variables") and weights_store:
         trackable.save_own_variables(weights_store.make(inner_path))
@@ -591,27 +600,38 @@
 
 def get_attr_skiplist(obj_type):
     skiplist = global_state.get_global_attribute(
         f"saving_attr_skiplist_{obj_type}", None
     )
     if skiplist is not None:
         return skiplist
+
+    skiplist = [
+        "_self_unconditional_dependency_names",
+    ]
     if obj_type == "Layer":
         ref_obj = Layer()
-        skiplist = dir(ref_obj)
+        skiplist += dir(ref_obj)
+    elif obj_type == "Functional":
+        ref_obj = Layer()
+        skiplist += dir(ref_obj) + ["operations", "_operations"]
+    elif obj_type == "Sequential":
+        ref_obj = Layer()
+        skiplist += dir(ref_obj) + ["_functional"]
     elif obj_type == "Metric":
-        ref_obj = Metric()
-        skiplist = dir(ref_obj)
+        ref_obj_a = Metric()
+        ref_obj_b = CompileMetrics([], [])
+        skiplist += dir(ref_obj_a) + dir(ref_obj_b)
     elif obj_type == "Optimizer":
         ref_obj = Optimizer(1.0)
-        skiplist = dir(ref_obj)
+        skiplist += dir(ref_obj)
         skiplist.remove("variables")
     elif obj_type == "Loss":
         ref_obj = Loss()
-        skiplist = dir(ref_obj)
+        skiplist += dir(ref_obj)
     else:
         raise ValueError(f"Invalid obj_type: {obj_type}")
     global_state.set_global_attribute(
         f"saving_attr_skiplist_{obj_type}", skiplist
     )
     return skiplist
```

### Comparing `keras-core-0.1.3/keras_core/src/saving/serialization_lib.py` & `keras-core-0.1.4/keras_core/src/saving/serialization_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,28 +41,30 @@
     """Scope to propagate safe mode flag to nested deserialization calls."""
 
     def __init__(self, safe_mode=True):
         self.safe_mode = safe_mode
 
     def __enter__(self):
         self.original_value = in_safe_mode()
-        global_state.set_global_setting("safe_mode_saving", self.safe_mode)
+        global_state.set_global_attribute("safe_mode_saving", self.safe_mode)
 
     def __exit__(self, *args, **kwargs):
-        global_state.set_global_setting("safe_mode_saving", self.original_value)
+        global_state.set_global_attribute(
+            "safe_mode_saving", self.original_value
+        )
 
 
 @keras_core_export("keras_core.config.enable_unsafe_deserialization")
 def enable_unsafe_deserialization():
     """Disables safe mode globally, allowing deserialization of lambdas."""
-    global_state.set_global_setting("safe_mode_saving", False)
+    global_state.set_global_attribute("safe_mode_saving", False)
 
 
 def in_safe_mode():
-    return global_state.get_global_setting("safe_mode_saving")
+    return global_state.get_global_attribute("safe_mode_saving")
 
 
 class ObjectSharingScope:
     """Scope to enable detection and reuse of previously seen objects."""
 
     def __enter__(self):
         global_state.set_global_attribute("shared_objects/id_to_obj_map", {})
```

### Comparing `keras-core-0.1.3/keras_core/src/testing/test_case.py` & `keras-core-0.1.4/keras_core/src/testing/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,19 @@
                 json.loads(serialized_json)
             )
         revived_config = revived_instance.get_config()
         revived_config_json = json.dumps(
             revived_config, sort_keys=True, indent=4
         )
         self.assertEqual(config_json, revived_config_json)
-        self.assertEqual(ref_dir, dir(revived_instance))
+        new_dir = dir(revived_instance)[:]
+        for lst in [ref_dir, new_dir]:
+            if "__annotations__" in lst:
+                lst.remove("__annotations__")
+        self.assertEqual(ref_dir, new_dir)
         return revived_instance
 
     def run_layer_test(
         self,
         layer_cls,
         init_kwargs,
         input_shape=None,
```

### Comparing `keras-core-0.1.3/keras_core/src/testing/test_utils.py` & `keras-core-0.1.4/keras_core/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/compile_utils.py` & `keras-core-0.1.4/keras_core/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/array_data_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/data_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/generator_data_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/data_adapters/torch_data_adapter.py` & `keras-core-0.1.4/keras_core/src/trainers/data_adapters/torch_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/epoch_iterator.py` & `keras-core-0.1.4/keras_core/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/trainers/trainer.py` & `keras-core-0.1.4/keras_core/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/__init__.py` & `keras-core-0.1.4/keras_core/src/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from keras_core.src.utils.dataset_utils import audio_dataset_from_directory
-from keras_core.src.utils.dataset_utils import image_dataset_from_directory
+from keras_core.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras_core.src.utils.dataset_utils import split_dataset
-from keras_core.src.utils.dataset_utils import text_dataset_from_directory
-from keras_core.src.utils.dataset_utils import timeseries_dataset_from_array
 from keras_core.src.utils.file_utils import get_file
+from keras_core.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras_core.src.utils.image_utils import array_to_img
 from keras_core.src.utils.image_utils import img_to_array
 from keras_core.src.utils.image_utils import load_img
 from keras_core.src.utils.image_utils import save_img
 from keras_core.src.utils.io_utils import disable_interactive_logging
 from keras_core.src.utils.io_utils import enable_interactive_logging
 from keras_core.src.utils.io_utils import is_interactive_logging_enabled
@@ -18,8 +16,12 @@
 from keras_core.src.utils.progbar import Progbar
 from keras_core.src.utils.python_utils import default
 from keras_core.src.utils.python_utils import is_default
 from keras_core.src.utils.python_utils import removeprefix
 from keras_core.src.utils.python_utils import removesuffix
 from keras_core.src.utils.rng_utils import set_random_seed
 from keras_core.src.utils.sequence_utils import pad_sequences
+from keras_core.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras_core.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras-core-0.1.3/keras_core/src/utils/argument_validation.py` & `keras-core-0.1.4/keras_core/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/backend_utils.py` & `keras-core-0.1.4/keras_core/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/code_stats.py` & `keras-core-0.1.4/keras_core/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/dtype_utils.py` & `keras-core-0.1.4/keras_core/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/file_utils.py` & `keras-core-0.1.4/keras_core/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/image_utils.py` & `keras-core-0.1.4/keras_core/src/utils/image_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -382,36 +382,46 @@
     shape = backend_module.shape(img)
     if data_format == "channels_last":
         height, width = shape[-3], shape[-2]
     else:
         height, width = shape[-2], shape[-1]
     target_height, target_width = size
 
-    crop_height = backend_module.cast(
-        backend_module.cast(width * target_height, "float32") / target_width,
-        "int32",
-    )
-    crop_width = backend_module.cast(
-        backend_module.cast(height * target_width, "float32") / target_height,
-        "int32",
-    )
-
     # Set back to input height / width if crop_height / crop_width is not
     # smaller.
-    crop_height = backend_module.numpy.minimum(height, crop_height)
-    crop_width = backend_module.numpy.minimum(width, crop_width)
-    crop_height = backend_module.cast(crop_height, "int32")
-    crop_width = backend_module.cast(crop_width, "int32")
+    if isinstance(height, int) and isinstance(width, int):
+        # For JAX, we need to keep the slice indices as static integers
+        crop_height = int(float(width * target_height) / target_width)
+        crop_height = min(height, crop_height)
+        crop_width = int(float(height * target_width) / target_height)
+        crop_width = min(width, crop_width)
+        crop_box_hstart = int(float(height - crop_height) / 2)
+        crop_box_wstart = int(float(width - crop_width) / 2)
+    else:
+        crop_height = backend_module.cast(
+            backend_module.cast(width * target_height, "float32")
+            / target_width,
+            "int32",
+        )
+        crop_height = backend_module.numpy.minimum(height, crop_height)
+        crop_height = backend_module.cast(crop_height, "int32")
+        crop_width = backend_module.cast(
+            backend_module.cast(height * target_width, "float32")
+            / target_height,
+            "int32",
+        )
+        crop_width = backend_module.numpy.minimum(width, crop_width)
+        crop_width = backend_module.cast(crop_width, "int32")
 
-    crop_box_hstart = backend_module.cast(
-        backend_module.cast(height - crop_height, "float32") / 2, "int32"
-    )
-    crop_box_wstart = backend_module.cast(
-        backend_module.cast(width - crop_width, "float32") / 2, "int32"
-    )
+        crop_box_hstart = backend_module.cast(
+            backend_module.cast(height - crop_height, "float32") / 2, "int32"
+        )
+        crop_box_wstart = backend_module.cast(
+            backend_module.cast(width - crop_width, "float32") / 2, "int32"
+        )
 
     if data_format == "channels_last":
         if len(img.shape) == 4:
             img = img[
                 :,
                 crop_box_hstart : crop_box_hstart + crop_height,
                 crop_box_wstart : crop_box_wstart + crop_width,
```

### Comparing `keras-core-0.1.3/keras_core/src/utils/io_utils.py` & `keras-core-0.1.4/keras_core/src/utils/io_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def enable_interactive_logging():
     """Turn on interactive logging.
 
     When interactive logging is enabled, Keras displays logs via stdout.
     This provides the best experience when using Keras in an interactive
     environment such as a shell or a notebook.
     """
-    global_state.set_global_setting("interactive_logging", True)
+    global_state.set_global_attribute("interactive_logging", True)
 
 
 @keras_core_export(
     [
         "keras_core.config.disable_interactive_logging",
         "keras_core.utils.disable_interactive_logging",
     ]
@@ -31,15 +31,15 @@
 def disable_interactive_logging():
     """Turn off interactive logging.
 
     When interactive logging is disabled, Keras sends logs to `absl.logging`.
     This is the best option when using Keras in a non-interactive
     way, such as running a training or inference job on a server.
     """
-    global_state.set_global_setting("interactive_logging", False)
+    global_state.set_global_attribute("interactive_logging", False)
 
 
 @keras_core_export(
     [
         "keras_core.config.is_interactive_logging_enabled",
         "keras_core.utils.is_interactive_logging_enabled",
     ]
@@ -51,15 +51,15 @@
     `keras.config.enable_interactive_logging()` and
     `keras.config.disable_interactie_logging()`.
 
     Returns:
         Boolean, `True` if interactive logging is enabled,
         and `False` otherwise.
     """
-    return global_state.get_global_setting("interactive_logging", True)
+    return global_state.get_global_attribute("interactive_logging", True)
 
 
 def set_logging_verbosity(level):
     """Sets the verbosity level for logging.
 
     Supported log levels are as follows:
```

### Comparing `keras-core-0.1.3/keras_core/src/utils/model_visualization.py` & `keras-core-0.1.4/keras_core/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/module_utils.py` & `keras-core-0.1.4/keras_core/src/utils/module_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,18 @@
         except ImportError:
             raise ImportError(
                 f"This requires the {self.name} module. "
                 f"You can install it via `pip install {self.pip_name}`"
             )
 
     def __getattr__(self, name):
+        if name == "_api_export_path":
+            raise AttributeError
         if self.module is None:
             self.initialize()
         return getattr(self.module, name)
 
 
 tensorflow = LazyModule("tensorflow")
-gfile = LazyModule("tensorflow.io.gfile")
+gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
+tensorflow_io = LazyModule("tensorflow_io")
```

### Comparing `keras-core-0.1.3/keras_core/src/utils/naming.py` & `keras-core-0.1.4/keras_core/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/nest.py` & `keras-core-0.1.4/keras_core/src/utils/nest.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/numerical_utils.py` & `keras-core-0.1.4/keras_core/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/progbar.py` & `keras-core-0.1.4/keras_core/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/python_utils.py` & `keras-core-0.1.4/keras_core/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/rng_utils.py` & `keras-core-0.1.4/keras_core/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/sequence_utils.py` & `keras-core-0.1.4/keras_core/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/shape_utils.py` & `keras-core-0.1.4/keras_core/src/utils/shape_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/summary_utils.py` & `keras-core-0.1.4/keras_core/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/src/utils/traceback_utils.py` & `keras-core-0.1.4/keras_core/src/utils/traceback_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     See also `keras_core.config.disable_traceback_filtering()` and
     `keras_core.config.is_traceback_filtering_enabled()`.
 
     If you have previously disabled traceback filtering via
     `keras_core.config.disable_traceback_filtering()`, you can re-enable it via
     `keras_core.config.enable_traceback_filtering()`.
     """
-    global_state.set_global_setting("traceback_filtering", True)
+    global_state.set_global_attribute("traceback_filtering", True)
 
 
 @keras_core_export("keras_core.config.disable_traceback_filtering")
 def disable_traceback_filtering():
     """Turn off traceback filtering.
 
     Raw Keras tracebacks (also known as stack traces)
@@ -51,15 +51,15 @@
     See also `keras_core.config.enable_traceback_filtering()` and
     `keras_core.config.is_traceback_filtering_enabled()`.
 
     If you have previously disabled traceback filtering via
     `keras_core.config.disable_traceback_filtering()`, you can re-enable it via
     `keras_core.config.enable_traceback_filtering()`.
     """
-    global_state.set_global_setting("traceback_filtering", False)
+    global_state.set_global_attribute("traceback_filtering", False)
 
 
 @keras_core_export("keras_core.config.is_traceback_filtering_enabled")
 def is_traceback_filtering_enabled():
     """Check if traceback filtering is enabled.
 
     Raw Keras tracebacks (also known as stack traces)
@@ -76,15 +76,15 @@
     `keras_core.config.disable_traceback_filtering()`, you can re-enable it via
     `keras_core.config.enable_traceback_filtering()`.
 
     Returns:
         Boolean, `True` if traceback filtering is enabled,
         and `False` otherwise.
     """
-    return global_state.get_global_setting("traceback_filtering", True)
+    return global_state.get_global_attribute("traceback_filtering", True)
 
 
 def include_frame(fname):
     for exclusion in _EXCLUDED_PATHS:
         if exclusion in fname:
             return False
     return True
```

### Comparing `keras-core-0.1.3/keras_core/src/utils/tracking.py` & `keras-core-0.1.4/keras_core/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.3/keras_core/utils/__init__.py` & `keras-core-0.1.4/keras_core/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 from keras_core.src.saving.object_registration import register_keras_serializable
 from keras_core.src.saving.serialization_lib import deserialize_keras_object
 from keras_core.src.saving.serialization_lib import serialize_keras_object
 from keras_core.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
 from keras_core.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
 from keras_core.src.trainers.data_adapters.py_dataset_adapter import PyDataset
 from keras_core.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
-from keras_core.src.utils.dataset_utils import audio_dataset_from_directory
-from keras_core.src.utils.dataset_utils import image_dataset_from_directory
+from keras_core.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras_core.src.utils.dataset_utils import split_dataset
-from keras_core.src.utils.dataset_utils import text_dataset_from_directory
-from keras_core.src.utils.dataset_utils import timeseries_dataset_from_array
 from keras_core.src.utils.file_utils import get_file
+from keras_core.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras_core.src.utils.image_utils import array_to_img
 from keras_core.src.utils.image_utils import img_to_array
 from keras_core.src.utils.image_utils import load_img
 from keras_core.src.utils.image_utils import save_img
 from keras_core.src.utils.io_utils import disable_interactive_logging
 from keras_core.src.utils.io_utils import enable_interactive_logging
 from keras_core.src.utils.io_utils import is_interactive_logging_enabled
 from keras_core.src.utils.model_visualization import model_to_dot
 from keras_core.src.utils.model_visualization import plot_model
 from keras_core.src.utils.numerical_utils import normalize
 from keras_core.src.utils.numerical_utils import to_categorical
 from keras_core.src.utils.progbar import Progbar
 from keras_core.src.utils.rng_utils import set_random_seed
 from keras_core.src.utils.sequence_utils import pad_sequences
+from keras_core.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras_core.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
 from keras_core.utils import legacy
```

### Comparing `keras-core-0.1.3/keras_core.egg-info/PKG-INFO` & `keras-core-0.1.4/keras_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras-core
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-core-0.1.3/keras_core.egg-info/SOURCES.txt` & `keras-core-0.1.4/keras_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 keras_core/src/backend/config.py
 keras_core/src/backend/device_placement.py
 keras_core/src/backend/exports.py
 keras_core/src/backend/common/__init__.py
 keras_core/src/backend/common/backend_utils.py
 keras_core/src/backend/common/global_state.py
 keras_core/src/backend/common/keras_tensor.py
+keras_core/src/backend/common/name_scope.py
 keras_core/src/backend/common/stateless_scope.py
 keras_core/src/backend/common/variables.py
 keras_core/src/backend/jax/__init__.py
 keras_core/src/backend/jax/core.py
 keras_core/src/backend/jax/image.py
 keras_core/src/backend/jax/layer.py
 keras_core/src/backend/jax/math.py
@@ -189,14 +190,15 @@
 keras_core/src/backend/torch/trainer.py
 keras_core/src/backend/torch/optimizers/__init__.py
 keras_core/src/backend/torch/optimizers/torch_adadelta.py
 keras_core/src/backend/torch/optimizers/torch_adagrad.py
 keras_core/src/backend/torch/optimizers/torch_adam.py
 keras_core/src/backend/torch/optimizers/torch_adamax.py
 keras_core/src/backend/torch/optimizers/torch_adamw.py
+keras_core/src/backend/torch/optimizers/torch_lion.py
 keras_core/src/backend/torch/optimizers/torch_nadam.py
 keras_core/src/backend/torch/optimizers/torch_optimizer.py
 keras_core/src/backend/torch/optimizers/torch_parallel_optimizer.py
 keras_core/src/backend/torch/optimizers/torch_rmsprop.py
 keras_core/src/backend/torch/optimizers/torch_sgd.py
 keras_core/src/callbacks/__init__.py
 keras_core/src/callbacks/callback.py
@@ -382,14 +384,15 @@
 keras_core/src/mixed_precision/__init__.py
 keras_core/src/mixed_precision/dtype_policy.py
 keras_core/src/models/__init__.py
 keras_core/src/models/cloning.py
 keras_core/src/models/functional.py
 keras_core/src/models/model.py
 keras_core/src/models/sequential.py
+keras_core/src/models/variable_mapping.py
 keras_core/src/ops/__init__.py
 keras_core/src/ops/core.py
 keras_core/src/ops/function.py
 keras_core/src/ops/image.py
 keras_core/src/ops/math.py
 keras_core/src/ops/nn.py
 keras_core/src/ops/node.py
@@ -402,14 +405,15 @@
 keras_core/src/optimizers/adafactor.py
 keras_core/src/optimizers/adagrad.py
 keras_core/src/optimizers/adam.py
 keras_core/src/optimizers/adamax.py
 keras_core/src/optimizers/adamw.py
 keras_core/src/optimizers/base_optimizer.py
 keras_core/src/optimizers/ftrl.py
+keras_core/src/optimizers/lion.py
 keras_core/src/optimizers/nadam.py
 keras_core/src/optimizers/optimizer.py
 keras_core/src/optimizers/rmsprop.py
 keras_core/src/optimizers/sgd.py
 keras_core/src/optimizers/schedules/__init__.py
 keras_core/src/optimizers/schedules/learning_rate_schedule.py
 keras_core/src/random/__init__.py
@@ -435,29 +439,34 @@
 keras_core/src/trainers/data_adapters/data_adapter_utils.py
 keras_core/src/trainers/data_adapters/generator_data_adapter.py
 keras_core/src/trainers/data_adapters/py_dataset_adapter.py
 keras_core/src/trainers/data_adapters/tf_dataset_adapter.py
 keras_core/src/trainers/data_adapters/torch_data_adapter.py
 keras_core/src/utils/__init__.py
 keras_core/src/utils/argument_validation.py
+keras_core/src/utils/audio_dataset_utils.py
 keras_core/src/utils/backend_utils.py
 keras_core/src/utils/code_stats.py
 keras_core/src/utils/dataset_utils.py
 keras_core/src/utils/dtype_utils.py
 keras_core/src/utils/file_utils.py
+keras_core/src/utils/image_dataset_utils.py
 keras_core/src/utils/image_utils.py
 keras_core/src/utils/io_utils.py
 keras_core/src/utils/model_visualization.py
 keras_core/src/utils/module_utils.py
 keras_core/src/utils/naming.py
 keras_core/src/utils/nest.py
 keras_core/src/utils/numerical_utils.py
 keras_core/src/utils/progbar.py
 keras_core/src/utils/python_utils.py
 keras_core/src/utils/rng_utils.py
 keras_core/src/utils/sequence_utils.py
 keras_core/src/utils/shape_utils.py
 keras_core/src/utils/summary_utils.py
+keras_core/src/utils/text_dataset_utils.py
+keras_core/src/utils/tf_utils.py
+keras_core/src/utils/timeseries_dataset_utils.py
 keras_core/src/utils/traceback_utils.py
 keras_core/src/utils/tracking.py
 keras_core/utils/__init__.py
 keras_core/utils/legacy/__init__.py
```

### Comparing `keras-core-0.1.3/setup.py` & `keras-core-0.1.4/setup.py`

 * *Files identical despite different names*

