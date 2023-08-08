# Comparing `tmp/sign_language_translator-0.6.0.tar.gz` & `tmp/sign_language_translator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sign_language_translator-0.6.0.tar", max compression
+gzip compressed data, was "sign_language_translator-0.6.1.tar", max compression
```

## Comparing `sign_language_translator-0.6.0.tar` & `sign_language_translator-0.6.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    26475 2023-08-07 12:18:55.242593 sign_language_translator-0.6.0/README.md
--rw-r--r--   0        0        0     1215 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2964 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/__init__.py
--rw-r--r--   0        0        0     6925 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/cli.py
--rw-r--r--   0        0        0      513 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/__init__.py
--rw-r--r--   0        0        0     6245 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/enums.py
--rw-r--r--   0        0        0     1736 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/helpers.py
--rw-r--r--   0        0        0     1768 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/settings.py
--rw-r--r--   0        0        0     2572 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/urls.yaml
--rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/__init__.py
--rwxr-xr-x   0        0        0    10252 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/completeness.py
--rwxr-xr-x   0        0        0     7713 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/scraping.py
--rwxr-xr-x   0        0        0     2107 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/synonyms.py
--rw-r--r--   0        0        0      250 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/__init__.py
--rw-r--r--   0        0        0      642 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/__init__.py
--rw-r--r--   0        0        0     4982 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/mapping_rules.py
--rw-r--r--   0        0        0     7989 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/pakistan_sign_language.py
--rw-r--r--   0        0        0     3773 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/sign_language.py
--rw-r--r--   0        0        0      355 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/__init__.py
--rw-r--r--   0        0        0       80 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/english.py
--rw-r--r--   0        0        0     1070 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/text_language.py
--rw-r--r--   0        0        0    13164 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/urdu.py
--rw-r--r--   0        0        0     2083 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/utils.py
--rw-r--r--   0        0        0    12432 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/vocab.py
--rw-r--r--   0        0        0     1773 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/__init__.py
--rw-r--r--   0        0        0     3297 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/_utils.py
--rw-r--r--   0        0        0     1958 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/__init__.py
--rwxr-xr-x   0        0        0     2699 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/abstract_language_model.py
--rwxr-xr-x   0        0        0     5407 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/beam_sampling.py
--rwxr-xr-x   0        0        0     7775 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/mixer.py
--rwxr-xr-x   0        0        0    11347 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/ngram_language_model.py
--rw-r--r--   0        0        0      873 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/__init__.py
--rw-r--r--   0        0        0    13121 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/layers.py
--rw-r--r--   0        0        0    18592 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/model.py
--rw-r--r--   0        0        0    15500 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/train.py
--rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/sign_to_text/__init__.py
--rw-r--r--   0        0        0      264 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/__init__.py
--rw-r--r--   0        0        0     3237 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
--rw-r--r--   0        0        0      536 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/t2s_model.py
--rw-r--r--   0        0        0    12989 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/utils.py
--rw-r--r--   0        0        0      466 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/__init__.py
--rwxr-xr-x   0        0        0     3320 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/metrics.py
--rwxr-xr-x   0        0        0      882 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/preprocess.py
--rwxr-xr-x   0        0        0     1333 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/subtitles.py
--rw-r--r--   0        0        0     4248 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/tagger.py
--rw-r--r--   0        0        0     4800 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/tokenizer.py
--rwxr-xr-x   0        0        0    12817 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/utils.py
--rwxr-xr-x   0        0        0      850 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/__init__.py
--rwxr-xr-x   0        0        0     3675 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/data_loader.py
--rw-r--r--   0        0        0     5076 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/download.py
--rwxr-xr-x   0        0        0    13542 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/landmarks_info.py
--rwxr-xr-x   0        0        0    10351 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/sign_data_attributes.py
--rwxr-xr-x   0        0        0     2822 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/tree.py
--rw-r--r--   0        0        0     1414 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/utils.py
--rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/__init__.py
--rwxr-xr-x   0        0        0    18024 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/concatenate.py
--rwxr-xr-x   0        0        0     7980 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/embed.py
--rwxr-xr-x   0        0        0    33628 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/transforms.py
--rwxr-xr-x   0        0        0    30236 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/visualization.py
--rw-r--r--   0        0        0    27995 1970-01-01 00:00:00.000000 sign_language_translator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    27467 2023-08-08 07:45:18.828359 sign_language_translator-0.6.1/README.md
+-rw-r--r--   0        0        0     1215 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/__init__.py
+-rw-r--r--   0        0        0     7029 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/cli.py
+-rw-r--r--   0        0        0      513 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/config/__init__.py
+-rw-r--r--   0        0        0     6483 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/config/enums.py
+-rw-r--r--   0        0        0     1736 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/config/helpers.py
+-rw-r--r--   0        0        0     1768 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/config/settings.py
+-rw-r--r--   0        0        0     2693 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/config/urls.yaml
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/data_collection/__init__.py
+-rwxr-xr-x   0        0        0    10252 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/data_collection/completeness.py
+-rwxr-xr-x   0        0        0     7713 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/data_collection/scraping.py
+-rwxr-xr-x   0        0        0     2107 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/data_collection/synonyms.py
+-rw-r--r--   0        0        0      250 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/sign/__init__.py
+-rw-r--r--   0        0        0     4982 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/sign/mapping_rules.py
+-rw-r--r--   0        0        0     7989 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/sign/pakistan_sign_language.py
+-rw-r--r--   0        0        0     3773 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/sign/sign_language.py
+-rw-r--r--   0        0        0      355 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/text/__init__.py
+-rw-r--r--   0        0        0       80 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/text/english.py
+-rw-r--r--   0        0        0     1070 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/text/text_language.py
+-rw-r--r--   0        0        0    13164 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/text/urdu.py
+-rw-r--r--   0        0        0     2083 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/utils.py
+-rw-r--r--   0        0        0    12432 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/languages/vocab.py
+-rw-r--r--   0        0        0     1773 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/__init__.py
+-rw-r--r--   0        0        0     3297 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/_utils.py
+-rw-r--r--   0        0        0     1958 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/__init__.py
+-rwxr-xr-x   0        0        0     2699 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/abstract_language_model.py
+-rwxr-xr-x   0        0        0     5407 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/beam_sampling.py
+-rwxr-xr-x   0        0        0     7775 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/mixer.py
+-rwxr-xr-x   0        0        0    11347 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/ngram_language_model.py
+-rw-r--r--   0        0        0      873 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/__init__.py
+-rw-r--r--   0        0        0    13121 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/layers.py
+-rw-r--r--   0        0        0    18592 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/model.py
+-rw-r--r--   0        0        0    15500 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/train.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/sign_to_text/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/text_to_sign/__init__.py
+-rw-r--r--   0        0        0     3237 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
+-rw-r--r--   0        0        0      536 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/text_to_sign/t2s_model.py
+-rw-r--r--   0        0        0    12989 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/models/utils.py
+-rw-r--r--   0        0        0      466 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/__init__.py
+-rwxr-xr-x   0        0        0     3320 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/metrics.py
+-rwxr-xr-x   0        0        0      882 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/preprocess.py
+-rwxr-xr-x   0        0        0     1333 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/subtitles.py
+-rw-r--r--   0        0        0     4248 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/tagger.py
+-rw-r--r--   0        0        0     4800 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/tokenizer.py
+-rwxr-xr-x   0        0        0    12817 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/text/utils.py
+-rwxr-xr-x   0        0        0      850 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3675 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/data_loader.py
+-rw-r--r--   0        0        0     5119 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/download.py
+-rwxr-xr-x   0        0        0    13542 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/landmarks_info.py
+-rwxr-xr-x   0        0        0    10351 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/sign_data_attributes.py
+-rwxr-xr-x   0        0        0     2822 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/tree.py
+-rw-r--r--   0        0        0     1414 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/vision/__init__.py
+-rwxr-xr-x   0        0        0    18024 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/vision/concatenate.py
+-rwxr-xr-x   0        0        0     7980 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/vision/embed.py
+-rwxr-xr-x   0        0        0    33628 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/vision/transforms.py
+-rwxr-xr-x   0        0        0    30236 2023-08-08 07:45:18.832359 sign_language_translator-0.6.1/sign_language_translator/vision/visualization.py
+-rw-r--r--   0        0        0    28987 1970-01-01 00:00:00.000000 sign_language_translator-0.6.1/PKG-INFO
```

### Comparing `sign_language_translator-0.6.0/README.md` & `sign_language_translator-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 3. [Usage](#usage)
    1. [Command Line](#command-line)
       <!-- 1. [configure](#configure) -->
       1. [$ slt download ...](#download)
       2. [$ slt translate ...](#translate)
       3. [$ slt complete ...](#complete)
    2. [Python](#python)
-      1. [basic translation](#basic-translation)
-      2. [text language processor](#text-language-processor)
-      3. [sign language processor](#sign-language-processor)
-      4. [video/feature processing](#vision)
-      5. [language models](#language-models)
+      1. [Translation](#basics)
+      2. [Text language processor](#text-language-processor)
+      3. [Sign language processor](#sign-language-processor)
+      4. [Video processing](#vision)
+      5. [Language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Upcoming/Roadmap](#upcomingroadmap)
 7. [How to Contribute](#how-to-contribute)
 8. [Credits and Gratitude](#credits-and-gratitude)
 9. [Bonus](#bonus)
    1. Number of lines of code
@@ -189,29 +189,32 @@
 Auto complete a sentence using our language models. This model can write sentences composed of supported words only:
 
 ```bash
 $ slt complete --end-token ">" --model-code urdu-mixed-ngram "<"
 ('<', 'وہ', ' ', 'یہ', ' ', 'نہیں', ' ', 'چاہتا', ' ', 'تھا', '۔', '>')
 ```
 
-These models predict next characters until a specified token appears. (e.g. generating names using a mixture of models):
+<details>
+<summary>These models predict next characters until a specified token appears. (e.g. generating names using a mixture of models):</summary>
 
 ```bash
 $ slt complete \
     --model-code unigram-names --model-weight 1 \
     --model-code bigram-names -w 2 \
     -m trigram-names -w 3 \
     --selection-strategy merge --beam-width 2.5 --end-token "]" \
     "[s"
 [shazala]
 ```
 
+</details>
+
 ### Python
 
-#### basic translation
+#### Basics
 
 ```python
 import sign_language_translator as slt
 
 # download dataset or models (if you need them separate)
 # (by default, dataset is auto-downloaded within the install directory)
 # slt.set_resource_dir("path/to/sign-language-datasets") # optional. Helps when data is synced with cloud
@@ -221,37 +224,39 @@
 
 print("All available models:")
 print(list(slt.ModelCodes)) # from slt.config.enums
 # print(list(slt.TextLanguageCodes))
 # print(list(slt.SignLanguageCodes))
 ```
 
-**Text to Sign**:
+**Text to Sign Translation**:
 
 ```python
 # Load text-to-sign model
 # deep_t2s_model = slt.get_model("t2s-flan-T5-base-01.pt") # pytorch
 # rule-based model (concatenates clips of each word)
 t2s_model = slt.get_model(
-    model_code = "concatenative-synthesis", # slt.ModelCodes.CONCATENATIVE_SYNTHESIS.value
+    model_code = "concatenative-synthesis", # slt.ModelCodes.CONCATENATIVE_SYNTHESIS
     text_language = "urdu", # or object of any child of slt.languages.text.text_language.TextLanguage class
     sign_language = "PakistanSignLanguage", # or object of any child of slt.languages.sign.sign_language.SignLanguage class
     sign_feature_model = "mediapipe_pose_v2_hand_v1",
 )
 
 text = "HELLO دنیا!" # HELLO treated as an acronym
 sign_language_sentence = t2s_model(text)
 
 # moviepy_video_object = sign_language_sentence.video()
 # moviepy_video_object.ipython_display()
 # moviepy_video_object.write_videofile(f"sentences/{text}.mp4")
 ```
 
-**Sign to text**
-dummy code: (will be finalized in v0.8+)
+**Sign to Text Translation**
+
+<details>
+<summary>dummy code: (will be finalized in v0.8+)</summary>
 
 ```python
 # load sign
 video = slt.read_video("video.mp4")
 # features = slt.extract_features(video, "mediapipe_pose_v2_hand_v1")
 
 # Load sign-to-text model
@@ -259,18 +264,21 @@
 features = deep_s2t_model.extract_features(video)
 
 # translate
 text = deep_s2t_model(features)
 print(text)
 ```
 
+</details>
+
 #### Text Language Processor
 
-```python
+Process text strings using language specific classes:
 
+```python
 from sign_language_translator.languages.text import Urdu
 ur_nlp = Urdu()
 
 text = "hello جاؤں COVID-19."
 
 normalized_text = ur_nlp.preprocess(text)
 # normalized_text = 'جاؤں COVID-19.'
@@ -306,15 +314,16 @@
 #   {'signs': [['pk-hfad-1_school']], 'weights': [1.0]},
 #   {'signs': [['pk-hfad-1_گیا']], 'weights': [1.0]}
 # ]
 ```
 
 #### Vision
 
-dummy code: (will be finalized in v0.7)
+<details>
+<summary>dummy code: (will be finalized in v0.7)</summary>
 
 ```python
 import sign_language_translator as slt
 
 # load video
 video = slt.read_video("sign.mp4")
 
@@ -328,17 +337,20 @@
 video = slt.vision.plot_landmarks(features)
 
 # display
 video.show()
 print(features.numpy())
 ```
 
+</details>
+
 #### Language models
 
-Simple statistical n-gram model:
+<details open>
+<summary>Simple statistical n-gram model:</summary>
 
 ```python
 from sign_language_translator.models.language_models import NgramLanguageModel
 
 names_data = [
     '[abeera]', '[areej]',  '[farida]',  '[hiba]',    '[kinza]',
     '[mishal]', '[nimra]',  '[rabbia]',  '[tehmina]', '[zoya]',
@@ -360,15 +372,18 @@
 print(name)
 # '[rabeej]'
 
 # see ngram model's implementation
 print(model.__dict__)
 ```
 
-Mash up multiple language models & complete generation through beam search:
+</details>
+
+<details open>
+<summary>Mash up multiple language models & complete generation through beam search:</summary>
 
 ```python
 from sign_language_translator.models.language_models import MixerLM, BeamSampling, NgramLanguageModel
 
 # using data from previous example
 names_data = [...] # or slt.languages.English().vocab.person_names # concat start/end symbols
 
@@ -395,38 +410,43 @@
 # use Beam Search to find high likelihood names
 sampler = BeamSampling(mixed_model, beam_width=3) #, scoring_function = ...)
 name = sampler.complete('[')
 print(name)
 # [rabbia]
 ```
 
-Write sentences composed of only those words for which sign videos are available so that the rule-based text-to-sign model can generate training examples for a deep learning model:
+</details>
+
+<details open>
+<summary>Write sentences composed of only those words for which sign videos are available so that the rule-based text-to-sign model can generate training examples for a deep learning model:</summary>
 
 ```python
 from sign_language_translator.models.language_models import TransformerLanguageModel
 
 # model = slt.get_model("ur-supported-gpt")
 model = TransformerLanguageModel.load("models/tlm_14.0M.pt")
 # sampler = BeamSampling(model, ...)
 # sampler.complete(["<"])
 
 # see probabilities of all tokens
 model.next_all(["میں", " ", "وزیراعظم", " ",])
 # (["سے", "عمران", ...], [0.1415926535, 0.7182818284, ...])
 ```
 
+</details>
+
 ## Directory Tree
 
 <pre>
 <big><b>sign-language-translator</b></big>
-├── <a href="">MANIFEST.in</a>
-├── <a href="">README.md</a>
-├── <a href="">poetry.lock</a>
-├── <a href="">pyproject.toml</a>
-├── <a href="">requirements.txt</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/MANIFEST.in">MANIFEST.in</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/README.md">README.md</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/poetry.lock">poetry.lock</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/pyproject.toml">pyproject.toml</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/requirements.txt">requirements.txt</a>
 ├── <b>tests</b>
 │   └── <a href="https://github.com/sign-language-translator/sign-language-translator/tree/main/tests">*</a>
 │
 └── <big><b>sign_language_translator</b></big>
     ├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/sign_language_translator/cli.py">cli.py</a>
     ├── <b>config</b>
     │   ├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/sign_language_translator/config/enums.py">enums.py</a>
@@ -498,52 +518,82 @@
 
 ## Research Paper
 
 Stay Tuned!
 
 ## Upcoming/Roadmap
 
+<details>
+<summary>CLEAN_ARCHITECTURE_VISION: v0.7</summary>
+
 ```python
-# :CLEAN_ARCHITECTURE_VISION: v0.7
-    # class according to feature type (pose/video/mesh)
-    # video loader
-    # feature extraction
-    # feature augmentation
-    # feature model names enums
-    # subtitles
-    # 2D/3D avatars
+# class according to feature type (pose/video/mesh)
+# video loader
+# feature extraction
+# feature augmentation
+# feature model names enums
+# subtitles
+# 2D/3D avatars
+```
+
+</details>
+
+<details>
+<summary>MISCELLANEOUS</summary>
 
-# push notebooks
+```python
+# clean demonstration notebooks
 # expand reference clip data by scraping everything
 # data info table
 # https://sign-language-translator.readthedocs.io/en/latest/
+# sequence diagram for creating a translator
+```
+
+</details>
+
+<details>
+<summary>DEEP_TRANSLATION: v0.8-v1.x</summary>
+
+```python
+# sign to text with fine-tuned whisper
+# pose vector generation with fine-tuned flan-T5
+# motion transfer
+# pose2video: stable diffusion or GAN?
+# speech to text
+# text to speech
+# LanguageModel: experiment by dropping space tokens
+# parallel text corpus
+```
+
+</details>
 
-# :DEEP_TRANSLATION: v0.8-v1.x
-    # sign to text with fine-tuned whisper
-    # pose vector generation with fine-tuned flan-T5
-    # motion transfer
-    # pose2video: stable diffusion or GAN?
-    # speech to text
-    # text to speech
-    # LanguageModel: experiment by dropping space tokens
-    # parallel text corpus
-
-# RESEARCH PAPERs
-    # datasets: clips, text, sentences, disambiguation
-    # rule based translation: describe entire repo
-    # deep sign-to-text: pipeline + experiments
-    # deep text-to-sign: pipeline + experiments
-
-# PRODUCT DEVELOPMENT
-    # ML inference server
-    # Django backend server
-    # React Frontend
-    # React Native mobile app
+<details>
+<summary>RESEARCH PAPERs</summary>
+
+```python
+# datasets: clips, text, sentences, disambiguation
+# rule based translation: describe entire repo
+# deep sign-to-text: pipeline + experiments
+# deep text-to-sign: pipeline + experiments
+```
+
+</details>
+
+<details>
+<summary>PRODUCT DEVELOPMENT</summary>
+
+```python
+# ML inference server
+# Django backend server
+# React Frontend
+# React Native mobile app
 ```
 
+</details>
+
 ## How to Contribute
 
 - Datasets:
   - Scrape and upload video datasets.
   - Label word mapping datasets.
   - Reach out to to Academies for Deaf and have them write down *sign language grammar*.
 - New Code
@@ -571,15 +621,15 @@
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **9248** + Tests: **877**):
+Count total number of **lines of code** (Package: **9259** + Tests: **885**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for `Fun`**
```

### Comparing `sign_language_translator-0.6.0/pyproject.toml` & `sign_language_translator-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sign_language_translator"
-version = "0.6.0"
+version = "0.6.1"
 description = "Translate between spoken/text languages and sign language videos using AI."
 authors = ["Mudassar Iqbal <mdsriqb@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "sign_language_translator"}]
 repository = "https://github.com/sign-language-translator/sign-language-translator"
 keywords = ["sign", "translation", "pose", "pakistan", "deep-learning", "computer-vision", "nlp", "sign-language", "sign-language-translation"]
```

### Comparing `sign_language_translator-0.6.0/sign_language_translator/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/cli.py` & `sign_language_translator-0.6.1/sign_language_translator/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Sign Language Translator (SLT) Command Line Interface
 
 This module provides a command line interface (CLI) for the Sign Language Translator (SLT) library.
-It allows you to perform various operations, such as downloading resource files and translating text to sign language or vice versa.
+It allows you to perform various operations such as translating text to sign language or vice versa,
+downloading resource files & completing text sequences using Language Models.
 
 Usage:
     slt [OPTIONS] COMMAND [ARGS]...
 
 Options:
     --help  Show this message and exit.
 
 Commands:
+    complete   Complete a sequence using Language Models.
     download   Download resource files.
     translate  Translate text into sign language or vice versa.
 """
 
 import click
 
 from sign_language_translator import __version__
```

### Comparing `sign_language_translator-0.6.0/sign_language_translator/config/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/config/enums.py` & `sign_language_translator-0.6.1/sign_language_translator/config/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,21 +156,25 @@
     Returns:
         str: The normalized short code.
 
     Raises:
         ValueError: If the provided short code is unknown.
     """
 
+    if isinstance(short_code, Enum):
+        short_code = short_code.value
+
     normalized_to_codes = {
         ModelCodes.CONCATENATIVE_SYNTHESIS.value: {
             "rule-based",
             "concatenative",
             "concatenativesynthesis",
             "concatenative-synthesis",
             "concatenative_synthesis",
+            "concat-synth",
         },
         TextLanguages.URDU.value: {
             "urdu",
             "ur",
         },
         SignLanguages.PAKISTAN_SIGN_LANGUAGE.value: {
             "psl",
@@ -186,17 +190,21 @@
             "bigram-names",
         },
         ModelCodes.NGRAM_LM_TRIGRAM_NAMES.value: {
             "trigram-names",
         },
         ModelCodes.MIXER_LM_NGRAM_URDU.value: {
             "urdu-mixed-ngram",
+            "urdu-supported-ngram",
+            "ur-mixed-ngram",
+            "ur-supported-ngram",
         },
         ModelCodes.TRANSFORMER_LM_UR_SUPPORTED.value: {
             "ur-supported-gpt",
+            "urdu-supported-gpt",
         },
     }
     normalized_to_codes = {k: v.union({k}) for k, v in normalized_to_codes.items()}
 
     normalized = search_in_values_to_retrieve_key(short_code, normalized_to_codes)
     if normalized:
         return normalized  # constructor called
```

### Comparing `sign_language_translator-0.6.0/sign_language_translator/config/helpers.py` & `sign_language_translator-0.6.1/sign_language_translator/config/helpers.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/config/settings.py` & `sign_language_translator-0.6.1/sign_language_translator/config/settings.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/config/urls.yaml` & `sign_language_translator-0.6.1/sign_language_translator/config/urls.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,24 @@
       - name: models/names-stat-lm-w2.json
         url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/names-stat-lm-w2.json
       - name: models/names-stat-lm-w3.json
         url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/names-stat-lm-w3.json
       - name: models/ur-supported-token-unambiguous-mixed-ngram-w1-w6-lm.pkl
         url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/ur-supported-token-unambiguous-mixed-ngram-w1-w6-lm.pkl
       - name: models/tlm_14.0M.pt
-        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/tlm_8.7M.pt
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/tlm_14.0M.pt
 
   - name: text-to-sign
     files:
       - name: x.x
-        url: https://
+        url: https://github.com/sign-language-translator/sign-language-translator
 
   - name: sign-to-text
     files:
       - name: x.y
-        url: https://
+        url: https://github.com/sign-language-translator/sign-language-translator
 
 others:
   - name: extra-url-files
     files:
       - name: extra_urls.yaml
         url: "https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/1456b64b4ed38247a7a792f706403af1ed2287b4/extra_urls.yaml"
```

### Comparing `sign_language_translator-0.6.0/sign_language_translator/data_collection/completeness.py` & `sign_language_translator-0.6.1/sign_language_translator/data_collection/completeness.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/data_collection/scraping.py` & `sign_language_translator-0.6.1/sign_language_translator/data_collection/scraping.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/data_collection/synonyms.py` & `sign_language_translator-0.6.1/sign_language_translator/data_collection/synonyms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/sign/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/sign/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/sign/mapping_rules.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/sign/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/sign/pakistan_sign_language.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/sign/pakistan_sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/sign/sign_language.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/sign/sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/text/text_language.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/text/text_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/text/urdu.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/text/urdu.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/utils.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/languages/vocab.py` & `sign_language_translator-0.6.1/sign_language_translator/languages/vocab.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/_utils.py` & `sign_language_translator-0.6.1/sign_language_translator/models/_utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/abstract_language_model.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/abstract_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/beam_sampling.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/beam_sampling.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/mixer.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/mixer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/ngram_language_model.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/ngram_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/layers.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/layers.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/model.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/train.py` & `sign_language_translator-0.6.1/sign_language_translator/models/language_models/transformer_language_model/train.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py` & `sign_language_translator-0.6.1/sign_language_translator/models/text_to_sign/concatenative_synthesis.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/t2s_model.py` & `sign_language_translator-0.6.1/sign_language_translator/models/text_to_sign/t2s_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/models/utils.py` & `sign_language_translator-0.6.1/sign_language_translator/models/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/metrics.py` & `sign_language_translator-0.6.1/sign_language_translator/text/metrics.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/preprocess.py` & `sign_language_translator-0.6.1/sign_language_translator/text/preprocess.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/subtitles.py` & `sign_language_translator-0.6.1/sign_language_translator/text/subtitles.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/tagger.py` & `sign_language_translator-0.6.1/sign_language_translator/text/tagger.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/tokenizer.py` & `sign_language_translator-0.6.1/sign_language_translator/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/text/utils.py` & `sign_language_translator-0.6.1/sign_language_translator/text/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/__init__.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/data_loader.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/download.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     if os.path.exists(file_path) and not overwrite:
         raise FileExistsError(f"There is already a file at {file_path}")
 
     try:
         response = requests.get(url, stream=True, timeout=timeout)
         response.raise_for_status()
 
-        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        if os.path.dirname(file_path):
+            os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
         with open(file_path, "wb") as fp:
             stream = response.iter_content(chunk_size=chunk_size)
 
             if progress_bar:
                 total_bytes = int(
                     response.headers.get("content-length", 0)
```

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/landmarks_info.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/landmarks_info.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/sign_data_attributes.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/sign_data_attributes.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/tree.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/tree.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/utils/utils.py` & `sign_language_translator-0.6.1/sign_language_translator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/vision/concatenate.py` & `sign_language_translator-0.6.1/sign_language_translator/vision/concatenate.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/vision/embed.py` & `sign_language_translator-0.6.1/sign_language_translator/vision/embed.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/vision/transforms.py` & `sign_language_translator-0.6.1/sign_language_translator/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/sign_language_translator/vision/visualization.py` & `sign_language_translator-0.6.1/sign_language_translator/vision/visualization.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.6.0/PKG-INFO` & `sign_language_translator-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sign-language-translator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Translate between spoken/text languages and sign language videos using AI.
 Home-page: https://github.com/sign-language-translator/sign-language-translator
 License: Apache-2.0
 Keywords: sign,translation,pose,pakistan,deep-learning,computer-vision,nlp,sign-language,sign-language-translation
 Author: Mudassar Iqbal
 Author-email: mdsriqb@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -45,19 +45,19 @@
 3. [Usage](#usage)
    1. [Command Line](#command-line)
       <!-- 1. [configure](#configure) -->
       1. [$ slt download ...](#download)
       2. [$ slt translate ...](#translate)
       3. [$ slt complete ...](#complete)
    2. [Python](#python)
-      1. [basic translation](#basic-translation)
-      2. [text language processor](#text-language-processor)
-      3. [sign language processor](#sign-language-processor)
-      4. [video/feature processing](#vision)
-      5. [language models](#language-models)
+      1. [Translation](#basics)
+      2. [Text language processor](#text-language-processor)
+      3. [Sign language processor](#sign-language-processor)
+      4. [Video processing](#vision)
+      5. [Language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Upcoming/Roadmap](#upcomingroadmap)
 7. [How to Contribute](#how-to-contribute)
 8. [Credits and Gratitude](#credits-and-gratitude)
 9. [Bonus](#bonus)
    1. Number of lines of code
@@ -223,29 +223,32 @@
 Auto complete a sentence using our language models. This model can write sentences composed of supported words only:
 
 ```bash
 $ slt complete --end-token ">" --model-code urdu-mixed-ngram "<"
 ('<', 'وہ', ' ', 'یہ', ' ', 'نہیں', ' ', 'چاہتا', ' ', 'تھا', '۔', '>')
 ```
 
-These models predict next characters until a specified token appears. (e.g. generating names using a mixture of models):
+<details>
+<summary>These models predict next characters until a specified token appears. (e.g. generating names using a mixture of models):</summary>
 
 ```bash
 $ slt complete \
     --model-code unigram-names --model-weight 1 \
     --model-code bigram-names -w 2 \
     -m trigram-names -w 3 \
     --selection-strategy merge --beam-width 2.5 --end-token "]" \
     "[s"
 [shazala]
 ```
 
+</details>
+
 ### Python
 
-#### basic translation
+#### Basics
 
 ```python
 import sign_language_translator as slt
 
 # download dataset or models (if you need them separate)
 # (by default, dataset is auto-downloaded within the install directory)
 # slt.set_resource_dir("path/to/sign-language-datasets") # optional. Helps when data is synced with cloud
@@ -255,37 +258,39 @@
 
 print("All available models:")
 print(list(slt.ModelCodes)) # from slt.config.enums
 # print(list(slt.TextLanguageCodes))
 # print(list(slt.SignLanguageCodes))
 ```
 
-**Text to Sign**:
+**Text to Sign Translation**:
 
 ```python
 # Load text-to-sign model
 # deep_t2s_model = slt.get_model("t2s-flan-T5-base-01.pt") # pytorch
 # rule-based model (concatenates clips of each word)
 t2s_model = slt.get_model(
-    model_code = "concatenative-synthesis", # slt.ModelCodes.CONCATENATIVE_SYNTHESIS.value
+    model_code = "concatenative-synthesis", # slt.ModelCodes.CONCATENATIVE_SYNTHESIS
     text_language = "urdu", # or object of any child of slt.languages.text.text_language.TextLanguage class
     sign_language = "PakistanSignLanguage", # or object of any child of slt.languages.sign.sign_language.SignLanguage class
     sign_feature_model = "mediapipe_pose_v2_hand_v1",
 )
 
 text = "HELLO دنیا!" # HELLO treated as an acronym
 sign_language_sentence = t2s_model(text)
 
 # moviepy_video_object = sign_language_sentence.video()
 # moviepy_video_object.ipython_display()
 # moviepy_video_object.write_videofile(f"sentences/{text}.mp4")
 ```
 
-**Sign to text**
-dummy code: (will be finalized in v0.8+)
+**Sign to Text Translation**
+
+<details>
+<summary>dummy code: (will be finalized in v0.8+)</summary>
 
 ```python
 # load sign
 video = slt.read_video("video.mp4")
 # features = slt.extract_features(video, "mediapipe_pose_v2_hand_v1")
 
 # Load sign-to-text model
@@ -293,18 +298,21 @@
 features = deep_s2t_model.extract_features(video)
 
 # translate
 text = deep_s2t_model(features)
 print(text)
 ```
 
+</details>
+
 #### Text Language Processor
 
-```python
+Process text strings using language specific classes:
 
+```python
 from sign_language_translator.languages.text import Urdu
 ur_nlp = Urdu()
 
 text = "hello جاؤں COVID-19."
 
 normalized_text = ur_nlp.preprocess(text)
 # normalized_text = 'جاؤں COVID-19.'
@@ -340,15 +348,16 @@
 #   {'signs': [['pk-hfad-1_school']], 'weights': [1.0]},
 #   {'signs': [['pk-hfad-1_گیا']], 'weights': [1.0]}
 # ]
 ```
 
 #### Vision
 
-dummy code: (will be finalized in v0.7)
+<details>
+<summary>dummy code: (will be finalized in v0.7)</summary>
 
 ```python
 import sign_language_translator as slt
 
 # load video
 video = slt.read_video("sign.mp4")
 
@@ -362,17 +371,20 @@
 video = slt.vision.plot_landmarks(features)
 
 # display
 video.show()
 print(features.numpy())
 ```
 
+</details>
+
 #### Language models
 
-Simple statistical n-gram model:
+<details open>
+<summary>Simple statistical n-gram model:</summary>
 
 ```python
 from sign_language_translator.models.language_models import NgramLanguageModel
 
 names_data = [
     '[abeera]', '[areej]',  '[farida]',  '[hiba]',    '[kinza]',
     '[mishal]', '[nimra]',  '[rabbia]',  '[tehmina]', '[zoya]',
@@ -394,15 +406,18 @@
 print(name)
 # '[rabeej]'
 
 # see ngram model's implementation
 print(model.__dict__)
 ```
 
-Mash up multiple language models & complete generation through beam search:
+</details>
+
+<details open>
+<summary>Mash up multiple language models & complete generation through beam search:</summary>
 
 ```python
 from sign_language_translator.models.language_models import MixerLM, BeamSampling, NgramLanguageModel
 
 # using data from previous example
 names_data = [...] # or slt.languages.English().vocab.person_names # concat start/end symbols
 
@@ -429,38 +444,43 @@
 # use Beam Search to find high likelihood names
 sampler = BeamSampling(mixed_model, beam_width=3) #, scoring_function = ...)
 name = sampler.complete('[')
 print(name)
 # [rabbia]
 ```
 
-Write sentences composed of only those words for which sign videos are available so that the rule-based text-to-sign model can generate training examples for a deep learning model:
+</details>
+
+<details open>
+<summary>Write sentences composed of only those words for which sign videos are available so that the rule-based text-to-sign model can generate training examples for a deep learning model:</summary>
 
 ```python
 from sign_language_translator.models.language_models import TransformerLanguageModel
 
 # model = slt.get_model("ur-supported-gpt")
 model = TransformerLanguageModel.load("models/tlm_14.0M.pt")
 # sampler = BeamSampling(model, ...)
 # sampler.complete(["<"])
 
 # see probabilities of all tokens
 model.next_all(["میں", " ", "وزیراعظم", " ",])
 # (["سے", "عمران", ...], [0.1415926535, 0.7182818284, ...])
 ```
 
+</details>
+
 ## Directory Tree
 
 <pre>
 <big><b>sign-language-translator</b></big>
-├── <a href="">MANIFEST.in</a>
-├── <a href="">README.md</a>
-├── <a href="">poetry.lock</a>
-├── <a href="">pyproject.toml</a>
-├── <a href="">requirements.txt</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/MANIFEST.in">MANIFEST.in</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/README.md">README.md</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/poetry.lock">poetry.lock</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/pyproject.toml">pyproject.toml</a>
+├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/requirements.txt">requirements.txt</a>
 ├── <b>tests</b>
 │   └── <a href="https://github.com/sign-language-translator/sign-language-translator/tree/main/tests">*</a>
 │
 └── <big><b>sign_language_translator</b></big>
     ├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/sign_language_translator/cli.py">cli.py</a>
     ├── <b>config</b>
     │   ├── <a href="https://github.com/sign-language-translator/sign-language-translator/blob/main/sign_language_translator/config/enums.py">enums.py</a>
@@ -532,52 +552,82 @@
 
 ## Research Paper
 
 Stay Tuned!
 
 ## Upcoming/Roadmap
 
+<details>
+<summary>CLEAN_ARCHITECTURE_VISION: v0.7</summary>
+
 ```python
-# :CLEAN_ARCHITECTURE_VISION: v0.7
-    # class according to feature type (pose/video/mesh)
-    # video loader
-    # feature extraction
-    # feature augmentation
-    # feature model names enums
-    # subtitles
-    # 2D/3D avatars
+# class according to feature type (pose/video/mesh)
+# video loader
+# feature extraction
+# feature augmentation
+# feature model names enums
+# subtitles
+# 2D/3D avatars
+```
+
+</details>
+
+<details>
+<summary>MISCELLANEOUS</summary>
 
-# push notebooks
+```python
+# clean demonstration notebooks
 # expand reference clip data by scraping everything
 # data info table
 # https://sign-language-translator.readthedocs.io/en/latest/
+# sequence diagram for creating a translator
+```
+
+</details>
+
+<details>
+<summary>DEEP_TRANSLATION: v0.8-v1.x</summary>
+
+```python
+# sign to text with fine-tuned whisper
+# pose vector generation with fine-tuned flan-T5
+# motion transfer
+# pose2video: stable diffusion or GAN?
+# speech to text
+# text to speech
+# LanguageModel: experiment by dropping space tokens
+# parallel text corpus
+```
+
+</details>
 
-# :DEEP_TRANSLATION: v0.8-v1.x
-    # sign to text with fine-tuned whisper
-    # pose vector generation with fine-tuned flan-T5
-    # motion transfer
-    # pose2video: stable diffusion or GAN?
-    # speech to text
-    # text to speech
-    # LanguageModel: experiment by dropping space tokens
-    # parallel text corpus
-
-# RESEARCH PAPERs
-    # datasets: clips, text, sentences, disambiguation
-    # rule based translation: describe entire repo
-    # deep sign-to-text: pipeline + experiments
-    # deep text-to-sign: pipeline + experiments
-
-# PRODUCT DEVELOPMENT
-    # ML inference server
-    # Django backend server
-    # React Frontend
-    # React Native mobile app
+<details>
+<summary>RESEARCH PAPERs</summary>
+
+```python
+# datasets: clips, text, sentences, disambiguation
+# rule based translation: describe entire repo
+# deep sign-to-text: pipeline + experiments
+# deep text-to-sign: pipeline + experiments
+```
+
+</details>
+
+<details>
+<summary>PRODUCT DEVELOPMENT</summary>
+
+```python
+# ML inference server
+# Django backend server
+# React Frontend
+# React Native mobile app
 ```
 
+</details>
+
 ## How to Contribute
 
 - Datasets:
   - Scrape and upload video datasets.
   - Label word mapping datasets.
   - Reach out to to Academies for Deaf and have them write down *sign language grammar*.
 - New Code
@@ -605,15 +655,15 @@
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **9248** + Tests: **877**):
+Count total number of **lines of code** (Package: **9259** + Tests: **885**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for `Fun`**
```

