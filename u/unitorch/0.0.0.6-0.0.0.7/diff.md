# Comparing `tmp/unitorch-0.0.0.6.tar.gz` & `tmp/unitorch-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitorch-0.0.0.6.tar", last modified: Mon Jul 24 07:53:46 2023, max compression
+gzip compressed data, was "unitorch-0.0.0.7.tar", last modified: Tue Aug  8 10:45:32 2023, max compression
```

## Comparing `unitorch-0.0.0.6.tar` & `unitorch-0.0.0.7.tar`

### file list

```diff
@@ -1,490 +1,491 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/.pytest_cache/
--rw-r--r--   0 root         (0) root         (0)      302 2023-07-24 07:53:35.000000 unitorch-0.0.0.6/.pytest_cache/README.md
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9222 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8187 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/benchmarks/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/benchmarks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.933258 unitorch-0.0.0.6/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.961258 unitorch-0.0.0.6/docs/search/
--rw-r--r--   0 root         (0) root         (0)  1081944 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/docs/search/search_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.965258 unitorch-0.0.0.6/examples/
--rw-r--r--   0 root         (0) root         (0)     2311 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.965258 unitorch-0.0.0.6/examples/configs/caption/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/blip.ini
--rw-r--r--   0 root         (0) root         (0)     2556 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/minigpt4.ini
--rw-r--r--   0 root         (0) root         (0)     2692 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/minigpt4_ds.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.969258 unitorch-0.0.0.6/examples/configs/classification/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)     1700 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/clip.ini
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/image_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/classification/lora/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1615 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1857 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1810 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1556 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/roberta.ini
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/swin.ini
--rw-r--r--   0 root         (0) root         (0)     1636 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/text_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/deepspeed/
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/deepspeed/adamw.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/diffusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.977258 unitorch-0.0.0.6/examples/configs/diffusion/controlnet/
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/controlnet/canny.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v1.5.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.1.ini
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.981258 unitorch-0.0.0.6/examples/configs/generation/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)     1651 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1667 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/chatglm.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/llama.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.981258 unitorch-0.0.0.6/examples/configs/generation/lora/
--rw-r--r--   0 root         (0) root         (0)     1608 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1582 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/mbart.ini
--rw-r--r--   0 root         (0) root         (0)     1597 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/mt5.ini
--rw-r--r--   0 root         (0) root         (0)     1655 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/pegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/t5.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/xpegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/xprophetnet.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/configs/pretrain/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/pretrain/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/configs/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/configs/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/services/zip_image/config.ini
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/services/zip_image/config_v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/caption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/classification/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/generation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/llama.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/xpegasus.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/notebooks/
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/notebooks/README.md
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 07:53:46.173260 unitorch-0.0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/src/unitorch/
--rw-r--r--   0 root         (0) root         (0)     2670 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.989258 unitorch-0.0.0.6/src/unitorch/cli/
--rw-r--r--   0 root         (0) root         (0)     6025 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.989258 unitorch-0.0.0.6/src/unitorch/cli/console/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/eval.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/infer.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/script.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/service.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/train.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.993258 unitorch-0.0.0.6/src/unitorch/cli/datasets/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12406 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/datasets/hf.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.993258 unitorch-0.0.0.6/src/unitorch/cli/loss/
--rw-r--r--   0 root         (0) root         (0)     4063 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.997258 unitorch-0.0.0.6/src/unitorch/cli/models/
--rw-r--r--   0 root         (0) root         (0)     2901 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.001258 unitorch-0.0.0.6/src/unitorch/cli/models/bart/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/fastapi.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.001258 unitorch-0.0.0.6/src/unitorch/cli/models/beit/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/bert/
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/blip/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22734 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7788 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8756 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.009258 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13812 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)     9111 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/classification_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.009258 unitorch-0.0.0.6/src/unitorch/cli/models/clip/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.013258 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/
--rw-r--r--   0 root         (0) root         (0)     4492 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing_v2.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/detection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.017259 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7500 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3879 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3838 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_stable.py
--rw-r--r--   0 root         (0) root         (0)     3126 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/label_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/llama/
--rw-r--r--   0 root         (0) root         (0)     3445 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14065 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8641 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7650 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10738 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/modeling.py
--rw-r--r--   0 root         (0) root         (0)    10044 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/processing.py
--rw-r--r--   0 root         (0) root         (0)    15281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/modeling_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.025258 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.025258 unitorch-0.0.0.6/src/unitorch/cli/models/peft/
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30598 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_bloom.py
--rw-r--r--   0 root         (0) root         (0)    30656 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_llama.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/processing.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/random_utils.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/ranking_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/segmentation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.033259 unitorch-0.0.0.6/src/unitorch/cli/models/swin/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.033259 unitorch-0.0.0.6/src/unitorch/cli/models/t5/
--rw-r--r--   0 root         (0) root         (0)     1282 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)     1310 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8538 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/vit/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)     2314 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7286 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/optim/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/scheduler/
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/score/
--rw-r--r--   0 root         (0) root         (0)    14139 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/score/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/scripts/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scripts/README.md
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/services/
--rw-r--r--   0 root         (0) root         (0)      257 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/tasks/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26512 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/deepspeed.py
--rw-r--r--   0 root         (0) root         (0)    31622 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/supervised.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/writer/
--rw-r--r--   0 root         (0) root         (0)    10544 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.053259 unitorch-0.0.0.6/src/unitorch/datasets/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6832 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/datasets/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/loss/
--rw-r--r--   0 root         (0) root         (0)     4712 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/prophetnet.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/models/
--rw-r--r--   0 root         (0) root         (0)     7498 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/models/bart/
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.061259 unitorch-0.0.0.6/src/unitorch/models/beit/
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.061259 unitorch-0.0.0.6/src/unitorch/models/bert/
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8355 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.065259 unitorch-0.0.0.6/src/unitorch/models/blip/
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30337 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.065259 unitorch-0.0.0.6/src/unitorch/models/blip2/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/modeling.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.069259 unitorch-0.0.0.6/src/unitorch/models/bloom/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10885 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     9108 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.073259 unitorch-0.0.0.6/src/unitorch/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11175 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)    55823 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11091 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/tokenization_chatglm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.077259 unitorch-0.0.0.6/src/unitorch/models/clip/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15100 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.077259 unitorch-0.0.0.6/src/unitorch/models/deberta/
--rw-r--r--   0 root         (0) root         (0)      424 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/processing_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.081259 unitorch-0.0.0.6/src/unitorch/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)      547 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6076 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     8201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_stable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.085259 unitorch-0.0.0.6/src/unitorch/models/llama/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11394 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8944 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.085259 unitorch-0.0.0.6/src/unitorch/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13976 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.089259 unitorch-0.0.0.6/src/unitorch/models/minigpt4/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17053 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/modeling.py
--rw-r--r--   0 root         (0) root         (0)    13727 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/processing.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/modeling_ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.089259 unitorch-0.0.0.6/src/unitorch/models/mt5/
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14250 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.093259 unitorch-0.0.0.6/src/unitorch/models/peft/
--rw-r--r--   0 root         (0) root         (0)     5424 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_lora.py
--rw-r--r--   0 root         (0) root         (0)    10125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9309 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_lora.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13652 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      179 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/roberta/
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.101259 unitorch-0.0.0.6/src/unitorch/models/swin/
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.101259 unitorch-0.0.0.6/src/unitorch/models/t5/
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13316 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.105259 unitorch-0.0.0.6/src/unitorch/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.105259 unitorch-0.0.0.6/src/unitorch/models/vit/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13741 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.113259 unitorch-0.0.0.6/src/unitorch/modules/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/modules/replace/
--rw-r--r--   0 root         (0) root         (0)      199 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14643 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/beam_search_v2.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/datasets_v2.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/hf_hub_v2.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/timm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/ops/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16794 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/dyhead.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/optim/
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/rl/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/rl/utils/buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/scheduler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.125259 unitorch-0.0.0.6/src/unitorch/score/
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/bleu.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/map.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/rouge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.125259 unitorch-0.0.0.6/src/unitorch/tasks/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.129259 unitorch-0.0.0.6/src/unitorch/utils/
--rw-r--r--   0 root         (0) root         (0)    13662 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/palette.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/torch_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/src/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9222 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13624 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.129259 unitorch-0.0.0.6/wiki/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.133259 unitorch-0.0.0.6/wiki/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/benchmarks/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.141259 unitorch-0.0.0.6/wiki/cli/
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/ast.md
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/csv.md
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/datatypes.md
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/deepspeed.md
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/jsonl.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/cli/models/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bert.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/index.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      359 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/minigpt4.md
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/parquet.md
--rw-r--r--   0 root         (0) root         (0)      851 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/postprocess.md
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/preprocess.md
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/supervised.md
--rw-r--r--   0 root         (0) root         (0)     4600 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/wiki/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/caption/
--rw-r--r--   0 root         (0) root         (0)     4659 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/caption/blip.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/classification/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/clip.md
--rw-r--r--   0 root         (0) root         (0)     4130 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/roberta.md
--rw-r--r--   0 root         (0) root         (0)     4525 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/swin.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/diffusion/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/diffusion/controlnet.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/examples/generation/
--rw-r--r--   0 root         (0) root         (0)     4145 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/generation/bart.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/examples/service/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/service/zip_image.md
--rw-r--r--   0 root         (0) root         (0)     1346 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/index.md
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/labs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/labs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/wiki/models/
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bert.md
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/index.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/minigpt4.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)     4524 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.545803 unitorch-0.0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.325800 unitorch-0.0.0.7/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 10:45:17.000000 unitorch-0.0.0.7/.pytest_cache/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-08-08 10:45:32.545803 unitorch-0.0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.325800 unitorch-0.0.0.7/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.313800 unitorch-0.0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.325800 unitorch-0.0.0.7/docs/search/
+-rw-r--r--   0 runner    (1001) docker     (123)  1081944 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/docs/search/search_index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.329800 unitorch-0.0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.313800 unitorch-0.0.0.7/examples/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.329800 unitorch-0.0.0.7/examples/configs/caption/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/caption/blip.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/caption/minigpt4.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/caption/minigpt4_ds.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.333800 unitorch-0.0.0.7/examples/configs/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/bert.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/clip.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.337800 unitorch-0.0.0.7/examples/configs/classification/lora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/roberta.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/swin.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.337800 unitorch-0.0.0.7/examples/configs/deepspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/deepspeed/adamw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.337800 unitorch-0.0.0.7/examples/configs/diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.337800 unitorch-0.0.0.7/examples/configs/diffusion/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/diffusion/controlnet/canny.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/diffusion/stable-v1.5.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/diffusion/stable-v2.1.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/diffusion/stable-v2.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.341800 unitorch-0.0.0.7/examples/configs/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/bart.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/bloom.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/llama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/llama.quant.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.345800 unitorch-0.0.0.7/examples/configs/generation/lora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/llama.quant.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/lora/llama_ds.quant.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/mbart.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/mt5.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/t5.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.345800 unitorch-0.0.0.7/examples/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/examples/configs/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/quantization/4bit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/quantization/8bit.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.313800 unitorch-0.0.0.7/examples/configs/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/examples/configs/services/zip_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.313800 unitorch-0.0.0.7/examples/hub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/examples/hub/caption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/caption/blip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/examples/hub/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/classification/bert.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/classification/clip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/examples/hub/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/generation/bart.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/generation/llama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.349800 unitorch-0.0.0.7/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:45:32.545803 unitorch-0.0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.313800 unitorch-0.0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.353800 unitorch-0.0.0.7/src/unitorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.353800 unitorch-0.0.0.7/src/unitorch/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.357800 unitorch-0.0.0.7/src/unitorch/cli/console/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/console/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.357800 unitorch-0.0.0.7/src/unitorch/cli/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.361801 unitorch-0.0.0.7/src/unitorch/cli/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.365800 unitorch-0.0.0.7/src/unitorch/cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.369800 unitorch-0.0.0.7/src/unitorch/cli/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bart/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.369800 unitorch-0.0.0.7/src/unitorch/cli/models/beit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.373801 unitorch-0.0.0.7/src/unitorch/cli/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.373801 unitorch-0.0.0.7/src/unitorch/cli/models/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22734 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.377801 unitorch-0.0.0.7/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/bloom/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.377801 unitorch-0.0.0.7/src/unitorch/cli/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.381801 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.385801 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.385801 unitorch-0.0.0.7/src/unitorch/cli/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.389801 unitorch-0.0.0.7/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mbart/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.389801 unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.393801 unitorch-0.0.0.7/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.393801 unitorch-0.0.0.7/src/unitorch/cli/models/peft/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.393801 unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.397801 unitorch-0.0.0.7/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.397801 unitorch-0.0.0.7/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.401801 unitorch-0.0.0.7/src/unitorch/cli/models/swin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.401801 unitorch-0.0.0.7/src/unitorch/cli/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.401801 unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.405801 unitorch-0.0.0.7/src/unitorch/cli/models/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.405801 unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.409801 unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.409801 unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.409801 unitorch-0.0.0.7/src/unitorch/cli/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.413801 unitorch-0.0.0.7/src/unitorch/cli/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.413801 unitorch-0.0.0.7/src/unitorch/cli/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.413801 unitorch-0.0.0.7/src/unitorch/cli/score/
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.413801 unitorch-0.0.0.7/src/unitorch/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.413801 unitorch-0.0.0.7/src/unitorch/cli/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.417801 unitorch-0.0.0.7/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.421801 unitorch-0.0.0.7/src/unitorch/cli/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26512 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31622 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.421801 unitorch-0.0.0.7/src/unitorch/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.425801 unitorch-0.0.0.7/src/unitorch/cli/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.425801 unitorch-0.0.0.7/src/unitorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.425801 unitorch-0.0.0.7/src/unitorch/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.429802 unitorch-0.0.0.7/src/unitorch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.429802 unitorch-0.0.0.7/src/unitorch/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.433802 unitorch-0.0.0.7/src/unitorch/models/beit/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.433802 unitorch-0.0.0.7/src/unitorch/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.437802 unitorch-0.0.0.7/src/unitorch/models/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30337 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.437802 unitorch-0.0.0.7/src/unitorch/models/blip2/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip2/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/blip2/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.437802 unitorch-0.0.0.7/src/unitorch/models/bloom/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.441802 unitorch-0.0.0.7/src/unitorch/models/chatglm/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11175 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55823 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.445802 unitorch-0.0.0.7/src/unitorch/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.449802 unitorch-0.0.0.7/src/unitorch/models/deberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.453802 unitorch-0.0.0.7/src/unitorch/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.453802 unitorch-0.0.0.7/src/unitorch/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.457802 unitorch-0.0.0.7/src/unitorch/models/mbart/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mbart/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.457802 unitorch-0.0.0.7/src/unitorch/models/minigpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/minigpt4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/minigpt4/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/minigpt4/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.461802 unitorch-0.0.0.7/src/unitorch/models/mt5/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.465802 unitorch-0.0.0.7/src/unitorch/models/peft/
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.465802 unitorch-0.0.0.7/src/unitorch/models/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.469802 unitorch-0.0.0.7/src/unitorch/models/prophetnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/prophetnet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.473802 unitorch-0.0.0.7/src/unitorch/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.473802 unitorch-0.0.0.7/src/unitorch/models/swin/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.473802 unitorch-0.0.0.7/src/unitorch/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.477802 unitorch-0.0.0.7/src/unitorch/models/visualbert/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.477802 unitorch-0.0.0.7/src/unitorch/models/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.481802 unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.481802 unitorch-0.0.0.7/src/unitorch/models/xpegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.485802 unitorch-0.0.0.7/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.485802 unitorch-0.0.0.7/src/unitorch/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.489802 unitorch-0.0.0.7/src/unitorch/modules/replace/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/modules/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.489802 unitorch-0.0.0.7/src/unitorch/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.493802 unitorch-0.0.0.7/src/unitorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/optim/lion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.493802 unitorch-0.0.0.7/src/unitorch/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.493802 unitorch-0.0.0.7/src/unitorch/rl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.493802 unitorch-0.0.0.7/src/unitorch/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.497803 unitorch-0.0.0.7/src/unitorch/score/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/score/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/score/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/score/rouge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.497803 unitorch-0.0.0.7/src/unitorch/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.501803 unitorch-0.0.0.7/src/unitorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.353800 unitorch-0.0.0.7/src/unitorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 10:45:32.000000 unitorch-0.0.0.7/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.505803 unitorch-0.0.0.7/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.505803 unitorch-0.0.0.7/wiki/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/benchmarks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.509803 unitorch-0.0.0.7/wiki/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/ast.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/csv.md
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/datatypes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/deepspeed.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/jsonl.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.521803 unitorch-0.0.0.7/wiki/cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/bart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/beit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/bert.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/blip.md
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/bloom.md
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/chatglm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/clip.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/deberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/diffusers.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/llama.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/mbart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/minigpt4.md
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/mt5.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/peft.md
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/pegasus.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/roberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/swin.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/t5.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/visualbert.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/vit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/parquet.md
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/postprocess.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/preprocess.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/cli/supervised.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/configuration.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.321800 unitorch-0.0.0.7/wiki/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.521803 unitorch-0.0.0.7/wiki/examples/caption/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/caption/blip.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.525803 unitorch-0.0.0.7/wiki/examples/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/classification/clip.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/classification/roberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/classification/swin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.525803 unitorch-0.0.0.7/wiki/examples/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.525803 unitorch-0.0.0.7/wiki/examples/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/generation/bart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.525803 unitorch-0.0.0.7/wiki/examples/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/examples/service/zip_image.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.525803 unitorch-0.0.0.7/wiki/labs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/labs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:45:32.545803 unitorch-0.0.0.7/wiki/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/bart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/beit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/bert.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/blip.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/bloom.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/chatglm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/clip.md
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/deberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/diffusers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/llama.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/mbart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/minigpt4.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/mt5.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/peft.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/pegasus.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/prophetnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/roberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/swin.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/t5.md
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/visualbert.md
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/vit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/xlm_roberta.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/xpegasus.md
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/models/xprophetnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-08 10:37:10.000000 unitorch-0.0.0.7/wiki/overview.md
```

### Comparing `unitorch-0.0.0.6/LICENSE` & `unitorch-0.0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/PKG-INFO` & `unitorch-0.0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
-Provides-Extra: accelerate
-Provides-Extra: chatglm
+Provides-Extra: quantization
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.6/README.md` & `unitorch-0.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/docs/search/search_index.json` & `unitorch-0.0.0.7/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/README.md` & `unitorch-0.0.0.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/caption/blip.ini` & `unitorch-0.0.0.7/examples/configs/caption/blip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/caption/minigpt4.ini` & `unitorch-0.0.0.7/examples/configs/caption/minigpt4.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/caption/minigpt4_ds.ini` & `unitorch-0.0.0.7/examples/configs/caption/minigpt4_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/bert.ini` & `unitorch-0.0.0.7/examples/configs/classification/bert.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/clip.ini` & `unitorch-0.0.0.7/examples/configs/classification/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/image_clip.ini` & `unitorch-0.0.0.7/examples/configs/classification/image_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/lora/bloom.ini` & `unitorch-0.0.0.7/examples/configs/classification/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/lora/bloom_ds.ini` & `unitorch-0.0.0.7/examples/configs/classification/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/lora/llama.ini` & `unitorch-0.0.0.7/examples/configs/classification/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/lora/llama_ds.ini` & `unitorch-0.0.0.7/examples/configs/classification/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/roberta.ini` & `unitorch-0.0.0.7/examples/configs/classification/roberta.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/swin.ini` & `unitorch-0.0.0.7/examples/configs/classification/swin.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/classification/text_clip.ini` & `unitorch-0.0.0.7/examples/configs/classification/text_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/diffusion/controlnet/canny.ini` & `unitorch-0.0.0.7/examples/configs/diffusion/controlnet/canny.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/diffusion/stable-v1.5.ini` & `unitorch-0.0.0.7/examples/configs/diffusion/stable-v1.5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.1.ini` & `unitorch-0.0.0.7/examples/configs/diffusion/stable-v2.1.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.ini` & `unitorch-0.0.0.7/examples/configs/diffusion/stable-v2.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/bart.ini` & `unitorch-0.0.0.7/examples/configs/generation/bart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/bloom.ini` & `unitorch-0.0.0.7/examples/configs/generation/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/chatglm.ini` & `unitorch-0.0.0.7/examples/configs/generation/chatglm.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/llama.ini` & `unitorch-0.0.0.7/examples/configs/generation/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/lora/bloom.ini` & `unitorch-0.0.0.7/examples/configs/generation/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/lora/bloom_ds.ini` & `unitorch-0.0.0.7/examples/configs/generation/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/lora/llama.ini` & `unitorch-0.0.0.7/examples/configs/generation/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/lora/llama_ds.ini` & `unitorch-0.0.0.7/examples/configs/generation/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/mbart.ini` & `unitorch-0.0.0.7/examples/configs/generation/mbart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/mt5.ini` & `unitorch-0.0.0.7/examples/configs/generation/mt5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/pegasus.ini` & `unitorch-0.0.0.7/examples/configs/generation/pegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/t5.ini` & `unitorch-0.0.0.7/examples/configs/generation/t5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/xpegasus.ini` & `unitorch-0.0.0.7/examples/configs/generation/xpegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/generation/xprophetnet.ini` & `unitorch-0.0.0.7/examples/configs/generation/xprophetnet.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/examples/configs/pretrain/clip.ini` & `unitorch-0.0.0.7/examples/configs/pretrain/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/pyproject.toml` & `unitorch-0.0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=40.0", "torch>=1.13", "torchvision", "torchaudio"]
+requires = ["setuptools>=62.1.0", "torch>=1.13", "torchvision", "torchaudio"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitorch"
 authors = [
     {name = "fuliucansheng", email = "fuliucansheng@gmail.com"},
 ]
@@ -25,18 +25,17 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["version", "dependencies"]
 
 [project.optional-dependencies]
 deepspeed = ["deepspeed==0.9.0", "mpi4py==3.1.4"]
-diffusers = ["diffusers==0.16.1"]
-accelerate = ["accelerate==0.20.3"]
-chatglm = ["protobuf==3.20.0", "icetk==0.0.4", "cpm_kernels==1.0.11"]
-all = ["unitorch[deepspeed,diffusers,accelerate,chatglm]"]
+diffusers = ["diffusers>=0.17.1"]
+quantization = ["bitsandbytes>=0.41.1"]
+all = ["unitorch[deepspeed,diffusers,quantization]"]
 
 [project.scripts]
 unitorch-train = "unitorch.cli.console.train:cli_main"
 unitorch-eval = "unitorch.cli.console.eval:cli_main"
 unitorch-infer = "unitorch.cli.console.infer:cli_main"
 unitorch-script= "unitorch.cli.console.script:cli_main"
 unitorch-service = "unitorch.cli.console.service:cli_main"
```

### Comparing `unitorch-0.0.0.6/src/unitorch/__init__.py` & `unitorch-0.0.0.7/src/unitorch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_cache_home():
     return UNITORCH_CACHE
 
 
 ### version
-VERSION = "0.0.0.6"
+VERSION = "0.0.0.7"
 
 ### is offline mode
 UNITORCH_OFFLINE = os.environ.get("UNITORCH_OFFLINE", "0").upper()
 
 
 def is_offline_mode():
     return UNITORCH_OFFLINE in ENV_VARS_TRUE_VALUES
@@ -91,14 +91,19 @@
     is_accelerate_available,
     is_megatron_available,
     is_diffusers_available,
     is_torch_available,
     is_torch2_available,
 )
 
+if is_diffusers_available():
+    import diffusers
+
+    diffusers.logging.set_verbosity_error()
+
 # imports from other files
 import unitorch.datasets
 import unitorch.loss
 import unitorch.score
 import unitorch.models
 import unitorch.modules
 import unitorch.optim
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/console/eval.py` & `unitorch-0.0.0.7/src/unitorch/cli/console/eval.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/console/infer.py` & `unitorch-0.0.0.7/src/unitorch/cli/console/infer.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/console/script.py` & `unitorch-0.0.0.7/src/unitorch/cli/console/script.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/console/service.py` & `unitorch-0.0.0.7/src/unitorch/cli/console/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/console/train.py` & `unitorch-0.0.0.7/src/unitorch/cli/console/train.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/core.py` & `unitorch-0.0.0.7/src/unitorch/cli/core.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/datasets/hf.py` & `unitorch-0.0.0.7/src/unitorch/cli/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/decorators.py` & `unitorch-0.0.0.7/src/unitorch/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/loss/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/loss/ranking.py` & `unitorch-0.0.0.7/src/unitorch/cli/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
 # import model classes & process functions
 import unitorch.cli.models.bart
 import unitorch.cli.models.bert
 import unitorch.cli.models.beit
 import unitorch.cli.models.blip
 import unitorch.cli.models.bloom
-import unitorch.cli.models.chatglm
 import unitorch.cli.models.clip
 import unitorch.cli.models.deberta
 import unitorch.cli.models.minigpt4
 import unitorch.cli.models.llama
 import unitorch.cli.models.mbart
 import unitorch.cli.models.mt5
 import unitorch.cli.models.pegasus
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bart/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bart/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bart/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/beit/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/beit/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/beit/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bert/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bert/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bert/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/blip/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/blip/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/blip/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/t5/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 # pretrained infos
-pretrained_chatglm_infos = {
-    # chatglm
-    "default-chatglm": {
-        "config": "https://huggingface.co/THUDM/chatglm-6b/resolve/main/config.json",
-        "vocab": "https://huggingface.co/THUDM/chatglm-6b/resolve/main/ice_text.model",
-        "tokenizer": "https://huggingface.co/THUDM/chatglm-6b/raw/main/tokenizer_config.json",
+pretrained_t5_infos = {
+    "default-t5": {
+        "config": "https://huggingface.co/t5-base/resolve/main/config.json",
+        "vocab": "https://huggingface.co/t5-base/resolve/main/spiece.model",
     },
-    "chatglm-6b": {
-        "config": "https://huggingface.co/THUDM/chatglm-6b/resolve/main/config.json",
-        "vocab": "https://huggingface.co/THUDM/chatglm-6b/resolve/main/ice_text.model",
-        "tokenizer": "https://huggingface.co/THUDM/chatglm-6b/raw/main/tokenizer_config.json",
-        "weight": [
-            f"https://huggingface.co/THUDM/chatglm-6b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00008.bin"
-            for i in range(1, 9)
-        ],
+    "t5-base": {
+        "config": "https://huggingface.co/t5-base/resolve/main/config.json",
+        "vocab": "https://huggingface.co/t5-base/resolve/main/spiece.model",
+        "weight": "https://huggingface.co/t5-base/resolve/main/pytorch_model.bin",
+    },
+    "t5-small": {
+        "config": "https://huggingface.co/t5-small/resolve/main/config.json",
+        "vocab": "https://huggingface.co/t5-small/resolve/main/spiece.model",
+        "weight": "https://huggingface.co/t5-small/resolve/main/pytorch_model.bin",
+    },
+    "t5-large": {
+        "config": "https://huggingface.co/t5-large/resolve/main/config.json",
+        "vocab": "https://huggingface.co/t5-large/resolve/main/spiece.model",
+        "weight": "https://huggingface.co/t5-large/resolve/main/pytorch_model.bin",
     },
 }
 
-import unitorch.cli.models.chatglm.modeling
-import unitorch.cli.models.chatglm.processing
-from unitorch.cli.models.chatglm.modeling import (
-    ChatGLMForClassification,
-    ChatGLMForPretrain,
-    ChatGLMForGeneration,
-)
-from unitorch.cli.models.chatglm.processing import ChatGLMProcessor
+import unitorch.cli.models.t5.modeling
+import unitorch.cli.models.t5.processing
+from unitorch.cli.models.t5.modeling import T5ForGeneration
+from unitorch.cli.models.t5.processing import T5Processor
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/llama/modeling.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,85 +2,98 @@
 # Licensed under the MIT License.
 
 import torch
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from torch.cuda.amp import autocast
 from transformers.utils import is_remote_url
 from unitorch.utils import pop_value, nested_dict_value
-from unitorch.models.chatglm import (
-    ChatGLMForClassification as _ChatGLMForClassification,
-    ChatGLMForGeneration as _ChatGLMForGeneration,
-    ChatGLMForPretrain as _ChatGLMForPretrain,
+from unitorch.models.llama import (
+    LlamaForClassification as _LlamaForClassification,
+    LlamaForGeneration as _LlamaForGeneration,
+    LlamaForPretrain as _LlamaForPretrain,
 )
 from unitorch.cli import (
     cached_path,
     add_default_section_for_init,
     add_default_section_for_function,
     register_model,
 )
 from unitorch.cli.models import generation_model_decorator
 from unitorch.cli.models import ClassificationOutputs, GenerationOutputs, LossOutputs
-from unitorch.cli.models.chatglm import pretrained_chatglm_infos
+from unitorch.cli.models.llama import pretrained_llama_infos
 
 
-@register_model("core/model/classification/chatglm")
-class ChatGLMForClassification(_ChatGLMForClassification):
-    """Classification model based on ChatGLM."""
+@register_model("core/model/classification/llama")
+class LlamaForClassification(_LlamaForClassification):
+    """Llama model for classification tasks."""
 
     def __init__(
         self,
         config_path: str,
+        quant_config_path: Optional[str] = None,
         num_classes: Optional[int] = 1,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the ChatGLMForClassification model.
+        Initialize the LlamaForClassification model.
 
         Args:
             config_path (str): The path to the model configuration file.
             num_classes (int, optional): The number of classes for classification. Defaults to 1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
+            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__(
             config_path=config_path,
+            quant_config_path=quant_config_path,
             num_classes=num_classes,
             gradient_checkpointing=gradient_checkpointing,
         )
 
     @classmethod
-    @add_default_section_for_init("core/model/classification/chatglm")
+    @add_default_section_for_init("core/model/classification/llama")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of ChatGLMForClassification from the core configuration.
+        Create an instance of LlamaForClassification from a core configuration.
 
         Args:
-            config (Config): The core configuration object.
+            config: The core configuration.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            ChatGLMForClassification: An instance of ChatGLMForClassification initialized with the provided configuration.
+            LlamaForClassification: An instance of LlamaForClassification.
         """
-        config.set_default_section("core/model/classification/chatglm")
-        pretrained_name = config.getoption("pretrained_name", "default-chatglm")
+        config.set_default_section("core/model/classification/llama")
+        pretrained_name = config.getoption("pretrained_name", "default-llama")
         config_path = config.getoption("config_path", None)
         config_path = pop_value(
             config_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "config"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
         )
 
         config_path = cached_path(config_path)
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
         gradient_checkpointing = config.getoption("gradient_checkpointing", False)
         num_classes = config.getoption("num_classes", 1)
 
-        inst = cls(config_path, num_classes, gradient_checkpointing)
+        inst = cls(
+            config_path,
+            quant_config_path=quant_config_path,
+            num_classes=num_classes,
+            gradient_checkpointing=gradient_checkpointing,
+        )
+
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
         weight_path = pop_value(
             pretrained_weight_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "weight"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
             check_none=False,
         )
+
         if weight_path is not None:
             inst.from_pretrained(
                 weight_path=weight_path,
             )
 
         return inst
 
@@ -88,83 +101,94 @@
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
     ):
         """
-        Perform forward pass of the ChatGLMForClassification model.
+        Perform a forward pass on the LlamaForClassification model.
 
         Args:
-            input_ids (torch.Tensor): The input sequence IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+            input_ids (torch.Tensor): The input tensor containing the input IDs.
+            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
+            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
 
         Returns:
-            ClassificationOutputs: The classification outputs.
+            ClassificationOutputs: The output of the classification model.
         """
         outputs = super().forward(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
         return ClassificationOutputs(outputs=outputs)
 
 
-@register_model("core/model/pretrain/chatglm")
-class ChatGLMForPretrain(_ChatGLMForPretrain):
-    """Pretraining model based on ChatGLM."""
+@register_model("core/model/pretrain/llama")
+class LlamaForPretrain(_LlamaForPretrain):
+    """Llama model for pretraining tasks."""
 
     def __init__(
         self,
         config_path: str,
+        quant_config_path: Optional[str] = None,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the ChatGLMForPretrain model.
+        Initialize the LlamaForPretrain model.
 
         Args:
             config_path (str): The path to the model configuration file.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
+            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__(
             config_path=config_path,
+            quant_config_path=quant_config_path,
             gradient_checkpointing=gradient_checkpointing,
         )
 
     @classmethod
-    @add_default_section_for_init("core/model/pretrain/chatglm")
+    @add_default_section_for_init("core/model/pretrain/llama")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of ChatGLMForPretrain from the core configuration.
+        Create an instance of LlamaForPretrain from a core configuration.
 
         Args:
-            config (Config): The core configuration object.
+            config: The core configuration.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            ChatGLMForPretrain: An instance of ChatGLMForPretrain initialized with the provided configuration.
+            LlamaForPretrain: An instance of LlamaForPretrain.
         """
-        config.set_default_section("core/model/pretrain/chatglm")
-        pretrained_name = config.getoption("pretrained_name", "default-chatglm")
+        config.set_default_section("core/model/pretrain/llama")
+        pretrained_name = config.getoption("pretrained_name", "default-llama")
         config_path = config.getoption("config_path", None)
         config_path = pop_value(
             config_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "config"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
         )
 
         config_path = cached_path(config_path)
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
         gradient_checkpointing = config.getoption("gradient_checkpointing", False)
 
-        inst = cls(config_path, gradient_checkpointing)
+        inst = cls(
+            config_path,
+            quant_config_path=quant_config_path,
+            gradient_checkpointing=gradient_checkpointing,
+        )
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
         weight_path = pop_value(
             pretrained_weight_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "weight"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
             check_none=False,
         )
+
         if weight_path is not None:
             inst.from_pretrained(
                 weight_path=weight_path,
             )
 
         return inst
 
@@ -174,87 +198,98 @@
         input_ids: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
         input_ids_label: Optional[torch.Tensor] = None,
         attention_mask_label: Optional[torch.Tensor] = None,
     ):
         """
-        Perform forward pass of the ChatGLMForPretrain model.
+        Perform a forward pass on the LlamaForPretrain model.
 
         Args:
-            input_ids (torch.Tensor): The input sequence IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
-            input_ids_label (torch.Tensor, optional): The input sequence IDs for the masked language model (MLM) labels.
-            attention_mask_label (torch.Tensor, optional): The attention mask for the MLM labels.
+            input_ids (torch.Tensor): The input tensor containing the input IDs.
+            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
+            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
+            input_ids_label (torch.Tensor, optional): The input tensor containing the input IDs for the masked language model. Defaults to None.
+            attention_mask_label (torch.Tensor, optional): The attention mask tensor for the masked language model. Defaults to None.
 
         Returns:
-            LossOutputs: The loss outputs.
+            LossOutputs: The output of the pretraining model.
         """
         outputs = super().forward(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
             input_ids_label=input_ids_label,
             attention_mask_label=attention_mask_label,
         )
         return LossOutputs(loss=outputs)
 
 
-@register_model("core/model/generation/chatglm", generation_model_decorator)
-class ChatGLMForGeneration(_ChatGLMForGeneration):
-    """Generation model based on ChatGLM."""
+@register_model("core/model/generation/llama", generation_model_decorator)
+class LlamaForGeneration(_LlamaForGeneration):
+    """Llama model for generation tasks."""
 
     def __init__(
         self,
         config_path: str,
+        quant_config_path: Optional[str] = None,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the ChatGLMForGeneration model.
+        Initialize the LlamaForGeneration model.
 
         Args:
             config_path (str): The path to the model configuration file.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
+            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__(
             config_path=config_path,
+            quant_config_path=quant_config_path,
             gradient_checkpointing=gradient_checkpointing,
         )
 
     @classmethod
-    @add_default_section_for_init("core/model/generation/chatglm")
+    @add_default_section_for_init("core/model/generation/llama")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of ChatGLMForGeneration from the core configuration.
+        Create an instance of LlamaForGeneration from a core configuration.
 
         Args:
-            config (Config): The core configuration object.
+            config: The core configuration.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            ChatGLMForGeneration: An instance of ChatGLMForGeneration initialized with the provided configuration.
+            LlamaForGeneration: An instance of LlamaForGeneration.
         """
-        config.set_default_section("core/model/generation/chatglm")
-        pretrained_name = config.getoption("pretrained_name", "default-chatglm")
+        config.set_default_section("core/model/generation/llama")
+        pretrained_name = config.getoption("pretrained_name", "default-llama")
         config_path = config.getoption("config_path", None)
         config_path = pop_value(
             config_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "config"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
         )
 
         config_path = cached_path(config_path)
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
         gradient_checkpointing = config.getoption("gradient_checkpointing", False)
 
-        inst = cls(config_path, gradient_checkpointing)
+        inst = cls(
+            config_path,
+            quant_config_path=quant_config_path,
+            gradient_checkpointing=gradient_checkpointing,
+        )
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
         weight_path = pop_value(
             pretrained_weight_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "weight"),
+            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
             check_none=False,
         )
+
         if weight_path is not None:
             inst.from_pretrained(
                 weight_path=weight_path,
             )
 
         return inst
 
@@ -262,39 +297,39 @@
     def forward(
         self,
         input_ids: Optional[torch.Tensor],
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
     ):
         """
-        Perform forward pass of the ChatGLMForGeneration model.
+        Perform a forward pass on the LlamaForGeneration model.
 
         Args:
-            input_ids (torch.Tensor, optional): The input sequence IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+            input_ids (torch.Tensor, optional): The input tensor containing the input IDs. Defaults to None.
+            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
+            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
 
         Returns:
-            GenerationOutputs: The generation outputs.
+            GenerationOutputs: The output of the generation model.
         """
         outputs = super().forward(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
         return GenerationOutputs(sequences=outputs)
 
-    @add_default_section_for_function("core/model/generation/chatglm")
+    @add_default_section_for_function("core/model/generation/llama")
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
-        decoder_start_token_id: Optional[int] = 2,
+        decoder_start_token_id: Optional[int] = 1,
         decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
@@ -303,21 +338,21 @@
         diversity_penalty: Optional[float] = 0.0,
         do_sample: Optional[bool] = False,
         temperature: Optional[float] = 1.0,
         top_k: Optional[int] = 50,
         top_p: Optional[float] = 1.0,
     ):
         """
-        Generate sequences using the ChatGLM model.
+        Generate sequences using the Llama model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
+            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/blip/processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,268 +1,231 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
+import os
+import torch
+import numpy as np
+from PIL import Image
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from unitorch.utils import pop_value, nested_dict_value
-from unitorch.models.chatglm import ChatGLMProcessor as _ChatGLMProcessor
-from unitorch.cli import (
-    cached_path,
-    add_default_section_for_init,
-    add_default_section_for_function,
-    register_process,
+from torchvision.transforms import Resize, CenterCrop, ToTensor, Normalize, Compose
+from transformers import BlipImageProcessor, BertTokenizer
+from transformers.image_utils import to_numpy_array, ChannelDimension
+from transformers.image_transforms import to_channel_dimension_format
+from unitorch.utils import pop_value
+from unitorch.models import (
+    HfTextClassificationProcessor,
+    HfTextGenerationProcessor,
+    HfImageClassificationProcessor,
+    GenericOutputs,
 )
-from unitorch.cli import WriterOutputs
-from unitorch.cli.models import (
-    TensorsInputs,
-    GenerationOutputs,
-    GenerationTargets,
-)
-from unitorch.cli.models.chatglm import pretrained_chatglm_infos
-
 
-class ChatGLMProcessor(_ChatGLMProcessor):
-    """Processor for the ChatGLM model."""
 
+class BlipProcessor(
+    HfTextClassificationProcessor,
+    HfTextGenerationProcessor,
+    HfImageClassificationProcessor,
+):
     def __init__(
         self,
         vocab_path: str,
-        tokenizer_path: str,
+        vision_config_path: str,
         max_seq_length: Optional[int] = 128,
-        max_gen_seq_length: Optional[int] = 128,
+        max_gen_seq_length: Optional[int] = 48,
+        position_start_id: Optional[int] = 0,
     ):
         """
-        Initialize the ChatGLMProcessor.
+        Initializes the BlipProcessor.
 
         Args:
             vocab_path (str): The path to the vocabulary file.
-            tokenizer_path (str): The path to the tokenizer file.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to 128.
-            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to 128.
+            vision_config_path (str): The path to the vision configuration file.
+            max_seq_length (Optional[int]): The maximum sequence length for text inputs. Defaults to 128.
+            max_gen_seq_length (Optional[int]): The maximum sequence length for generated outputs. Defaults to 48.
+            position_start_id (Optional[int]): The position start ID. Defaults to 0.
         """
-        super().__init__(
+        vision_processor = BlipImageProcessor.from_json_file(vision_config_path)
+        HfImageClassificationProcessor.__init__(self, vision_processor=vision_processor)
+
+        tokenizer = BertTokenizer(
             vocab_file=vocab_path,
-            tokenizer_file=tokenizer_path,
+        )
+        tokenizer.bos_token = tokenizer.cls_token
+        tokenizer.bos_token_id = tokenizer.cls_token_id
+        tokenizer.eos_token = tokenizer.sep_token
+        tokenizer.eos_token_id = tokenizer.sep_token_id
+        HfTextClassificationProcessor.__init__(
+            self,
+            tokenizer=tokenizer,
+            max_seq_length=max_seq_length,
+            source_type_id=0,
+            target_type_id=0,
+            position_start_id=position_start_id,
+        )
+
+        HfTextGenerationProcessor.__init__(
+            self,
+            tokenizer=tokenizer,
             max_seq_length=max_seq_length,
             max_gen_seq_length=max_gen_seq_length,
         )
 
-    @classmethod
-    @add_default_section_for_init("core/process/chatglm")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of ChatGLMProcessor from a core configuration.
-
-        Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            dict: A dictionary containing the processor's initialization arguments.
-        """
-        config.set_default_section("core/process/chatglm")
-        pretrained_name = config.getoption("pretrained_name", "default-chatglm")
-        vocab_path = config.getoption("vocab_path", None)
-        vocab_path = pop_value(
-            vocab_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "vocab"),
-        )
-        vocab_path = cached_path(vocab_path)
-
-        tokenizer_path = config.getoption("tokenizer_path", None)
-        tokenizer_path = pop_value(
-            tokenizer_path,
-            nested_dict_value(pretrained_chatglm_infos, pretrained_name, "tokenizer"),
-        )
-        tokenizer_path = cached_path(tokenizer_path)
-
-        return {
-            "vocab_path": vocab_path,
-            "tokenizer_path": tokenizer_path,
-        }
-
-    @register_process("core/process/chatglm/classification")
-    def _classification(
+    def text_classification(
         self,
         text: str,
-        text_pair: Optional[str] = None,
         max_seq_length: Optional[int] = None,
-    ):
+    ) -> GenericOutputs:
         """
-        Process text inputs for classification.
+        Performs text classification on the given input text.
 
         Args:
-            text (str): The input text.
-            text_pair (str, optional): The input text pair. Defaults to None.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
+            text (str): The input text to classify.
+            max_seq_length (Optional[int]): The maximum sequence length for the text. If None, the default value from initialization is used.
 
         Returns:
-            TensorsInputs: The processed inputs as tensors.
+            GenericOutputs: The outputs of the text classification.
         """
-        outputs = super().classification(
+        outputs = HfTextClassificationProcessor.classification(
+            self,
             text=text,
-            text_pair=text_pair,
             max_seq_length=max_seq_length,
         )
-        return TensorsInputs(
+        return GenericOutputs(
             input_ids=outputs.input_ids,
             attention_mask=outputs.attention_mask,
             position_ids=outputs.position_ids,
         )
 
-    @register_process("core/process/chatglm/pretrain")
-    def _pretrain(
+    def image_classification(
         self,
-        text: str,
-        text_pair: Optional[str] = None,
-        max_seq_length: Optional[int] = None,
-        max_gen_seq_length: Optional[int] = None,
-    ):
+        image: Image.Image,
+    ) -> GenericOutputs:
         """
-        Process text inputs for pretraining.
+        Performs image classification on the given input image.
 
         Args:
-            text (str): The input text.
-            text_pair (str, optional): The input text pair. Defaults to None.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
-            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to None.
+            image (PIL.Image.Image): The input image to classify.
 
         Returns:
-            TensorsInputs: The processed inputs as tensors.
+            GenericOutputs: The outputs of the image classification.
         """
-        outputs = super().generation(
-            text=text,
-            text_pair=text_pair,
-            max_seq_length=max_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
+        outputs = HfImageClassificationProcessor.classification(
+            self,
+            image=image,
         )
-        return TensorsInputs(
-            input_ids=outputs.input_ids,
-            attention_mask=outputs.attention_mask,
-            position_ids=outputs.position_ids,
-            input_ids_label=outputs.input_ids_label,
-            attention_mask_label=outputs.attention_mask_label,
+
+        return GenericOutputs(
+            pixel_values=outputs.pixel_values,
         )
 
-    @register_process("core/process/chatglm/prompt")
-    def _prompt(
+    def classification(
         self,
         text: str,
+        image: Image.Image,
         max_seq_length: Optional[int] = None,
-    ):
+    ) -> GenericOutputs:
         """
-        Process text inputs for prompting.
+        Performs classification using both text and image inputs.
 
         Args:
-            text (str): The input text.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
+            text (str): The input text to classify.
+            image (PIL.Image.Image): The input image to classify.
+            max_seq_length (Optional[int]): The maximum sequence length for the text. If None, the default value from initialization is used.
 
         Returns:
-            TensorsInputs: The processed inputs as tensors.
+            GenericOutputs: The outputs of the classification.
         """
-        outputs = super().prompt(
-            text=text,
-            max_seq_length=max_seq_length,
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
         )
-        return TensorsInputs(input_ids=outputs.input_ids)
 
-    @register_process("core/process/chatglm/generation/inputs")
-    def _generation_inputs(
+        text_outputs = self.text_classification(text, max_seq_length)
+        pixel_outputs = self.image_classification(image)
+
+        return GenericOutputs(
+            input_ids=text_outputs.input_ids,
+            attention_mask=text_outputs.attention_mask,
+            position_ids=text_outputs.position_ids,
+            pixel_values=pixel_outputs.pixel_values,
+        )
+
+    def generation_inputs(
         self,
         text: str,
         max_seq_length: Optional[int] = None,
-    ):
+    ) -> GenericOutputs:
         """
-        Preprocess the input text for generation tasks.
+        Generate inputs for text generation.
 
         Args:
             text (str): The input text.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
 
         Returns:
-            TensorsInputs: The processed input tensors.
+            GenericOutputs: The generated input tokens and attention mask.
         """
-        outputs = super().generation_inputs(
+        outputs = HfTextGenerationProcessor.generation_inputs(
+            self,
             text=text,
             max_seq_length=max_seq_length,
         )
-        return TensorsInputs(input_ids=outputs.input_ids)
+        return GenericOutputs(
+            input_ids=outputs.input_ids,
+            attention_mask=outputs.attention_mask,
+        )
 
-    @register_process("core/process/chatglm/generation/labels")
-    def _generation_labels(
+    def generation_labels(
         self,
         text: str,
         max_gen_seq_length: Optional[int] = None,
-    ):
+    ) -> GenericOutputs:
         """
-        Preprocess the target text for generation tasks.
+        Generates labels for text generation based on the given input text.
 
         Args:
-            text (str): The target text.
-            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to None.
+            text (str): The input text for generating labels.
+            max_gen_seq_length (Optional[int]): The maximum sequence length for the generated labels. If None, the default value from initialization is used.
 
         Returns:
-            GenerationTargets: The processed generation targets.
+            GenericOutputs: The generated labels.
         """
-        outputs = super().generation_labels(
+        outputs = HfTextGenerationProcessor.generation_labels(
+            self,
             text=text,
             max_gen_seq_length=max_gen_seq_length,
         )
-        return GenerationTargets(
-            refs=outputs.input_ids,
-            masks=outputs.attention_mask,
+        return GenericOutputs(
+            input_ids=outputs.input_ids,
+            attention_mask=outputs.attention_mask,
         )
 
-    @register_process("core/process/chatglm/generation")
-    def _generation(
+    def generation(
         self,
         text: str,
-        text_pair: Optional[str] = None,
-        max_seq_length: Optional[int] = None,
+        image: Image.Image,
         max_gen_seq_length: Optional[int] = None,
-    ):
+    ) -> GenericOutputs:
         """
-        Preprocess the input and target texts for generation tasks.
+        Generate inputs, labels, and tokens for image to text generation.
 
         Args:
             text (str): The input text.
-            text_pair (str, optional): The paired input text. Defaults to None.
-            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
-            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to None.
+            image (Image.Image): The input image to caption.
+            max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to None.
 
         Returns:
-            Tuple[TensorsInputs, GenerationTargets]: The processed input tensors and generation targets.
-        """
-        outputs = super().generation(
-            text=text,
-            text_pair=text_pair,
-            max_seq_length=max_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-        )
-        return TensorsInputs(
-            input_ids=outputs.input_ids,
-            attention_mask=outputs.attention_mask,
-            position_ids=outputs.position_ids,
-        ), GenerationTargets(
-            refs=outputs.input_ids_label,
-            masks=outputs.attention_mask_label,
-        )
-
-    @register_process("core/postprocess/chatglm/detokenize")
-    def _detokenize(
-        self,
-        outputs: GenerationOutputs,
-    ):
+            GenericOutputs: The generated input tokens, attention masks, label tokens, and attention masks.
         """
-        Detokenize the generated sequences.
 
-        Args:
-            outputs (GenerationOutputs): The generation outputs.
+        max_gen_seq_length = pop_value(max_gen_seq_length, self.max_gen_seq_length)
 
-        Returns:
-            WriterOutputs: The detokenized writer outputs.
-        """
-        results = outputs.to_pandas()
-        assert results.shape[0] == 0 or results.shape[0] == outputs.sequences.shape[0]
+        tokens = self.generation_inputs(text, max_gen_seq_length)
+        pixels = self.image_classification(image)
+        labels = self.generation_labels(text, max_gen_seq_length)
 
-        decoded = super().detokenize(sequences=outputs.sequences)
-        results["decoded"] = decoded
-        return WriterOutputs(results)
+        return GenericOutputs(
+            input_ids=tokens.input_ids,
+            attention_mask=tokens.attention_mask,
+            pixel_values=pixels.pixel_values,
+            input_ids_label=labels.input_ids,
+            attention_mask_label=labels.attention_mask,
+        )
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/classification_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/classification_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/clip/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/clip/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/clip/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling_v2.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing_v2.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/detection_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/detection_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/modeling_controlnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def __init__(
         self,
         config_path: str,
         text_config_path: str,
         vae_config_path: str,
         controlnet_config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 4,
         out_channels: Optional[int] = 4,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         freeze_vae_encoder: Optional[bool] = True,
         freeze_text_encoder: Optional[bool] = True,
@@ -41,27 +42,25 @@
     ):
         super().__init__(
             config_path=config_path,
             text_config_path=text_config_path,
             vae_config_path=vae_config_path,
             controlnet_config_path=controlnet_config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             freeze_vae_encoder=freeze_vae_encoder,
             freeze_text_encoder=freeze_text_encoder,
             freeze_unet_encoder=freeze_unet_encoder,
             seed=seed,
         )
-        for n, p in self.named_parameters():
-            if "blocks" in n:
-                p.requires_grad = False
 
     @classmethod
     @add_default_section_for_init("core/model/diffusion/controlnet")
     def from_core_configure(cls, config, **kwargs):
         config.set_default_section("core/model/diffusion/controlnet")
         pretrained_name = config.getoption("pretrained_name", "controlnet-canny")
         pretrain_infos = nested_dict_value(pretrained_diffusers_infos, pretrained_name)
@@ -97,14 +96,18 @@
         scheduler_config_path = config.getoption("scheduler_config_path", None)
         scheduler_config_path = pop_value(
             scheduler_config_path,
             nested_dict_value(pretrain_infos, "scheduler"),
         )
         scheduler_config_path = cached_path(scheduler_config_path)
 
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
+
         image_size = config.getoption("image_size", 224)
         in_channels = config.getoption("in_channels", 4)
         out_channels = config.getoption("out_channels", 4)
         num_train_timesteps = config.getoption("num_train_timesteps", 1000)
         num_infer_timesteps = config.getoption("num_infer_timesteps", 50)
         freeze_vae_encoder = config.getoption("freeze_vae_encoder", True)
         freeze_text_encoder = config.getoption("freeze_text_encoder", True)
@@ -113,14 +116,15 @@
 
         inst = cls(
             config_path=config_path,
             text_config_path=text_config_path,
             vae_config_path=vae_config_path,
             controlnet_config_path=controlnet_config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             freeze_vae_encoder=freeze_vae_encoder,
             freeze_text_encoder=freeze_text_encoder,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/modeling_stable.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 
 @register_model("core/model/diffusion/stable/image", diffusion_model_decorator)
 class StableForImageGeneration(_StableForImageGeneration):
     def __init__(
         self,
         config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 3,
         out_channels: Optional[int] = 3,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         seed: Optional[int] = 1123,
     ):
         super().__init__(
             config_path=config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             seed=seed,
         )
@@ -60,25 +62,29 @@
 
         scheduler_config_path = config.getoption("scheduler_config_path", None)
         scheduler_config_path = pop_value(
             scheduler_config_path,
             nested_dict_value(pretrained_diffusers_infos, pretrained_name, "scheduler"),
         )
         scheduler_config_path = cached_path(scheduler_config_path)
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
 
         image_size = config.getoption("image_size", 224)
         in_channels = config.getoption("in_channels", 3)
         out_channels = config.getoption("out_channels", 3)
         num_train_timesteps = config.getoption("num_train_timesteps", 1000)
         num_infer_timesteps = config.getoption("num_infer_timesteps", 50)
         seed = config.getoption("seed", 1123)
 
         inst = cls(
             config_path=config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             seed=seed,
         )
@@ -116,28 +122,30 @@
 class StableForText2ImageGeneration(_StableForText2ImageGeneration):
     def __init__(
         self,
         config_path: str,
         text_config_path: str,
         vae_config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 4,
         out_channels: Optional[int] = 4,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         freeze_vae_encoder: Optional[bool] = True,
         freeze_text_encoder: Optional[bool] = True,
         seed: Optional[int] = 1123,
     ):
         super().__init__(
             config_path=config_path,
             text_config_path=text_config_path,
             vae_config_path=vae_config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             freeze_vae_encoder=freeze_vae_encoder,
             freeze_text_encoder=freeze_text_encoder,
@@ -175,28 +183,33 @@
         scheduler_config_path = config.getoption("scheduler_config_path", None)
         scheduler_config_path = pop_value(
             scheduler_config_path,
             nested_dict_value(pretrain_infos, "scheduler"),
         )
         scheduler_config_path = cached_path(scheduler_config_path)
 
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
+
         image_size = config.getoption("image_size", 224)
         in_channels = config.getoption("in_channels", 4)
         out_channels = config.getoption("out_channels", 4)
         num_train_timesteps = config.getoption("num_train_timesteps", 1000)
         num_infer_timesteps = config.getoption("num_infer_timesteps", 50)
         freeze_vae_encoder = config.getoption("freeze_vae_encoder", True)
         freeze_text_encoder = config.getoption("freeze_text_encoder", True)
         seed = config.getoption("seed", 1123)
 
         inst = cls(
             config_path=config_path,
             text_config_path=text_config_path,
             vae_config_path=vae_config_path,
             scheduler_config_path=scheduler_config_path,
+            quant_config_path=quant_config_path,
             image_size=image_size,
             in_channels=in_channels,
             out_channels=out_channels,
             num_train_timesteps=num_train_timesteps,
             num_infer_timesteps=num_infer_timesteps,
             freeze_vae_encoder=freeze_vae_encoder,
             freeze_text_encoder=freeze_text_encoder,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_stable.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/diffusion_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/diffusion_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/generation_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/image_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/label_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/label_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/llama/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/llama/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/peft/modeling_bloom.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,300 +1,291 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
+import os
+import logging
 import torch
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from torch.cuda.amp import autocast
 from transformers.utils import is_remote_url
 from unitorch.utils import pop_value, nested_dict_value
-from unitorch.models.llama import (
-    LlamaForClassification as _LlamaForClassification,
-    LlamaForGeneration as _LlamaForGeneration,
-    LlamaForPretrain as _LlamaForPretrain,
+from unitorch.models.peft import (
+    BloomLoraForClassification as _BloomLoraForClassification,
+    BloomLoraForGeneration as _BloomLoraForGeneration,
 )
 from unitorch.cli import (
     cached_path,
     add_default_section_for_init,
     add_default_section_for_function,
     register_model,
 )
 from unitorch.cli.models import generation_model_decorator
 from unitorch.cli.models import ClassificationOutputs, GenerationOutputs, LossOutputs
-from unitorch.cli.models.llama import pretrained_llama_infos
+from unitorch.cli.models.bloom import pretrained_bloom_infos
 
 
-@register_model("core/model/classification/llama")
-class LlamaForClassification(_LlamaForClassification):
-    """Llama model for classification tasks."""
-
+@register_model("core/model/classification/peft/lora/bloom")
+class BloomLoraForClassification(_BloomLoraForClassification):
     def __init__(
         self,
         config_path: str,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
         num_classes: Optional[int] = 1,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the LlamaForClassification model.
+        Initialize the BloomLoraForClassification model.
 
         Args:
             config_path (str): The path to the model configuration file.
-            num_classes (int, optional): The number of classes for classification. Defaults to 1.
+            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
+            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
+            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
+            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
+            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
+            num_classes (int, optional): The number of classes. Defaults to 1.
             gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__(
             config_path=config_path,
+            lora_r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
             num_classes=num_classes,
             gradient_checkpointing=gradient_checkpointing,
         )
 
     @classmethod
-    @add_default_section_for_init("core/model/classification/llama")
+    @add_default_section_for_init("core/model/classification/peft/lora/bloom")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of LlamaForClassification from a core configuration.
+        Create an instance of BloomLoraForClassification from a core configuration.
 
         Args:
             config: The core configuration.
             **kwargs: Additional keyword arguments.
 
         Returns:
-            LlamaForClassification: An instance of LlamaForClassification.
+            BloomLoraForClassification: The initialized BloomLoraForClassification instance.
         """
-        config.set_default_section("core/model/classification/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
+        config.set_default_section("core/model/classification/peft/lora/bloom")
+        pretrained_name = config.getoption("pretrained_name", "default-bloom")
         config_path = config.getoption("config_path", None)
         config_path = pop_value(
             config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
+            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
         )
-
         config_path = cached_path(config_path)
+
+        lora_r = config.getoption("lora_r", 16)
+        lora_alpha = config.getoption("lora_alpha", 32)
+        lora_dropout = config.getoption("lora_dropout", 0.05)
+        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
+        target_modules = config.getoption("target_modules", ["query_key_value"])
+
         gradient_checkpointing = config.getoption("gradient_checkpointing", False)
         num_classes = config.getoption("num_classes", 1)
 
-        inst = cls(config_path, num_classes, gradient_checkpointing)
+        inst = cls(
+            config_path,
+            lora_r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
+            num_classes=num_classes,
+            gradient_checkpointing=gradient_checkpointing,
+        )
 
+        weight_path = []
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        weight_path = pop_value(
+        pretrained_weight_path = pop_value(
             pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
+            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
             check_none=False,
         )
+        if pretrained_weight_path is not None:
+            if isinstance(pretrained_weight_path, str):
+                weight_path.append(pretrained_weight_path)
+            elif isinstance(pretrained_weight_path, list):
+                weight_path.extend(pretrained_weight_path)
+
+        pretrained_lora_weight_path = config.getoption(
+            "pretrained_lora_weight_path", None
+        )
+        if pretrained_lora_weight_path is not None:
+            weight_path.append(pretrained_lora_weight_path)
 
-        if weight_path is not None:
+        if len(weight_path) > 0:
             inst.from_pretrained(
                 weight_path=weight_path,
             )
 
         return inst
 
     @autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
     ):
         """
-        Perform a forward pass on the LlamaForClassification model.
+        Perform forward pass of the BloomLoraForClassification model.
 
         Args:
-            input_ids (torch.Tensor): The input tensor containing the input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
-            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
+            input_ids (torch.Tensor): The input IDs.
+            attention_mask (torch.Tensor, optional): The attention mask.
+            position_ids (torch.Tensor, optional): The position IDs.
 
         Returns:
-            ClassificationOutputs: The output of the classification model.
+            ClassificationOutputs: The output of the classification task.
         """
         outputs = super().forward(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
         return ClassificationOutputs(outputs=outputs)
 
 
-@register_model("core/model/pretrain/llama")
-class LlamaForPretrain(_LlamaForPretrain):
-    """Llama model for pretraining tasks."""
+@register_model("core/model/generation/peft/lora/bloom", generation_model_decorator)
+class BloomLoraForGeneration(_BloomLoraForGeneration):
+    """BloomLora model for generation tasks."""
 
     def __init__(
         self,
         config_path: str,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the LlamaForPretrain model.
+        Initialize the BloomLoraForGeneration model.
 
         Args:
             config_path (str): The path to the model configuration file.
+            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
+            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
+            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
+            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
+            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
             gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__(
             config_path=config_path,
+            lora_r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
             gradient_checkpointing=gradient_checkpointing,
         )
 
     @classmethod
-    @add_default_section_for_init("core/model/pretrain/llama")
+    @add_default_section_for_init("core/model/generation/peft/lora/bloom")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of LlamaForPretrain from a core configuration.
+        Create an instance of BloomLoraForGeneration from a core configuration.
 
         Args:
             config: The core configuration.
             **kwargs: Additional keyword arguments.
 
         Returns:
-            LlamaForPretrain: An instance of LlamaForPretrain.
+            BloomLoraForGeneration: The initialized BloomLoraForGeneration instance.
         """
-        config.set_default_section("core/model/pretrain/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
+        config.set_default_section("core/model/generation/peft/lora/bloom")
+        pretrained_name = config.getoption("pretrained_name", "default-bloom")
         config_path = config.getoption("config_path", None)
         config_path = pop_value(
             config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
+            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
         )
-
         config_path = cached_path(config_path)
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(config_path, gradient_checkpointing)
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
 
-        if weight_path is not None:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
+        lora_r = config.getoption("lora_r", 16)
+        lora_alpha = config.getoption("lora_alpha", 32)
+        lora_dropout = config.getoption("lora_dropout", 0.05)
+        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
+        target_modules = config.getoption("target_modules", ["query_key_value"])
 
-        return inst
-
-    @autocast()
-    def forward(
-        self,
-        input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-        input_ids_label: Optional[torch.Tensor] = None,
-        attention_mask_label: Optional[torch.Tensor] = None,
-    ):
-        """
-        Perform a forward pass on the LlamaForPretrain model.
-
-        Args:
-            input_ids (torch.Tensor): The input tensor containing the input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
-            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
-            input_ids_label (torch.Tensor, optional): The input tensor containing the input IDs for the masked language model. Defaults to None.
-            attention_mask_label (torch.Tensor, optional): The attention mask tensor for the masked language model. Defaults to None.
-
-        Returns:
-            LossOutputs: The output of the pretraining model.
-        """
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-            input_ids_label=input_ids_label,
-            attention_mask_label=attention_mask_label,
-        )
-        return LossOutputs(loss=outputs)
-
-
-@register_model("core/model/generation/llama", generation_model_decorator)
-class LlamaForGeneration(_LlamaForGeneration):
-    """Llama model for generation tasks."""
-
-    def __init__(
-        self,
-        config_path: str,
-        gradient_checkpointing: Optional[bool] = False,
-    ):
-        """
-        Initialize the LlamaForGeneration model.
-
-        Args:
-            config_path (str): The path to the model configuration file.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/generation/llama")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of LlamaForGeneration from a core configuration.
-
-        Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
+        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
 
-        Returns:
-            LlamaForGeneration: An instance of LlamaForGeneration.
-        """
-        config.set_default_section("core/model/generation/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
+        inst = cls(
             config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
+            lora_r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
+            gradient_checkpointing=gradient_checkpointing,
         )
 
-        config_path = cached_path(config_path)
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(config_path, gradient_checkpointing)
+        weight_path = []
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        weight_path = pop_value(
+        pretrained_weight_path = pop_value(
             pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
+            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
             check_none=False,
         )
+        if pretrained_weight_path is not None:
+            if isinstance(pretrained_weight_path, str):
+                weight_path.append(pretrained_weight_path)
+            elif isinstance(pretrained_weight_path, list):
+                weight_path.extend(pretrained_weight_path)
+
+        pretrained_lora_weight_path = config.getoption(
+            "pretrained_lora_weight_path", None
+        )
+        if pretrained_lora_weight_path is not None:
+            weight_path.append(pretrained_lora_weight_path)
 
-        if weight_path is not None:
+        if len(weight_path) > 0:
             inst.from_pretrained(
                 weight_path=weight_path,
             )
 
         return inst
 
     @autocast()
     def forward(
         self,
         input_ids: Optional[torch.Tensor],
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
     ):
         """
-        Perform a forward pass on the LlamaForGeneration model.
+        Perform forward pass of the BloomLoraForGeneration model.
 
         Args:
-            input_ids (torch.Tensor, optional): The input tensor containing the input IDs. Defaults to None.
-            attention_mask (torch.Tensor, optional): The attention mask tensor. Defaults to None.
-            position_ids (torch.Tensor, optional): The position IDs tensor. Defaults to None.
+            input_ids (torch.Tensor, optional): The input IDs.
+            attention_mask (torch.Tensor, optional): The attention mask.
+            position_ids (torch.Tensor, optional): The position IDs.
 
         Returns:
-            GenerationOutputs: The output of the generation model.
+            GenerationOutputs: The output of the generation task.
         """
         outputs = super().forward(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
         return GenerationOutputs(sequences=outputs)
 
-    @add_default_section_for_function("core/model/generation/llama")
+    @add_default_section_for_function("core/model/generation/peft/lora/bloom")
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
@@ -310,21 +301,21 @@
         diversity_penalty: Optional[float] = 0.0,
         do_sample: Optional[bool] = False,
         temperature: Optional[float] = 1.0,
         top_k: Optional[int] = 50,
         top_p: Optional[float] = 1.0,
     ):
         """
-        Generate sequences using the Llama model.
+        Generate sequences using the Bloom model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 1.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
+            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/llama/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/modeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     It inherits from the _MiniGPT4Blip2LlamaForGeneration class.
     """
 
     def __init__(
         self,
         blip2_config_path: str,
         llama_config_path: str,
+        quant_config_path: Optional[str] = None,
         pad_token_id: Optional[int] = 0,
         freeze_vision_model: Optional[bool] = True,
         freeze_qformer_model: Optional[bool] = True,
         freeze_llama_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
@@ -48,14 +49,15 @@
             freeze_qformer_model (bool, optional): Whether to freeze the query transformer model. Defaults to True.
             freeze_llama_model (bool, optional): Whether to freeze the Llama model. Defaults to True.
             gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
         """
         super().__init__(
             blip2_config_path=blip2_config_path,
             llama_config_path=llama_config_path,
+            quant_config_path=quant_config_path,
             pad_token_id=pad_token_id,
             freeze_vision_model=freeze_vision_model,
             freeze_qformer_model=freeze_qformer_model,
             freeze_llama_model=freeze_llama_model,
             gradient_checkpointing=gradient_checkpointing,
         )
 
@@ -89,22 +91,27 @@
             llama_config_path,
             nested_dict_value(
                 pretrained_minigpt4_infos, pretrained_name, "llama_config_path"
             ),
         )
         llama_config_path = cached_path(llama_config_path)
 
+        quant_config_path = config.getoption("quant_config_path", None)
+        if quant_config_path is not None:
+            quant_config_path = cached_path(quant_config_path)
+
         freeze_vision_model = config.getoption("freeze_vision_model", True)
         freeze_qformer_model = config.getoption("freeze_qformer_model", True)
         freeze_llama_model = config.getoption("freeze_llama_model", True)
         gradient_checkpointing = config.getoption("gradient_checkpointing", False)
 
         inst = cls(
             blip2_config_path,
             llama_config_path,
+            quant_config_path=quant_config_path,
             freeze_vision_model=freeze_vision_model,
             freeze_qformer_model=freeze_qformer_model,
             freeze_llama_model=freeze_llama_model,
             gradient_checkpointing=gradient_checkpointing,
         )
         pretrained_weight_path = config.getoption("pretrained_weight_path", None)
         weight_path = pop_value(
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/minigpt4/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/modeling_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_bloom.py` & `unitorch-0.0.0.7/src/unitorch/cli/tasks/deepspeed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,741 +1,711 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import os
-import logging
 import torch
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from torch.cuda.amp import autocast
-from transformers.utils import is_remote_url
-from unitorch.utils import pop_value, nested_dict_value
-from unitorch.models.peft import (
-    BloomAdaLoraForClassification as _BloomAdaLoraForClassification,
-    BloomAdaLoraForGeneration as _BloomAdaLoraForGeneration,
-    BloomLoraForClassification as _BloomLoraForClassification,
-    BloomLoraForGeneration as _BloomLoraForGeneration,
+import time
+import json
+import logging
+import deepspeed
+import numpy as np
+import pandas as pd
+import torch.distributed as dist
+import torch.nn as nn
+import torch.nn.functional as F
+from copy import deepcopy
+from itertools import chain
+from collections.abc import Iterable
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, Iterator
+from torch.utils.data import DataLoader, Dataset, SequentialSampler
+from torch.utils.data.distributed import DistributedSampler
+from torch.cuda.amp import autocast, GradScaler
+from torch.multiprocessing import Process, Queue
+from unitorch import set_seed, is_torch2_available
+from unitorch.models import ExponentialMovingAverage
+from unitorch.utils import get_local_rank
+from unitorch.utils import (
+    DistributedSkipSampler,
+    RandomSkipSampler,
+    SequentialSkipSampler,
+    PostProcess,
+    IOProcess,
+    GENERATE_FINISHED,
 )
+from unitorch.models import GenericOutputs
+from unitorch.utils import ActiveGPUJob
 from unitorch.cli import (
     cached_path,
+    register_task,
+    registered_model,
+    registered_optim,
+    registered_dataset,
+    registered_loss,
+    registered_score,
+    registered_scheduler,
+    registered_writer,
+    init_registered_module,
+    init_registered_process,
     add_default_section_for_init,
     add_default_section_for_function,
-    register_model,
 )
-from unitorch.cli.models import generation_model_decorator
-from unitorch.cli.models import ClassificationOutputs, GenerationOutputs, LossOutputs
-from unitorch.cli.models.bloom import pretrained_bloom_infos
+from unitorch.cli.models import (
+    ModelInputs,
+    ModelOutputs,
+    ModelTargets,
+    LossOutputs,
+    CombineTensorsInputs,
+    CombineTensorsTargets,
+)
+from unitorch.cli.tasks.supervised import (
+    DatasetFeature,
+    collate_fn,
+    infer,
+    monitor,
+    save_checkpoint,
+)
 
 
-@register_model("core/model/classification/peft/adalora/bloom")
-class BloomAdaLoraForClassification(_BloomAdaLoraForClassification):
-    """BloomAdaLora model for classification tasks."""
+@register_task("core/task/deepspeed/supervised")
+class DeepspeedTask:
+    """Task class for deepspeed supervised learning."""
 
     def __init__(
         self,
-        config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
-        num_classes: Optional[int] = 1,
-        gradient_checkpointing: Optional[bool] = False,
+        configure,
+        model,
+        datasets,
+        local_rank: Optional[int] = -1,
+        seed: Optional[int] = 1123,
     ):
         """
-        Initialize the BloomAdaLoraForClassification model.
-
-        Args:
-            config_path (str): The path to the model configuration file.
-            target_r (int, optional): The target rank. Defaults to 8.
-            init_r (int, optional): The initial rank. Defaults to 12.
-            tinit (int, optional): The initial temperature. Defaults to 0.
-            tfinal (int, optional): The final temperature. Defaults to 0.
-            deltaT (int, optional): The temperature change rate. Defaults to 1.
-            beta1 (float, optional): The value of beta1 for optimizer. Defaults to 0.85.
-            beta2 (float, optional): The value of beta2 for optimizer. Defaults to 0.85.
-            orth_reg_weight (float, optional): The weight of the orthogonality regularization. Defaults to 0.5.
-            total_step (int, optional): The total number of training steps. Defaults to None.
-            rank_pattern (dict, optional): The rank pattern. Defaults to None.
-            num_classes (int, optional): The number of classes. Defaults to 1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/classification/peft/adalora/bloom")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of BloomAdaLoraForClassification from a core configuration.
+        Initialize the DeepspeedTask.
 
         Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            BloomAdaLoraForClassification: The initialized BloomAdaLoraForClassification instance.
-        """
-        config.set_default_section("core/model/classification/peft/adalora/bloom")
-        pretrained_name = config.getoption("pretrained_name", "default-bloom")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        target_r = config.getoption("target_r", 8)
-        init_r = config.getoption("init_r", 12)
-        tinit = config.getoption("tinit", 0)
-        tfinal = config.getoption("tfinal", 0)
-        deltaT = config.getoption("deltaT", 1)
-        beta1 = config.getoption("beta1", 0.85)
-        beta2 = config.getoption("beta2", 0.85)
-        orth_reg_weight = config.getoption("orth_reg_weight", 0.5)
-        total_step = config.getoption("total_step", None)
-        rank_pattern = config.getoption("rank_pattern", None)
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-        num_classes = config.getoption("num_classes", 1)
-
-        inst = cls(
-            config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_adalora_weight_path = config.getoption(
-            "pretrained_adalora_weight_path", None
-        )
-        if pretrained_adalora_weight_path is not None:
-            weight_path.append(pretrained_adalora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
-
-        return inst
-
-    @autocast()
-    def forward(
-        self,
-        input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-    ):
+            configure: The configuration object.
+            model: The model for supervised learning.
+            datasets: The datasets for training and evaluation.
+            local_rank (optional): The local rank for distributed training. Defaults to -1.
+            seed (optional): The random seed. Defaults to 1123.
         """
-        Perform forward pass of the BloomAdaLoraForClassification model.
+        set_seed(seed)
+        self.n_gpu = 1 if torch.cuda.is_available() else 0
+        if dist.is_initialized():
+            self.n_gpu = dist.get_world_size()
 
-        Args:
-            input_ids (torch.Tensor): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+        self.config = configure
+        self.model = model
+        self.datasets = datasets
+        self.local_rank = local_rank
 
-        Returns:
-            ClassificationOutputs: The output of the classification task.
-        """
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-        )
-        return ClassificationOutputs(outputs=outputs)
+        if self.local_rank != -1:
+            torch.cuda.set_device(self.local_rank)
 
+        if torch.cuda.is_available():
+            self.model = self.model.cuda()
 
-@register_model("core/model/generation/peft/adalora/bloom", generation_model_decorator)
-class BloomAdaLoraForGeneration(_BloomAdaLoraForGeneration):
-    """BloomAdaLora model for generation tasks."""
-
-    def __init__(
-        self,
-        config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
-        gradient_checkpointing: Optional[bool] = False,
-    ):
-        """
-        Initialize the BloomAdaLoraForGeneration model.
-
-        Args:
-            config_path (str): The path to the model configuration file.
-            target_r (int, optional): The target rank. Defaults to 8.
-            init_r (int, optional): The initial rank. Defaults to 12.
-            tinit (int, optional): The initial temperature. Defaults to 0.
-            tfinal (int, optional): The final temperature. Defaults to 0.
-            deltaT (int, optional): The temperature change rate. Defaults to 1.
-            beta1 (float, optional): The value of beta1 for optimizer. Defaults to 0.85.
-            beta2 (float, optional): The value of beta2 for optimizer. Defaults to 0.85.
-            orth_reg_weight (float, optional): The weight of the orthogonality regularization. Defaults to 0.5.
-            total_step (int, optional): The total number of training steps. Defaults to None.
-            rank_pattern (dict, optional): The rank pattern. Defaults to None.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            gradient_checkpointing=gradient_checkpointing,
-        )
+        self.best_score = -np.inf
 
     @classmethod
-    @add_default_section_for_init("core/model/generation/peft/adalora/bloom")
+    @add_default_section_for_init("core/task/deepspeed/supervised")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create an instance of BloomAdaLoraForGeneration from a core configuration.
+        Create a DeepspeedTask instance from a core configuration.
 
         Args:
             config: The core configuration.
             **kwargs: Additional keyword arguments.
 
         Returns:
-            BloomAdaLoraForGeneration: The initialized BloomAdaLoraForGeneration instance.
+            A DeepspeedTask instance.
         """
-        config.set_default_section("core/model/generation/peft/adalora/bloom")
-        pretrained_name = config.getoption("pretrained_name", "default-bloom")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
+        try:
+            deepspeed.init_distributed(dist_backend="nccl", init_method="env://")
+        except:
+            logging.info("PyTorch is not in distributed mode")
 
-        target_r = config.getoption("target_r", 8)
-        init_r = config.getoption("init_r", 12)
-        tinit = config.getoption("tinit", 0)
-        tfinal = config.getoption("tfinal", 0)
-        deltaT = config.getoption("deltaT", 1)
-        beta1 = config.getoption("beta1", 0.85)
-        beta2 = config.getoption("beta2", 0.85)
-        orth_reg_weight = config.getoption("orth_reg_weight", 0.5)
-        total_step = config.getoption("total_step", None)
-        rank_pattern = config.getoption("rank_pattern", None)
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(
-            config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            gradient_checkpointing=gradient_checkpointing,
-        )
+        config.set_default_section("core/task/deepspeed/supervised")
 
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
+        model = config.getoption("model", None)
+        dataset = config.getoption("dataset", None)
 
-        pretrained_adalora_weight_path = config.getoption(
-            "pretrained_adalora_weight_path", None
-        )
-        if pretrained_adalora_weight_path is not None:
-            weight_path.append(pretrained_adalora_weight_path)
+        if model is not None:
+            model = init_registered_module(model, config, registered_model)
 
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
+        if dataset is not None:
+            dataset = init_registered_module(dataset, config, registered_dataset)
 
-        return inst
-
-    @autocast()
-    def forward(
-        self,
-        input_ids: Optional[torch.Tensor],
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-    ):
-        """
-        Perform forward pass of the BloomAdaLoraForGeneration model.
-
-        Args:
-            input_ids (torch.Tensor, optional): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
-
-        Returns:
-            GenerationOutputs: The output of the generation task.
-        """
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
+        local_rank = config.getdefault(
+            "core/cli",
+            "local_rank",
+            get_local_rank(),
         )
-        return GenerationOutputs(sequences=outputs)
 
-    @add_default_section_for_function("core/model/generation/peft/adalora/bloom")
-    @torch.no_grad()
-    @autocast()
-    def generate(
-        self,
-        input_ids: torch.Tensor,
-        num_beams: Optional[int] = 5,
-        decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
-        num_return_sequences: Optional[int] = 1,
-        min_gen_seq_length: Optional[int] = 0,
-        max_gen_seq_length: Optional[int] = 48,
-        repetition_penalty: Optional[float] = 1.0,
-        no_repeat_ngram_size: Optional[int] = 0,
-        early_stopping: Optional[bool] = True,
-        length_penalty: Optional[float] = 1.0,
-        num_beam_groups: Optional[int] = 1,
-        diversity_penalty: Optional[float] = 0.0,
-        do_sample: Optional[bool] = False,
-        temperature: Optional[float] = 1.0,
-        top_k: Optional[int] = 50,
-        top_p: Optional[float] = 1.0,
-    ):
-        """
-        Generate sequences using the Bloom model.
-
-        Args:
-            input_ids (torch.Tensor): Input token IDs.
-            num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
-            num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
-            min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
-            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
-            repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
-            no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
-            early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
-            length_penalty (float, optional): Length penalty. Defaults to 1.0.
-            num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.
-            diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.
-            do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.
-            temperature (float, optional): Sampling temperature. Defaults to 1.0.
-            top_k (int, optional): Top-k sampling parameter. Defaults to 50.
-            top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.
-
-        Returns:
-            GenerationOutputs: The generation outputs.
-        """
-        outputs = super().generate(
-            input_ids,
-            num_beams=num_beams,
-            decoder_start_token_id=decoder_start_token_id,
-            decoder_end_token_id=decoder_end_token_id,
-            num_return_sequences=num_return_sequences,
-            min_gen_seq_length=min_gen_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-            repetition_penalty=repetition_penalty,
-            no_repeat_ngram_size=no_repeat_ngram_size,
-            early_stopping=early_stopping,
-            length_penalty=length_penalty,
-            num_beam_groups=num_beam_groups,
-            diversity_penalty=diversity_penalty,
-            do_sample=do_sample,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-        )
-
-        return GenerationOutputs(
-            sequences=outputs.sequences,
-            sequences_scores=outputs.sequences_scores,
+        return dict(
+            configure=config,
+            model=model,
+            datasets=dataset,
+            local_rank=local_rank,
         )
 
-
-@register_model("core/model/classification/peft/lora/bloom")
-class BloomLoraForClassification(_BloomLoraForClassification):
-    def __init__(
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def train(
         self,
         config_path: str,
-        lora_r: Optional[int] = 16,
-        lora_alpha: Optional[int] = 32,
-        lora_dropout: Optional[float] = 0.05,
-        fan_in_fan_out: Optional[bool] = True,
-        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
-        num_classes: Optional[int] = 1,
-        gradient_checkpointing: Optional[bool] = False,
+        optim: str,
+        loss_fn: str,
+        score_fn: str,
+        monitor_fns: Optional[Union[str, List[str]]] = None,
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        to_ckpt_dir: Optional[str] = "./to_ckpt",
+        train_batch_size: Optional[int] = 128,
+        dev_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        save_optimizer: Optional[bool] = False,
+        save_scheduler: Optional[bool] = False,
+        log_freq: Optional[int] = 100,
+        ckpt_freq: Optional[int] = 10000,
+        grad_acc_step: Optional[int] = 1,
+        max_grad_norm: Optional[float] = 1.0,
+        learning_rate: Optional[float] = None,
+        max_warmup_learning_rate: Optional[float] = None,
+        num_warmup_steps: Optional[int] = None,
+        epochs: Optional[int] = 5,
+        use_ema: Optional[bool] = False,
+        ema_decay: Optional[float] = 0.9999,
+        ema_tau: Optional[int] = 2000,
+        gpu_mode: Optional[bool] = False,
     ):
         """
-        Initialize the BloomLoraForClassification model.
-
-        Args:
-            config_path (str): The path to the model configuration file.
-            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
-            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
-            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
-            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
-            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
-            num_classes (int, optional): The number of classes. Defaults to 1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/classification/peft/lora/bloom")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of BloomLoraForClassification from a core configuration.
+        Train the model using deepspeed.
 
         Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            BloomLoraForClassification: The initialized BloomLoraForClassification instance.
-        """
-        config.set_default_section("core/model/classification/peft/lora/bloom")
-        pretrained_name = config.getoption("pretrained_name", "default-bloom")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
+            config_path: The path to the deepspeed configuration file.
+            optim: The optimizer used for training.
+            loss_fn: The loss function used for training.
+            score_fn: The score function used for evaluation.
+            monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to "./to_ckpt".
+            train_batch_size (optional): The batch size for training. Defaults to 128.
+            dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            save_optimizer (optional): Whether to save the optimizer state. Defaults to False.
+            save_scheduler (optional): Whether to save the scheduler state. Defaults to False.
+            log_freq (optional): The frequency of logging. Defaults to 100.
+            ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.
+            grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.
+            max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.
+            learning_rate (optional): The learning rate for the optimizer. Defaults to None.
+            max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.
+            num_warmup_steps (optional): The number of warmup steps. Defaults to None.
+            epochs (optional): The number of training epochs. Defaults to 5.
+            use_ema (optional): Whether to use exponential moving average. Defaults to False.
+            ema_decay (optional): The decay factor for exponential moving average. Defaults to 0.9999.
+            ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
+        """
+        if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:
+            os.makedirs(to_ckpt_dir, exist_ok=True)
+
+        if loss_fn is not None:
+            loss_fn = init_registered_module(loss_fn, self.config, registered_loss)
+
+        if score_fn is not None:
+            score_fn = init_registered_module(score_fn, self.config, registered_score)
+
+        if monitor_fns is not None:
+            monitor_fns = [
+                init_registered_module(monitor_fn, self.config, registered_score)
+                for monitor_fn in monitor_fns
+                if monitor_fn in registered_score
+            ]
+
+        config_file = cached_path(config_path)
+        config_dict = json.load(open(config_file, "r"))
+        config_dict["train_micro_batch_size_per_gpu"] = train_batch_size
+
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
+
+        if os.path.exists(to_ckpt_dir):
+            self.model.from_checkpoint(
+                to_ckpt_dir,
+                weight_name="pytorch_model_latest.bin",
+            )
 
-        lora_r = config.getoption("lora_r", 16)
-        lora_alpha = config.getoption("lora_alpha", 32)
-        lora_dropout = config.getoption("lora_dropout", 0.05)
-        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
-        target_modules = config.getoption("target_modules", ["query_key_value"])
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-        num_classes = config.getoption("num_classes", 1)
-
-        inst = cls(
-            config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
+        params = self.model.parameters()
+        params = filter(lambda x: x.requires_grad, params)
 
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
+        assert "optimizer" in config_dict
 
-        pretrained_lora_weight_path = config.getoption(
-            "pretrained_lora_weight_path", None
-        )
-        if pretrained_lora_weight_path is not None:
-            weight_path.append(pretrained_lora_weight_path)
+        if "params" not in config_dict["optimizer"]:
+            config_dict["optimizer"]["params"] = dict()
 
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
+        if "scheduler" in config_dict:
+            if "params" not in config_dict["scheduler"]:
+                config_dict["scheduler"]["params"] = dict()
+
+        if learning_rate is not None:
+            config_dict["optimizer"]["params"]["lr"] = learning_rate
+            if "scheduler" in config_dict:
+                config_dict["scheduler"]["params"]["warmup_max_lr"] = learning_rate
+
+        if max_warmup_learning_rate is not None and "scheduler" in config_dict:
+            config_dict["scheduler"]["params"][
+                "warmup_max_lr"
+            ] = max_warmup_learning_rate
+
+        if num_warmup_steps is not None and "scheduler" in config_dict:
+            if "params" not in config_dict["scheduler"]:
+                config_dict["scheduler"]["params"] = dict()
+            config_dict["scheduler"]["params"]["warmup_num_steps"] = num_warmup_steps
+
+        info_path = os.path.join(to_ckpt_dir, "info.json")
+        if os.path.exists(info_path):
+            info = json.load(open(os.path.join(to_ckpt_dir, "info.json")))
+        else:
+            info = dict()
+
+        global_epoch = info.get("global_epoch", 0)
+        global_step = info.get("global_step", 0)
+        self.best_score = info.get("best_score", self.best_score)
+
+        logging.info(f"the best score is {self.best_score}")
+
+        self.ema_model = None
+        if use_ema:
+            num_ema_steps = info.get("num_ema_steps", 0)
+            self.ema_model = ExponentialMovingAverage(
+                self.model,
+                decay=ema_decay,
+                tau=ema_tau,
+                num_steps=num_ema_steps,
+            )
+            if os.path.exists(from_ckpt_dir):
+                self.ema_model.from_checkpoint(
+                    from_ckpt_dir,
+                    weight_name="pytorch_ema_model.bin",
+                )
+            if os.path.exists(to_ckpt_dir):
+                self.ema_model.from_checkpoint(
+                    to_ckpt_dir,
+                    weight_name="pytorch_ema_model_latest.bin",
+                )
+
+        for n, p in self.model.named_parameters():
+            logging.debug(
+                f"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}"
             )
 
-        return inst
+        self.model, optim, _, scheduler = deepspeed.initialize(
+            model=self.model,
+            config=config_dict,
+            model_parameters=params,
+        )
+
+        global_rank = -1
+        if self.n_gpu > 1:
+            global_rank = dist.get_rank()
+
+        train_sampler = DistributedSkipSampler if self.n_gpu > 1 else RandomSkipSampler
+        dev_sampler = DistributedSampler if self.n_gpu > 1 else SequentialSampler
+
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_train = self.datasets.get("train")
+                dataset_dev = self.datasets.get("dev")
+        else:
+            dataset_train = self.datasets.get("train")
+            dataset_dev = self.datasets.get("dev")
+
+        iter_train = DataLoader(
+            dataset_train,
+            sampler=train_sampler(dataset_train)
+            if not isinstance(dataset_train, Iterable)
+            else None,
+            batch_size=train_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        iter_dev = DataLoader(
+            dataset_dev,
+            sampler=dev_sampler(dataset_dev)
+            if not isinstance(dataset_dev, Iterable)
+            else None,
+            batch_size=dev_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        log_loss = 0
+        dev_epoch = 0
+        for e in range(0, epochs):
+            torch.cuda.empty_cache()
+            if e < global_epoch:
+                continue
+
+            if hasattr(dataset_train, "set_epoch"):
+                dataset_train.set_epoch(e)
+
+            if hasattr(dataset_train, "set_skip_step"):
+                dataset_train.set_skip_step(global_step * train_batch_size)
+
+            if hasattr(iter_train.sampler, "set_epoch"):
+                iter_train.sampler.set_epoch(e)
+
+            if hasattr(iter_train.sampler, "set_skip_step"):
+                iter_train.sampler.set_skip_step(global_step * train_batch_size)
+
+            self.model.train()
+            is_update_step = True
+            for step, (inputs, targets) in enumerate(iter_train):
+                step = step + global_step
+                is_update_step = False
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                    targets = targets.cuda()
+
+                if is_torch2_available():
+                    with torch.cuda.amp.autocast(
+                        enabled=True
+                    ) as autocast, torch.backends.cuda.sdp_kernel(
+                        enable_flash=False
+                    ) as disable:
+                        outputs = self.model(**inputs.dict())
+                        if isinstance(outputs, LossOutputs):
+                            loss = outputs.loss / grad_acc_step
+                        else:
+                            loss = (
+                                loss_fn(outputs=outputs, targets=targets)
+                                / grad_acc_step
+                            )
+                else:
+                    with torch.cuda.amp.autocast(enabled=True) as autocast:
+                        outputs = self.model(**inputs.dict())
+                        if isinstance(outputs, LossOutputs):
+                            loss = outputs.loss / grad_acc_step
+                        else:
+                            loss = (
+                                loss_fn(outputs=outputs, targets=targets)
+                                / grad_acc_step
+                            )
+
+                nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)
+                self.model.backward(loss)
+
+                log_loss += loss.data * grad_acc_step
+                if (step + 1) % grad_acc_step == 0:
+                    is_update_step = True
+                    optim.step()
+                    if scheduler is not None:
+                        scheduler.step()
+                    optim.zero_grad()
+
+                    if use_ema and self.ema_model is not None:
+                        self.ema_model.step(
+                            self.model.module if self.n_gpu > 1 else self.model
+                        )
+
+                if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:
+                    logging.info(
+                        f"epoch {e} step {step}: loss -- { log_loss / log_freq }"
+                    )
+                    log_loss = 0
+
+                if (step + 1) % ckpt_freq == 0:
+                    if hasattr(dataset_dev, "set_epoch"):
+                        dataset_dev.set_epoch(dev_epoch)
+
+                    if hasattr(iter_dev.sampler, "set_epoch"):
+                        iter_dev.sampler.set_epoch(dev_epoch)
+
+                    dev_epoch += 1
+                    self.best_score = save_checkpoint(
+                        self.model.module if self.n_gpu > 1 else self.model,
+                        to_ckpt_dir,
+                        iter_dev,
+                        score_fn,
+                        monitor_fns,
+                        optim=optim if save_optimizer else None,
+                        scheduler=scheduler if save_scheduler else None,
+                        ema_model=self.ema_model if use_ema else None,
+                        best_score=self.best_score,
+                        info_path=info_path,
+                        local_rank=self.local_rank,
+                        global_epoch=e,
+                        global_step=step + 1,
+                    )
+
+            if not is_update_step:
+                optim.step()
+                if scheduler is not None:
+                    scheduler.step()
+                optim.zero_grad()
+
+                if use_ema and self.ema_model is not None:
+                    self.ema_model.step(
+                        self.model.module if self.n_gpu > 1 else self.model
+                    )
+
+            log_loss = 0
+
+            if hasattr(dataset_dev, "set_epoch"):
+                dataset_dev.set_epoch(dev_epoch)
+
+            if hasattr(iter_dev.sampler, "set_epoch"):
+                iter_dev.sampler.set_epoch(dev_epoch)
+
+            dev_epoch += 1
+
+            global_step = 0
+            self.best_score = save_checkpoint(
+                self.model.module if self.n_gpu > 1 else self.model,
+                to_ckpt_dir,
+                iter_dev,
+                score_fn,
+                monitor_fns,
+                optim=optim if save_optimizer else None,
+                scheduler=scheduler if save_scheduler else None,
+                ema_model=self.ema_model if use_ema else None,
+                best_score=self.best_score,
+                info_path=info_path,
+                local_rank=self.local_rank,
+                global_epoch=e,
+                global_step=0,
+            )
 
-    @autocast()
-    def forward(
+    @torch.no_grad()
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def eval(
         self,
-        input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
+        monitor_fns: Union[str, List[str]],
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        dev_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        gpu_mode: Optional[bool] = False,
     ):
         """
-        Perform forward pass of the BloomLoraForClassification model.
+        Evaluate the model.
 
         Args:
-            input_ids (torch.Tensor): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
-
-        Returns:
-            ClassificationOutputs: The output of the classification task.
-        """
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-        )
-        return ClassificationOutputs(outputs=outputs)
-
+            monitor_fns: The monitoring functions for evaluation.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
+        """
+        monitor_fns = [
+            init_registered_module(monitor_fn, self.config, registered_score)
+            for monitor_fn in monitor_fns
+            if monitor_fn in registered_score
+        ]
+
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
+
+        global_rank = -1
+        if self.n_gpu > 1:
+            self.model = nn.parallel.DistributedDataParallel(
+                self.model,
+                device_ids=[self.local_rank],
+                output_device=self.local_rank,
+                find_unused_parameters=False,
+                broadcast_buffers=False,
+            )
+            global_rank = dist.get_rank()
 
-@register_model("core/model/generation/peft/lora/bloom", generation_model_decorator)
-class BloomLoraForGeneration(_BloomLoraForGeneration):
-    """BloomLora model for generation tasks."""
+        dev_sampler = DistributedSampler if self.n_gpu > 1 else SequentialSampler
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_dev = self.datasets.get("dev")
+        else:
+            dataset_dev = self.datasets.get("dev")
+        iter_dev = DataLoader(
+            dataset_dev,
+            sampler=dev_sampler(dataset_dev)
+            if not isinstance(dataset_dev, Iterable)
+            else None,
+            batch_size=dev_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        results = infer(self.model.module if self.n_gpu > 1 else self.model, iter_dev)
+        if self.local_rank in [-1, 0]:
+            monitor(
+                outputs=results.outputs,
+                targets=results.targets,
+                monitor_fns=monitor_fns,
+            )
 
-    def __init__(
+    @torch.no_grad()
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def infer(
         self,
-        config_path: str,
-        lora_r: Optional[int] = 16,
-        lora_alpha: Optional[int] = 32,
-        lora_dropout: Optional[float] = 0.05,
-        fan_in_fan_out: Optional[bool] = True,
-        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
-        gradient_checkpointing: Optional[bool] = False,
+        postprocess_fn: str,
+        writer: str,
+        test_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        max_size: Optional[int] = 10000,
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        output_header: Optional[List] = None,
+        output_path: Optional[str] = "./cache/predict.txt",
+        postprocess_workers: Optional[int] = 2,
+        gpu_mode: Optional[bool] = False,
     ):
         """
-        Initialize the BloomLoraForGeneration model.
+        Perform inference using the trained model.
 
         Args:
-            config_path (str): The path to the model configuration file.
-            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
-            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
-            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
-            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
-            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/generation/peft/lora/bloom")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of BloomLoraForGeneration from a core configuration.
-
-        Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            BloomLoraForGeneration: The initialized BloomLoraForGeneration instance.
-        """
-        config.set_default_section("core/model/generation/peft/lora/bloom")
-        pretrained_name = config.getoption("pretrained_name", "default-bloom")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        lora_r = config.getoption("lora_r", 16)
-        lora_alpha = config.getoption("lora_alpha", 32)
-        lora_dropout = config.getoption("lora_dropout", 0.05)
-        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
-        target_modules = config.getoption("target_modules", ["query_key_value"])
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(
-            config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_bloom_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_lora_weight_path = config.getoption(
-            "pretrained_lora_weight_path", None
-        )
-        if pretrained_lora_weight_path is not None:
-            weight_path.append(pretrained_lora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
+            postprocess_fn: The post-processing function for inference.
+            writer: The writer for writing the results.
+            test_batch_size (optional): The batch size for inference. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            max_size (optional): The maximum size of the dataset for inference. Defaults to 10000.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            output_header (optional): The header for the output file. Defaults to None.
+            output_path (optional): The path to save the output file. Defaults to "./cache/predict.txt".
+            postprocess_workers (optional): The number of worker processes for post-processing. Defaults to 2.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
+        """
+        assert self.n_gpu <= 1
+        assert writer is not None
+
+        output_dir = os.path.dirname(output_path)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir, exist_ok=True)
+
+        if postprocess_fn is not None:
+            postprocess_fn = init_registered_process(postprocess_fn, self.config)
+
+        if writer is not None:
+            writer = init_registered_module(
+                writer,
+                self.config,
+                registered_writer,
+                output_file=output_path,
             )
 
-        return inst
+        skip_step = writer.skip_n_samples
 
-    @autocast()
-    def forward(
-        self,
-        input_ids: Optional[torch.Tensor],
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-    ):
-        """
-        Perform forward pass of the BloomLoraForGeneration model.
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
 
-        Args:
-            input_ids (torch.Tensor, optional): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+        if skip_step == 0:
+            sampler = SequentialSampler
+        else:
+            sampler = SequentialSkipSampler
+
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_test = self.datasets.get("test")
+        else:
+            dataset_test = self.datasets.get("test")
+
+        iter_test = DataLoader(
+            dataset_test,
+            sampler=sampler(dataset_test)
+            if not isinstance(dataset_test, Iterable)
+            else None,
+            batch_size=test_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        if skip_step > 0:
+            output_file = open(output_path, "a")
+        else:
+            output_file = open(output_path, "w")
+
+        if skip_step > 0 and hasattr(dataset_test, "set_skip_step"):
+            dataset_test.set_skip_step(skip_step)
+
+        if skip_step > 0 and hasattr(iter_test.sampler, "set_skip_step"):
+            iter_test.sampler.set_skip_step(skip_step)
+
+        if hasattr(dataset_test, "dataset"):
+            data_info = dataset_test.dataset
+            data_info = DatasetFeature(data_info)
+            iter_data = DataLoader(
+                deepcopy(data_info),
+                sampler=sampler(data_info)
+                if not isinstance(dataset_test, Iterable)
+                else None,
+                batch_size=test_batch_size,
+                shuffle=False,
+                pin_memory=pin_memory,
+                num_workers=num_workers,
+                collate_fn=None,
+            )
+        else:
+            iter_data = None
 
-        Returns:
-            GenerationOutputs: The output of the generation task.
-        """
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-        )
-        return GenerationOutputs(sequences=outputs)
+        if skip_step > 0 and hasattr(iter_data.sampler, "set_skip_step"):
+            iter_data.sampler.set_skip_step(skip_step)
 
-    @add_default_section_for_function("core/model/generation/peft/lora/bloom")
-    @torch.no_grad()
-    @autocast()
-    def generate(
-        self,
-        input_ids: torch.Tensor,
-        num_beams: Optional[int] = 5,
-        decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
-        num_return_sequences: Optional[int] = 1,
-        min_gen_seq_length: Optional[int] = 0,
-        max_gen_seq_length: Optional[int] = 48,
-        repetition_penalty: Optional[float] = 1.0,
-        no_repeat_ngram_size: Optional[int] = 0,
-        early_stopping: Optional[bool] = True,
-        length_penalty: Optional[float] = 1.0,
-        num_beam_groups: Optional[int] = 1,
-        diversity_penalty: Optional[float] = 0.0,
-        do_sample: Optional[bool] = False,
-        temperature: Optional[float] = 1.0,
-        top_k: Optional[int] = 50,
-        top_p: Optional[float] = 1.0,
-    ):
-        """
-        Generate sequences using the Bloom model.
+        self.model.eval()
+        start = time.time()
 
-        Args:
-            input_ids (torch.Tensor): Input token IDs.
-            num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
-            num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
-            min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
-            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
-            repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
-            no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
-            early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
-            length_penalty (float, optional): Length penalty. Defaults to 1.0.
-            num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.
-            diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.
-            do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.
-            temperature (float, optional): Sampling temperature. Defaults to 1.0.
-            top_k (int, optional): Top-k sampling parameter. Defaults to 50.
-            top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.
+        data_queue = Queue(maxsize=max_size)
+        msg_queue = Queue(maxsize=max_size)
+        postprocess_list = []
+        for _ in range(postprocess_workers):
+            p = PostProcess(
+                postprocess_fn,
+                data_queue,
+                msg_queue,
+            )
+            postprocess_list.append(p)
+            p.start()
 
-        Returns:
-            GenerationOutputs: The generation outputs.
-        """
-        outputs = super().generate(
-            input_ids,
-            num_beams=num_beams,
-            decoder_start_token_id=decoder_start_token_id,
-            decoder_end_token_id=decoder_end_token_id,
-            num_return_sequences=num_return_sequences,
-            min_gen_seq_length=min_gen_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-            repetition_penalty=repetition_penalty,
-            no_repeat_ngram_size=no_repeat_ngram_size,
-            early_stopping=early_stopping,
-            length_penalty=length_penalty,
-            num_beam_groups=num_beam_groups,
-            diversity_penalty=diversity_penalty,
-            do_sample=do_sample,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-        )
+        io_process = IOProcess(msg_queue, writer=writer)
+        io_process.start()
 
-        return GenerationOutputs(
-            sequences=outputs.sequences,
-            sequences_scores=outputs.sequences_scores,
+        if iter_data is None:
+            for step, (inputs, _) in enumerate(iter_test):
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                outputs = self.model(**inputs.dict())
+                outputs = outputs.cpu()
+                data_queue.put((step, outputs))
+        else:
+            for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                outputs = self.model(**inputs.dict())
+                outputs = outputs.cpu()
+                if output_header is not None:
+                    _infos = {k: _infos[k] for k in output_header if k in _infos}
+                    outputs.from_pandas(pd.DataFrame(_infos))
+                data_queue.put((step, outputs))
+
+        data_queue.put((-1, GENERATE_FINISHED))
+        for p in postprocess_list:
+            p.join()
+
+        msg_queue.put((-1, GENERATE_FINISHED))
+        io_process.join()
+
+        end = time.time()
+        ms = (end - start) * 1000
+        logging.info(
+            "{:.2f} ms, {:.1f} sample/s".format(
+                ms,
+                ((len(dataset_test) - skip_step) / ms * 1000),
+            )
         )
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_llama.py` & `unitorch-0.0.0.7/src/unitorch/models/blip/modeling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,688 +1,717 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import os
+import json
+import math
+import random
 import logging
+import transformers
 import torch
+import torch.nn as nn
+import torch.nn.functional as F
+import torch.distributed as dist
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from torch.cuda.amp import autocast
-from transformers.utils import is_remote_url
-from unitorch.utils import pop_value, nested_dict_value
-from unitorch.models.peft import (
-    LlamaAdaLoraForClassification as _LlamaAdaLoraForClassification,
-    LlamaAdaLoraForGeneration as _LlamaAdaLoraForGeneration,
-    LlamaLoraForClassification as _LlamaLoraForClassification,
-    LlamaLoraForGeneration as _LlamaLoraForGeneration,
-)
-from unitorch.cli import (
-    cached_path,
-    add_default_section_for_init,
-    add_default_section_for_function,
-    register_model,
+
+from transformers.models.blip.modeling_blip import (
+    BlipConfig,
+    BlipTextModel,
+    BlipVisionModel,
+    BlipForConditionalGeneration,
 )
-from unitorch.cli.models import generation_model_decorator
-from unitorch.cli.models import ClassificationOutputs, GenerationOutputs, LossOutputs
-from unitorch.cli.models.llama import pretrained_llama_infos
+from transformers.models.blip.modeling_blip_text import apply_chunking_to_forward
+from unitorch.utils.decorators import replace
+from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models.clip.modeling import AllGather
+
 
+def _contrastive_loss(logits: torch.Tensor) -> torch.Tensor:
+    return nn.functional.cross_entropy(
+        logits, torch.arange(len(logits), device=logits.device)
+    )
 
-@register_model("core/model/classification/peft/adalora/llama")
-class LlamaAdaLoraForClassification(_LlamaAdaLoraForClassification):
-    """LlamaAdaLora model for classification tasks."""
 
+def _blip_loss(similarity: torch.Tensor) -> torch.Tensor:
+    caption_loss = _contrastive_loss(similarity)
+    image_loss = _contrastive_loss(similarity.T)
+    return (caption_loss + image_loss) / 2.0
+
+
+@replace(transformers.models.blip.modeling_blip_text.BlipTextSelfAttention)
+class BlipTextSelfAttentionV2(
+    transformers.models.blip.modeling_blip_text.BlipTextSelfAttention
+):
+    def __init__(
+        self,
+        config,
+        is_cross_attention=False,
+    ):
+        super().__init__(
+            config=config,
+            is_cross_attention=is_cross_attention,
+        )
+
+    def forward(
+        self,
+        hidden_states,
+        attention_mask: Optional[torch.Tensor] = None,
+        head_mask=None,
+        encoder_hidden_states=None,
+        encoder_attention_mask: Optional[torch.Tensor] = None,
+        past_key_value=None,
+        output_attentions=False,
+    ):
+        mixed_query_layer = self.query(hidden_states)
+
+        # If this is instantiated as a cross-attention module, the keys
+        # and values come from an encoder; the attention mask needs to be
+        # such that the encoder's padding tokens are not attended to.
+        is_cross_attention = encoder_hidden_states is not None
+        bsz, tgt_len, embed_dim = hidden_states.size()
+        kv_bsz = bsz
+
+        if is_cross_attention and past_key_value is not None:
+            # reuse k,v, cross_attentions
+            key_layer = past_key_value[0]
+            value_layer = past_key_value[1]
+            kv_bsz = key_layer.size(0)
+            attention_mask = encoder_attention_mask
+        elif is_cross_attention:
+            key_layer = self.transpose_for_scores(self.key(encoder_hidden_states))
+            value_layer = self.transpose_for_scores(self.value(encoder_hidden_states))
+            attention_mask = encoder_attention_mask
+        elif past_key_value is not None:
+            key_layer = self.transpose_for_scores(self.key(hidden_states))
+            value_layer = self.transpose_for_scores(self.value(hidden_states))
+            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+        else:
+            key_layer = self.transpose_for_scores(self.key(hidden_states))
+            value_layer = self.transpose_for_scores(self.value(hidden_states))
+
+        query_layer = self.transpose_for_scores(mixed_query_layer)
+
+        past_key_value = (key_layer, value_layer)
+
+        # Take the dot product between "query" and "key" to get the raw attention scores.
+        attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
+        if is_cross_attention and kv_bsz != bsz:
+            attention_scores = torch.einsum(
+                "bxhtd,bhsd->bxhts",
+                query_layer.view(kv_bsz, -1, self.num_heads, *query_layer.size()[1:]),
+                key_layer.view(kv_bsz, self.num_heads, *key_layer.size()[1:]),
+            )
+            attention_scores = attention_scores.reshape(
+                -1, *attention_scores.size()[-2:]
+            )
+        else:
+            attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
+
+        if (
+            self.position_embedding_type == "relative_key"
+            or self.position_embedding_type == "relative_key_query"
+        ):
+            seq_length = hidden_states.size()[1]
+            position_ids_l = torch.arange(
+                seq_length, dtype=torch.long, device=hidden_states.device
+            ).view(-1, 1)
+            position_ids_r = torch.arange(
+                seq_length, dtype=torch.long, device=hidden_states.device
+            ).view(1, -1)
+            distance = position_ids_l - position_ids_r
+            positional_embedding = self.distance_embedding(
+                distance + self.max_position_embeddings - 1
+            )
+            positional_embedding = positional_embedding.to(
+                dtype=query_layer.dtype
+            )  # fp16 compatibility
+
+            if self.position_embedding_type == "relative_key":
+                relative_position_scores = torch.einsum(
+                    "bhld,lrd->bhlr", query_layer, positional_embedding
+                )
+                attention_scores = attention_scores + relative_position_scores
+            elif self.position_embedding_type == "relative_key_query":
+                relative_position_scores_query = torch.einsum(
+                    "bhld,lrd->bhlr", query_layer, positional_embedding
+                )
+                relative_position_scores_key = torch.einsum(
+                    "bhrd,lrd->bhlr", key_layer, positional_embedding
+                )
+                if kv_bsz != bsz:
+                    shape = relative_position_scores_query.size()
+                    relative_position_scores_key = (
+                        relative_position_scores_key.unsqueeze(1)
+                        .expand(kv_bsz, bsz // kv_bsz, *shape[1:])
+                        .contiguous()
+                        .view(bsz, *shape[1:])
+                    )
+                attention_scores = (
+                    attention_scores
+                    + relative_position_scores_query
+                    + relative_position_scores_key
+                )
+
+        attention_scores = attention_scores / math.sqrt(self.attention_head_size)
+        if attention_mask is not None:
+            # Apply the attention mask is (precomputed for all layers in BlipTextModel forward() function)
+            attention_scores = attention_scores + attention_mask.to(
+                attention_scores.device
+            )
+
+        # Normalize the attention scores to probabilities.
+        attention_probs = nn.Softmax(dim=-1)(attention_scores)
+
+        # This is actually dropping out entire tokens to attend to, which might
+        # seem a bit unusual, but is taken from the original Transformer paper.
+        attention_probs_dropped = self.dropout(attention_probs)
+
+        # Mask heads if we want to
+        if head_mask is not None:
+            attention_probs_dropped = attention_probs_dropped * head_mask
+
+        if is_cross_attention and kv_bsz != bsz:
+            context_layer = torch.einsum(
+                "bxhtd,bhsd->bxhts",
+                attention_probs_dropped.view(
+                    kv_bsz, -1, self.num_heads, *query_layer.size()[1:]
+                ),
+                value_layer.view(kv_bsz, self.num_heads, *key_layer.size()[1:]),
+            )
+            context_layer = context_layer.reshape(-1, *context_layer.size()[-2:])
+        else:
+            context_layer = torch.matmul(attention_probs_dropped, value_layer)
+
+        context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
+        new_context_layer_shape = context_layer.size()[:-2] + (self.all_head_size,)
+        context_layer = context_layer.view(*new_context_layer_shape)
+
+        outputs = (
+            (context_layer, attention_probs) if output_attentions else (context_layer,)
+        )
+
+        outputs = outputs + (past_key_value,)
+        return outputs
+
+
+@replace(transformers.models.blip.modeling_blip_text.BlipTextLayer)
+class BlipTextLayerV2(transformers.models.blip.modeling_blip_text.BlipTextLayer):
+    def __init__(self, config, layer_num):
+        super().__init__(
+            config=config,
+            layer_num=layer_num,
+        )
+
+    def forward(
+        self,
+        hidden_states,
+        attention_mask: Optional[torch.Tensor] = None,
+        head_mask=None,
+        encoder_hidden_states=None,
+        encoder_attention_mask: Optional[torch.Tensor] = None,
+        past_key_value=None,
+        output_attentions=False,
+    ):
+        # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
+        self_attn_past_key_value = (
+            past_key_value[:2] if past_key_value is not None else None
+        )
+        self_attention_outputs = self.attention(
+            hidden_states,
+            attention_mask,
+            head_mask,
+            output_attentions=output_attentions,
+            past_key_value=self_attn_past_key_value,
+        )
+        attention_output = self_attention_outputs[0]
+
+        outputs = self_attention_outputs[1:-1]
+        present_key_value = self_attention_outputs[-1]
+
+        if encoder_hidden_states is not None:
+            cross_attn_past_key_value = (
+                past_key_value[2:] if past_key_value is not None else None
+            )
+            cross_attention_outputs = self.crossattention(
+                attention_output,
+                attention_mask,
+                head_mask,
+                encoder_hidden_states,
+                encoder_attention_mask,
+                output_attentions=output_attentions,
+                past_key_value=cross_attn_past_key_value,
+            )
+            attention_output = cross_attention_outputs[0]
+            outputs = (
+                outputs + cross_attention_outputs[1:-1]
+            )  # add cross attentions if we output attention weights
+            present_key_value = present_key_value + cross_attention_outputs[-1]
+
+        layer_output = apply_chunking_to_forward(
+            self.feed_forward_chunk,
+            self.chunk_size_feed_forward,
+            self.seq_len_dim,
+            attention_output,
+        )
+        outputs = (layer_output,) + outputs
+
+        outputs = outputs + (present_key_value,)
+
+        return outputs
+
+
+class BlipForPretrain(GenericModel):
     def __init__(
         self,
         config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
-        num_classes: Optional[int] = 1,
+        projection_dim: Optional[int] = 512,
+        freeze_base_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
+        use_all_gather: Optional[bool] = True,
     ):
         """
-        Initialize the LlamaAdaLoraForClassification model.
+        Initializes the BlipForPretrain model.
 
         Args:
-            config_path (str): The path to the model configuration file.
-            target_r (int, optional): The target rank. Defaults to 8.
-            init_r (int, optional): The initial rank. Defaults to 12.
-            tinit (int, optional): The initial temperature. Defaults to 0.
-            tfinal (int, optional): The final temperature. Defaults to 0.
-            deltaT (int, optional): The temperature change rate. Defaults to 1.
-            beta1 (float, optional): The value of beta1 for optimizer. Defaults to 0.85.
-            beta2 (float, optional): The value of beta2 for optimizer. Defaults to 0.85.
-            orth_reg_weight (float, optional): The weight of the orthogonality regularization. Defaults to 0.5.
-            total_step (int, optional): The total number of training steps. Defaults to None.
-            rank_pattern (dict, optional): The rank pattern. Defaults to None.
-            num_classes (int, optional): The number of classes. Defaults to 1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+            use_all_gather (Optional[bool], optional): Whether to use all_gather operation for distributed training. Defaults to True.
         """
-        super().__init__(
-            config_path=config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/classification/peft/adalora/llama")
-    def from_core_configure(cls, config, **kwargs):
+        super().__init__()
+
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        vision_config = config.vision_config
+        text_config.gradient_checkpointing = gradient_checkpointing
+        vision_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
+        self.use_all_gather = use_all_gather
+
+        self.text_embed_dim = text_config.hidden_size
+        self.vision_embed_dim = vision_config.hidden_size
+
+        self.text_model = BlipTextModel(text_config)
+        self.vision_model = BlipVisionModel(vision_config)
+
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.logit_scale = nn.Parameter(torch.ones([]) * config.logit_scale_init_value)
+
+        self.init_weights()
+
+        if freeze_base_model:
+            for p in self.text_model.parameters():
+                p.requires_grad = False
+
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def _all_gather(self, input):
         """
-        Create an instance of LlamaAdaLoraForClassification from a core configuration.
+        Applies all_gather operation for distributed training.
 
         Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
+            input: Input tensor to gather.
 
         Returns:
-            LlamaAdaLoraForClassification: The initialized LlamaAdaLoraForClassification instance.
+            output: Gathered tensor across all workers.
         """
-        config.set_default_section("core/model/classification/peft/adalora/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        target_r = config.getoption("target_r", 8)
-        init_r = config.getoption("init_r", 12)
-        tinit = config.getoption("tinit", 0)
-        tfinal = config.getoption("tfinal", 0)
-        deltaT = config.getoption("deltaT", 1)
-        beta1 = config.getoption("beta1", 0.85)
-        beta2 = config.getoption("beta2", 0.85)
-        orth_reg_weight = config.getoption("orth_reg_weight", 0.5)
-        total_step = config.getoption("total_step", None)
-        rank_pattern = config.getoption("rank_pattern", None)
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-        num_classes = config.getoption("num_classes", 1)
-
-        inst = cls(
-            config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_adalora_weight_path = config.getoption(
-            "pretrained_adalora_weight_path", None
-        )
-        if pretrained_adalora_weight_path is not None:
-            weight_path.append(pretrained_adalora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
-
-        return inst
+        output = AllGather.apply(input)
+        output = output.view(-1, *(output.shape[2:]))
+        return output
 
-    @autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
+        pixel_values: torch.Tensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
     ):
         """
-        Perform forward pass of the LlamaAdaLoraForClassification model.
+        Forward pass of the BlipForPretrain model.
 
         Args:
-            input_ids (torch.Tensor): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+            input_ids (torch.Tensor): Input token IDs.
+            pixel_values (torch.Tensor): Pixel values of the images.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
 
         Returns:
-            ClassificationOutputs: The output of the classification task.
+            (torch.Tensor):Output loss for the pretraining task.
         """
-        outputs = super().forward(
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
+        )
+
+        text_outputs = self.text_model(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
-        return ClassificationOutputs(outputs=outputs)
 
+        image_embeds = vision_outputs[1]
+        image_embeds = self.visual_projection(image_embeds)
 
-@register_model("core/model/generation/peft/adalora/llama", generation_model_decorator)
-class LlamaAdaLoraForGeneration(_LlamaAdaLoraForGeneration):
-    """LlamaAdaLora model for generation tasks."""
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
 
+        # normalized features
+        image_embeds = image_embeds / image_embeds.norm(dim=-1, keepdim=True)
+        text_embeds = text_embeds / text_embeds.norm(dim=-1, keepdim=True)
+
+        logit_scale = self.logit_scale.exp()
+        if self.use_all_gather and dist.is_initialized():
+            text_embeds = self._all_gather(text_embeds)
+            image_embeds = self._all_gather(image_embeds)
+        logits_per_text = torch.matmul(text_embeds, image_embeds.t()) * logit_scale
+        return _blip_loss(logits_per_text)
+
+
+class BlipForClassification(nn.Module):
     def __init__(
         self,
         config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
+        projection_dim: Optional[int] = 512,
+        num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the LlamaAdaLoraForGeneration model.
+        Initializes the BlipForClassification model.
 
         Args:
-            config_path (str): The path to the model configuration file.
-            target_r (int, optional): The target rank. Defaults to 8.
-            init_r (int, optional): The initial rank. Defaults to 12.
-            tinit (int, optional): The initial temperature. Defaults to 0.
-            tfinal (int, optional): The final temperature. Defaults to 0.
-            deltaT (int, optional): The temperature change rate. Defaults to 1.
-            beta1 (float, optional): The value of beta1 for optimizer. Defaults to 0.85.
-            beta2 (float, optional): The value of beta2 for optimizer. Defaults to 0.85.
-            orth_reg_weight (float, optional): The weight of the orthogonality regularization. Defaults to 0.5.
-            total_step (int, optional): The total number of training steps. Defaults to None.
-            rank_pattern (dict, optional): The rank pattern. Defaults to None.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
-        """
-        super().__init__(
-            config_path=config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/model/generation/peft/adalora/llama")
-    def from_core_configure(cls, config, **kwargs):
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
         """
-        Create an instance of LlamaAdaLoraForGeneration from a core configuration.
+        super().__init__()
 
-        Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        vision_config = config.vision_config
 
-        Returns:
-            LlamaAdaLoraForGeneration: The initialized LlamaAdaLoraForGeneration instance.
-        """
-        config.set_default_section("core/model/generation/peft/adalora/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        target_r = config.getoption("target_r", 8)
-        init_r = config.getoption("init_r", 12)
-        tinit = config.getoption("tinit", 0)
-        tfinal = config.getoption("tfinal", 0)
-        deltaT = config.getoption("deltaT", 1)
-        beta1 = config.getoption("beta1", 0.85)
-        beta2 = config.getoption("beta2", 0.85)
-        orth_reg_weight = config.getoption("orth_reg_weight", 0.5)
-        total_step = config.getoption("total_step", None)
-        rank_pattern = config.getoption("rank_pattern", None)
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(
-            config_path,
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_adalora_weight_path = config.getoption(
-            "pretrained_adalora_weight_path", None
-        )
-        if pretrained_adalora_weight_path is not None:
-            weight_path.append(pretrained_adalora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
+        # Set gradient checkpointing option
+        text_config.gradient_checkpointing = gradient_checkpointing
+        vision_config.gradient_checkpointing = gradient_checkpointing
 
-        return inst
+        self.projection_dim = projection_dim
 
-    @autocast()
-    def forward(
-        self,
-        input_ids: Optional[torch.Tensor],
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-    ):
-        """
-        Perform forward pass of the LlamaAdaLoraForGeneration model.
+        self.text_embed_dim = text_config.hidden_size
+        self.vision_embed_dim = vision_config.hidden_size
 
-        Args:
-            input_ids (torch.Tensor, optional): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+        # Initialize the text and vision models
+        self.text_model = BlipTextModel(text_config)
+        self.vision_model = BlipVisionModel(vision_config)
 
-        Returns:
-            GenerationOutputs: The output of the generation task.
-        """
-
-        outputs = super().forward(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
+        # Projection layers for text and vision embeddings
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
         )
-        return GenerationOutputs(sequences=outputs)
 
-    @add_default_section_for_function("core/model/generation/peft/adalora/llama")
-    @torch.no_grad()
-    @autocast()
-    def generate(
+        # Classifier layer
+        self.classifier = nn.Linear(self.projection_dim * 2, num_classes)
+
+        # Initialize the weights of the model
+        self.init_weights()
+
+        if freeze_base_model:
+            # Freeze the parameters of the base models if specified
+            for p in self.text_model.parameters():
+                p.requires_grad = False
+
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        # Set gradient checkpointing option for encoders
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def forward(
         self,
         input_ids: torch.Tensor,
-        num_beams: Optional[int] = 5,
-        decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
-        num_return_sequences: Optional[int] = 1,
-        min_gen_seq_length: Optional[int] = 0,
-        max_gen_seq_length: Optional[int] = 48,
-        repetition_penalty: Optional[float] = 1.0,
-        no_repeat_ngram_size: Optional[int] = 0,
-        early_stopping: Optional[bool] = True,
-        length_penalty: Optional[float] = 1.0,
-        num_beam_groups: Optional[int] = 1,
-        diversity_penalty: Optional[float] = 0.0,
-        do_sample: Optional[bool] = False,
-        temperature: Optional[float] = 1.0,
-        top_k: Optional[int] = 50,
-        top_p: Optional[float] = 1.0,
+        pixel_values: torch.Tensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
     ):
         """
-        Generate sequences using the Llama model.
+        Forward pass of the BlipForClassification model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
-            num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
-            num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
-            min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
-            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
-            repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
-            no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
-            early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
-            length_penalty (float, optional): Length penalty. Defaults to 1.0.
-            num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.
-            diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.
-            do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.
-            temperature (float, optional): Sampling temperature. Defaults to 1.0.
-            top_k (int, optional): Top-k sampling parameter. Defaults to 50.
-            top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.
+            pixel_values (torch.Tensor): Pixel values of the images.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
 
         Returns:
-            GenerationOutputs: The generation outputs.
+            (torch.Tensor):Output logits for classification.
         """
-        outputs = super().generate(
-            input_ids,
-            num_beams=num_beams,
-            decoder_start_token_id=decoder_start_token_id,
-            decoder_end_token_id=decoder_end_token_id,
-            num_return_sequences=num_return_sequences,
-            min_gen_seq_length=min_gen_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-            repetition_penalty=repetition_penalty,
-            no_repeat_ngram_size=no_repeat_ngram_size,
-            early_stopping=early_stopping,
-            length_penalty=length_penalty,
-            num_beam_groups=num_beam_groups,
-            diversity_penalty=diversity_penalty,
-            do_sample=do_sample,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
+        # Process the vision modality
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
         )
 
-        return GenerationOutputs(
-            sequences=outputs.sequences,
-            sequences_scores=outputs.sequences_scores,
+        # Process the text modality
+        text_outputs = self.text_model(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
         )
 
+        # Project vision embeddings to the specified dimensionality
+        image_embeds = vision_outputs[1]
+        image_embeds = self.visual_projection(image_embeds)
 
-@register_model("core/model/classification/peft/lora/llama")
-class LlamaLoraForClassification(_LlamaLoraForClassification):
-    """LlamaLora model for classification tasks."""
+        # Project text embeddings to the specified dimensionality
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
 
+        # Concatenate and classify the projected embeddings
+        return self.classifier(F.relu(torch.cat([image_embeds, text_embeds], axis=1)))
+
+
+class BlipForTextClassification(GenericModel):
     def __init__(
         self,
         config_path: str,
-        lora_r: Optional[int] = 16,
-        lora_alpha: Optional[int] = 32,
-        lora_dropout: Optional[float] = 0.05,
-        fan_in_fan_out: Optional[bool] = True,
-        target_modules: Optional[Union[List[str], str]] = ["q_proj", "v_proj"],
+        projection_dim: Optional[int] = 512,
         num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the LlamaLoraForClassification model.
+        Initializes the BlipForTextClassification model.
 
         Args:
-            config_path (str): The path to the model configuration file.
-            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
-            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
-            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
-            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
-            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
-            num_classes (int, optional): The number of classes. Defaults to 1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
         """
-        super().__init__(
-            config_path=config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
+        super().__init__()
+
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        text_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
+        self.text_embed_dim = text_config.hidden_size
+
+        # Initialize the BLIP text model
+        self.text_model = BlipTextModel(text_config)
+
+        # Project text embeddings to the desired dimension
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
         )
 
-    @classmethod
-    @add_default_section_for_init("core/model/classification/peft/lora/llama")
-    def from_core_configure(cls, config, **kwargs):
-        """
-        Create an instance of LlamaLoraForClassification from a core configuration.
+        # Classifier layer for classification task
+        self.classifier = nn.Linear(self.projection_dim, num_classes)
 
-        Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
+        # Initialize the model weights
+        self.init_weights()
 
-        Returns:
-            LlamaLoraForClassification: The initialized LlamaLoraForClassification instance.
-        """
-        config.set_default_section("core/model/classification/peft/lora/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        lora_r = config.getoption("lora_r", 16)
-        lora_alpha = config.getoption("lora_alpha", 32)
-        lora_dropout = config.getoption("lora_dropout", 0.05)
-        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
-        target_modules = config.getoption("target_modules", ["q_proj", "v_proj"])
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-        num_classes = config.getoption("num_classes", 1)
-
-        inst = cls(
-            config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            num_classes=num_classes,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_lora_weight_path = config.getoption(
-            "pretrained_lora_weight_path", None
-        )
-        if pretrained_lora_weight_path is not None:
-            weight_path.append(pretrained_lora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
+        # Freeze the base model if specified
+        if freeze_base_model:
+            for p in self.text_model.parameters():
+                p.requires_grad = False
 
-        return inst
+        # Set gradient checkpointing for the encoder
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
 
-    @autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
     ):
         """
-        Perform forward pass of the LlamaLoraForClassification model.
+        Forward pass of the BlipForTextClassification model.
 
         Args:
-            input_ids (torch.Tensor): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+            input_ids (torch.Tensor): Input token IDs.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
 
         Returns:
-            ClassificationOutputs: The output of the classification task.
+            (torch.Tensor):Output logits for classification.
         """
-        outputs = super().forward(
+        # Pass the input through the BLIP text model
+        text_outputs = self.text_model(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )
-        return ClassificationOutputs(outputs=outputs)
 
+        # Extract text embeddings and project to desired dimension
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
 
-@register_model("core/model/generation/peft/lora/llama", generation_model_decorator)
-class LlamaLoraForGeneration(_LlamaLoraForGeneration):
-    """LlamaLora model for generation tasks."""
+        # Apply ReLU activation and pass through the classifier layer
+        return self.classifier(nn.functional.relu(text_embeds))
 
+
+class BlipForImageClassification(GenericModel):
     def __init__(
         self,
         config_path: str,
-        lora_r: Optional[int] = 16,
-        lora_alpha: Optional[int] = 32,
-        lora_dropout: Optional[float] = 0.05,
-        fan_in_fan_out: Optional[bool] = True,
-        target_modules: Optional[Union[List[str], str]] = ["q_proj", "v_proj"],
+        projection_dim: Optional[int] = 512,
+        num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initialize the LlamaLoraForGeneration model.
+        Initializes the BlipForImageClassification model.
 
         Args:
-            config_path (str): The path to the model configuration file.
-            lora_r (int, optional): The number of Lora ranks. Defaults to 16.
-            lora_alpha (int, optional): The Lora alpha value. Defaults to 32.
-            lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.
-            fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.
-            target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to ["q_proj", "v_proj"].
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
         """
-        super().__init__(
-            config_path=config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            gradient_checkpointing=gradient_checkpointing,
+        super().__init__()
+
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        vision_config = config.vision_config
+        vision_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
+        self.vision_embed_dim = vision_config.hidden_size
+
+        self.vision_model = BlipVisionModel(vision_config)
+
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
         )
 
-    @classmethod
-    @add_default_section_for_init("core/model/generation/peft/lora/llama")
-    def from_core_configure(cls, config, **kwargs):
+        self.classifier = nn.Linear(self.projection_dim, num_classes)
+
+        self.init_weights()
+
+        if freeze_base_model:
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def forward(
+        self,
+        pixel_values: torch.Tensor,
+    ):
         """
-        Create an instance of LlamaLoraForGeneration from a core configuration.
+        Forward pass of the BlipForImageClassification model.
 
         Args:
-            config: The core configuration.
-            **kwargs: Additional keyword arguments.
+            pixel_values (torch.Tensor): Input pixel values.
 
         Returns:
-            LlamaLoraForGeneration: The initialized LlamaLoraForGeneration instance.
+            (torch.Tensor):Output logits for classification.
         """
-        config.set_default_section("core/model/generation/peft/lora/llama")
-        pretrained_name = config.getoption("pretrained_name", "default-llama")
-        config_path = config.getoption("config_path", None)
-        config_path = pop_value(
-            config_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "config"),
-        )
-        config_path = cached_path(config_path)
-
-        lora_r = config.getoption("lora_r", 16)
-        lora_alpha = config.getoption("lora_alpha", 32)
-        lora_dropout = config.getoption("lora_dropout", 0.05)
-        fan_in_fan_out = config.getoption("fan_in_fan_out", True)
-        target_modules = config.getoption("target_modules", ["q_proj", "v_proj"])
-
-        gradient_checkpointing = config.getoption("gradient_checkpointing", False)
-
-        inst = cls(
-            config_path,
-            lora_r=lora_r,
-            lora_alpha=lora_alpha,
-            lora_dropout=lora_dropout,
-            fan_in_fan_out=fan_in_fan_out,
-            target_modules=target_modules,
-            gradient_checkpointing=gradient_checkpointing,
-        )
-
-        weight_path = []
-        pretrained_weight_path = config.getoption("pretrained_weight_path", None)
-        pretrained_weight_path = pop_value(
-            pretrained_weight_path,
-            nested_dict_value(pretrained_llama_infos, pretrained_name, "weight"),
-            check_none=False,
-        )
-        if pretrained_weight_path is not None:
-            if isinstance(pretrained_weight_path, str):
-                weight_path.append(pretrained_weight_path)
-            elif isinstance(pretrained_weight_path, list):
-                weight_path.extend(pretrained_weight_path)
-
-        pretrained_lora_weight_path = config.getoption(
-            "pretrained_lora_weight_path", None
-        )
-        if pretrained_lora_weight_path is not None:
-            weight_path.append(pretrained_lora_weight_path)
-
-        if len(weight_path) > 0:
-            inst.from_pretrained(
-                weight_path=weight_path,
-            )
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
+        )
+
+        image_embeds = vision_outputs[1]
+
+        image_embeds = self.visual_projection(image_embeds)
+
+        image_embeds = F.relu(image_embeds)
+
+        return self.classifier(image_embeds)
+
+
+class BlipForImageCaption(GenericModel):
+    prefix_keys_in_state_dict = {"^(?!model\.).*": "model."}
+
+    def __init__(
+        self,
+        config_path: str,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
+        """
+        Initializes the BlipForImageCaption model.
 
-        return inst
+        Args:
+            config_path (str): Path to the configuration file.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+        self.config = BlipConfig.from_json_file(config_path)
+        self.config.vision_config.gradient_checkpointing = gradient_checkpointing
+        self.config.text_config.gradient_checkpointing = gradient_checkpointing
+        self.model = BlipForConditionalGeneration(self.config)
+        self.init_weights()
 
-    @autocast()
     def forward(
         self,
-        input_ids: Optional[torch.Tensor],
+        pixel_values: torch.Tensor,
+        input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
     ):
         """
-        Perform forward pass of the LlamaLoraForGeneration model.
+        Forward pass of the BlipForImageCaption model.
 
         Args:
-            input_ids (torch.Tensor, optional): The input IDs.
-            attention_mask (torch.Tensor, optional): The attention mask.
-            position_ids (torch.Tensor, optional): The position IDs.
+            pixel_values (torch.Tensor): Input pixel values.
+            input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.
+            attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.
 
         Returns:
-            GenerationOutputs: The output of the generation task.
+            (torch.Tensor):Logits for caption generation.
         """
-        outputs = super().forward(
+        outputs = self.model(
+            pixel_values=pixel_values,
             input_ids=input_ids,
             attention_mask=attention_mask,
-            position_ids=position_ids,
+            return_dict=True,
         )
-        return GenerationOutputs(sequences=outputs)
+        logits = outputs.decoder_logits
+        return logits
 
-    @add_default_section_for_function("core/model/generation/peft/lora/llama")
     @torch.no_grad()
-    @autocast()
     def generate(
         self,
-        input_ids: torch.Tensor,
+        pixel_values: torch.Tensor,
+        input_ids: Optional[torch.Tensor] = None,
+        attention_mask: Optional[torch.Tensor] = None,
         num_beams: Optional[int] = 5,
-        decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
+        decoder_start_token_id: Optional[int] = 101,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 102,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -690,55 +719,71 @@
         diversity_penalty: Optional[float] = 0.0,
         do_sample: Optional[bool] = False,
         temperature: Optional[float] = 1.0,
         top_k: Optional[int] = 50,
         top_p: Optional[float] = 1.0,
     ):
         """
-        Generate sequences using the Llama model.
+        Generates captions for the given input images.
 
         Args:
-            input_ids (torch.Tensor): Input token IDs.
-            num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
-            num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
-            min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
-            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
-            repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
-            no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
-            early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
-            length_penalty (float, optional): Length penalty. Defaults to 1.0.
-            num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.
-            diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.
-            do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.
-            temperature (float, optional): Sampling temperature. Defaults to 1.0.
-            top_k (int, optional): Top-k sampling parameter. Defaults to 50.
-            top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.
+            pixel_values (torch.Tensor): Input pixel values.
+            input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.
+            attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.
+            num_beams (Optional[int], optional): Number of beams for beam search. Defaults to 5.
+            decoder_start_token_id (Optional[int], optional): ID of the start token for decoding. Defaults to 30522.
+            decoder_end_token_id (int or List[int], optional): ID of the end token for decoding. Defaults to 2.
+            num_return_sequences (Optional[int], optional): Number of caption sequences to return. Defaults to 1.
+            min_gen_seq_length (Optional[int], optional): Minimum length of generated sequences. Defaults to 0.
+            max_gen_seq_length (Optional[int], optional): Maximum length of generated sequences. Defaults to 48.
+            repetition_penalty (Optional[float], optional): Repetition penalty value. Defaults to 1.0.
+            no_repeat_ngram_size (Optional[int], optional): Size of n-grams to avoid repetition. Defaults to 0.
+            early_stopping (Optional[bool], optional): Whether to stop generation early. Defaults to True.
+            length_penalty (Optional[float], optional): Length penalty value. Defaults to 1.0.
+            num_beam_groups (Optional[int], optional): Number of groups for diverse beam search. Defaults to 1.
+            diversity_penalty (Optional[float], optional): Diversity penalty value. Defaults to 0.0.
+            do_sample (Optional[bool], optional): Whether to use sampling for generation. Defaults to False.
+            temperature (Optional[float], optional): Temperature value for sampling. Defaults to 1.0.
+            top_k (Optional[int], optional): Value of k for top-k sampling. Defaults to 50.
+            top_p (Optional[float], optional): Value of p for top-p sampling. Defaults to 1.0.
 
         Returns:
-            GenerationOutputs: The generation outputs.
+            GenericOutputs: Generated caption sequences and their scores.
         """
-        outputs = super().generate(
-            input_ids,
+        outputs = self.model.generate(
+            pixel_values=pixel_values,
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            max_length=max_gen_seq_length,
+            min_length=min_gen_seq_length,
             num_beams=num_beams,
+            do_sample=do_sample,
             decoder_start_token_id=decoder_start_token_id,
-            decoder_end_token_id=decoder_end_token_id,
-            num_return_sequences=num_return_sequences,
-            min_gen_seq_length=min_gen_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-            repetition_penalty=repetition_penalty,
             no_repeat_ngram_size=no_repeat_ngram_size,
             early_stopping=early_stopping,
             length_penalty=length_penalty,
+            repetition_penalty=repetition_penalty,
+            num_return_sequences=num_return_sequences,
+            bos_token_id=decoder_start_token_id,
             num_beam_groups=num_beam_groups,
             diversity_penalty=diversity_penalty,
-            do_sample=do_sample,
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
+            return_dict_in_generate=True,
+            output_scores=True,
         )
 
-        return GenerationOutputs(
-            sequences=outputs.sequences,
-            sequences_scores=outputs.sequences_scores,
+        sequences = outputs.sequences.reshape(
+            -1, num_return_sequences, outputs.sequences.size(-1)
+        )
+        outputs.sequences = torch.zeros(
+            sequences.size(0), num_return_sequences, max_gen_seq_length
+        ).to(device=sequences.device)
+        outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)
+
+        if num_return_sequences == 1:
+            outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)
+
+        return GenericOutputs(
+            sequences=outputs.sequences, sequences_scores=outputs.sequences_scores
         )
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/processing_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/random_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/ranking_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/ranking_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/segmentation_utils.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/swin/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/swin/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/swin/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/t5/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 # pretrained infos
-pretrained_t5_infos = {
-    "default-t5": {
-        "config": "https://huggingface.co/t5-base/resolve/main/config.json",
-        "vocab": "https://huggingface.co/t5-base/resolve/main/spiece.model",
-    },
-    "t5-base": {
-        "config": "https://huggingface.co/t5-base/resolve/main/config.json",
-        "vocab": "https://huggingface.co/t5-base/resolve/main/spiece.model",
-        "weight": "https://huggingface.co/t5-base/resolve/main/pytorch_model.bin",
+
+pretrained_visualbert_infos = {
+    "default-visualbert": {
+        "config": "https://huggingface.co/uclanlp/visualbert-vqa-coco-pre/resolve/main/config.json",
+        "vocab": "https://huggingface.co/bert-base-uncased/resolve/main/vocab.txt",
     },
-    "t5-small": {
-        "config": "https://huggingface.co/t5-small/resolve/main/config.json",
-        "vocab": "https://huggingface.co/t5-small/resolve/main/spiece.model",
-        "weight": "https://huggingface.co/t5-small/resolve/main/pytorch_model.bin",
+    "visualbert-vqa-coco-pre": {
+        "config": "https://huggingface.co/uclanlp/visualbert-vqa-coco-pre/resolve/main/config.json",
+        "vocab": "https://huggingface.co/bert-base-uncased/resolve/main/vocab.txt",
+        "weight": "https://huggingface.co/uclanlp/visualbert-vqa-coco-pre/resolve/main/pytorch_model.bin",
     },
-    "t5-large": {
-        "config": "https://huggingface.co/t5-large/resolve/main/config.json",
-        "vocab": "https://huggingface.co/t5-large/resolve/main/spiece.model",
-        "weight": "https://huggingface.co/t5-large/resolve/main/pytorch_model.bin",
+    "visualbert-nlvr2-coco-pre": {
+        "config": "https://huggingface.co/uclanlp/visualbert-nlvr2-coco-pre/resolve/main/config.json",
+        "vocab": "https://huggingface.co/bert-base-multilingual-uncased/resolve/main/vocab.txt",
+        "weight": "https://huggingface.co/uclanlp/visualbert-nlvr2-coco-pre/resolve/main/pytorch_model.bin",
     },
 }
 
-import unitorch.cli.models.t5.modeling
-import unitorch.cli.models.t5.processing
-from unitorch.cli.models.t5.modeling import T5ForGeneration
-from unitorch.cli.models.t5.processing import T5Processor
+import unitorch.cli.models.visualbert.modeling
+import unitorch.cli.models.visualbert.processing
+from unitorch.cli.models.visualbert.modeling import (
+    VisualBertForClassification,
+    VisualBertForPretrain,
+)
+from unitorch.cli.models.visualbert.processing import VisualBertProcessor
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/t5/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/t5/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/vit/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/vit/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/vit/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/modeling.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/processing.py` & `unitorch-0.0.0.7/src/unitorch/cli/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/optim/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/optim/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,7 +62,47 @@
     @add_default_section_for_init("core/optim/adamw")
     def from_core_configure(cls, config, **kwargs):
         pass
 
 
 # more optims
 import unitorch.cli.optim.lion
+
+# bitsandbytes
+from unitorch.utils import is_bitsandbytes_available
+
+if is_bitsandbytes_available():
+    from unitorch.optim import Adam8bit, AdamW8bit
+
+    @register_optim("core/optim/adam8bit")
+    class Adam8bitOptimizer(Adam8bit, CheckpointMixin):
+        def __init__(
+            self,
+            params,
+            learning_rate: Optional[float] = 0.00001,
+        ):
+            super().__init__(
+                params=params,
+                lr=learning_rate,
+            )
+
+        @classmethod
+        @add_default_section_for_init("core/optim/adam8bit")
+        def from_core_configure(cls, config, **kwargs):
+            pass
+
+    @register_optim("core/optim/adamw8bit")
+    class AdamW8bitOptimizer(AdamW8bit, CheckpointMixin):
+        def __init__(
+            self,
+            params,
+            learning_rate: Optional[float] = 0.00001,
+        ):
+            super().__init__(
+                params=params,
+                lr=learning_rate,
+            )
+
+        @classmethod
+        @add_default_section_for_init("core/optim/adamw8bit")
+        def from_core_configure(cls, config, **kwargs):
+            pass
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/optim/lion.py` & `unitorch-0.0.0.7/src/unitorch/cli/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/scheduler/warmup.py` & `unitorch-0.0.0.7/src/unitorch/cli/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/score/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/service.py` & `unitorch-0.0.0.7/src/unitorch/cli/services/zip_image/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/tasks/deepspeed.py` & `unitorch-0.0.0.7/src/unitorch/cli/tasks/supervised.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # Licensed under the MIT License.
 
 import os
 import torch
 import time
 import json
 import logging
-import deepspeed
 import numpy as np
 import pandas as pd
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 from copy import deepcopy
+from PIL import Image
 from itertools import chain
 from collections.abc import Iterable
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, Iterator
 from torch.utils.data import DataLoader, Dataset, SequentialSampler
 from torch.utils.data.distributed import DistributedSampler
 from torch.cuda.amp import autocast, GradScaler
 from torch.multiprocessing import Process, Queue
@@ -52,41 +52,190 @@
     ModelInputs,
     ModelOutputs,
     ModelTargets,
     LossOutputs,
     CombineTensorsInputs,
     CombineTensorsTargets,
 )
-from unitorch.cli.tasks.supervised import (
-    DatasetFeature,
-    collate_fn,
-    infer,
-    monitor,
-    save_checkpoint,
-)
 
 
-@register_task("core/task/deepspeed/supervised")
-class DeepspeedTask:
-    """Task class for deepspeed supervised learning."""
+class DatasetFeature(Dataset):
+    def __init__(self, dataset):
+        self.dataset = dataset
+
+    def __getitem__(self, idx):
+        row = self.dataset[idx]
+        ret = {}
+        for k, v in row.items():
+            if isinstance(v, Image.Image):
+                v = np.array(v).tolist()
+            if not isinstance(v, str):
+                v = json.dumps(v)
+            ret[k] = v
+        return ret
+
+    def __len__(self):
+        return len(self.dataset)
+
+
+def collate_fn(bufs):
+    combine_inputs, combine_targets = list(zip(*bufs))
+    if isinstance(combine_inputs[0], ModelInputs):
+        inputs = type(combine_inputs[0]).stack(*combine_inputs)
+    else:
+        combine_inputs = [
+            type(_inputs[0]).stack(*_inputs) for _inputs in list(zip(*combine_inputs))
+        ]
+        inputs = CombineTensorsInputs()
+        for _inputs in combine_inputs:
+            inputs.add(_inputs)
+
+    if isinstance(combine_targets[0], ModelTargets):
+        targets = type(combine_targets[0]).stack(*combine_targets)
+    else:
+        combine_targets = [
+            type(_targets[0]).stack(*_targets)
+            for _targets in list(zip(*combine_targets))
+        ]
+        targets = CombineTensorsTargets()
+        for _targets in combine_targets:
+            targets.add(_targets)
+
+    return inputs, targets
+
+
+@torch.no_grad()
+def infer(model, iter_data):
+    model.eval()
+    outputs, targets = [], []
+    for _, (_inputs, _targets) in enumerate(iter_data):
+        if torch.cuda.is_available():
+            _inputs = _inputs.cuda()
+            _targets = _targets.cuda()
+        _outputs = model(**_inputs.dict())
+        outputs.append(_outputs)
+        targets.append(_targets)
+
+    if isinstance(outputs[0], LossOutputs):
+        outputs = LossOutputs(
+            loss=torch.tensor([output.loss for output in outputs]).to(
+                device=outputs[0].loss.device
+            )
+        )
+        if dist.is_initialized():
+            outputs = outputs.cuda().sync().cpu()
+        else:
+            outputs = outputs.cpu()
+    else:
+        outputs = type(outputs[0]).union(*outputs)
+        targets = type(targets[0]).union(*targets)
 
+        if dist.is_initialized():
+            outputs = outputs.cuda().sync().cpu()
+            targets = targets.cuda().sync().cpu()
+        else:
+            outputs = outputs.cpu()
+            targets = targets.cpu()
+    model.train()
+    return GenericOutputs(outputs=outputs, targets=targets)
+
+
+def monitor(outputs, targets, monitor_fns):
+    if monitor_fns is None:
+        return
+
+    for monitor_fn in monitor_fns:
+        score = monitor_fn(outputs=outputs, targets=targets)
+        info = str(type(monitor_fn).__name__)
+        logging.info(f"{info} is {score}")
+    return
+
+
+def save_checkpoint(
+    model,
+    ckpt_dir,
+    iter_dev,
+    score_fn,
+    monitor_fns,
+    optim,
+    scheduler,
+    ema_model=None,
+    best_score=-np.inf,
+    info_path=None,
+    local_rank=-1,
+    **kwargs,
+):
+    if not os.path.exists(ckpt_dir):
+        os.makedirs(ckpt_dir, exist_ok=True)
+
+    if ema_model is not None:
+        base_model = ema_model
+    else:
+        base_model = model
+
+    results = infer(base_model, iter_dev)
+    if local_rank in [-1, 0]:
+        new_score = score_fn(outputs=results.outputs, targets=results.targets)
+        monitor(results.outputs, results.targets, monitor_fns)
+        if new_score > best_score:
+            best_score = new_score
+            if model:
+                model.save_checkpoint(
+                    ckpt_dir=ckpt_dir, weight_name="pytorch_model.bin"
+                )
+            if ema_model:
+                ema_model.save_checkpoint(
+                    ckpt_dir=ckpt_dir, weight_name="pytorch_ema_model.bin"
+                )
+            if optim:
+                optim.save_checkpoint(
+                    ckpt_dir=ckpt_dir, weight_name="pytorch_optim.bin"
+                )
+            if scheduler:
+                scheduler.save_checkpoint(
+                    ckpt_dir=ckpt_dir, weight_name="pytorch_scheduler.bin"
+                )
+        if model:
+            model.save_checkpoint(
+                ckpt_dir=ckpt_dir, weight_name="pytorch_model_latest.bin"
+            )
+        if ema_model:
+            ema_model.save_checkpoint(
+                ckpt_dir=ckpt_dir, weight_name="pytorch_ema_model_latest.bin"
+            )
+            kwargs["num_ema_steps"] = ema_model.num_steps
+        if optim:
+            optim.save_checkpoint(
+                ckpt_dir=ckpt_dir, weight_name="pytorch_optim_latest.bin"
+            )
+        if scheduler:
+            scheduler.save_checkpoint(
+                ckpt_dir=ckpt_dir, weight_name="pytorch_scheduler_latest.bin"
+            )
+        if info_path is not None:
+            json.dump({"best_score": best_score, **kwargs}, open(info_path, "w"))
+    return best_score
+
+
+@register_task("core/task/supervised")
+class SupervisedTask:
     def __init__(
         self,
         configure,
         model,
         datasets,
         local_rank: Optional[int] = -1,
         seed: Optional[int] = 1123,
     ):
         """
-        Initialize the DeepspeedTask.
+        Initialize the SupervisedTask.
 
         Args:
             configure: The configuration object.
-            model: The model for supervised learning.
+            model: The model for the task.
             datasets: The datasets for training and evaluation.
             local_rank (optional): The local rank for distributed training. Defaults to -1.
             seed (optional): The random seed. Defaults to 1123.
         """
         set_seed(seed)
         self.n_gpu = 1 if torch.cuda.is_available() else 0
         if dist.is_initialized():
@@ -102,32 +251,32 @@
 
         if torch.cuda.is_available():
             self.model = self.model.cuda()
 
         self.best_score = -np.inf
 
     @classmethod
-    @add_default_section_for_init("core/task/deepspeed/supervised")
+    @add_default_section_for_init("core/task/supervised")
     def from_core_configure(cls, config, **kwargs):
         """
-        Create a DeepspeedTask instance from a core configuration.
+        Create a SupervisedTask instance from the core configuration.
 
         Args:
-            config: The core configuration.
+            config: The core configuration object.
             **kwargs: Additional keyword arguments.
 
         Returns:
-            A DeepspeedTask instance.
+            A dictionary containing the configuration, model, datasets, and local rank.
         """
         try:
-            deepspeed.init_distributed(dist_backend="nccl", init_method="env://")
+            torch.distributed.init_process_group(backend="nccl", init_method="env://")
         except:
             logging.info("PyTorch is not in distributed mode")
 
-        config.set_default_section("core/task/deepspeed/supervised")
+        config.set_default_section("core/task/supervised")
 
         model = config.getoption("model", None)
         dataset = config.getoption("dataset", None)
 
         if model is not None:
             model = init_registered_module(model, config, registered_model)
 
@@ -143,71 +292,69 @@
         return dict(
             configure=config,
             model=model,
             datasets=dataset,
             local_rank=local_rank,
         )
 
-    @add_default_section_for_function("core/task/deepspeed/supervised")
+    @add_default_section_for_function("core/task/supervised")
     def train(
         self,
-        config_path: str,
         optim: str,
         loss_fn: str,
         score_fn: str,
         monitor_fns: Optional[Union[str, List[str]]] = None,
+        scheduler: Optional[str] = None,
         from_ckpt_dir: Optional[str] = "./from_ckpt",
         to_ckpt_dir: Optional[str] = "./to_ckpt",
         train_batch_size: Optional[int] = 128,
         dev_batch_size: Optional[int] = 128,
         pin_memory: Optional[bool] = True,
         num_workers: Optional[int] = 4,
-        save_optimizer: Optional[bool] = False,
-        save_scheduler: Optional[bool] = False,
+        save_optimizer: Optional[bool] = True,
+        save_scheduler: Optional[bool] = True,
         log_freq: Optional[int] = 100,
         ckpt_freq: Optional[int] = 10000,
         grad_acc_step: Optional[int] = 1,
         max_grad_norm: Optional[float] = 1.0,
-        learning_rate: Optional[float] = None,
-        max_warmup_learning_rate: Optional[float] = None,
-        num_warmup_steps: Optional[int] = None,
+        num_training_samples: Optional[int] = 1000000000,
         epochs: Optional[int] = 5,
         use_ema: Optional[bool] = False,
         ema_decay: Optional[float] = 0.9999,
         ema_tau: Optional[int] = 2000,
+        use_amp: Optional[bool] = True,
         gpu_mode: Optional[bool] = False,
     ):
         """
-        Train the model using deepspeed.
+        Train the model.
 
         Args:
-            config_path: The path to the deepspeed configuration file.
-            optim: The optimizer used for training.
-            loss_fn: The loss function used for training.
-            score_fn: The score function used for evaluation.
+            optim: The optimizer for training.
+            loss_fn: The loss function for training.
+            score_fn: The scoring function for evaluation.
             monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.
+            scheduler (optional): The scheduler for adjusting the learning rate. Defaults to None.
             from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
             to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to "./to_ckpt".
             train_batch_size (optional): The batch size for training. Defaults to 128.
             dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
             pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
             num_workers (optional): The number of worker processes for data loading. Defaults to 4.
-            save_optimizer (optional): Whether to save the optimizer state. Defaults to False.
-            save_scheduler (optional): Whether to save the scheduler state. Defaults to False.
-            log_freq (optional): The frequency of logging. Defaults to 100.
+            save_optimizer (optional): Whether to save the optimizer. Defaults to True.
+            save_scheduler (optional): Whether to save the scheduler. Defaults to True.
+            log_freq (optional): The frequency of logging training information. Defaults to 100.
             ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.
             grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.
-            max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.
-            learning_rate (optional): The learning rate for the optimizer. Defaults to None.
-            max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.
-            num_warmup_steps (optional): The number of warmup steps. Defaults to None.
+            max_grad_norm (optional): The maximum gradient norm for gradient clipping. Defaults to 1.0.
+            num_training_samples (optional): The number of training samples. Defaults to 1000000000.
             epochs (optional): The number of training epochs. Defaults to 5.
             use_ema (optional): Whether to use exponential moving average. Defaults to False.
-            ema_decay (optional): The decay factor for exponential moving average. Defaults to 0.9999.
+            ema_decay (optional): The decay rate for exponential moving average. Defaults to 0.9999.
             ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.
+            use_amp (optional): Whether to use automatic mixed precision. Defaults to True.
             gpu_mode (optional): Whether to make GPU active. Defaults to False.
         """
         if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:
             os.makedirs(to_ckpt_dir, exist_ok=True)
 
         if loss_fn is not None:
             loss_fn = init_registered_module(loss_fn, self.config, registered_loss)
@@ -218,53 +365,38 @@
         if monitor_fns is not None:
             monitor_fns = [
                 init_registered_module(monitor_fn, self.config, registered_score)
                 for monitor_fn in monitor_fns
                 if monitor_fn in registered_score
             ]
 
-        config_file = cached_path(config_path)
-        config_dict = json.load(open(config_file, "r"))
-        config_dict["train_micro_batch_size_per_gpu"] = train_batch_size
+        if optim is not None and self.model is not None:
+            optim = init_registered_module(
+                optim,
+                self.config,
+                registered_optim,
+                params=self.model.parameters(),
+            )
 
         if os.path.exists(from_ckpt_dir):
             self.model.from_checkpoint(from_ckpt_dir)
+            optim.from_checkpoint(
+                from_ckpt_dir,
+                weight_name="pytorch_optim.bin",
+            )
 
         if os.path.exists(to_ckpt_dir):
             self.model.from_checkpoint(
                 to_ckpt_dir,
                 weight_name="pytorch_model_latest.bin",
             )
-
-        params = self.model.parameters()
-        params = filter(lambda x: x.requires_grad, params)
-
-        assert "optimizer" in config_dict
-
-        if "params" not in config_dict["optimizer"]:
-            config_dict["optimizer"]["params"] = dict()
-
-        if "scheduler" in config_dict:
-            if "params" not in config_dict["scheduler"]:
-                config_dict["scheduler"]["params"] = dict()
-
-        if learning_rate is not None:
-            config_dict["optimizer"]["params"]["lr"] = learning_rate
-            if "scheduler" in config_dict:
-                config_dict["scheduler"]["params"]["warmup_max_lr"] = learning_rate
-
-        if max_warmup_learning_rate is not None and "scheduler" in config_dict:
-            config_dict["scheduler"]["params"][
-                "warmup_max_lr"
-            ] = max_warmup_learning_rate
-
-        if num_warmup_steps is not None and "scheduler" in config_dict:
-            if "params" not in config_dict["scheduler"]:
-                config_dict["scheduler"]["params"] = dict()
-            config_dict["scheduler"]["params"]["warmup_num_steps"] = num_warmup_steps
+            optim.from_checkpoint(
+                to_ckpt_dir,
+                weight_name="pytorch_optim_latest.bin",
+            )
 
         info_path = os.path.join(to_ckpt_dir, "info.json")
         if os.path.exists(info_path):
             info = json.load(open(os.path.join(to_ckpt_dir, "info.json")))
         else:
             info = dict()
 
@@ -295,22 +427,23 @@
                 )
 
         for n, p in self.model.named_parameters():
             logging.debug(
                 f"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}"
             )
 
-        self.model, optim, _, scheduler = deepspeed.initialize(
-            model=self.model,
-            config=config_dict,
-            model_parameters=params,
-        )
-
         global_rank = -1
         if self.n_gpu > 1:
+            self.model = nn.parallel.DistributedDataParallel(
+                self.model,
+                device_ids=[self.local_rank],
+                output_device=self.local_rank,
+                find_unused_parameters=False,
+                broadcast_buffers=False,
+            )
             global_rank = dist.get_rank()
 
         train_sampler = DistributedSkipSampler if self.n_gpu > 1 else RandomSkipSampler
         dev_sampler = DistributedSampler if self.n_gpu > 1 else SequentialSampler
 
         if gpu_mode:
             with ActiveGPUJob() as _:
@@ -340,14 +473,49 @@
             batch_size=dev_batch_size,
             shuffle=False,
             pin_memory=pin_memory,
             num_workers=num_workers,
             collate_fn=collate_fn,
         )
 
+        if scheduler is not None:
+            if not isinstance(dataset_train, Iterable):
+                num_training_steps = int(
+                    epochs
+                    * len(dataset_train)
+                    // train_batch_size
+                    // max(1, self.n_gpu)
+                    // grad_acc_step
+                )
+            else:
+                num_training_steps = int(
+                    epochs
+                    * num_training_samples
+                    // train_batch_size
+                    // max(1, self.n_gpu)
+                    // grad_acc_step
+                )
+
+            scheduler = init_registered_module(
+                scheduler,
+                self.config,
+                registered_scheduler,
+                optimizer=optim,
+                num_training_steps=num_training_steps,
+            )
+
+        if scheduler and os.path.exists(to_ckpt_dir):
+            scheduler.from_checkpoint(
+                to_ckpt_dir,
+                weight_name="pytorch_scheduler_latest.bin",
+            )
+
+        if use_amp:
+            scaler = GradScaler()
+
         log_loss = 0
         dev_epoch = 0
         for e in range(0, epochs):
             torch.cuda.empty_cache()
             if e < global_epoch:
                 continue
 
@@ -394,20 +562,26 @@
                         else:
                             loss = (
                                 loss_fn(outputs=outputs, targets=targets)
                                 / grad_acc_step
                             )
 
                 nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)
-                self.model.backward(loss)
-
+                if use_amp:
+                    scaler.scale(loss).backward()
+                else:
+                    loss.backward()
                 log_loss += loss.data * grad_acc_step
                 if (step + 1) % grad_acc_step == 0:
                     is_update_step = True
-                    optim.step()
+                    if use_amp:
+                        scaler.step(optim)
+                        scaler.update()
+                    else:
+                        optim.step()
                     if scheduler is not None:
                         scheduler.step()
                     optim.zero_grad()
 
                     if use_ema and self.ema_model is not None:
                         self.ema_model.step(
                             self.model.module if self.n_gpu > 1 else self.model
@@ -440,15 +614,16 @@
                         info_path=info_path,
                         local_rank=self.local_rank,
                         global_epoch=e,
                         global_step=step + 1,
                     )
 
             if not is_update_step:
-                optim.step()
+                scaler.step(optim)
+                scaler.update()
                 if scheduler is not None:
                     scheduler.step()
                 optim.zero_grad()
 
                 if use_ema and self.ema_model is not None:
                     self.ema_model.step(
                         self.model.module if self.n_gpu > 1 else self.model
@@ -478,26 +653,26 @@
                 info_path=info_path,
                 local_rank=self.local_rank,
                 global_epoch=e,
                 global_step=0,
             )
 
     @torch.no_grad()
-    @add_default_section_for_function("core/task/deepspeed/supervised")
+    @add_default_section_for_function("core/task/supervised")
     def eval(
         self,
         monitor_fns: Union[str, List[str]],
         from_ckpt_dir: Optional[str] = "./from_ckpt",
         dev_batch_size: Optional[int] = 128,
         pin_memory: Optional[bool] = True,
         num_workers: Optional[int] = 4,
         gpu_mode: Optional[bool] = False,
     ):
         """
-        Evaluate the model.
+        Perform evaluation on the model.
 
         Args:
             monitor_fns: The monitoring functions for evaluation.
             from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
             dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
             pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
             num_workers (optional): The number of worker processes for data loading. Defaults to 4.
@@ -546,15 +721,15 @@
             monitor(
                 outputs=results.outputs,
                 targets=results.targets,
                 monitor_fns=monitor_fns,
             )
 
     @torch.no_grad()
-    @add_default_section_for_function("core/task/deepspeed/supervised")
+    @add_default_section_for_function("core/task/supervised")
     def infer(
         self,
         postprocess_fn: str,
         writer: str,
         test_batch_size: Optional[int] = 128,
         pin_memory: Optional[bool] = True,
         num_workers: Optional[int] = 4,
@@ -562,27 +737,27 @@
         from_ckpt_dir: Optional[str] = "./from_ckpt",
         output_header: Optional[List] = None,
         output_path: Optional[str] = "./cache/predict.txt",
         postprocess_workers: Optional[int] = 2,
         gpu_mode: Optional[bool] = False,
     ):
         """
-        Perform inference using the trained model.
+        Perform inference using the model.
 
         Args:
-            postprocess_fn: The post-processing function for inference.
-            writer: The writer for writing the results.
+            postprocess_fn: The postprocessing function for inference.
+            writer: The writer to save the inference results.
             test_batch_size (optional): The batch size for inference. Defaults to 128.
             pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
             num_workers (optional): The number of worker processes for data loading. Defaults to 4.
-            max_size (optional): The maximum size of the dataset for inference. Defaults to 10000.
+            max_size (optional): The maximum number of samples to process. Defaults to 10000.
             from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
             output_header (optional): The header for the output file. Defaults to None.
             output_path (optional): The path to save the output file. Defaults to "./cache/predict.txt".
-            postprocess_workers (optional): The number of worker processes for post-processing. Defaults to 2.
+            postprocess_workers (optional): The number of worker processes for postprocessing. Defaults to 2.
             gpu_mode (optional): Whether to make GPU active. Defaults to False.
         """
         assert self.n_gpu <= 1
         assert writer is not None
 
         output_dir = os.path.dirname(output_path)
         if not os.path.exists(output_dir):
@@ -623,19 +798,14 @@
             batch_size=test_batch_size,
             shuffle=False,
             pin_memory=pin_memory,
             num_workers=num_workers,
             collate_fn=collate_fn,
         )
 
-        if skip_step > 0:
-            output_file = open(output_path, "a")
-        else:
-            output_file = open(output_path, "w")
-
         if skip_step > 0 and hasattr(dataset_test, "set_skip_step"):
             dataset_test.set_skip_step(skip_step)
 
         if skip_step > 0 and hasattr(iter_test.sampler, "set_skip_step"):
             iter_test.sampler.set_skip_step(skip_step)
 
         if hasattr(dataset_test, "dataset"):
```

### Comparing `unitorch-0.0.0.6/src/unitorch/cli/writer/__init__.py` & `unitorch-0.0.0.7/src/unitorch/cli/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/datasets/hf.py` & `unitorch-0.0.0.7/src/unitorch/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/loss/__init__.py` & `unitorch-0.0.0.7/src/unitorch/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/loss/prophetnet.py` & `unitorch-0.0.0.7/src/unitorch/loss/prophetnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/loss/ranking.py` & `unitorch-0.0.0.7/src/unitorch/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/__init__.py` & `unitorch-0.0.0.7/src/unitorch/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,22 +196,22 @@
 
 from unitorch.models.processing_utils import (
     HfTextGenerationProcessor,
     HfTextClassificationProcessor,
     HfImageClassificationProcessor,
 )
 from unitorch.models.modeling_ema import ExponentialMovingAverage
+from unitorch.models.quantization import QuantizationConfig, QuantizationMixin
 
 # import models
 import unitorch.models.bart
 import unitorch.models.beit
 import unitorch.models.bert
 import unitorch.models.blip
 import unitorch.models.bloom
-import unitorch.models.chatglm
 import unitorch.models.clip
 import unitorch.models.deberta
 import unitorch.models.diffusers
 import unitorch.models.minigpt4
 import unitorch.models.llama
 import unitorch.models.mbart
 import unitorch.models.mt5
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bart/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/bart/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,14 @@
             input_ids=input_ids,
             attention_mask=attention_mask,
             decoder_input_ids=decoder_input_ids,
             decoder_attention_mask=decoder_attention_mask,
             return_dict=True,
         )
         logits = outputs.logits
-        print("model :", logits[0, 0, 0].item(), logits[0, 0, 41552].item())
         return logits
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bart/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/beit/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/beit/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bert/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bert/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/blip/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/modeling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,199 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
-import os
 import torch
-import numpy as np
-from PIL import Image
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from torchvision.transforms import Resize, CenterCrop, ToTensor, Normalize, Compose
-from transformers import BlipImageProcessor, BertTokenizer
-from transformers.image_utils import to_numpy_array, ChannelDimension
-from transformers.image_transforms import to_channel_dimension_format
-from unitorch.utils import pop_value
-from unitorch.models import (
-    HfTextClassificationProcessor,
-    HfTextGenerationProcessor,
-    HfImageClassificationProcessor,
-    GenericOutputs,
+import torch.nn as nn
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from transformers.models.xlm_roberta.modeling_xlm_roberta import (
+    XLMRobertaConfig,
+    XLMRobertaModel,
 )
+from transformers.models.xlm_roberta_xl.modeling_xlm_roberta_xl import (
+    XLMRobertaXLConfig,
+    XLMRobertaXLModel,
+)
+
+from transformers.models.roberta.modeling_roberta import RobertaLMHead
+from unitorch.models import GenericModel
 
 
-class BlipProcessor(
-    HfTextClassificationProcessor,
-    HfTextGenerationProcessor,
-    HfImageClassificationProcessor,
-):
+class XLMRobertaForClassification(GenericModel):
+    """
+    XLM-RoBERTa model for classification tasks.
+    """
+
     def __init__(
         self,
-        vocab_path: str,
-        vision_config_path: str,
-        max_seq_length: Optional[int] = 128,
-        max_gen_seq_length: Optional[int] = 48,
-        position_start_id: Optional[int] = 0,
+        config_path: str,
+        num_classes: Optional[int] = 1,
+        gradient_checkpointing: Optional[bool] = False,
     ):
         """
-        Initializes the BlipProcessor.
+        Initializes the XLMRobertaForClassification model.
 
         Args:
-            vocab_path (str): The path to the vocabulary file.
-            vision_config_path (str): The path to the vision configuration file.
-            max_seq_length (Optional[int]): The maximum sequence length for text inputs. Defaults to 128.
-            max_gen_seq_length (Optional[int]): The maximum sequence length for generated outputs. Defaults to 48.
-            position_start_id (Optional[int]): The position start ID. Defaults to 0.
-        """
-        vision_processor = BlipImageProcessor.from_json_file(vision_config_path)
-        HfImageClassificationProcessor.__init__(self, vision_processor=vision_processor)
-
-        tokenizer = BertTokenizer(
-            vocab_file=vocab_path,
-        )
-        tokenizer.bos_token = tokenizer.cls_token
-        tokenizer.bos_token_id = tokenizer.cls_token_id
-        tokenizer.eos_token = tokenizer.sep_token
-        tokenizer.eos_token_id = tokenizer.sep_token_id
-        HfTextClassificationProcessor.__init__(
-            self,
-            tokenizer=tokenizer,
-            max_seq_length=max_seq_length,
-            source_type_id=0,
-            target_type_id=0,
-            position_start_id=position_start_id,
-        )
-
-        HfTextGenerationProcessor.__init__(
-            self,
-            tokenizer=tokenizer,
-            max_seq_length=max_seq_length,
-            max_gen_seq_length=max_gen_seq_length,
-        )
-
-    def text_classification(
-        self,
-        text: str,
-        max_seq_length: Optional[int] = None,
-    ) -> GenericOutputs:
+            config_path (str): Path to the configuration file.
+            num_classes (Optional[int]): Number of classes. Defaults to 1.
+            gradient_checkpointing (Optional[bool]): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+        self.config = XLMRobertaConfig.from_json_file(config_path)
+        self.config.gradient_checkpointing = gradient_checkpointing
+        self.roberta = XLMRobertaModel(self.config)
+        self.dropout = nn.Dropout(self.config.hidden_dropout_prob)
+        self.classifier = nn.Linear(self.config.hidden_size, num_classes)
+        self.init_weights()
+
+    def forward(
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        token_type_ids: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.Tensor] = None,
+    ):
         """
-        Performs text classification on the given input text.
+        Forward pass of the XLMRobertaForClassification model.
 
         Args:
-            text (str): The input text to classify.
-            max_seq_length (Optional[int]): The maximum sequence length for the text. If None, the default value from initialization is used.
+            input_ids (torch.Tensor): Input tensor of shape [batch_size, sequence_length].
+            attention_mask (Optional[torch.Tensor]): Attention mask tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            token_type_ids (Optional[torch.Tensor]): Token type IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            position_ids (Optional[torch.Tensor]): Position IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
 
         Returns:
-            GenericOutputs: The outputs of the text classification.
+            (torch.Tensor):Output logits of shape [batch_size, num_classes].
         """
-        outputs = HfTextClassificationProcessor.classification(
-            self,
-            text=text,
-            max_seq_length=max_seq_length,
-        )
-        return GenericOutputs(
-            input_ids=outputs.input_ids,
-            attention_mask=outputs.attention_mask,
-            position_ids=outputs.position_ids,
+        outputs = self.roberta(
+            input_ids,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
         )
+        pooled_output = outputs[1]
 
-    def image_classification(
-        self,
-        image: Image.Image,
-    ) -> GenericOutputs:
-        """
-        Performs image classification on the given input image.
-
-        Args:
-            image (PIL.Image.Image): The input image to classify.
+        pooled_output = self.dropout(pooled_output)
+        logits = self.classifier(pooled_output)
+        return logits
 
-        Returns:
-            GenericOutputs: The outputs of the image classification.
-        """
-        outputs = HfImageClassificationProcessor.classification(
-            self,
-            image=image,
-        )
 
-        return GenericOutputs(
-            pixel_values=outputs.pixel_values,
-        )
+class XLMRobertaForMaskLM(GenericModel):
+    """
+    XLM-RoBERTa model for masked language modeling tasks.
+    """
 
-    def classification(
+    def __init__(
         self,
-        text: str,
-        image: Image.Image,
-        max_seq_length: Optional[int] = None,
-    ) -> GenericOutputs:
+        config_path: str,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
         """
-        Performs classification using both text and image inputs.
+        Initializes the XLMRobertaForMaskLM model.
 
         Args:
-            text (str): The input text to classify.
-            image (PIL.Image.Image): The input image to classify.
-            max_seq_length (Optional[int]): The maximum sequence length for the text. If None, the default value from initialization is used.
-
-        Returns:
-            GenericOutputs: The outputs of the classification.
+            config_path (str): Path to the configuration file.
+            gradient_checkpointing (Optional[bool]): Whether to use gradient checkpointing. Defaults to False.
         """
-        max_seq_length = pop_value(
-            max_seq_length,
-            self.max_seq_length,
-        )
-
-        text_outputs = self.text_classification(text, max_seq_length)
-        pixel_outputs = self.image_classification(image)
-
-        return GenericOutputs(
-            input_ids=text_outputs.input_ids,
-            attention_mask=text_outputs.attention_mask,
-            position_ids=text_outputs.position_ids,
-            pixel_values=pixel_outputs.pixel_values,
-        )
-
-    def generation_inputs(
-        self,
-        text: str,
-        max_seq_length: Optional[int] = None,
-    ) -> GenericOutputs:
+        super().__init__()
+        self.config = XLMRobertaConfig.from_json_file(config_path)
+        self.config.gradient_checkpointing = gradient_checkpointing
+        self.roberta = XLMRobertaModel(self.config, add_pooling_layer=False)
+        self.lm_head = RobertaLMHead(self.config)
+        self.init_weights()
+        self.roberta.embeddings.word_embeddings.weight = self.lm_head.decoder.weight
+
+    def forward(
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        token_type_ids: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.Tensor] = None,
+    ):
         """
-        Generate inputs for text generation.
+        Forward pass of the XLMRobertaForMaskLM model.
 
         Args:
-            text (str): The input text.
-            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+            input_ids (torch.Tensor): Input tensor of shape [batch_size, sequence_length].
+            attention_mask (Optional[torch.Tensor]): Attention mask tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            token_type_ids (Optional[torch.Tensor]): Token type IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            position_ids (Optional[torch.Tensor]): Position IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
 
         Returns:
-            GenericOutputs: The generated input tokens and attention mask.
+            (torch.Tensor):Output logits of shape [batch_size, sequence_length, vocabulary_size].
         """
-        outputs = HfTextGenerationProcessor.generation_inputs(
-            self,
-            text=text,
-            max_seq_length=max_seq_length,
-        )
-        return GenericOutputs(
-            input_ids=outputs.input_ids,
-            attention_mask=outputs.attention_mask,
+        outputs = self.roberta(
+            input_ids,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
         )
+        sequence_output = outputs[0]
+        logits = self.lm_head(sequence_output)
+        return logits
 
-    def generation_labels(
-        self,
-        text: str,
-        max_gen_seq_length: Optional[int] = None,
-    ) -> GenericOutputs:
-        """
-        Generates labels for text generation based on the given input text.
 
-        Args:
-            text (str): The input text for generating labels.
-            max_gen_seq_length (Optional[int]): The maximum sequence length for the generated labels. If None, the default value from initialization is used.
+class XLMRobertaXLForClassification(GenericModel):
+    """
+    XLM-RoBERTa XL model for classification tasks.
+    """
 
-        Returns:
-            GenericOutputs: The generated labels.
+    def __init__(
+        self,
+        config_path: str,
+        num_classes: Optional[int] = 1,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
         """
-        outputs = HfTextGenerationProcessor.generation_labels(
-            self,
-            text=text,
-            max_gen_seq_length=max_gen_seq_length,
-        )
-        return GenericOutputs(
-            input_ids=outputs.input_ids,
-            attention_mask=outputs.attention_mask,
-        )
+        Initializes the XLMRobertaXLForClassification model.
 
-    def generation(
-        self,
-        text: str,
-        image: Image.Image,
-        max_gen_seq_length: Optional[int] = None,
-    ) -> GenericOutputs:
+        Args:
+            config_path (str): Path to the configuration file.
+            num_classes (Optional[int]): Number of classes for classification. Defaults to 1.
+            gradient_checkpointing (Optional[bool]): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+        self.config = XLMRobertaXLConfig.from_json_file(config_path)
+        self.config.gradient_checkpointing = gradient_checkpointing
+        self.roberta = XLMRobertaXLModel(self.config)
+        self.dropout = nn.Dropout(self.config.hidden_dropout_prob)
+        self.classifier = nn.Linear(self.config.hidden_size, num_classes)
+        self.init_weights()
+
+    def forward(
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        token_type_ids: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.Tensor] = None,
+    ):
         """
-        Generate inputs, labels, and tokens for image to text generation.
+        Forward pass of the XLMRobertaXLForClassification model.
 
         Args:
-            text (str): The input text.
-            image (Image.Image): The input image to caption.
-            max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to None.
+            input_ids (torch.Tensor): Input tensor of shape [batch_size, sequence_length].
+            attention_mask (Optional[torch.Tensor]): Attention mask tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            token_type_ids (Optional[torch.Tensor]): Token type IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
+            position_ids (Optional[torch.Tensor]): Position IDs tensor of shape [batch_size, sequence_length].
+                Defaults to None.
 
         Returns:
-            GenericOutputs: The generated input tokens, attention masks, label tokens, and attention masks.
+            (torch.Tensor):Output logits of shape [batch_size, num_classes].
         """
-
-        max_gen_seq_length = pop_value(max_gen_seq_length, self.max_gen_seq_length)
-
-        tokens = self.generation_inputs(text, max_gen_seq_length)
-        pixels = self.image_classification(image)
-        labels = self.generation_labels(text, max_gen_seq_length)
-
-        return GenericOutputs(
-            input_ids=tokens.input_ids,
-            attention_mask=tokens.attention_mask,
-            pixel_values=pixels.pixel_values,
-            input_ids_label=labels.input_ids,
-            attention_mask_label=labels.attention_mask,
+        outputs = self.roberta(
+            input_ids,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
         )
+        pooled_output = outputs[1]
+
+        pooled_output = self.dropout(pooled_output)
+        logits = self.classifier(pooled_output)
+        return logits
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/blip2/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/blip2/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/blip2/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/blip2/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bloom/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/bloom/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/configuration_chatglm.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling_chatglm.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/quantization.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/chatglm/tokenization_chatglm.py` & `unitorch-0.0.0.7/src/unitorch/models/chatglm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/clip/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/clip/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/deberta/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/deberta/modeling_v2.py` & `unitorch-0.0.0.7/src/unitorch/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/deberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/deberta/processing_v2.py` & `unitorch-0.0.0.7/src/unitorch/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/diffusers/__init__.py` & `unitorch-0.0.0.7/src/unitorch/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.7/src/unitorch/models/diffusers/modeling_controlnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,23 @@
     AutoencoderKL,
 )
 from diffusers.schedulers import (
     DDPMScheduler,
     PNDMScheduler,
 )
 from diffusers.pipelines import StableDiffusionControlNetPipeline
-from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models import (
+    GenericModel,
+    GenericOutputs,
+    QuantizationConfig,
+    QuantizationMixin,
+)
 
 
-class ControlNetForImageGeneration(GenericModel):
+class ControlNetForImageGeneration(GenericModel, QuantizationMixin):
     prefix_keys_in_state_dict = {
         # unet weights
         "^conv_in.*": "unet.",
         "^conv_norm_out.*": "unet.",
         "^conv_out.*": "unet.",
         "^time_embedding.*": "unet.",
         "^up_blocks.*": "unet.",
@@ -49,14 +54,15 @@
     def __init__(
         self,
         config_path: str,
         text_config_path: str,
         vae_config_path: str,
         controlnet_config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 4,
         out_channels: Optional[int] = 4,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         freeze_vae_encoder: Optional[bool] = True,
         freeze_text_encoder: Optional[bool] = True,
@@ -92,14 +98,18 @@
 
         if freeze_text_encoder:
             self.text.requires_grad = False
 
         if freeze_unet_encoder:
             self.unet.requires_grad = False
 
+        if quant_config_path is not None:
+            self.quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            self.quantize(self.quant_config, ignore_modules=["lm_head"])
+
     def forward(
         self,
         input_ids: torch.Tensor,
         pixel_values: torch.Tensor,
         condition_pixel_values: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
     ):
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.7/src/unitorch/models/diffusers/modeling_stable.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,18 +19,23 @@
 from diffusers.pipelines import (
     DDPMPipeline,
     StableDiffusionPipeline,
     StableDiffusionUpscalePipeline,
     StableDiffusionInpaintPipeline,
     StableDiffusionDepth2ImgPipeline,
 )
-from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models import (
+    GenericModel,
+    GenericOutputs,
+    QuantizationConfig,
+    QuantizationMixin,
+)
 
 
-class StableForImageGeneration(GenericModel):
+class StableForImageGeneration(GenericModel, QuantizationMixin):
     prefix_keys_in_state_dict = {
         # unet weights
         "^conv_in.*": "unet.",
         "^conv_norm_out.*": "unet.",
         "^conv_out.*": "unet.",
         "^time_embedding.*": "unet.",
         "^up_blocks.*": "unet.",
@@ -43,14 +48,15 @@
         "^quant_conv.*": "vae.",
     }
 
     def __init__(
         self,
         config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 3,
         out_channels: Optional[int] = 3,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         seed: Optional[int] = 1123,
     ):
@@ -68,14 +74,18 @@
             }
         )
         self.unet = UNet2DModel.from_config(config_dict)
 
         scheduler_config_dict = json.load(open(scheduler_config_path))
         self.scheduler = DDPMScheduler.from_config(scheduler_config_dict)
 
+        if quant_config_path is not None:
+            self.quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            self.quantize(self.quant_config)
+
     def forward(self, pixel_values: torch.Tensor):
         noise = torch.randn(pixel_values.shape).to(pixel_values.device)
         batch = pixel_values.size(0)
 
         timesteps = torch.randint(
             0,
             self.scheduler.num_train_timesteps,
@@ -103,15 +113,15 @@
             batch_size=batch_size,
             generator=torch.Generator(device=pipeline.device).manual_seed(self.seed),
         ).images
 
         return GenericOutputs(images=images)
 
 
-class StableForText2ImageGeneration(GenericModel):
+class StableForText2ImageGeneration(GenericModel, QuantizationMixin):
     prefix_keys_in_state_dict = {
         # unet weights
         "^conv_in.*": "unet.",
         "^conv_norm_out.*": "unet.",
         "^conv_out.*": "unet.",
         "^time_embedding.*": "unet.",
         "^up_blocks.*": "unet.",
@@ -135,14 +145,15 @@
 
     def __init__(
         self,
         config_path: str,
         text_config_path: str,
         vae_config_path: str,
         scheduler_config_path: str,
+        quant_config_path: Optional[str] = None,
         image_size: Optional[int] = 224,
         in_channels: Optional[int] = 4,
         out_channels: Optional[int] = 4,
         num_train_timesteps: Optional[int] = 1000,
         num_infer_timesteps: Optional[int] = 50,
         freeze_vae_encoder: Optional[bool] = True,
         freeze_text_encoder: Optional[bool] = True,
@@ -177,14 +188,18 @@
 
         if freeze_vae_encoder:
             self.vae.requires_grad = False
 
         if freeze_text_encoder:
             self.text.requires_grad = False
 
+        if quant_config_path is not None:
+            self.quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            self.quantize(self.quant_config)
+
     def forward(
         self,
         pixel_values: torch.Tensor,
         input_ids: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
     ):
         latents = self.vae.encode(pixel_values).latent_dist.sample()
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.7/src/unitorch/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_stable.py` & `unitorch-0.0.0.7/src/unitorch/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/llama/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/peft/modeling_llama_lora.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
-import os
-import logging
+import json
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
-import transformers
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from peft import LoraConfig, PeftModelForCausalLM
 from transformers import LlamaModel, LlamaConfig, LlamaForCausalLM
-from unitorch.utils.decorators import replace
-from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models import (
+    GenericModel,
+    GenericOutputs,
+    QuantizationConfig,
+    QuantizationMixin,
+)
+from unitorch.models.quantization import quantize_model
+from unitorch.models.peft import PeftModelForSequenceClassification, GenericPeftModel
 
 
-class LlamaForClassification(GenericModel):
+class LlamaLoraForClassification(GenericPeftModel, QuantizationMixin):
+    prefix_keys_in_state_dict = {
+        "^(?!peft_model\.base_model\.model\.).*": "peft_model.base_model."
+    }
+
     def __init__(
         self,
         config_path: str,
+        quant_config_path: Optional[str] = None,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["q_proj", "v_proj"],
         num_classes: Optional[int] = 1,
         hidden_dropout_prob: Optional[float] = 0.1,
         gradient_checkpointing: Optional[bool] = False,
     ):
-        """
-        Llama model for classification tasks.
-
-        Args:
-            config_path (str): Path to the model configuration file.
-            num_classes (int, optional): Number of classes for classification. Defaults to 1.
-            hidden_dropout_prob (float, optional): Dropout probability for hidden layers. Defaults to 0.1.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
-        """
         super().__init__()
         self.config = LlamaConfig.from_json_file(config_path)
         self.config.gradient_checkpointing = gradient_checkpointing
-        self.model = LlamaModel(self.config)
+        self.peft_config = LoraConfig(
+            r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
+        )
+        model = LlamaModel(self.config)
+        if quant_config_path is not None:
+            quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            ignore_modules = target_modules + ["lm_head"]
+            model = quantize_model(model, quant_config, ignore_modules=ignore_modules)
+        self.peft_model = PeftModelForSequenceClassification(model, self.peft_config)
         self.dropout = nn.Dropout(hidden_dropout_prob)
         self.classifier = nn.Linear(self.config.hidden_size, num_classes)
         self.init_weights()
 
     def forward(
         self,
         input_ids: torch.Tensor,
@@ -51,110 +68,58 @@
             input_ids (torch.Tensor): Input tensor of shape (batch_size, sequence_length).
             attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.
             position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.
 
         Returns:
             torch Output logits.Tensor: tensor of shape (batch_size, num_classes).
         """
-        outputs = self.model(
+        outputs = self.peft_model(
             input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
         )[0]
         pooled_output = outputs[:, -1]
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         return logits
 
 
-class LlamaForPretrain(GenericModel):
-    def __init__(
-        self,
-        config_path: str,
-        gradient_checkpointing: Optional[bool] = False,
-    ):
-        """
-        Llama model for pretraining tasks.
-
-        Args:
-            config_path (str): Path to the model configuration file.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
-        """
-        super().__init__()
-        self.config = LlamaConfig.from_json_file(config_path)
-        self.config.gradient_checkpointing = gradient_checkpointing
-        self.model = LlamaModel(self.config)
-        self.lm_head = nn.Linear(
-            self.config.hidden_size, self.config.vocab_size, bias=False
-        )
-        self.init_weights()
-
-    def forward(
-        self,
-        input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.Tensor] = None,
-        input_ids_label: Optional[torch.Tensor] = None,
-        attention_mask_label: Optional[torch.Tensor] = None,
-    ):
-        """
-        Forward pass of the pretraining model.
-
-        Args:
-            input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.
-            attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.
-            position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.
-            input_ids_label (torch.Tensor, optional): Labeled input tensor of shape (batch_size, sequence_length). Defaults to None.
-            attention_mask_label (torch.Tensor, optional): Labeled attention mask tensor of shape (batch_size, sequence_length). Defaults to None.
-
-        Returns:
-            torch Output loss.Tensor: Loss value.
-        """
-        outputs = self.model(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-        )
-        predict_logits = self.lm_head(outputs[0])
-        batch_size, seq_len, num_classes = predict_logits.size()
-        logits = predict_logits.contiguous().view(batch_size * seq_len, num_classes)
-        targets = input_ids_label.contiguous().view(-1).long()
-        masks = attention_mask_label.contiguous().view(-1)
-        loss = nn.CrossEntropyLoss(reduction="none")(logits, targets)
-        loss = loss * masks.float()
-        loss = loss.contiguous().view(batch_size, seq_len).sum(1) / torch.max(
-            masks.contiguous().view(batch_size, seq_len).float().sum(1),
-            torch.ones(batch_size).to(masks.device),
-        )
-        loss = torch.mean(loss)
-        return loss
-
-
-class LlamaForGeneration(GenericModel):
+class LlamaLoraForGeneration(GenericPeftModel):
     prefix_keys_in_state_dict = {
-        "^(?!model\.model\.|model\.lm_head\.)model\.": "model.",
-        "^lm_head.": "model.",
+        "^(?!peft_model\.base_model\.model\.model\.)model\.": "peft_model.base_model.model.",
+        "^lm_head.": "peft_model.base_model.model.",
     }
 
     def __init__(
         self,
         config_path: str,
+        quant_config_path: Optional[str] = None,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["q_proj", "v_proj"],
         gradient_checkpointing: Optional[bool] = False,
     ):
-        """
-        Llama model for text generation tasks.
-
-        Args:
-            config_path (str): Path to the model configuration file.
-            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
-        """
         super().__init__()
         self.config = LlamaConfig.from_json_file(config_path)
         self.config.gradient_checkpointing = gradient_checkpointing
-        self.model = LlamaForCausalLM(self.config)
+        self.peft_config = LoraConfig(
+            r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
+        )
+        model = LlamaForCausalLM(self.config)
+        if quant_config_path is not None:
+            quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            ignore_modules = target_modules + ["lm_head"]
+            model = quantize_model(model, quant_config, ignore_modules=ignore_modules)
+        self.peft_model = PeftModelForCausalLM(model, self.peft_config)
         self.init_weights()
 
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
@@ -166,15 +131,15 @@
             input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.
             attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.
             position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.
 
         Returns:
             torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).
         """
-        outputs = self.model(
+        outputs = self.peft_model(
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
             return_dict=True,
         )
         logits = outputs.logits
         return logits
@@ -222,16 +187,16 @@
             top_k (int, optional): Top-k value for sampling. Defaults to 50.
             top_p (float, optional): Top-p value for sampling. Defaults to 1.0.
 
         Returns:
             GenericOutputs: Generated sequences and their scores.
         """
         input_seq_length = input_ids.size(1)
-        outputs = self.model.generate(
-            input_ids,
+        outputs = self.peft_model.generate(
+            input_ids=input_ids,
             max_length=max_gen_seq_length + input_seq_length,
             min_length=min_gen_seq_length + input_seq_length,
             num_beams=num_beams,
             do_sample=do_sample,
             decoder_start_token_id=decoder_start_token_id,
             no_repeat_ngram_size=no_repeat_ngram_size,
             early_stopping=early_stopping,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/llama/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/mbart/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/mbart/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/minigpt4/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/minigpt4/modeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from transformers import LlamaConfig, LlamaForCausalLM
 from transformers.models.blip_2.modeling_blip_2 import (
     Blip2Config,
     Blip2VisionModel,
     Blip2QFormerModel,
 )
 from unitorch.utils.decorators import replace
-from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models import (
+    GenericModel,
+    GenericOutputs,
+    QuantizationConfig,
+    QuantizationMixin,
+)
 from unitorch.models.clip.modeling import AllGather
 
 
 class MiniGPT4Blip2LlamaModel(nn.Module):
     """
     MiniGPT4Blip2LlamaModel is a model that combines the Blip2VisionModel, Blip2QFormerModel, and LlamaForCausalLM
     models for generation. It inherits from the nn.Module class.
@@ -221,32 +226,34 @@
             attention_mask=attention_mask,
             **generate_kwargs,
         )
 
         return outputs
 
 
-class MiniGPT4Blip2LlamaForGeneration(GenericModel):
+class MiniGPT4Blip2LlamaForGeneration(GenericModel, QuantizationMixin):
     """
     MiniGPT4Blip2LlamaForGeneration is a generation model that combines the MiniGPT4Blip2LlamaModel with generation
     capabilities. It inherits from the GenericModel class.
     """
 
     prefix_keys_in_state_dict = {
-        "^qformer.": "model.",
-        "^query_tokens": "model.",
-        "^vision_model.": "model.",
-        "^(?!model\.llama\.|model\.language_projection\.|model\.qformer\.|model\.query_tokens|model\.vision_model\.)model\.": "model.llama.",
-        "^lm_head.": "model.llama.",
+        "^qformer.": "base_model.",
+        "^query_tokens": "base_model.",
+        "^vision_model.": "base_model.",
+        "^model.language_projection.": "base_",
+        "^(?!model\.language_projection\.)model\.": "base_model.llama.",
+        "^lm_head.": "base_model.llama.",
     }
 
     def __init__(
         self,
         blip2_config_path: str,
         llama_config_path: str,
+        quant_config_path: Optional[str] = None,
         pad_token_id: Optional[int] = 0,
         freeze_vision_model: Optional[bool] = True,
         freeze_qformer_model: Optional[bool] = True,
         freeze_llama_model: Optional[bool] = True,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
@@ -262,29 +269,35 @@
             gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
         """
         super().__init__()
         self.blip2_config = Blip2Config.from_json_file(blip2_config_path)
         self.blip2_config.pad_token_id = pad_token_id
         self.llama_config = LlamaConfig.from_json_file(llama_config_path)
         self.llama_config.gradient_checkpointing = gradient_checkpointing
-        self.model = MiniGPT4Blip2LlamaModel(self.blip2_config, self.llama_config)
+        self.base_model = MiniGPT4Blip2LlamaModel(self.blip2_config, self.llama_config)
         self.init_weights()
 
         if freeze_vision_model:
-            for param in self.model.vision_model.parameters():
+            for param in self.base_model.vision_model.parameters():
                 param.requires_grad = False
 
         if freeze_qformer_model:
-            for param in self.model.qformer.parameters():
+            for param in self.base_model.qformer.parameters():
                 param.requires_grad = False
 
         if freeze_llama_model:
-            for param in self.model.llama.parameters():
+            for param in self.base_model.llama.parameters():
                 param.requires_grad = False
 
+        if quant_config_path is not None:
+            self.quant_config = QuantizationConfig.from_json_file(quant_config_path)
+            self.quantize(
+                self.quant_config, ignore_modules=["language_projection", "lm_head"]
+            )
+
     def forward(
         self,
         pixel_values: torch.Tensor,
         prefix_input_ids: torch.Tensor,
         suffix_input_ids: torch.Tensor,
         decoder_input_ids: torch.Tensor,
         prefix_attention_mask: Optional[torch.Tensor] = None,
@@ -302,15 +315,15 @@
             prefix_attention_mask (torch.Tensor, optional): The attention mask for the prefix tokens.
             suffix_attention_mask (torch.Tensor, optional): The attention mask for the suffix tokens.
             decoder_attention_mask (torch.Tensor, optional): The attention mask for the decoder tokens.
 
         Returns:
             logits: The output logits.
         """
-        outputs = self.model(
+        outputs = self.base_model(
             pixel_values=pixel_values,
             prefix_input_ids=prefix_input_ids,
             suffix_input_ids=suffix_input_ids,
             decoder_input_ids=decoder_input_ids,
             prefix_attention_mask=prefix_attention_mask,
             suffix_attention_mask=suffix_attention_mask,
             decoder_attention_mask=decoder_attention_mask,
@@ -366,15 +379,15 @@
             temperature (float, optional): The temperature value for sampling. Defaults to 1.0.
             top_k (int, optional): The value for top-k sampling. Defaults to 50.
             top_p (float, optional): The value for top-p sampling. Defaults to 1.0.
 
         Returns:
             outputs (GenericOutputs): The generated sequences and their scores.
         """
-        outputs = self.model.generate(
+        outputs = self.base_model.generate(
             pixel_values=pixel_values,
             prefix_input_ids=prefix_input_ids,
             suffix_input_ids=suffix_input_ids,
             max_length=max_gen_seq_length,
             min_length=min_gen_seq_length,
             num_beams=num_beams,
             do_sample=do_sample,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/minigpt4/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/minigpt4/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/modeling_ema.py` & `unitorch-0.0.0.7/src/unitorch/models/modeling_ema.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/mt5/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/mt5/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/peft/__init__.py` & `unitorch-0.0.0.7/src/unitorch/models/peft/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import os
 import warnings
 import logging
 import torch
+import torch.nn as nn
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from peft import (
     PeftConfig,
     PeftType,
     PromptLearningConfig,
     PeftModelForSequenceClassification,
 )
 from unitorch.utils import replace
+from unitorch.models import CheckpointMixin
 
 
 @replace(PeftModelForSequenceClassification)
 class PeftModelForSequenceClassification(PeftModelForSequenceClassification):
     def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
         super().__init__(model, peft_config, adapter_name)
 
@@ -86,15 +88,15 @@
                 inputs_embeds = self.word_embeddings(input_ids)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
             inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
             return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
 
 
-class PeftCheckpointMixin:
+class PeftCheckpointMixin(CheckpointMixin):
     checkpoint_name = "pytorch_peft_model.bin"
 
     def save_checkpoint(
         self,
         ckpt_dir: str,
         weight_name: str = None,
         **kwargs,
@@ -141,23 +143,64 @@
         state_dict = torch.load(weight_path, map_location="cpu")
         self.load_state_dict(state_dict, strict=False)
         logging.info(
             f"{type(self).__name__} model load weight from checkpoint {weight_path}"
         )
 
 
-from unitorch.models.peft.modeling_bloom_adalora import (
-    BloomAdaLoraForClassification,
-    BloomAdaLoraForGeneration,
-)
+class GenericPeftModel(nn.Module, PeftCheckpointMixin):
+    def __init__(self):
+        super().__init__()
+        pass
+
+    def _init_weights(self, module):
+        """
+        Initialize the weights of the given module.
+
+        Args:
+            module (nn.Module): The module to initialize weights for.
+        """
+        if isinstance(module, (nn.Linear, nn.Embedding)):
+            module.weight.data.normal_(mean=0.0, std=0.02)
+
+        if isinstance(module, nn.LayerNorm):
+            module.bias.data.zero_()
+            module.weight.data.fill_(1.0)
+
+        if isinstance(module, nn.Linear) and module.bias is not None:
+            module.bias.data.zero_()
+
+    def init_weights(self):
+        """
+        Initialize the weights of the model.
+        """
+        self.apply(self._init_weights)
+
+    @property
+    def dtype(self) -> torch.dtype:
+        """
+        Returns the data type of the model's parameters.
+
+        Returns:
+            torch.dtype: The data type of the model's parameters.
+        """
+        return next(self.parameters()).dtype
+
+    @property
+    def device(self):
+        """
+        Returns the device of the model's parameters.
+
+        Returns:
+            torch.device: The device of the model's parameters.
+        """
+        return next(self.parameters()).device
+
+
 from unitorch.models.peft.modeling_bloom_lora import (
     BloomLoraForClassification,
     BloomLoraForGeneration,
 )
-from unitorch.models.peft.modeling_llama_adalora import (
-    LlamaAdaLoraForClassification,
-    LlamaAdaLoraForGeneration,
-)
 from unitorch.models.peft.modeling_llama_lora import (
     LlamaLoraForClassification,
     LlamaLoraForGeneration,
 )
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_adalora.py` & `unitorch-0.0.0.7/src/unitorch/models/peft/modeling_bloom_lora.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,46 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import json
 import torch
 import torch.nn as nn
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from peft import AdaLoraConfig, PeftModelForCausalLM
+from peft import LoraConfig, PeftModelForCausalLM
 from transformers import BloomModel, BloomConfig, BloomForCausalLM
 from unitorch.models import GenericModel, GenericOutputs
-from unitorch.models.peft import PeftModelForSequenceClassification, PeftCheckpointMixin
+from unitorch.models.peft import PeftModelForSequenceClassification, GenericPeftModel
 
 
-class BloomAdaLoraForClassification(GenericModel, PeftCheckpointMixin):
-    """
-    BloomAdaLora model for classification tasks.
-    """
-
+class BloomLoraForClassification(GenericPeftModel):
     prefix_keys_in_state_dict = {
         "^(?!peft_model\.base_model\.model\.).*": "peft_model.base_model.model."
     }
 
     def __init__(
         self,
         config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
         num_classes: Optional[int] = 1,
         hidden_dropout_prob: Optional[float] = 0.1,
         gradient_checkpointing: Optional[bool] = False,
     ):
         super().__init__()
         self.config = BloomConfig.from_json_file(config_path)
         self.config.gradient_checkpointing = gradient_checkpointing
-        self.peft_config = AdaLoraConfig(
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
+        self.peft_config = LoraConfig(
+            r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
         )
         self.peft_model = PeftModelForSequenceClassification(
             BloomModel(self.config), self.peft_config
         )
         self.dropout = nn.Dropout(hidden_dropout_prob)
         self.classifier = nn.Linear(self.config.hidden_size, num_classes)
         self.init_weights()
@@ -83,52 +69,45 @@
         )[0]
         pooled_output = outputs[:, -1]
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         return logits
 
 
-class BloomAdaLoraForGeneration(GenericModel, PeftCheckpointMixin):
-    """
-    BloomAdaLora model for generation tasks.
-    """
-
+class BloomLoraForGeneration(GenericPeftModel):
     prefix_keys_in_state_dict = {
         "^(?!peft_model\.base_model\.model\.).*": "peft_model.base_model.model.transformer."
     }
 
     def __init__(
         self,
         config_path: str,
-        target_r: Optional[int] = 8,
-        init_r: Optional[int] = 12,
-        tinit: Optional[int] = 0,
-        tfinal: Optional[int] = 0,
-        deltaT: Optional[int] = 1,
-        beta1: Optional[float] = 0.85,
-        beta2: Optional[float] = 0.85,
-        orth_reg_weight: Optional[float] = 0.5,
-        total_step: Optional[int] = None,
-        rank_pattern: Optional[dict] = None,
+        lora_r: Optional[int] = 16,
+        lora_alpha: Optional[int] = 32,
+        lora_dropout: Optional[float] = 0.05,
+        fan_in_fan_out: Optional[bool] = True,
+        target_modules: Optional[Union[List[str], str]] = ["query_key_value"],
         gradient_checkpointing: Optional[bool] = False,
     ):
+        """
+        Bloom Loar model for text generation tasks.
+
+        Args:
+            config_path (str): Path to the model configuration file.
+            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
+        """
         super().__init__()
         self.config = BloomConfig.from_json_file(config_path)
         self.config.gradient_checkpointing = gradient_checkpointing
-        self.peft_config = AdaLoraConfig(
-            target_r=target_r,
-            init_r=init_r,
-            tinit=tinit,
-            tfinal=tfinal,
-            deltaT=deltaT,
-            beta1=beta1,
-            beta2=beta2,
-            orth_reg_weight=orth_reg_weight,
-            total_step=total_step,
-            rank_pattern=rank_pattern,
+        self.peft_config = LoraConfig(
+            r=lora_r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            fan_in_fan_out=fan_in_fan_out,
+            target_modules=target_modules,
         )
         self.peft_model = PeftModelForCausalLM(
             BloomForCausalLM(self.config), self.peft_config
         )
         self.init_weights()
 
     def forward(
```

### Comparing `unitorch-0.0.0.6/src/unitorch/models/pegasus/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/pegasus/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/processing_utils.py` & `unitorch-0.0.0.7/src/unitorch/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/prophetnet/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/prophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/prophetnet/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/prophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/roberta/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/roberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/swin/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/swin/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/t5/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/t5/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/visualbert/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/visualbert/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/vit/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/vit/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/xpegasus/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/xpegasus/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/xprophetnet/modeling.py` & `unitorch-0.0.0.7/src/unitorch/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/models/xprophetnet/processing.py` & `unitorch-0.0.0.7/src/unitorch/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/modules/classifier.py` & `unitorch-0.0.0.7/src/unitorch/modules/classifier.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/modules/replace/beam_search_v2.py` & `unitorch-0.0.0.7/src/unitorch/modules/replace/beam_search_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/modules/replace/datasets_v2.py` & `unitorch-0.0.0.7/src/unitorch/modules/replace/datasets_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/modules/replace/hf_hub_v2.py` & `unitorch-0.0.0.7/src/unitorch/modules/replace/hf_hub_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/modules/timm.py` & `unitorch-0.0.0.7/src/unitorch/modules/timm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/ops/dyhead.py` & `unitorch-0.0.0.7/src/unitorch/ops/dyhead.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/ops/ngram_repeat_block.py` & `unitorch-0.0.0.7/src/unitorch/ops/ngram_repeat_block.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/optim/lion.py` & `unitorch-0.0.0.7/src/unitorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/scheduler/warmup.py` & `unitorch-0.0.0.7/src/unitorch/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/score/__init__.py` & `unitorch-0.0.0.7/src/unitorch/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/score/bleu.py` & `unitorch-0.0.0.7/src/unitorch/score/bleu.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/score/map.py` & `unitorch-0.0.0.7/src/unitorch/score/map.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/score/rouge.py` & `unitorch-0.0.0.7/src/unitorch/score/rouge.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/__init__.py` & `unitorch-0.0.0.7/src/unitorch/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     is_deepspeed_available,
     is_accelerate_available,
     is_megatron_available,
     is_fastapi_available,
     is_diffusers_available,
     is_torch_available,
     is_torch2_available,
+    is_bitsandbytes_available,
 )
 from unitorch.utils.io import GenericWriter, IOProcess, PostProcess, GENERATE_FINISHED
 from unitorch.utils.torch_utils import get_local_rank
 from unitorch.utils.torch_utils import (
     DistributedSkipSampler,
     RandomSkipSampler,
     SequentialSkipSampler,
```

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/decorators.py` & `unitorch-0.0.0.7/src/unitorch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/functional.py` & `unitorch-0.0.0.7/src/unitorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/image_utils.py` & `unitorch-0.0.0.7/src/unitorch/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/import_utils.py` & `unitorch-0.0.0.7/src/unitorch/utils/import_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,7 +84,20 @@
 
 def is_torch_available():
     return _torch_available or is_offline_debug_mode()
 
 
 def is_torch2_available():
     return _torch_available and _torch_version >= "2.0.0"
+
+
+# bitsandbytes
+_bitsandbytes_available = importlib.util.find_spec("bitsandbytes") is not None
+try:
+    _bitsandbytes_version = importlib_metadata.version("bitsandbytes")
+    logging.debug(f"Successfully imported bitsandbytes version {_bitsandbytes_version}")
+except importlib_metadata.PackageNotFoundError:
+    _bitsandbytes_available = False
+
+
+def is_bitsandbytes_available():
+    return _bitsandbytes_available or is_offline_debug_mode()
```

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/io.py` & `unitorch-0.0.0.7/src/unitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/palette.py` & `unitorch-0.0.0.7/src/unitorch/utils/palette.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch/utils/torch_utils.py` & `unitorch-0.0.0.7/src/unitorch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/src/unitorch.egg-info/PKG-INFO` & `unitorch-0.0.0.7/src/unitorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
-Provides-Extra: accelerate
-Provides-Extra: chatglm
+Provides-Extra: quantization
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.6/src/unitorch.egg-info/SOURCES.txt` & `unitorch-0.0.0.7/src/unitorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,30 @@
 examples/configs/diffusion/stable-v2.1.ini
 examples/configs/diffusion/stable-v2.ini
 examples/configs/diffusion/controlnet/canny.ini
 examples/configs/generation/bart.ini
 examples/configs/generation/bloom.ini
 examples/configs/generation/chatglm.ini
 examples/configs/generation/llama.ini
+examples/configs/generation/llama.quant.ini
 examples/configs/generation/mbart.ini
 examples/configs/generation/mt5.ini
 examples/configs/generation/pegasus.ini
 examples/configs/generation/t5.ini
 examples/configs/generation/xpegasus.ini
 examples/configs/generation/xprophetnet.ini
 examples/configs/generation/lora/bloom.ini
 examples/configs/generation/lora/bloom_ds.ini
 examples/configs/generation/lora/llama.ini
+examples/configs/generation/lora/llama.quant.ini
 examples/configs/generation/lora/llama_ds.ini
+examples/configs/generation/lora/llama_ds.quant.ini
 examples/configs/pretrain/clip.ini
+examples/configs/quantization/4bit.json
+examples/configs/quantization/8bit.json
 examples/configs/services/zip_image/config.ini
 examples/configs/services/zip_image/config_v2.ini
 examples/hub/caption/blip.ini
 examples/hub/classification/bert.ini
 examples/hub/classification/clip.ini
 examples/hub/generation/bart.ini
 examples/hub/generation/llama.ini
@@ -95,17 +100,14 @@
 src/unitorch/cli/models/bert/processing.py
 src/unitorch/cli/models/blip/__init__.py
 src/unitorch/cli/models/blip/modeling.py
 src/unitorch/cli/models/blip/processing.py
 src/unitorch/cli/models/bloom/__init__.py
 src/unitorch/cli/models/bloom/modeling.py
 src/unitorch/cli/models/bloom/processing.py
-src/unitorch/cli/models/chatglm/__init__.py
-src/unitorch/cli/models/chatglm/modeling.py
-src/unitorch/cli/models/chatglm/processing.py
 src/unitorch/cli/models/clip/__init__.py
 src/unitorch/cli/models/clip/modeling.py
 src/unitorch/cli/models/clip/processing.py
 src/unitorch/cli/models/deberta/__init__.py
 src/unitorch/cli/models/deberta/modeling.py
 src/unitorch/cli/models/deberta/modeling_v2.py
 src/unitorch/cli/models/deberta/processing.py
@@ -181,14 +183,15 @@
 src/unitorch/datasets/hf.py
 src/unitorch/loss/__init__.py
 src/unitorch/loss/prophetnet.py
 src/unitorch/loss/ranking.py
 src/unitorch/models/__init__.py
 src/unitorch/models/modeling_ema.py
 src/unitorch/models/processing_utils.py
+src/unitorch/models/quantization.py
 src/unitorch/models/bart/__init__.py
 src/unitorch/models/bart/modeling.py
 src/unitorch/models/bart/processing.py
 src/unitorch/models/beit/__init__.py
 src/unitorch/models/beit/modeling.py
 src/unitorch/models/beit/processing.py
 src/unitorch/models/bert/__init__.py
@@ -232,17 +235,15 @@
 src/unitorch/models/minigpt4/__init__.py
 src/unitorch/models/minigpt4/modeling.py
 src/unitorch/models/minigpt4/processing.py
 src/unitorch/models/mt5/__init__.py
 src/unitorch/models/mt5/modeling.py
 src/unitorch/models/mt5/processing.py
 src/unitorch/models/peft/__init__.py
-src/unitorch/models/peft/modeling_bloom_adalora.py
 src/unitorch/models/peft/modeling_bloom_lora.py
-src/unitorch/models/peft/modeling_llama_adalora.py
 src/unitorch/models/peft/modeling_llama_lora.py
 src/unitorch/models/peft/processing.py
 src/unitorch/models/pegasus/__init__.py
 src/unitorch/models/pegasus/modeling.py
 src/unitorch/models/pegasus/processing.py
 src/unitorch/models/prophetnet/__init__.py
 src/unitorch/models/prophetnet/modeling.py
```

### Comparing `unitorch-0.0.0.6/wiki/cli/models/blip.md` & `unitorch-0.0.0.7/wiki/cli/models/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/bloom.md` & `unitorch-0.0.0.7/wiki/cli/models/bloom.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/chatglm.md` & `unitorch-0.0.0.7/wiki/cli/models/chatglm.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/clip.md` & `unitorch-0.0.0.7/wiki/cli/models/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/deberta.md` & `unitorch-0.0.0.7/wiki/cli/models/deberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/llama.md` & `unitorch-0.0.0.7/wiki/cli/models/llama.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/peft.md` & `unitorch-0.0.0.7/wiki/cli/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/visualbert.md` & `unitorch-0.0.0.7/wiki/cli/models/visualbert.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/models/xlm_roberta.md` & `unitorch-0.0.0.7/wiki/cli/models/xlm_roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/cli/postprocess.md` & `unitorch-0.0.0.7/wiki/cli/postprocess.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/configuration.md` & `unitorch-0.0.0.7/wiki/configuration.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/caption/blip.md` & `unitorch-0.0.0.7/wiki/examples/caption/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/classification/clip.md` & `unitorch-0.0.0.7/wiki/examples/classification/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/classification/roberta.md` & `unitorch-0.0.0.7/wiki/examples/classification/roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/classification/swin.md` & `unitorch-0.0.0.7/wiki/examples/classification/swin.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/generation/bart.md` & `unitorch-0.0.0.7/wiki/examples/generation/bart.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/examples/service/zip_image.md` & `unitorch-0.0.0.7/wiki/examples/service/zip_image.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/index.md` & `unitorch-0.0.0.7/wiki/index.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/installation.md` & `unitorch-0.0.0.7/wiki/installation.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/models/peft.md` & `unitorch-0.0.0.7/wiki/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.6/wiki/overview.md` & `unitorch-0.0.0.7/wiki/overview.md`

 * *Files identical despite different names*

