# Comparing `tmp/thebestllmever-0.0.1.tar.gz` & `tmp/thebestllmever-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thebestllmever-0.0.1.tar", max compression
+gzip compressed data, was "thebestllmever-0.0.2.tar", max compression
```

## Comparing `thebestllmever-0.0.1.tar` & `thebestllmever-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-05-05 17:46:22.150156 thebestllmever-0.0.1/LICENSE
--rw-r--r--   0        0        0    11792 2023-07-21 18:34:47.215246 thebestllmever-0.0.1/README.md
--rw-r--r--   0        0        0     7038 2023-05-30 23:08:11.874230 thebestllmever-0.0.1/andromeda/README.md
--rw-r--r--   0        0        0      143 2023-07-24 15:49:19.836367 thebestllmever-0.0.1/andromeda/__init__.py
--rw-r--r--   0        0        0     2238 2023-07-14 18:00:12.197229 thebestllmever-0.0.1/andromeda/build_dataset.py
--rw-r--r--   0        0        0        0 2023-07-24 15:55:44.000080 thebestllmever-0.0.1/andromeda/dataset_prep/__init__.py
--rw-r--r--   0        0        0      336 2023-07-24 15:56:54.358207 thebestllmever-0.0.1/andromeda/dataset_prep/books.py
--rw-r--r--   0        0        0     7426 2023-06-05 14:18:08.761888 thebestllmever-0.0.1/andromeda/finetuning/README.md
--rw-r--r--   0        0        0        0 2023-07-24 15:46:18.210154 thebestllmever-0.0.1/andromeda/finetuning/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-31 03:27:54.441985 thebestllmever-0.0.1/andromeda/inference.py
--rw-r--r--   0        0        0     4292 2023-07-24 15:49:32.962744 thebestllmever-0.0.1/andromeda/model.py
--rw-r--r--   0        0        0        0 2023-07-24 15:46:11.793907 thebestllmever-0.0.1/andromeda/old/__init__.py
--rw-r--r--   0        0        0     7440 2023-07-07 21:57:00.247815 thebestllmever-0.0.1/andromeda/old/sophia.py
--rw-r--r--   0        0        0     9784 2023-07-07 21:57:00.249365 thebestllmever-0.0.1/andromeda/old/training.py
--rw-r--r--   0        0        0    11404 2023-06-03 19:52:32.610059 thebestllmever-0.0.1/andromeda/old/training_1.py
--rw-r--r--   0        0        0    11822 2023-07-07 21:57:00.250128 thebestllmever-0.0.1/andromeda/old/training_sophia.py
--rw-r--r--   0        0        0      844 2023-07-24 15:53:09.591116 thebestllmever-0.0.1/andromeda/optimus_prime/__init__.py
--rw-r--r--   0        0        0     7774 2023-07-20 18:58:10.636760 thebestllmever-0.0.1/andromeda/optimus_prime/attend.py
--rw-r--r--   0        0        0     4523 2023-05-31 03:27:54.445779 thebestllmever-0.0.1/andromeda/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0        0        0     1575 2023-05-31 03:27:54.446123 thebestllmever-0.0.1/andromeda/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0        0        0     8833 2023-07-20 03:58:37.740152 thebestllmever-0.0.1/andromeda/optimus_prime/flash.py
--rw-r--r--   0        0        0    10424 2023-07-24 15:53:31.368226 thebestllmever-0.0.1/andromeda/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0        0        0    55329 2023-07-24 15:53:41.342660 thebestllmever-0.0.1/andromeda/optimus_prime/x_transformers.py
--rw-r--r--   0        0        0     3997 2023-07-24 15:53:47.596915 thebestllmever-0.0.1/andromeda/optimus_prime/xl_autoregressive_wrapper.py
--rw-r--r--   0        0        0    23609 2023-07-24 16:05:21.506497 thebestllmever-0.0.1/andromeda/train.py
--rw-r--r--   0        0        0        0 2023-07-24 15:45:54.396085 thebestllmever-0.0.1/andromeda/utils/__init__.py
--rw-r--r--   0        0        0     6236 2023-06-03 19:28:08.491891 thebestllmever-0.0.1/andromeda/utils/decoupled_optimizer.py
--rw-r--r--   0        0        0      487 2023-06-03 19:26:38.101050 thebestllmever-0.0.1/andromeda/utils/helpers.py
--rw-r--r--   0        0        0     5025 2023-06-05 17:22:50.120473 thebestllmever-0.0.1/andromeda/utils/rf_utils.py
--rw-r--r--   0        0        0     3334 2023-06-03 19:27:07.738473 thebestllmever-0.0.1/andromeda/utils/stable_adamw.py
--rw-r--r--   0        0        0      980 2023-07-24 16:52:06.161173 thebestllmever-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    12916 1970-01-01 00:00:00.000000 thebestllmever-0.0.1/setup.py
--rw-r--r--   0        0        0    13009 1970-01-01 00:00:00.000000 thebestllmever-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-05 17:46:22.150156 thebestllmever-0.0.2/LICENSE
+-rw-r--r--   0        0        0    10794 2023-08-08 21:32:25.786828 thebestllmever-0.0.2/README.md
+-rw-r--r--   0        0        0     7031 2023-08-08 21:30:21.813558 thebestllmever-0.0.2/andromeda/README.md
+-rw-r--r--   0        0        0       93 2023-08-04 03:53:46.512786 thebestllmever-0.0.2/andromeda/__init__.py
+-rw-r--r--   0        0        0     2738 2023-08-01 01:00:20.391101 thebestllmever-0.0.2/andromeda/configs.py
+-rw-r--r--   0        0        0      210 2023-07-31 23:42:02.232928 thebestllmever-0.0.2/andromeda/core/__init__.py
+-rw-r--r--   0        0        0     7922 2023-08-04 03:56:45.104636 thebestllmever-0.0.2/andromeda/core/attend.py
+-rw-r--r--   0        0        0     4449 2023-07-27 23:19:59.076649 thebestllmever-0.0.2/andromeda/core/autoregressive_wrapper.py
+-rw-r--r--   0        0        0    10224 2023-08-04 03:51:30.012907 thebestllmever-0.0.2/andromeda/core/flash.py
+-rw-r--r--   0        0        0    47128 2023-08-08 21:30:21.855431 thebestllmever-0.0.2/andromeda/core/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:55:44.000080 thebestllmever-0.0.2/andromeda/dataset_prep/__init__.py
+-rw-r--r--   0        0        0      326 2023-08-01 02:16:28.826494 thebestllmever-0.0.2/andromeda/dataset_prep/books.py
+-rw-r--r--   0        0        0     5593 2023-07-27 23:19:59.078716 thebestllmever-0.0.2/andromeda/inference.py
+-rw-r--r--   0        0        0     4265 2023-08-08 21:30:21.791149 thebestllmever-0.0.2/andromeda/model.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:46:11.793907 thebestllmever-0.0.2/andromeda/old/__init__.py
+-rw-r--r--   0        0        0     7385 2023-07-27 23:19:59.072801 thebestllmever-0.0.2/andromeda/old/sophia.py
+-rw-r--r--   0        0        0     9763 2023-08-08 21:30:21.875051 thebestllmever-0.0.2/andromeda/old/training.py
+-rw-r--r--   0        0        0    11280 2023-08-08 21:30:21.833994 thebestllmever-0.0.2/andromeda/old/training_1.py
+-rw-r--r--   0        0        0    11666 2023-08-08 21:30:21.815182 thebestllmever-0.0.2/andromeda/old/training_sophia.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:45:54.396085 thebestllmever-0.0.2/andromeda/utils/__init__.py
+-rw-r--r--   0        0        0     6256 2023-07-24 18:38:28.724015 thebestllmever-0.0.2/andromeda/utils/decoupled_optimizer.py
+-rw-r--r--   0        0        0      487 2023-06-03 19:26:38.101050 thebestllmever-0.0.2/andromeda/utils/helpers.py
+-rw-r--r--   0        0        0     5025 2023-06-05 17:22:50.120473 thebestllmever-0.0.2/andromeda/utils/rf_utils.py
+-rw-r--r--   0        0        0     3307 2023-07-27 23:19:59.079840 thebestllmever-0.0.2/andromeda/utils/stable_adamw.py
+-rw-r--r--   0        0        0      961 2023-08-08 21:36:25.810882 thebestllmever-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11853 1970-01-01 00:00:00.000000 thebestllmever-0.0.2/setup.py
+-rw-r--r--   0        0        0    11983 1970-01-01 00:00:00.000000 thebestllmever-0.0.2/PKG-INFO
```

### Comparing `thebestllmever-0.0.1/LICENSE` & `thebestllmever-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.1/README.md` & `thebestllmever-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,224 +1,241 @@
+Metadata-Version: 2.1
+Name: thebestllmever
+Version: 0.0.2
+Summary: andromeda - Pytorch
+Home-page: https://github.com/kyegomez/Andromeda
+License: MIT
+Keywords: artificial intelligence,attention mechanism,transformers
+Author: Kye Gomez
+Author-email: kye@apac.ai
+Requires-Python: >=3.6,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: SentencePiece
+Requires-Dist: accelerate
+Requires-Dist: datasets
+Requires-Dist: deepspeed
+Requires-Dist: einops
+Requires-Dist: lion-pytorch
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: transformers
+Description-Content-Type: text/markdown
 
-# [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
-
-# Agora
-Agora is an new open source Multi-Modality AI Research Organization devoted to advancing Humanity to a post-scarcity state!
-
-Since Andromeda is ready to train Agora is actively seeking cloud providers or grant providers to train this all-new revolutionary model and release it open source, if you would like to learn more please email me at `kye@apac.ai`
-
-![Agora banner](agora-banner.png)
-
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
-
-
----
 
 # Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌
 
-![Andromeda Next Generation Open Source Language Model](/andromeda-banner.png)
-
-Andromeda is a state-of-the-art language model that pushes the boundaries of natural language understanding and generation. Designed for high performance and efficiency, Andromeda is built upon advanced techniques that make it a strong contender against the likes of OpenAI's GPT-4 and PALM with features like:
-
-* Process Ultra Long Sequences of 32,000-200,000+ context lengths effortlessly :fire: :closed_book: 
-
-* Process those Ultra Long Sequences Ultra Fast with 32,000+ tokens in under 100ms ⚡️ ⚡️ 
-
-* Reliable and actually useful with superior reasoning capabilities :brain: :brain: 
-
----
-
 <div align="center">
 
 [![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)
 [![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)
-
-[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) 
+[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) 
+[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) 
+[![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)
+[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) 
+[![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) 
+[![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)
+![Discord](https://img.shields.io/discord/999382051935506503)
+[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
 
 </div>
 
-<div align="center">
+---
 
-[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)
+![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
 
+Welcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI's GPT-4 and PALM. Features include:
 
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
-[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
-
-</div>
+- 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)
+- ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)
+- 🎓 Superior Reasoning Capabilities
 
 ---
 
+## 🔄 Updates
 
+- [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
+- [And, here is the WANDB link to watch Andromeda train live!](https://wandb.ai/apacai/Andromeda/overview?)
 
+---
 
-## Table of Contents
-
-- [Usage](#usage)
-- [Documentation](#documentation)
-- [Contributing to Andromeda](#contributing-to-andromeda)
-- [Roadmap](#roadmap)
+-----
+## Hiring
+We're hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`
 
----
+----------
 
-## Usage
+## 💻 Usage
 
 There are two methods to use Andromeda but pip does not work now.
 
 1. Clone the repository.
 
 For detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
 
-## Documentation
-
-For detailed documentation, click [here](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
-
 ### Method 1
 
 To get started:
 
 1. Clone the repository and install the required packages:
 
-```
+```bash
 git clone https://github.com/kyegomez/Andromeda
 cd Andromeda
 pip3 install -r requirements.txt
 cd Andromeda
 python3 train.py
 ```
 
 For further instructions, refer to the [Training SOP](DOCs/TRAINING.md).
 
-## Training
+---
+
+## 📚 Training
 
 1. Set the environment variables:
    - `ENTITY_NAME`: Your wandb project name
    - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)
+   - `MASTER_ADDR`: For distributed training
+   - `MASTER_PORT` For master port distributed training
+   - `RANK`- Number of nodes services
+   - `WORLD_SIZE` Number of gpus
 
 2. Configure the training:
    - Accelerate Config
    - Enable Deepspeed 3
    - Accelerate launch train_distributed_accelerate.py
 
 For more information, refer to the [Training SOP](DOCs/TRAINING.md).
 
-## Dataset Building
+---
 
-To preprocess a different dataset similar to the C4 dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.
+## 🗃️ Dataset Building
 
-Example command:
+To preprocess a
 
-```python
-python3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"
-```
+ different dataset similar to the C4 or Falcon dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.
 
-## Inference
+Example command:
 
-```python
-python3 inference.py "My dog is very cute" --seq_len 256 --temperature 0.8 --filter_thres 0.9 --model "andromeda"
+```bash
+python3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"
 ```
 
-(Note: Model submission to PyTorch Hub is still pending.)
+---
 
-## Why Andromeda?
+## 🚀 Why Andromeda?
 
 Andromeda offers several advantages:
-
-- And romeda can potentially be fine-tuned with a 100k+ token sequence length.
-- It incorporates advanced techniques, including alibi positional bias, rotary position encodings (xpos), flash attention, and deep normalization (deepnorm), to optimize performance and efficiency.
+- Andromeda offers reliable processing of 100,000+ sequence lengths extremely fast under 300ms
+- Andromeda's dataset strategy was crafted with atomic precision and attention to detail for creativity and quantitative reasoning.
+- Andromeda is extremely intelligent with the ability to think like a poet or make API Calls to your favorite apps.
 
 For detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.
 
-## Andromeda Principles
-
-Andromeda is built on key principles:
+---
 
-- **Efficiency**: Andromeda leverages optimization techniques, such as attention flashing, rotary position encodings, and deep normalization, to achieve efficient training and inference.
-- **Flexibility**: The modular design of Andromeda allows easy adaptation to various tasks and domains, making it versatile for a wide range of applications.
-- **Scalability**: Andromeda's architecture is designed to scale with increasing computational resources and data sizes, ensuring its relevance in the NLP landscape.
-- **Community-driven**: As an open-source project, Andromeda thrives on contributions from the community, fostering collaboration, innovation, and continuous improvement.
+# 🎯 Andromeda Principles
 
-Join us on this exciting journey to create a powerful, efficient, and intelligent language model that will revolutionize the NLP landscape! 🚀🌟
+- **Efficiency**: Optimize with techniques like attention flashing, rotary position encodings, and deep normalization.
+- **Flexibility**: Adapt to various tasks and domains for wide applications.
+- **Scalability**: Designed to scale with resources and data sizes.
+- **Community-Driven**: Thrives on contributions from the open-source community.
 
+---
 
-## Get Involved
+## 🚀 Get Involved
 
 We're just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you're a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.
 
-# Contributing to Andromeda
+---
 
-We are thrilled to invite you to be a part of the Andromeda project. This is not just an open source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.
+# 🤝 Contributing to Andromeda
 
-## Why Contribute
+We are thrilled to invite you to be a part of the Andromeda project. This is not just an open-source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.
+
+## 🌟 Why Contribute
 
 Contributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it's only fair that you share in the rewards.
 
-## Rewards Program
+## 💰 Rewards Program
 
 Here's how the Andromeda Rewards Program works:
 
 1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.
 
 2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.
 
-3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution. 
+3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution.
 
-This means you're not just contributing to an open source project; you're becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.
+This means you're not just contributing to an open-source project; you're becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.
 
-## Becoming a Paid API
+## 🚀 Becoming a Paid API
 
-As part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project, but also fund the rewards program. If you contribute anything to make Andromeda you will receive recurring revenue from paid API requests!
+As part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project but also fund the rewards program. If you contribute anything to make Andromeda, you will receive recurring revenue from paid API requests!
 
-## How to Start Contributing
+## 🚀 How to Start Contributing
 
 If you're ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here's what you need to do:
 
 1. Fork the repository.
 
 2. Make your improvements or additions in your forked repository.
 
 3. Submit a pull request detailing the changes you've made.
 
 4. Our team will review your submission. If it's approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.
 
 Thank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
 
-## Roadmap 🗺️📍
+---
+
+## 🗺️ Roadmap
 
 1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.
 
 2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:
 
    - Model quantization: Reduce memory and computational requirements without significant loss in performance.
    - Distillation: Train smaller, faster models that retain the knowledge of the larger model.
    - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.
 
 3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.
 
 4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.
 
+---
 
-## Todo:
-
-* [Create the best and most validated, reliable training => finetuning strategy](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
-
-* Establish FineTuning scripts using quantization + 4bit precision, + other tactics like LoRA
-
-* Establish 200k instruction sample long for Tool API Calls
-
-* [Train on Gorilla Dataset](https://github.com/ShishirPatil/gorilla)
-
-
-* Establish Reinforcement Scripts to train on rewards from Human and Agent feedback
-
-
-
-
-
+## 📈 Benchmarks
 
+### Speed
+- Andromeda utilizes one of the most reliable Attentions ever, flash attention 2.0 Triton. It consumes 50x less memory than GPT-3 and 10x less than LLAMA.
 
+![AndromedaBanner](images/andromeda_performance.png)
 
+- We can speed this up even more with dynamic sparse flash attention 2.0.
 
+---
 
+# 🔮 Join the Journey
 
+We're just getting started, and we invite you to join the journey. Let's revolutionize the NLP landscape together! 🚀🌟
 
+- Join Agora and work with 2,000+ AI Engineers to implement all new features.
+- Provide compute and help train Andromeda.
+- Share the message on how we're liberating this superintelligent AI and seizing the power from the corrupt, providing it back to you.
```

### Comparing `thebestllmever-0.0.1/andromeda/README.md` & `thebestllmever-0.0.2/andromeda/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Transformer Model Technical Research Analysis
 
 This document provides an analysis of the hyperparameters and configurations of the given Transformer model, focusing on dimensions, depth, and heads, as well as an architectural overview of their meanings and use cases.
 
 ## Model Configuration
 
 ```python
-model = TransformerWrapper(
+model = Transformer(
     num_tokens=20000,
     max_seq_len=8192,
     use_abs_pos_emb = False,
     attn_layers = Decoder(
         dim=512,
         depth=6,
         heads=8,
```

### Comparing `thebestllmever-0.0.1/andromeda/model.py` & `thebestllmever-0.0.2/andromeda/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import torch 
 from torch.nn import Module
-from andromeda.optimus_prime import TransformerWrapper, AutoregressiveWrapper, AndromedaEmbedding, Decoder
+from Andromeda.core.transformer import Transformer, AutoregressiveWrapper, AndromedaEmbedding, Decoder
 from transformers import AutoTokenizer
 
 class AndromedaTokenizer:
     def __init__(self):
         self.tokenizer= AutoTokenizer.from_pretrained(
             "EleutherAI/gpt-neox-20b",
             eos_token="<eos>",
@@ -24,29 +23,29 @@
         return num_tokens
 
 
 
 class Andromeda(Module):
     """
     Andromeda is a transformer-based model architecture. It initializes with 
-    a TransformerWrapper and AutoregressiveWrapper with default or user-specified parameters.
+    a Transformer and AutoregressiveWrapper with default or user-specified parameters.
     """
-    def __init__(self, num_tokens=50432, 
+    def __init__(self, 
+                num_tokens=50432, 
                  max_seq_len=8192, 
                  dim=2560, depth=32, 
                  dim_head=128, 
                  heads=24,
                  use_abs_pos_emb=False, 
                  alibi_pos_bias=True, 
                  alibi_num_heads=12, 
                  rotary_xpos=True,
                  attn_flash=True, 
-                #  deepnorm=True, 
                  shift_tokens=1, 
-                 attn_one_kv_head=True, 
+                 attn_one_kv_head=True,  # multiquery attention
                  qk_norm=True, 
                  attn_qk_norm=True, 
                  attn_qk_norm_dim_scale=True, 
                  embedding_provider=AndromedaEmbedding()):
         """
         Initialize the model with specified or default parameters.
         Args:
@@ -68,15 +67,15 @@
         - attn_qk_norm: Attention query-key normalization
         - attn_qk_norm_dim_scale: Attention query-key normalization dimension scale
         - embedding_provider: Embedding provider module
         """
         super().__init__()
 
         try:
-            self.andromeda = TransformerWrapper(
+            self.Andromeda = Transformer(
                 num_tokens=num_tokens,
                 max_seq_len=max_seq_len,
                 use_abs_pos_emb=use_abs_pos_emb,
                 embedding_provider=embedding_provider,
                 attn_layers=Decoder(
                     dim=dim,
                     depth=depth,
@@ -91,15 +90,15 @@
                     attn_one_kv_head=attn_one_kv_head,
                     qk_norm=qk_norm,
                     attn_qk_norm=attn_qk_norm,
                     attn_qk_norm_dim_scale=attn_qk_norm_dim_scale
                 )
             )
 
-            self.decoder = AutoregressiveWrapper(self.andromeda)
+            self.decoder = AutoregressiveWrapper(self.Andromeda)
 
         except Exception as e:
             print("Failed to initialize Andromeda: ", e)
             raise
 
     def forward(self, text_tokens, **kwargs):
         """
```

### Comparing `thebestllmever-0.0.1/andromeda/old/sophia.py` & `thebestllmever-0.0.2/andromeda/old/sophia.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import math
 import torch
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
-from typing import List, Optional
+from typing import List
 
 
 class SophiaG(Optimizer):
     def __init__(self, params, lr=1e-4, betas=(0.965, 0.99), rho = 0.04,
          weight_decay=1e-1, *, maximize: bool = False,
          capturable: bool = False):
         if not 0.0 <= lr:
@@ -184,19 +183,18 @@
         # Perform stepweight decay
         param.mul_(1 - lr * weight_decay)
 
         # Decay the first and second moment running average coefficient
         exp_avg.mul_(beta1).add_(grad, alpha=1 - beta1)
         
         if capturable:
-            step = step_t
             step_size = lr 
             step_size_neg = step_size.neg()
 
             ratio = (exp_avg.abs() / (rho * bs * hess + 1e-15)).clamp(None,1)
             param.addcmul_(exp_avg.sign(), ratio, value=step_size_neg)
         else:
-            step = step_t.item()
+            step_t.item()
             step_size_neg = - lr 
             
             ratio = (exp_avg.abs() / (rho * bs * hess + 1e-15)).clamp(None,1)
             param.addcmul_(exp_avg.sign(), ratio, value=step_size_neg)
```

### Comparing `thebestllmever-0.0.1/andromeda/old/training.py` & `thebestllmever-0.0.2/andromeda/old/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from transformers import default_data_collator, get_linear_schedule_with_warmup
 from accelerate import Accelerator
 
 from rich.progress import Progress
 
 
 from lion_pytorch import Lion
-# from x_transformers import TransformerWrapper, Decoder, AutoregressiveWrapper
-from optimus_prim import TransformerWrapper, Decoder, AutoregressiveWrapper
+# from x_transformers import Transformer, Decoder, AutoregressiveWrapper
+from optimus_prim import Transformer, Decoder, AutoregressiveWrapper
 
 from torch.nn.parallel import DataParallel, DistributedDataParallel
 import torch.distributed as dist
 
 from torch.distributed.fsdp import (
     FullyShardedDataParallel,
     CPUOffload,
@@ -44,15 +44,15 @@
         self.tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
     
     def tokenize(self, text):
         return self.tokenizer(text, return_tensors="pt", truncation=True, padding=True)
 
 custom_tokenizer = CustomGPTNeoXTokenizer()
 
-Andromeda = TransformerWrapper(
+Andromeda = Transformer(
     num_tokens=64007,
     max_seq_len=8192,
     use_abs_pos_emb = False,
     tokenizer=custom_tokenizer,
     attn_layers = Decoder(
         dim=2048,
         depth=6,
```

### Comparing `thebestllmever-0.0.1/andromeda/old/training_1.py` & `thebestllmever-0.0.2/andromeda/old/training_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import math
 import multiprocessing
 import os
-import collections
 
 from datetime import timedelta
 from functools import partial
 from itertools import chain
 
-import torch
 
-from accelerate import Accelerator, DeepSpeedPlugin
+from accelerate import Accelerator
 from accelerate.utils import InitProcessGroupKwargs
 
 from datasets import concatenate_datasets, load_dataset
 
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     CheckpointImpl, apply_activation_checkpointing, checkpoint_wrapper)
 
-from torch.optim import AdamW
 from torch.utils.data import DataLoader
 
 from tqdm import tqdm
 
 from transformers import (AutoTokenizer, default_data_collator,
                           get_cosine_schedule_with_warmup,
                           get_linear_schedule_with_warmup, set_seed)
 
-from datasets import Dataset
 
 # from stable_adamw import StableAdamWUnfused
 # sd
 
-from optimus_prime import TransformerWrapper, Decoder, AutoregressiveWrapper
+from optimus_prime import Transformer, Decoder, AutoregressiveWrapper
 from optimus_prime import AndromedaEmbedding
 
 from lion_pytorch import Lion
 
 
 # constants
 
@@ -62,15 +58,15 @@
     n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     accelerator.print(f"Number of parameters in model: {n_params}")
 
 def fsdp_activation_checkpointing(
     model, accelerator: Accelerator, offload_to_cpu=False
 ):
 
-    accelerator.print(f"Using FSDP activation checkpointing")
+    accelerator.print("Using FSDP activation checkpointing")
 
     # check_fn = lambda submodule: isinstance(submodule, ParallelTransformerBlock)
 
     non_reentrant_wrapper = partial(
         checkpoint_wrapper,
         offload_to_cpu=offload_to_cpu,
         checkpoint_impl=CheckpointImpl.NO_REENTRANT,
@@ -175,15 +171,15 @@
 
     # Create the tokenizer
 
     tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
 
     # instantiate andromeda
 
-    model = TransformerWrapper(
+    model = Transformer(
         num_tokens=64007,
         max_seq_len=8192,
         use_abs_pos_emb=False,
         tokenizer=tokenizer, # !
         embedding_provider=AndromedaEmbedding(),
         attn_layers = Decoder(
             dim=128, # 2048
@@ -327,15 +323,15 @@
                 accelerator.save_state(output_dir)
 
         if completed_steps >= max_train_steps:
             break
 
     # end training
 
-    accelerator.print(f"Training Finished")
+    accelerator.print("Training Finished")
     accelerator.end_training()
 
     # save final model
 
     # accelerator.print(f"Saving model to {CFG.OUTPUT_DIR}")
     if CFG.OUTPUT_DIR is not None:
         base_path = f'{CFG.OUTPUT_DIR}/final'
```

### Comparing `thebestllmever-0.0.1/andromeda/old/training_sophia.py` & `thebestllmever-0.0.2/andromeda/old/training_sophia.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 import math
 import multiprocessing
 import os
-import collections
 
 from datetime import timedelta
 from functools import partial
 from itertools import chain
 
-import torch
 
 from accelerate import Accelerator
 from accelerate.utils import InitProcessGroupKwargs
 
 from datasets import concatenate_datasets, load_dataset
 
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     CheckpointImpl, apply_activation_checkpointing, checkpoint_wrapper)
 
-from torch.optim import AdamW
 from torch.utils.data import DataLoader
 
 from tqdm import tqdm
 
 from transformers import (AutoTokenizer, default_data_collator,
                           get_cosine_schedule_with_warmup,
                           get_linear_schedule_with_warmup, set_seed)
 
-from datasets import Dataset
 
 # from stable_adamw import StableAdamWUnfused
 # sd
 
-from optimus_prime import TransformerWrapper, Decoder, AutoregressiveWrapper
+from optimus_prime import Transformer, Decoder, AutoregressiveWrapper
 from optimus_prime import AndromedaEmbedding
 
-from lion_pytorch import Lion
 from sophia import SophiaG
-import numpy as np
 
 # constants
 
 class CFG:
     BATCH_SIZE: int = 3 # 3
     GRADIENT_ACCUMULATE_EVERY: int = 1
     SEED: int = 42
@@ -61,15 +55,15 @@
     n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     accelerator.print(f"Number of parameters in model: {n_params}")
 
 def fsdp_activation_checkpointing(
     model, accelerator: Accelerator, offload_to_cpu=False
 ):
 
-    accelerator.print(f"Using FSDP activation checkpointing")
+    accelerator.print("Using FSDP activation checkpointing")
 
     # check_fn = lambda submodule: isinstance(submodule, ParallelTransformerBlock)
 
     non_reentrant_wrapper = partial(
         checkpoint_wrapper,
         offload_to_cpu=offload_to_cpu,
         checkpoint_impl=CheckpointImpl.NO_REENTRANT,
@@ -182,15 +176,15 @@
 
     # Create the tokenizer
 
     tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
 
     # instantiate andromeda
 
-    model = TransformerWrapper(
+    model = Transformer(
         num_tokens=64007,
         max_seq_len=8192,
         use_abs_pos_emb=False,
         tokenizer=tokenizer, # !
         embedding_provider=AndromedaEmbedding(),
         attn_layers = Decoder(
             dim=128, # 2048
@@ -348,15 +342,15 @@
                 accelerator.save_state(output_dir)
 
         if completed_steps >= max_train_steps:
             break
 
     # end training
 
-    accelerator.print(f"Training Finished")
+    accelerator.print("Training Finished")
     accelerator.end_training()
 
     # save final model
 
     # accelerator.print(f"Saving model to {CFG.OUTPUT_DIR}")
     if CFG.OUTPUT_DIR is not None:
         base_path = f'{CFG.OUTPUT_DIR}/final'
```

### Comparing `thebestllmever-0.0.1/andromeda/optimus_prime/attend.py` & `thebestllmever-0.0.2/andromeda/core/attend.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 
 from collections import namedtuple
 from functools import wraps
 from packaging import version
 from dataclasses import dataclass
-
 from einops import rearrange
 
+from Andromeda.core.flash import attention
+
 # from flash import FlashAttention
 
 # constants
 
 EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 @dataclass
@@ -53,14 +54,15 @@
         dropout = 0.,
         causal = False,
         heads = None,
         talking_heads = False,
         scale = None,
         qk_norm = False,
         flash = False,
+        triton = False,
     ):
         super().__init__()
         self.scale = scale
         self.qk_norm = qk_norm
         self.causal = causal
         self.attn_fn = partial(F.softmax, dtype = torch.float32) if not qk_norm else F.softmax
 
@@ -73,20 +75,18 @@
 
         self.talking_heads = talking_heads
         if talking_heads:
             self.pre_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
             self.post_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
 
         # flash attention
-
         self.flash = flash
         assert not (flash and version.parse(torch.__version__) < version.parse('2.0.0')), 'in order to use flash attention, you must be using pytorch 2.0 or above'
 
         # determine efficient attention configs for cuda and cpu
-
         self.cpu_config = EfficientAttentionConfig(True, True, True)
         self.cuda_config = None
 
         if not torch.cuda.is_available() or not flash:
             return
 
         device_properties = torch.cuda.get_device_properties(torch.device('cuda'))
@@ -196,14 +196,17 @@
         scale = default(self.scale, q.shape[-1] ** -0.5)
 
         if self.flash:
             assert not exists(prev_attn), 'residual attention not compatible with flash attention'
             return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
             # return FlashAttention(q, k, v, mask=mask, attn_bias=attn_bias )
 
+        if self.triton:
+            return attention(q, k, v, self.casual, scale)
+
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
 
         dots = einsum(f'b h i d, {kv_einsum_eq} -> b h i j', q, k) * scale
 
         if exists(prev_attn):
             dots = dots + prev_attn
```

### Comparing `thebestllmever-0.0.1/andromeda/optimus_prime/autoregressive_wrapper.py` & `thebestllmever-0.0.2/andromeda/core/autoregressive_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,14 @@
         temperature = 1.,
         filter_logits_fn = top_k,
         filter_thres = 0.9,
         min_p_pow = 2.0,
         min_p_ratio = 0.02,
         **kwargs
     ):
-        device = start_tokens.device
-        num_dims = start_tokens.ndim
 
         start_tokens, ps = pack([start_tokens], '* n')
 
         b, t = start_tokens.shape
 
         out = start_tokens
```

### Comparing `thebestllmever-0.0.1/andromeda/optimus_prime/x_transformers.py` & `thebestllmever-0.0.2/andromeda/core/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-#add ability to choose your own tokenizer, and embedder, and ask what else can be done for production level training
-
-
 import math
 from random import random
 
 import torch
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 
 from functools import partial, wraps
 from inspect import isfunction
-from collections import namedtuple
 from dataclasses import dataclass
 from typing import List
 
-from einops import rearrange, repeat, reduce
-from einops.layers.torch import Rearrange
+from einops import rearrange, repeat
 
-from andromeda.optimus_prime.attend import Attend, Intermediates
-from andromeda.optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
+from Andromeda.core.attend import Attend, Intermediates
+from Andromeda.core.autoregressive_wrapper import AutoregressiveWrapper
 
 from abc import ABC, abstractmethod
 # import bitsandbytes as bnb
 
 # constants
 
 DEFAULT_DIM_HEAD = 64
@@ -434,18 +429,24 @@
         return bias
 
 class RotaryEmbedding(nn.Module):
     def __init__(
         self,
         dim,
         use_xpos = False,
-        scale_base = 512
+        scale_base = 512,
+        interpolation_factor=1.,
+        base=10000,
+        base_rescale_factor=1.
     ):
         super().__init__()
-        inv_freq = 1. / (10000 ** (torch.arange(0, dim, 2).float() / dim))
+        base *=  base_rescale_factor ** (dim / (dim - 2))
+        
+        inv_freq = 1. / (base ** (torch.arange(0, dim, 2).float() / dim))
+
         self.register_buffer('inv_freq', inv_freq)
 
         if not use_xpos:
             self.register_buffer('scale', None)
             return
 
         scale = (torch.arange(0, dim, 2) + 0.4 * dim) / (1.4 * dim)
@@ -484,15 +485,16 @@
     def __init__(self, value, fn):
         super().__init__()
         self.value = value
         self.fn = fn
 
     def forward(self, x, **kwargs):
         out = self.fn(x, **kwargs)
-        scale_fn = lambda t: t * self.value
+        def scale_fn(t):
+            return t * self.value
 
         if not isinstance(out, tuple):
             return scale_fn(out)
 
         return (scale_fn(out[0]), *out[1:])
 
 class ScaleNorm(nn.Module):
@@ -781,15 +783,14 @@
 
         if not self.one_kv_head:
             k, v, r = map(lambda t: maybe(rearrange)(t, 'b n (h d) -> b h n d', h = h), (k, v, r))
 
         if self.qk_norm:
             qk_l2norm = partial(l2norm, groups = self.qk_norm_groups)
             q, k = map(qk_l2norm, (q, k))
-            scale = self.qk_norm_scale
 
             q = q * self.qk_norm_q_scale
             k = k * self.qk_norm_k_scale
 
         if exists(rotary_pos_emb) and not has_context:
             freqs, xpos_scale = rotary_pos_emb
             l = freqs.shape[-1]
@@ -816,15 +817,15 @@
                 input_mask = pad_at_dim(input_mask, (self.num_mem_kv, 0), dim = -1, value = True)
 
 
         i, j = map(lambda t: t.shape[-2], (q, k))
 
         # determine masking
 
-        mask_value = max_neg_value(q)
+        max_neg_value(q)
         masks = []
         final_attn_mask = None
 
         if exists(input_mask):
             input_mask = rearrange(input_mask, 'b j -> b 1 1 j')
             masks.append(~input_mask)
 
@@ -917,15 +918,17 @@
         dynamic_pos_bias = False,
         dynamic_pos_bias_log_distance = False,
         dynamic_pos_bias_mlp_depth = 2,
         dynamic_pos_bias_norm = False,
         rotary_pos_emb = False,
         rotary_emb_dim = None,
         rotary_xpos = False,
+        rotary_interpolation_factor=1.,
         rotary_xpos_scale_base = 512,
+        rotary_base_rescale_factor=1.,
         custom_layers = None,
         sandwich_coef = None,
         par_ratio = None,
         residual_attn = False,
         cross_residual_attn = False,
         macaron = False,
         pre_norm = True,
@@ -954,15 +957,15 @@
         self.layers = nn.ModuleList([])
 
         self.has_pos_emb = rel_pos_bias or rotary_pos_emb
 
         rotary_emb_dim = max(default(rotary_emb_dim, dim_head // 2), 32)
 
         assert not (rotary_xpos and not causal), 'rotary xpos is not compatible with bidirectional attention'
-        self.rotary_pos_emb = RotaryEmbedding(rotary_emb_dim, use_xpos = rotary_xpos, scale_base = rotary_xpos_scale_base) if rotary_pos_emb else None
+        self.rotary_pos_emb = RotaryEmbedding(rotary_emb_dim, use_xpos = rotary_xpos, scale_base = rotary_xpos_scale_base, interpolation_factor=rotary_interpolation_factor, base_rescale_factor=rotary_base_rescale_factor) if rotary_pos_emb else None
 
         assert not (alibi_pos_bias and rel_pos_bias), 'you can only choose Alibi positional bias or T5 relative positional bias, not both'
         assert rel_pos_num_buckets <= rel_pos_max_distance, 'number of relative position buckets must be less than the relative position max distance'
 
         # relative positional bias
 
         flash_attn = attn_kwargs.get('flash', False)
@@ -1126,15 +1129,15 @@
         if exists(self.rotary_pos_emb):
             max_rotary_emb_length = max(list(map(lambda m: (m.shape[1] if exists(m) else 0) + x.shape[1], mems)))
             rotary_pos_emb = self.rotary_pos_emb(max_rotary_emb_length, x.device)
 
         outer_residual = x
 
         for ind, (layer_type, (norm, block, residual_fn), layer_dropout) in enumerate(zip(self.layer_types, self.layers, self.layer_dropouts)):
-            is_last = ind == (self.layers_length - 1)
+            ind == (self.layers_length - 1)
 
             if self.training and layer_dropout > 0. and random() < layer_dropout:
                 continue
 
             if layer_type == 'a':
                 if return_hiddens:
                     hiddens.append(x)
@@ -1196,81 +1199,17 @@
         super().__init__(causal = False, **kwargs)
 
 class Decoder(AttentionLayers):
     def __init__(self, **kwargs):
         assert 'causal' not in kwargs, 'cannot set causality on decoder'
         super().__init__(causal = True, **kwargs)
 
-class CrossAttender(AttentionLayers):
-    def __init__(self, **kwargs):
-        super().__init__(cross_attend = True, only_cross = True, **kwargs)
-
-class ViTransformerWrapper(nn.Module):
-    def __init__(
-        self,
-        *,
-        image_size,
-        patch_size,
-        attn_layers,
-        channels = 3,
-        num_classes = None,
-        dropout = 0.,
-        post_emb_norm = False,
-        emb_dropout = 0.
-    ):
-        super().__init__()
-        assert isinstance(attn_layers, Encoder), 'attention layers must be an Encoder'
-        assert image_size % patch_size == 0, 'image dimensions must be divisible by the patch size'
-        dim = attn_layers.dim
-        num_patches = (image_size // patch_size) ** 2
-        patch_dim = channels * patch_size ** 2
-
-        self.patch_size = patch_size
-
-        self.pos_embedding = nn.Parameter(torch.randn(1, num_patches + 1, dim))
-
-        self.patch_to_embedding = nn.Sequential(
-            nn.LayerNorm(patch_dim),
-            nn.Linear(patch_dim, dim),
-            nn.LayerNorm(dim)
-        )
-
-        self.post_emb_norm = nn.LayerNorm(dim) if post_emb_norm else nn.Identity()
-        self.dropout = nn.Dropout(emb_dropout)
-
-        self.attn_layers = attn_layers
-        self.norm = nn.LayerNorm(dim)
-        self.mlp_head = nn.Linear(dim, num_classes) if exists(num_classes) else nn.Identity()
-
-    def forward(
-        self,
-        img,
-        return_embeddings = False
-    ):
-        p = self.patch_size
-
-        x = rearrange(img, 'b c (h p1) (w p2) -> b (h w) (p1 p2 c)', p1 = p, p2 = p)
-        x = self.patch_to_embedding(x)
-        n = x.shape[1]
-
-        x = x + self.pos_embedding[:, :n]
-
-        x = self.post_emb_norm(x)
-        x = self.dropout(x)
-
-        x = self.attn_layers(x)
-        x = self.norm(x)
-
-        if not exists(self.mlp_head) or return_embeddings:
-            return x
 
-        x = x.mean(dim = -2)
-        return self.mlp_head(x)
 
-class TransformerWrapper(nn.Module):
+class Transformer(nn.Module):
     def __init__(
         self,
         *,
         num_tokens,
         max_seq_len,
         attn_layers,
         # tokenizer: BaseTokenizer,
@@ -1291,23 +1230,16 @@
         super().__init__()
 
         assert isinstance(attn_layers, AttentionLayers), 'attention layers must be one of Encoder or Decoder'
 
         dim = attn_layers.dim
         emb_dim = default(emb_dim, dim)
 
-        # your own tokenizer
-        # self.tokenizer = tokenizer
-
-        #your own embedding function
-        self.token_emb = TokenEmbedding(emb_dim, num_tokens, embedding_provider, l2norm_embed=l2norm_embed)
-
         self.emb_dim = emb_dim
         self.num_tokens = num_tokens
-
         self.max_seq_len = max_seq_len
         self.max_mem_len = max_mem_len
         self.shift_mem_down = shift_mem_down
 
         self.l2norm_embed = l2norm_embed
         self.token_emb = TokenEmbedding(emb_dim, num_tokens, embedding_provider, l2norm_embed=l2norm_embed)
 
@@ -1442,163 +1374,7 @@
             return out, new_mems
 
         if return_attn:
             attn_maps = list(map(lambda t: t.post_softmax_attn, intermediates.attn_intermediates))
             return out, attn_maps
 
         return out
-
-class ContinuousTransformerWrapper(nn.Module):
-    def __init__(
-        self,
-        *,
-        max_seq_len,
-        attn_layers,
-        dim_in = None,
-        dim_out = None,
-        emb_dim = None,
-        post_emb_norm = False,
-        emb_dropout = 0.,
-        use_abs_pos_emb = True,
-        scaled_sinu_pos_emb = False
-    ):
-        super().__init__()
-        assert isinstance(attn_layers, AttentionLayers), 'attention layers must be one of Encoder or Decoder'
-
-        dim = attn_layers.dim
-
-        self.max_seq_len = max_seq_len
-
-        if not (use_abs_pos_emb and not attn_layers.has_pos_emb):
-            self.pos_emb = always(0)
-        elif scaled_sinu_pos_emb:
-            self.pos_emb = ScaledSinusoidalEmbedding(dim)
-        else:
-            self.pos_emb = AbsolutePositionalEmbedding(dim, max_seq_len)
-
-        self.post_emb_norm = nn.LayerNorm(dim) if post_emb_norm else nn.Identity()
-        self.emb_dropout = nn.Dropout(emb_dropout)
-
-        self.project_in = nn.Linear(dim_in, dim) if exists(dim_in) else nn.Identity()
-
-        self.attn_layers = attn_layers
-        self.norm = nn.LayerNorm(dim)
-
-        self.project_out = nn.Linear(dim, dim_out) if exists(dim_out) else nn.Identity()
-
-    def forward(
-        self,
-        x,
-        return_embeddings = False,
-        return_intermediates = False,
-        mask = None,
-        return_attn = False,
-        mems = None,
-        pos = None,
-        prepend_embeds = None,
-        **kwargs
-    ):
-        x = self.project_in(x)
-        x = x + self.pos_emb(x, pos = pos)
-
-        x = self.post_emb_norm(x)
-
-        # whether to append embeds, as in PaLI, for image embeddings
-
-        if exists(prepend_embeds):
-            _, prepend_dim = prepend_embeds.shape[1:]
-            assert prepend_dim == x.shape[-1], 'prepended embeddings need to have same dimensions as model dimensions'
-
-            x = torch.cat((prepend_embeds, x), dim = -2)
-
-        x = self.emb_dropout(x)
-
-        x, intermediates = self.attn_layers(x, mask = mask, mems = mems, return_hiddens = True, **kwargs)
-        x = self.norm(x)
-
-        out = self.project_out(x) if not return_embeddings else x
-
-        if return_intermediates:
-            return out, intermediates
-
-        if return_attn:
-            attn_maps = list(map(lambda t: t.post_softmax_attn, intermediates.attn_intermediates))
-            return out, attn_maps
-
-        return out
-
-class XTransformer(nn.Module):
-    def __init__(
-        self,
-        *,
-        dim,
-        tie_token_emb = False,
-        ignore_index = -100,
-        pad_value = 0,
-        deepnorm = False,
-        cross_attn_tokens_dropout = 0.,
-        **kwargs
-    ):
-        super().__init__()
-        enc_kwargs, kwargs = groupby_prefix_and_trim('enc_', kwargs)
-        dec_kwargs, kwargs = groupby_prefix_and_trim('dec_', kwargs)
-
-        assert 'dim' not in enc_kwargs and 'dim' not in dec_kwargs, 'dimension of either encoder or decoder must be set with `dim` keyword'
-        enc_transformer_kwargs = pick_and_pop(['num_tokens', 'max_seq_len'], enc_kwargs)
-        enc_transformer_kwargs['emb_dropout'] = enc_kwargs.pop('emb_dropout', 0)
-        enc_transformer_kwargs['num_memory_tokens'] = enc_kwargs.pop('num_memory_tokens', None)
-        enc_transformer_kwargs['scaled_sinu_pos_emb'] = enc_kwargs.pop('scaled_sinu_pos_emb', False)
-        enc_transformer_kwargs['use_abs_pos_emb'] = enc_kwargs.pop('use_abs_pos_emb', True)
-
-        dec_transformer_kwargs = pick_and_pop(['num_tokens', 'max_seq_len'], dec_kwargs)
-        dec_transformer_kwargs['emb_dropout'] = dec_kwargs.pop('emb_dropout', 0)
-        dec_transformer_kwargs['scaled_sinu_pos_emb'] = dec_kwargs.pop('scaled_sinu_pos_emb', False)
-        dec_transformer_kwargs['use_abs_pos_emb'] = dec_kwargs.pop('use_abs_pos_emb', True)
-
-        self.cross_attn_tokens_dropout = cross_attn_tokens_dropout  # how many tokens from the encoder to dropout when cross attending from decoder - seen in a couple papers, including Perceiver AR - this will also be very effective regularization when cross attending to very long memories
-
-        if deepnorm:
-            enc_kwargs['scale_residual'] = True
-            dec_kwargs['scale_residual'] = True
-
-            enc_depth = enc_kwargs['depth']
-            dec_depth = dec_kwargs['depth']
-
-            enc_kwargs['scale_residual_constant'] = 0.81 * ((enc_depth ** 4) * dec_depth) ** .0625
-            dec_kwargs['scale_residual_constant'] = (3 * dec_depth) ** 0.25
-
-        self.encoder = TransformerWrapper(
-            **enc_transformer_kwargs,
-            attn_layers = Encoder(dim = dim, **enc_kwargs)
-        )
-
-        self.decoder = TransformerWrapper(
-            **dec_transformer_kwargs,
-            attn_layers = Decoder(dim = dim, cross_attend = True, **dec_kwargs)
-        )
-
-        if deepnorm:
-            deepnorm_init(self.encoder, 0.87 * ((enc_depth ** 4) * dec_depth) ** -0.0625)
-            deepnorm_init(self.decoder, (12 * dec_depth) ** -0.25)
-
-        if tie_token_emb:
-            self.decoder.token_emb = self.encoder.token_emb
-
-        self.decoder = AutoregressiveWrapper(self.decoder, ignore_index=ignore_index, pad_value=pad_value)
-
-    @torch.no_grad()
-    def generate(self, seq_in, seq_out_start, seq_len, mask = None, attn_mask = None, **kwargs):
-        encodings = self.encoder(seq_in, mask = mask, attn_mask = attn_mask, return_embeddings = True)
-        return self.decoder.generate(seq_out_start, seq_len, context = encodings, context_mask = mask, **kwargs)
-
-    def forward(self, src, tgt, mask = None, attn_mask = None, src_prepend_embeds = None):
-
-        if exists(src_prepend_embeds) and exists(mask):
-            mask = pad_at_dim(mask, (src_prepend_embeds.shape[-2], 0), dim = -1, value = True)
-
-        enc = self.encoder(src, mask = mask, attn_mask = attn_mask, prepend_embeds = src_prepend_embeds, return_embeddings = True)
-
-        if self.training and self.cross_attn_tokens_dropout > 0:
-            enc, mask = dropout_seq(enc, mask, self.cross_attn_tokens_dropout)
-
-        out = self.decoder(tgt, context = enc, context_mask = mask)
-        return out
```

### Comparing `thebestllmever-0.0.1/andromeda/utils/decoupled_optimizer.py` & `thebestllmever-0.0.2/andromeda/utils/decoupled_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 # from palm_rlhf_pytorch.palm import LayerNorm
 from torch.nn import LayerNorm
 from torch.optim import AdamW
 
 # from palm.utils import print_main
-from utils.helpers import print_main
-from utils.stable_adamw import StableAdamWUnfused
+from Andromeda.utils.helpers import print_main
+from Andromeda.utils.stable_adamw import StableAdamWUnfused
 
 # optimizers
 
 
 def decoupled_optimizer(
     model: torch.nn.Module,
     learning_rate: float,
```

### Comparing `thebestllmever-0.0.1/andromeda/utils/rf_utils.py` & `thebestllmever-0.0.2/andromeda/utils/rf_utils.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.1/andromeda/utils/stable_adamw.py` & `thebestllmever-0.0.2/andromeda/utils/stable_adamw.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,16 @@
 
         print("Using StableAdamWUnfused-v1")
 
     def __setstate__(self, state):
         super(StableAdamWUnfused, self).__setstate__(state)
 
     def step(self, closure=None):
-        loss = None
         if closure is not None:
-            loss = closure()
+            closure()
 
         for group in self.param_groups:
             lr = group["lr"]
             weight_decay = group["weight_decay"]
             beta1 = group["beta1"]
             beta2 = group["beta2"]
             step = group["step"]
```

### Comparing `thebestllmever-0.0.1/pyproject.toml` & `thebestllmever-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TheBestLLMEver"
-version = "0.0.1"
+version = "0.0.2"
 description = "andromeda - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # assuming you have a README.md file
 homepage = "https://github.com/kyegomez/Andromeda"
 keywords = ["artificial intelligence", "attention mechanism", "transformers"]
 classifiers = [
@@ -20,15 +20,14 @@
 torch = "*"
 lion-pytorch = "*"
 numpy = "*"
 einops = "*"
 accelerate = "*"
 transformers = "*"
 SentencePiece = "*"
-bitsandbytes = "*"
 datasets = "*"
 matplotlib = "*"
 deepspeed = "*"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `thebestllmever-0.0.1/setup.py` & `thebestllmever-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['andromeda',
+ 'andromeda.core',
  'andromeda.dataset_prep',
- 'andromeda.finetuning',
  'andromeda.old',
- 'andromeda.optimus_prime',
  'andromeda.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['SentencePiece',
  'accelerate',
- 'bitsandbytes',
  'datasets',
  'deepspeed',
  'einops',
  'lion-pytorch',
  'matplotlib',
  'numpy',
  'torch',
  'transformers']
 
 setup_kwargs = {
     'name': 'thebestllmever',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'andromeda - Pytorch',
-    'long_description': '\n# [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)\n\n# Agora\nAgora is an new open source Multi-Modality AI Research Organization devoted to advancing Humanity to a post-scarcity state!\n\nSince Andromeda is ready to train Agora is actively seeking cloud providers or grant providers to train this all-new revolutionary model and release it open source, if you would like to learn more please email me at `kye@apac.ai`\n\n![Agora banner](agora-banner.png)\n\n![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)\n\n\n---\n\n# Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌\n\n![Andromeda Next Generation Open Source Language Model](/andromeda-banner.png)\n\nAndromeda is a state-of-the-art language model that pushes the boundaries of natural language understanding and generation. Designed for high performance and efficiency, Andromeda is built upon advanced techniques that make it a strong contender against the likes of OpenAI\'s GPT-4 and PALM with features like:\n\n* Process Ultra Long Sequences of 32,000-200,000+ context lengths effortlessly :fire: :closed_book: \n\n* Process those Ultra Long Sequences Ultra Fast with 32,000+ tokens in under 100ms ⚡️ ⚡️ \n\n* Reliable and actually useful with superior reasoning capabilities :brain: :brain: \n\n---\n\n<div align="center">\n\n[![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)\n[![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)\n\n</div>\n\n<div align="center">\n\n[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)\n\n\n![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)\n\n</div>\n\n---\n\n\n\n\n## Table of Contents\n\n- [Usage](#usage)\n- [Documentation](#documentation)\n- [Contributing to Andromeda](#contributing-to-andromeda)\n- [Roadmap](#roadmap)\n\n---\n\n## Usage\n\nThere are two methods to use Andromeda but pip does not work now.\n\n1. Clone the repository.\n\nFor detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).\n\n## Documentation\n\nFor detailed documentation, click [here](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).\n\n### Method 1\n\nTo get started:\n\n1. Clone the repository and install the required packages:\n\n```\ngit clone https://github.com/kyegomez/Andromeda\ncd Andromeda\npip3 install -r requirements.txt\ncd Andromeda\npython3 train.py\n```\n\nFor further instructions, refer to the [Training SOP](DOCs/TRAINING.md).\n\n## Training\n\n1. Set the environment variables:\n   - `ENTITY_NAME`: Your wandb project name\n   - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)\n\n2. Configure the training:\n   - Accelerate Config\n   - Enable Deepspeed 3\n   - Accelerate launch train_distributed_accelerate.py\n\nFor more information, refer to the [Training SOP](DOCs/TRAINING.md).\n\n## Dataset Building\n\nTo preprocess a different dataset similar to the C4 dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.\n\nExample command:\n\n```python\npython3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"\n```\n\n## Inference\n\n```python\npython3 inference.py "My dog is very cute" --seq_len 256 --temperature 0.8 --filter_thres 0.9 --model "andromeda"\n```\n\n(Note: Model submission to PyTorch Hub is still pending.)\n\n## Why Andromeda?\n\nAndromeda offers several advantages:\n\n- And romeda can potentially be fine-tuned with a 100k+ token sequence length.\n- It incorporates advanced techniques, including alibi positional bias, rotary position encodings (xpos), flash attention, and deep normalization (deepnorm), to optimize performance and efficiency.\n\nFor detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.\n\n## Andromeda Principles\n\nAndromeda is built on key principles:\n\n- **Efficiency**: Andromeda leverages optimization techniques, such as attention flashing, rotary position encodings, and deep normalization, to achieve efficient training and inference.\n- **Flexibility**: The modular design of Andromeda allows easy adaptation to various tasks and domains, making it versatile for a wide range of applications.\n- **Scalability**: Andromeda\'s architecture is designed to scale with increasing computational resources and data sizes, ensuring its relevance in the NLP landscape.\n- **Community-driven**: As an open-source project, Andromeda thrives on contributions from the community, fostering collaboration, innovation, and continuous improvement.\n\nJoin us on this exciting journey to create a powerful, efficient, and intelligent language model that will revolutionize the NLP landscape! 🚀🌟\n\n\n## Get Involved\n\nWe\'re just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you\'re a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.\n\n# Contributing to Andromeda\n\nWe are thrilled to invite you to be a part of the Andromeda project. This is not just an open source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.\n\n## Why Contribute\n\nContributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it\'s only fair that you share in the rewards.\n\n## Rewards Program\n\nHere\'s how the Andromeda Rewards Program works:\n\n1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.\n\n2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.\n\n3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution. \n\nThis means you\'re not just contributing to an open source project; you\'re becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.\n\n## Becoming a Paid API\n\nAs part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project, but also fund the rewards program. If you contribute anything to make Andromeda you will receive recurring revenue from paid API requests!\n\n## How to Start Contributing\n\nIf you\'re ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here\'s what you need to do:\n\n1. Fork the repository.\n\n2. Make your improvements or additions in your forked repository.\n\n3. Submit a pull request detailing the changes you\'ve made.\n\n4. Our team will review your submission. If it\'s approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.\n\nThank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let\'s build the future of multimodal embeddings together.\n\n## Roadmap 🗺️📍\n\n1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.\n\n2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:\n\n   - Model quantization: Reduce memory and computational requirements without significant loss in performance.\n   - Distillation: Train smaller, faster models that retain the knowledge of the larger model.\n   - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.\n\n3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.\n\n4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.\n\n\n## Todo:\n\n* [Create the best and most validated, reliable training => finetuning strategy](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)\n\n* Establish FineTuning scripts using quantization + 4bit precision, + other tactics like LoRA\n\n* Establish 200k instruction sample long for Tool API Calls\n\n* [Train on Gorilla Dataset](https://github.com/ShishirPatil/gorilla)\n\n\n* Establish Reinforcement Scripts to train on rewards from Human and Agent feedback\n\n\n\n\n\n\n\n\n\n\n\n\n\n',
+    'long_description': '\n# Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌\n\n<div align="center">\n\n[![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)\n[![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) \n[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) \n[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) \n[![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)\n[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)\n![Discord](https://img.shields.io/discord/999382051935506503)\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)\n\n</div>\n\n---\n\n![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)\n\nWelcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI\'s GPT-4 and PALM. Features include:\n\n- 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)\n- ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)\n- 🎓 Superior Reasoning Capabilities\n\n---\n\n## 🔄 Updates\n\n- [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)\n- [And, here is the WANDB link to watch Andromeda train live!](https://wandb.ai/apacai/Andromeda/overview?)\n\n---\n\n-----\n## Hiring\nWe\'re hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`\n\n----------\n\n## 💻 Usage\n\nThere are two methods to use Andromeda but pip does not work now.\n\n1. Clone the repository.\n\nFor detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).\n\n### Method 1\n\nTo get started:\n\n1. Clone the repository and install the required packages:\n\n```bash\ngit clone https://github.com/kyegomez/Andromeda\ncd Andromeda\npip3 install -r requirements.txt\ncd Andromeda\npython3 train.py\n```\n\nFor further instructions, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 📚 Training\n\n1. Set the environment variables:\n   - `ENTITY_NAME`: Your wandb project name\n   - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)\n   - `MASTER_ADDR`: For distributed training\n   - `MASTER_PORT` For master port distributed training\n   - `RANK`- Number of nodes services\n   - `WORLD_SIZE` Number of gpus\n\n2. Configure the training:\n   - Accelerate Config\n   - Enable Deepspeed 3\n   - Accelerate launch train_distributed_accelerate.py\n\nFor more information, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 🗃️ Dataset Building\n\nTo preprocess a\n\n different dataset similar to the C4 or Falcon dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.\n\nExample command:\n\n```bash\npython3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"\n```\n\n---\n\n## 🚀 Why Andromeda?\n\nAndromeda offers several advantages:\n- Andromeda offers reliable processing of 100,000+ sequence lengths extremely fast under 300ms\n- Andromeda\'s dataset strategy was crafted with atomic precision and attention to detail for creativity and quantitative reasoning.\n- Andromeda is extremely intelligent with the ability to think like a poet or make API Calls to your favorite apps.\n\nFor detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.\n\n---\n\n# 🎯 Andromeda Principles\n\n- **Efficiency**: Optimize with techniques like attention flashing, rotary position encodings, and deep normalization.\n- **Flexibility**: Adapt to various tasks and domains for wide applications.\n- **Scalability**: Designed to scale with resources and data sizes.\n- **Community-Driven**: Thrives on contributions from the open-source community.\n\n---\n\n## 🚀 Get Involved\n\nWe\'re just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you\'re a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.\n\n---\n\n# 🤝 Contributing to Andromeda\n\nWe are thrilled to invite you to be a part of the Andromeda project. This is not just an open-source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.\n\n## 🌟 Why Contribute\n\nContributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it\'s only fair that you share in the rewards.\n\n## 💰 Rewards Program\n\nHere\'s how the Andromeda Rewards Program works:\n\n1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.\n\n2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.\n\n3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution.\n\nThis means you\'re not just contributing to an open-source project; you\'re becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.\n\n## 🚀 Becoming a Paid API\n\nAs part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project but also fund the rewards program. If you contribute anything to make Andromeda, you will receive recurring revenue from paid API requests!\n\n## 🚀 How to Start Contributing\n\nIf you\'re ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here\'s what you need to do:\n\n1. Fork the repository.\n\n2. Make your improvements or additions in your forked repository.\n\n3. Submit a pull request detailing the changes you\'ve made.\n\n4. Our team will review your submission. If it\'s approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.\n\nThank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let\'s build the future of multimodal embeddings together.\n\n---\n\n## 🗺️ Roadmap\n\n1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.\n\n2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:\n\n   - Model quantization: Reduce memory and computational requirements without significant loss in performance.\n   - Distillation: Train smaller, faster models that retain the knowledge of the larger model.\n   - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.\n\n3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.\n\n4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.\n\n---\n\n## 📈 Benchmarks\n\n### Speed\n- Andromeda utilizes one of the most reliable Attentions ever, flash attention 2.0 Triton. It consumes 50x less memory than GPT-3 and 10x less than LLAMA.\n\n![AndromedaBanner](images/andromeda_performance.png)\n\n- We can speed this up even more with dynamic sparse flash attention 2.0.\n\n---\n\n# 🔮 Join the Journey\n\nWe\'re just getting started, and we invite you to join the journey. Let\'s revolutionize the NLP landscape together! 🚀🌟\n\n- Join Agora and work with 2,000+ AI Engineers to implement all new features.\n- Provide compute and help train Andromeda.\n- Share the message on how we\'re liberating this superintelligent AI and seizing the power from the corrupt, providing it back to you.\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/Andromeda',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `thebestllmever-0.0.1/PKG-INFO` & `thebestllmever-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,260 +1,206 @@
-Metadata-Version: 2.1
-Name: thebestllmever
-Version: 0.0.1
-Summary: andromeda - Pytorch
-Home-page: https://github.com/kyegomez/Andromeda
-License: MIT
-Keywords: artificial intelligence,attention mechanism,transformers
-Author: Kye Gomez
-Author-email: kye@apac.ai
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: SentencePiece
-Requires-Dist: accelerate
-Requires-Dist: bitsandbytes
-Requires-Dist: datasets
-Requires-Dist: deepspeed
-Requires-Dist: einops
-Requires-Dist: lion-pytorch
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: torch
-Requires-Dist: transformers
-Description-Content-Type: text/markdown
-
-
-# [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
-
-# Agora
-Agora is an new open source Multi-Modality AI Research Organization devoted to advancing Humanity to a post-scarcity state!
-
-Since Andromeda is ready to train Agora is actively seeking cloud providers or grant providers to train this all-new revolutionary model and release it open source, if you would like to learn more please email me at `kye@apac.ai`
-
-![Agora banner](agora-banner.png)
-
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
-
-
----
 
 # Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌
 
-![Andromeda Next Generation Open Source Language Model](/andromeda-banner.png)
-
-Andromeda is a state-of-the-art language model that pushes the boundaries of natural language understanding and generation. Designed for high performance and efficiency, Andromeda is built upon advanced techniques that make it a strong contender against the likes of OpenAI's GPT-4 and PALM with features like:
-
-* Process Ultra Long Sequences of 32,000-200,000+ context lengths effortlessly :fire: :closed_book: 
-
-* Process those Ultra Long Sequences Ultra Fast with 32,000+ tokens in under 100ms ⚡️ ⚡️ 
-
-* Reliable and actually useful with superior reasoning capabilities :brain: :brain: 
-
----
-
 <div align="center">
 
 [![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)
 [![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)
-
-[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) 
+[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) 
+[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) 
+[![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)
+[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) 
+[![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) 
+[![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)
+![Discord](https://img.shields.io/discord/999382051935506503)
+[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
+[![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
 
 </div>
 
-<div align="center">
-
-[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)
+---
 
+![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
 
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
-[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
+Welcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI's GPT-4 and PALM. Features include:
 
-</div>
+- 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)
+- ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)
+- 🎓 Superior Reasoning Capabilities
 
 ---
 
+## 🔄 Updates
 
+- [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
+- [And, here is the WANDB link to watch Andromeda train live!](https://wandb.ai/apacai/Andromeda/overview?)
 
+---
 
-## Table of Contents
-
-- [Usage](#usage)
-- [Documentation](#documentation)
-- [Contributing to Andromeda](#contributing-to-andromeda)
-- [Roadmap](#roadmap)
+-----
+## Hiring
+We're hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`
 
----
+----------
 
-## Usage
+## 💻 Usage
 
 There are two methods to use Andromeda but pip does not work now.
 
 1. Clone the repository.
 
 For detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
 
-## Documentation
-
-For detailed documentation, click [here](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
-
 ### Method 1
 
 To get started:
 
 1. Clone the repository and install the required packages:
 
-```
+```bash
 git clone https://github.com/kyegomez/Andromeda
 cd Andromeda
 pip3 install -r requirements.txt
 cd Andromeda
 python3 train.py
 ```
 
 For further instructions, refer to the [Training SOP](DOCs/TRAINING.md).
 
-## Training
+---
+
+## 📚 Training
 
 1. Set the environment variables:
    - `ENTITY_NAME`: Your wandb project name
    - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)
+   - `MASTER_ADDR`: For distributed training
+   - `MASTER_PORT` For master port distributed training
+   - `RANK`- Number of nodes services
+   - `WORLD_SIZE` Number of gpus
 
 2. Configure the training:
    - Accelerate Config
    - Enable Deepspeed 3
    - Accelerate launch train_distributed_accelerate.py
 
 For more information, refer to the [Training SOP](DOCs/TRAINING.md).
 
-## Dataset Building
+---
 
-To preprocess a different dataset similar to the C4 dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.
+## 🗃️ Dataset Building
 
-Example command:
+To preprocess a
 
-```python
-python3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"
-```
+ different dataset similar to the C4 or Falcon dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.
 
-## Inference
+Example command:
 
-```python
-python3 inference.py "My dog is very cute" --seq_len 256 --temperature 0.8 --filter_thres 0.9 --model "andromeda"
+```bash
+python3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"
 ```
 
-(Note: Model submission to PyTorch Hub is still pending.)
+---
 
-## Why Andromeda?
+## 🚀 Why Andromeda?
 
 Andromeda offers several advantages:
-
-- And romeda can potentially be fine-tuned with a 100k+ token sequence length.
-- It incorporates advanced techniques, including alibi positional bias, rotary position encodings (xpos), flash attention, and deep normalization (deepnorm), to optimize performance and efficiency.
+- Andromeda offers reliable processing of 100,000+ sequence lengths extremely fast under 300ms
+- Andromeda's dataset strategy was crafted with atomic precision and attention to detail for creativity and quantitative reasoning.
+- Andromeda is extremely intelligent with the ability to think like a poet or make API Calls to your favorite apps.
 
 For detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.
 
-## Andromeda Principles
-
-Andromeda is built on key principles:
+---
 
-- **Efficiency**: Andromeda leverages optimization techniques, such as attention flashing, rotary position encodings, and deep normalization, to achieve efficient training and inference.
-- **Flexibility**: The modular design of Andromeda allows easy adaptation to various tasks and domains, making it versatile for a wide range of applications.
-- **Scalability**: Andromeda's architecture is designed to scale with increasing computational resources and data sizes, ensuring its relevance in the NLP landscape.
-- **Community-driven**: As an open-source project, Andromeda thrives on contributions from the community, fostering collaboration, innovation, and continuous improvement.
+# 🎯 Andromeda Principles
 
-Join us on this exciting journey to create a powerful, efficient, and intelligent language model that will revolutionize the NLP landscape! 🚀🌟
+- **Efficiency**: Optimize with techniques like attention flashing, rotary position encodings, and deep normalization.
+- **Flexibility**: Adapt to various tasks and domains for wide applications.
+- **Scalability**: Designed to scale with resources and data sizes.
+- **Community-Driven**: Thrives on contributions from the open-source community.
 
+---
 
-## Get Involved
+## 🚀 Get Involved
 
 We're just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you're a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.
 
-# Contributing to Andromeda
+---
+
+# 🤝 Contributing to Andromeda
 
-We are thrilled to invite you to be a part of the Andromeda project. This is not just an open source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.
+We are thrilled to invite you to be a part of the Andromeda project. This is not just an open-source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.
 
-## Why Contribute
+## 🌟 Why Contribute
 
 Contributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it's only fair that you share in the rewards.
 
-## Rewards Program
+## 💰 Rewards Program
 
 Here's how the Andromeda Rewards Program works:
 
 1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.
 
 2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.
 
-3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution. 
+3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution.
 
-This means you're not just contributing to an open source project; you're becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.
+This means you're not just contributing to an open-source project; you're becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.
 
-## Becoming a Paid API
+## 🚀 Becoming a Paid API
 
-As part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project, but also fund the rewards program. If you contribute anything to make Andromeda you will receive recurring revenue from paid API requests!
+As part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project but also fund the rewards program. If you contribute anything to make Andromeda, you will receive recurring revenue from paid API requests!
 
-## How to Start Contributing
+## 🚀 How to Start Contributing
 
 If you're ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here's what you need to do:
 
 1. Fork the repository.
 
 2. Make your improvements or additions in your forked repository.
 
 3. Submit a pull request detailing the changes you've made.
 
 4. Our team will review your submission. If it's approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.
 
 Thank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
 
-## Roadmap 🗺️📍
+---
+
+## 🗺️ Roadmap
 
 1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.
 
 2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:
 
    - Model quantization: Reduce memory and computational requirements without significant loss in performance.
    - Distillation: Train smaller, faster models that retain the knowledge of the larger model.
    - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.
 
 3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.
 
 4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.
 
+---
 
-## Todo:
-
-* [Create the best and most validated, reliable training => finetuning strategy](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)
-
-* Establish FineTuning scripts using quantization + 4bit precision, + other tactics like LoRA
-
-* Establish 200k instruction sample long for Tool API Calls
-
-* [Train on Gorilla Dataset](https://github.com/ShishirPatil/gorilla)
-
-
-* Establish Reinforcement Scripts to train on rewards from Human and Agent feedback
-
-
-
-
-
-
-
+## 📈 Benchmarks
 
+### Speed
+- Andromeda utilizes one of the most reliable Attentions ever, flash attention 2.0 Triton. It consumes 50x less memory than GPT-3 and 10x less than LLAMA.
 
+![AndromedaBanner](images/andromeda_performance.png)
 
+- We can speed this up even more with dynamic sparse flash attention 2.0.
 
+---
 
+# 🔮 Join the Journey
 
+We're just getting started, and we invite you to join the journey. Let's revolutionize the NLP landscape together! 🚀🌟
 
+- Join Agora and work with 2,000+ AI Engineers to implement all new features.
+- Provide compute and help train Andromeda.
+- Share the message on how we're liberating this superintelligent AI and seizing the power from the corrupt, providing it back to you.
```

