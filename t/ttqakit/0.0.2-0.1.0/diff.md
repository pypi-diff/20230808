# Comparing `tmp/ttqakit-0.0.2.tar.gz` & `tmp/ttqakit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ttqakit-0.0.2.tar", last modified: Wed Aug  2 10:44:52 2023, max compression
+gzip compressed data, was "dist\ttqakit-0.1.0.tar", last modified: Tue Aug  8 09:13:49 2023, max compression
```

## Comparing `ttqakit-0.0.2.tar` & `ttqakit-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,189 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/
--rw-rw-rw-   0        0        0     1106 2023-08-01 16:10:08.000000 ttqakit-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      790 2023-08-02 10:44:52.000000 ttqakit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-08-02 10:44:38.000000 ttqakit-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 10:44:52.000000 ttqakit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1289 2023-08-02 10:44:50.000000 ttqakit-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:21:22.000000 ttqakit-0.0.2/src/ttqakit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit/evaluation/
--rw-rw-rw-   0        0        0       78 2023-07-29 07:13:46.000000 ttqakit-0.0.2/src/ttqakit/evaluation/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-07-29 07:16:09.000000 ttqakit-0.0.2/src/ttqakit/evaluation/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit/icl/
--rw-rw-rw-   0        0        0      240 2023-07-30 04:02:39.000000 ttqakit-0.0.2/src/ttqakit/icl/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-07-30 04:02:21.000000 ttqakit-0.0.2/src/ttqakit/icl/dataset.py
--rw-rw-rw-   0        0        0    10380 2023-07-31 09:05:34.000000 ttqakit-0.0.2/src/ttqakit/icl/infer.py
--rw-rw-rw-   0        0        0     2092 2023-07-31 08:59:07.000000 ttqakit-0.0.2/src/ttqakit/icl/model.py
--rw-rw-rw-   0        0        0     1576 2023-07-31 08:47:55.000000 ttqakit-0.0.2/src/ttqakit/icl/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit/llama/
--rw-rw-rw-   0        0        0      137 2023-07-28 05:05:47.000000 ttqakit-0.0.2/src/ttqakit/llama/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-07-24 12:08:29.000000 ttqakit-0.0.2/src/ttqakit/llama/data_collator.py
--rw-rw-rw-   0        0        0     6954 2023-07-28 04:56:28.000000 ttqakit-0.0.2/src/ttqakit/llama/dataset.py
--rw-rw-rw-   0        0        0    13616 2023-07-24 12:48:49.000000 ttqakit-0.0.2/src/ttqakit/llama/model.py
--rw-rw-rw-   0        0        0     5944 2023-07-24 12:25:57.000000 ttqakit-0.0.2/src/ttqakit/llama/peft_trainer.py
--rw-rw-rw-   0        0        0     3491 2023-07-24 12:33:59.000000 ttqakit-0.0.2/src/ttqakit/llama/seq2seq.py
--rw-rw-rw-   0        0        0     2634 2023-07-25 14:29:07.000000 ttqakit-0.0.2/src/ttqakit/llama/template.py
--rw-rw-rw-   0        0        0     4638 2023-07-25 14:30:35.000000 ttqakit-0.0.2/src/ttqakit/llama/trainer.py
--rw-rw-rw-   0        0        0    15388 2023-07-26 05:28:20.000000 ttqakit-0.0.2/src/ttqakit/llama/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit/retriever/
--rw-rw-rw-   0        0        0      161 2023-07-28 08:35:13.000000 ttqakit-0.0.2/src/ttqakit/retriever/__init__.py
--rw-rw-rw-   0        0        0     1200 2023-07-24 12:55:17.000000 ttqakit-0.0.2/src/ttqakit/retriever/dataset.py
--rw-rw-rw-   0        0        0     2265 2023-07-26 04:49:46.000000 ttqakit-0.0.2/src/ttqakit/retriever/model.py
--rw-rw-rw-   0        0        0    24036 2023-07-31 08:26:11.000000 ttqakit-0.0.2/src/ttqakit/retriever/trainer.py
--rw-rw-rw-   0        0        0     5220 2023-07-28 03:40:30.000000 ttqakit-0.0.2/src/ttqakit/retriever/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/
--rw-rw-rw-   0        0        0      790 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 10:44:52.000000 ttqakit-0.0.2/src/ttqakit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 09:12:42.000000 ttqakit-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    11286 2023-08-08 09:13:49.000000 ttqakit-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10330 2023-08-08 09:12:42.000000 ttqakit-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/__init__.py
+-rw-rw-rw-   0        0        0    20626 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/app.py
+-rw-rw-rw-   0        0        0      154 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/cli.py
+-rw-rw-rw-   0        0        0      219 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/gunicorn_config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/icl/
+-rw-rw-rw-   0        0        0      248 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/icl/__init__.py
+-rw-rw-rw-   0        0        0     5712 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/icl/dataset.py
+-rw-rw-rw-   0        0        0    11567 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/icl/infer.py
+-rw-rw-rw-   0        0        0     3517 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/icl/model.py
+-rw-rw-rw-   0        0        0     1576 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/icl/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/llama/
+-rw-rw-rw-   0        0        0     4638 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/Trainer.py
+-rw-rw-rw-   0        0        0      146 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/__init__.py
+-rw-rw-rw-   0        0        0     2841 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/data_collator.py
+-rw-rw-rw-   0        0        0     8255 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/dataset.py
+-rw-rw-rw-   0        0        0    13616 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/model.py
+-rw-rw-rw-   0        0        0     6085 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/peft_trainer.py
+-rw-rw-rw-   0        0        0     3580 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/seq2seq.py
+-rw-rw-rw-   0        0        0     2701 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/template.py
+-rw-rw-rw-   0        0        0    15388 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/llama/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/loaders/
+-rw-rw-rw-   0        0        0     3119 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/FinQA.py
+-rw-rw-rw-   0        0        0     4164 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/HiTab.py
+-rw-rw-rw-   0        0        0     4245 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/HybridQA.py
+-rw-rw-rw-   0        0        0     2744 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/MultiHiertt.py
+-rw-rw-rw-   0        0        0     6566 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/MultimodalQA.py
+-rw-rw-rw-   0        0        0     3356 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/SpreadSheetQA.py
+-rw-rw-rw-   0        0        0     2569 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/TATQA.py
+-rw-rw-rw-   0        0        0     2914 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/WikiSQL.py
+-rw-rw-rw-   0        0        0     2323 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/WikiTableQuestions.py
+-rw-rw-rw-   0        0        0      663 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/loaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/
+-rw-rw-rw-   0        0        0      112 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/__init__.py
+-rw-rw-rw-   0        0        0     4742 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/dataset.py
+-rw-rw-rw-   0        0        0     2292 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/model.py
+-rw-rw-rw-   0        0        0    11079 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/trainer.py
+-rw-rw-rw-   0        0        0     5492 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/classifier_module/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/
+-rw-rw-rw-   0        0        0       29 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/__init__.py
+-rw-rw-rw-   0        0        0     3013 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/args.py
+-rw-rw-rw-   0        0        0     9860 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/main.py
+-rw-rw-rw-   0        0        0    11580 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/mmqa.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/qa/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/qa/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/qa/openai_qa.py
+-rw-rw-rw-   0        0        0     4405 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/qa/prompt.py
+-rw-rw-rw-   0        0        0     6053 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/mmhqa_icl/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/
+-rw-rw-rw-   0        0        0      111 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/__init__.py
+-rw-rw-rw-   0        0        0     8063 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/dataset.py
+-rw-rw-rw-   0        0        0     2147 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/model.py
+-rw-rw-rw-   0        0        0    11722 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/trainer.py
+-rw-rw-rw-   0        0        0     5484 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/retriever_module/utils.py
+-rw-rw-rw-   0        0        0      398 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/test_classifier.py
+-rw-rw-rw-   0        0        0      200 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/test_mmhqa_icl.py
+-rw-rw-rw-   0        0        0      363 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/test_retriever.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/utils/
+-rw-rw-rw-   0        0        0       26 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/utils/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/utils/eval_retriever.py
+-rw-rw-rw-   0        0        0      774 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/utils/image_stuff.py
+-rw-rw-rw-   0        0        0     3707 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/mmqa_utils/utils/retriever.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/multihop/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/multihop/Noise_free/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Noise_free/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Noise_free/evaluate_script.py
+-rw-rw-rw-   0        0        0    22071 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Noise_free/read.py
+-rw-rw-rw-   0        0        0    20935 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Noise_free/retrieve.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/
+-rw-rw-rw-   0        0        0      129 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/__init__.py
+-rw-rw-rw-   0        0        0     9878 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/dataset.py
+-rw-rw-rw-   0        0        0     2918 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/evaluate_script1.py
+-rw-rw-rw-   0        0        0     1972 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/model.py
+-rw-rw-rw-   0        0        0    13242 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/trainer.py
+-rw-rw-rw-   0        0        0     1400 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Read/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/
+-rw-rw-rw-   0        0        0      106 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/__init__.py
+-rw-rw-rw-   0        0        0     6306 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/dataset.py
+-rw-rw-rw-   0        0        0     1419 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/model.py
+-rw-rw-rw-   0        0        0     5697 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/trainer.py
+-rw-rw-rw-   0        0        0     2052 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/Retrieval/utils.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/__init__.py
+-rw-rw-rw-   0        0        0     1316 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/main_reader.py
+-rw-rw-rw-   0        0        0     1160 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/multihop/main_retriever.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/__init__.py
+-rw-rw-rw-   0        0        0     3662 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/data_util.py
+-rw-rw-rw-   0        0        0      761 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/dataset_util.py
+-rw-rw-rw-   0        0        0    47637 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/file_utils.py
+-rw-rw-rw-   0        0        0      828 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/in_order.py
+-rw-rw-rw-   0        0        0     1882 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/pre_order.py
+-rw-rw-rw-   0        0        0      942 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/pre_order_ext.py
+-rw-rw-rw-   0        0        0    18432 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/tatqa_batch_gen.py
+-rw-rw-rw-   0        0        0    64258 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/tatqa_dataset.py
+-rw-rw-rw-   0        0        0    52249 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/tatqa_dataset_test.py
+-rw-rw-rw-   0        0        0    15666 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/tatqa_test_batch_gen.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/dummy_flax_objects.py
+-rw-rw-rw-   0        0        0    46876 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/dummy_pt_objects.py
+-rw-rw-rw-   0        0        0     2510 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/dummy_sentencepiece_objects.py
+-rw-rw-rw-   0        0        0    29492 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/dummy_tf_objects.py
+-rw-rw-rw-   0        0        0     6065 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/dummy_tokenizers_objects.py
+-rw-rw-rw-   0        0        0     4512 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/hp_naming.py
+-rw-rw-rw-   0        0        0     7267 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/logging.py
+-rw-rw-rw-   0        0        0    14640 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/notebook.py
+-rw-rw-rw-   0        0        0    40169 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/data/utils/sentencepiece_model_pb2.py
+-rw-rw-rw-   0        0        0     3126 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/options.py
+-rw-rw-rw-   0        0        0     4342 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/predictor.py
+-rw-rw-rw-   0        0        0     2438 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/prepare_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/
+-rw-rw-rw-   0        0        0     1991 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/Vocabulary.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/functions.py
+-rw-rw-rw-   0        0        0     3695 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/masked_cross_entropy.py
+-rw-rw-rw-   0        0        0     6779 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/model.py
+-rw-rw-rw-   0        0        0     9672 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/model_functions.py
+-rw-rw-rw-   0        0        0     9506 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/model_utils.py
+-rw-rw-rw-   0        0        0    18102 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/modeling_reghnt.py
+-rw-rw-rw-   0        0        0    10411 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/modeling_tree.py
+-rw-rw-rw-   0        0        0    38128 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/new_model.py
+-rw-rw-rw-   0        0        0     7088 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/tools/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/tools/__init__.py
+-rw-rw-rw-   0        0        0    62605 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/tools/allennlp.py
+-rw-rw-rw-   0        0        0     8882 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/tools/util.py
+-rw-rw-rw-   0        0        0     4472 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/util.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/dummy_flax_objects.py
+-rw-rw-rw-   0        0        0    46876 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/dummy_pt_objects.py
+-rw-rw-rw-   0        0        0     2510 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/dummy_sentencepiece_objects.py
+-rw-rw-rw-   0        0        0    29492 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/dummy_tf_objects.py
+-rw-rw-rw-   0        0        0     6065 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/dummy_tokenizers_objects.py
+-rw-rw-rw-   0        0        0     4512 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/hp_naming.py
+-rw-rw-rw-   0        0        0     7267 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/logging.py
+-rw-rw-rw-   0        0        0    14640 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/notebook.py
+-rw-rw-rw-   0        0        0    40169 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/reghnt/utils/sentencepiece_model_pb2.py
+-rw-rw-rw-   0        0        0     4627 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/reg_hnt/trainer.py
+-rw-rw-rw-   0        0        0     2296 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/tatqa_eval.py
+-rw-rw-rw-   0        0        0    14420 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/tatqa_metric.py
+-rw-rw-rw-   0        0        0     5243 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/tatqa_metric_test.py
+-rw-rw-rw-   0        0        0     5805 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/tatqa_utils.py
+-rw-rw-rw-   0        0        0     1261 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/Pointer/tatqa_utils_test.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/
+-rw-rw-rw-   0        0        0      161 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/__init__.py
+-rw-rw-rw-   0        0        0     1200 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/dataset.py
+-rw-rw-rw-   0        0        0     2265 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/model.py
+-rw-rw-rw-   0        0        0    24685 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/trainer.py
+-rw-rw-rw-   0        0        0     5220 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/numerical/retriever/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/retriever/
+-rw-rw-rw-   0        0        0      163 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/retriever/__init__.py
+-rw-rw-rw-   0        0        0     1200 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/retriever/dataset.py
+-rw-rw-rw-   0        0        0     2265 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/retriever/model.py
+-rw-rw-rw-   0        0        0    24610 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/retriever/trainer.py
+-rw-rw-rw-   0        0        0     5220 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/retriever/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/structs/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/structs/__init__.py
+-rw-rw-rw-   0        0        0     6081 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/structs/data.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/structuredqa/
+-rw-rw-rw-   0        0        0       30 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/structuredqa/__init__.py
+-rw-rw-rw-   0        0        0    28462 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/structuredqa/structuredqakit.py
+-rw-rw-rw-   0        0        0     2357 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/structuredqa/test.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/TableQAKit/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/utils/__init__.py
+-rw-rw-rw-   0        0        0     5066 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/utils/excel.py
+-rw-rw-rw-   0        0        0     8481 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/utils/export.py
+-rw-rw-rw-   0        0        0     3474 2023-08-08 09:12:42.000000 ttqakit-0.1.0/TableQAKit/utils/program_to_instruction.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 09:13:49.000000 ttqakit-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2000 2023-08-08 09:13:37.000000 ttqakit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/
+-rw-rw-rw-   0        0        0    11286 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6997 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 09:13:49.000000 ttqakit-0.1.0/ttqakit.egg-info/top_level.txt
```

### Comparing `ttqakit-0.0.2/LICENSE` & `ttqakit-0.1.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 ÚFAL MFF UK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ttqakit-0.0.2/src/ttqakit/icl/dataset.py` & `ttqakit-0.1.0/TableQAKit/icl/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,7 +137,36 @@
     def read_demos(self, demo_path: str) -> List[Dict[str, any]]:
         if demo_path is not None:
             return json.load(
                 open(demo_path, 'r', encoding='utf-8')
             )
         else:
             return []
+
+
+class TAT_QA(GPTDataSet):
+    def read_data(self, data_path: str) -> List[Dict[str, any]]:
+        data_list = []
+        data = json.load(
+            open(data_path, 'r', encoding='utf-8')
+        )
+        for one in data:
+            rows = one["table"]["table"]
+            texts = []
+            for p in one["paragraphs"]:
+                texts.append(p["text"])
+            for question in one["questions"]:
+                data_list.append({
+                    "id": question["uid"],
+                    "question": question["question"],
+                    "texts": texts,
+                    "rows": rows,
+                })
+        return data_list
+
+    def read_demos(self, demo_path: str) -> List[Dict[str, any]]:
+        if demo_path is not None:
+            return json.load(
+                open(demo_path, 'r', encoding='utf-8')
+            )
+        else:
+            return []
```

### Comparing `ttqakit-0.0.2/src/ttqakit/icl/infer.py` & `ttqakit-0.1.0/TableQAKit/icl/infer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 import os
 import sys
 from abc import ABC, abstractmethod
-from typing import List, Union, Dict
+from typing import List, Union, Dict, Optional
 from transformers import HfArgumentParser
 from icl import GPT, fix_seed, Logger, print_time, ICLArguments
 from icl import GPTDataSet
 
 
 class ICL(ABC):
     def __init__(self, model: GPT, dataset: GPTDataSet):
         self.args = HfArgumentParser(ICLArguments).parse_args_into_dataclasses()[0]
         self.model = model
         self.dataset = dataset
         fix_seed(self.args.random_seed)
 
-    def infer(self, cot_trigger, answer_trigger):
+    def infer(self, demo_prefix: Optional[str], cot_trigger: Optional[str], answer_trigger: str):
         print('-' * 20)
         print(self.args)
         print('-' * 20)
         if not os.path.exists(self.args.logging_dir):
             os.mkdir(self.args.logging_dir)
         sys.stdout = Logger(os.path.join(self.args.logging_dir, print_time(1) + '.log'), sys.stdout)
         print_time()
-        demo_input = self.create_demo_input(self.dataset.demos, cot_trigger, answer_trigger)
+        demo_input = self.create_demo_input(self.dataset.demos, demo_prefix, cot_trigger, answer_trigger)
 
         self.model.set_prompt(demo_input)
         for i, one in enumerate(self.dataset.data):
             if i < self.args.resume_id - 1:
                 continue
             print('-' * 20)
             print("{}st data".format(i + 1))
@@ -80,21 +80,23 @@
                 res += ("| " + cell + " ")
             else:
                 res += "| - "
         return res + "|"
 
     @abstractmethod
     def create_demo_input(
-        self,
-        demos: List[Dict[str, str]],
-        cot_trigger: str,
-        answer_trigger: str,
+            self,
+            demos: List[Dict[str, str]],
+            demo_prefix: Optional[str],
+            cot_trigger: Optional[str],
+            answer_trigger: str,
     ) -> Union[str, List[Dict[str, str]]]:
         """
         According to the demos from the dataset, create the demo that will be input to the openai model
+        :param demo_prefix: The prefix of demo_input like "Reading the texts and tables and try your best to answer the question."
         :param demos: demos list from the dataset.create_demos()
         :param cot_trigger: the prompt to trigger cot like "Let's think step by step."
         :param answer_trigger: the prompt to trigger the answer like "Therefore, the answer is "
         :return: str for davinci like
         "Q: demo1
          A: answer1
 
@@ -106,19 +108,19 @@
          {"role": "user", "content": demo2}, {"role": "assistant", "content": answer2},
          ……]
         """
         pass
 
     @abstractmethod
     def create_data_input(
-        self,
-        data: Dict[str, str],
-        cot_trigger: str,
-        answer_trigger: str,
-        truncation: int
+            self,
+            data: Dict[str, str],
+            cot_trigger: Optional[str],
+            answer_trigger: str,
+            truncation: int
     ) -> str:
         """
         According to the data from the dataset, create the data that will be input to the openai model
         :param data: one data from the dataset
         :param cot_trigger: the prompt to trigger cot like "Let's think step by step."
         :param answer_trigger: the prompt to trigger the answer like "Therefore, the answer is "
         :param truncation: cut off the max length of content
@@ -137,44 +139,53 @@
         :param answer_extract: answer from gpt_output.split(answer_trigger)[-1]
         :return: processing the answer if needed.
         """
         pass
 
     @abstractmethod
     def save_prediction(
-        self,
-        output_path: str,
-        data: Dict[str, str],
-        answer: str
+            self,
+            output_path: str,
+            data: Dict[str, str],
+            answer: str
     ) -> None:
         """
         Saving the answer with the form that you are fond of
         :param output_path: your arg input
         :param data: one data from the dataset
         :param answer: the answer after post-processing.
         :return: None
         """
         pass
 
 
 class turboICL(ICL):
-    def create_demo_input(self, demos: List[dict], cot_trigger: str, answer_trigger: str) -> Union[str, List[Dict[str, str]]]:
-        demo_input = [{"role": "user", "content": "Reading the texts and tables and try your best to answer the question."}]
+    def create_demo_input(self, demos: List[dict], demo_prefix: Optional[str], cot_trigger: Optional[str], answer_trigger: str) -> Union[str, List[Dict[str, str]]]:
+        if demo_prefix is not None:
+            demo_input = [{"role": "user", "content": demo_prefix}]
+        else:
+            demo_input = []
         for demo in demos:
             demo_input.append({
                 "role": "user",
                 "content": demo["question"]
             })
-            demo_input.append({
-                "role": "assistant",
-                "content": cot_trigger + demo["rationale"] + answer_trigger + demo["answer"]
-            })
+            if cot_trigger is not None:
+                demo_input.append({
+                    "role": "assistant",
+                    "content": cot_trigger + demo["rationale"] + answer_trigger + demo["answer"]
+                })
+            else:
+                demo_input.append({
+                    "role": "assistant",
+                    "content": answer_trigger + demo["answer"]
+                })
         return demo_input
 
-    def create_data_input(self, data: dict, cot_trigger: str, answer_trigger: str, truncation: int) -> str:
+    def create_data_input(self, data: dict, cot_trigger: Optional[str], answer_trigger: Optional[str], truncation: int) -> str:
         heads = []
         content = ""
         if data["texts"] is not None and len(data["texts"]):
             content += "paragraphs:\n"
             for text in data["texts"]:
                 content += (text + "\n")
         if data["rows"] is not None and len(data["rows"]):
@@ -185,49 +196,59 @@
                 elif self.args.use_table_flatten:
                     if i == 0:
                         heads = row
                     else:
                         content += (self.table_flatten(heads, row) + "\n")
                 else:
                     raise NotImplementedError
-        question = "question:\n" + data["question"] + "\n" + cot_trigger
+        if cot_trigger is not None:
+            question = "question:\n" + data["question"] + "\n" + cot_trigger
+        else:
+            question = "question:\n" + data["question"]
         if len(content) > truncation - len(question):
-            content = content[:truncation - len(question)]
+            content = content[:truncation - len(question) - 1] + '\n'
         content += question
         return content
 
     def answer_post_proc(self, answer_extract: str) -> str:
         return answer_extract
 
     def save_prediction(self, output_path: str, data: dict, answer: str) -> None:
         if not os.path.isfile(output_path):
             with open(output_path, 'w') as file:
                 json.dump([], file)
         output_data = {
             "uid": data["id"],
             "predicted_program": [],
             "predicted_ans": answer
-            }
+        }
         with open(output_path, 'r+') as file:
             file_data = json.load(file)
             file_data.append(output_data)
             file.seek(0)
             json.dump(file_data, file, indent=4)
 
 
 class davinciICL(ICL):
-    def create_demo_input(self, demos: List[dict], cot_trigger: str, answer_trigger: str) -> Union[str, List[Dict[str, str]]]:
-        demo_input = "Reading the texts and tables and try your best to answer the question.\n\n"
+    def create_demo_input(self, demos: List[dict], demo_prefix: Optional[str], cot_trigger: Optional[str], answer_trigger: str) -> Union[str, List[Dict[str, str]]]:
+        if demo_prefix is not None:
+            demo_input = demo_prefix + "\n"
+        else:
+            demo_input = ""
         for demo in demos:
-            demo_input += ("Q: " + demo["question"] + "\n" +
-                           "A: " + cot_trigger + demo["rationale"] +
-                           answer_trigger + demo["answer"] + "\n\n")
+            if cot_trigger is not None:
+                demo_input += ("Q: " + demo["question"] + "\n" +
+                               "A: " + cot_trigger + demo["rationale"] +
+                               answer_trigger + demo["answer"] + "\n\n")
+            else:
+                demo_input += ("Q: " + demo["question"] + "\n" +
+                               "A: " + answer_trigger + demo["answer"] + "\n\n")
         return demo_input
 
-    def create_data_input(self, data: dict, cot_trigger: str, answer_trigger: str, truncation: int) -> str:
+    def create_data_input(self, data: dict, cot_trigger: Optional[str], answer_trigger: str, truncation: int) -> str:
         heads = []
         content = "Q: \n"
         if data["texts"] is not None and len(data["texts"]):
             content += "paragraphs:\n"
             for text in data["texts"]:
                 content += (text + "\n")
         if data["rows"] is not None and len(data["rows"]):
@@ -238,30 +259,33 @@
                 elif self.args.use_table_flatten:
                     if i == 0:
                         heads = row
                     else:
                         content += (self.table_flatten(heads, row) + "\n")
                 else:
                     raise NotImplementedError
-        question = "question:\n" + data["question"] + "\n" + "A: " + cot_trigger
+        if cot_trigger is not None:
+            question = "question:\n" + data["question"] + "\n" + "A: " + cot_trigger
+        else:
+            question = "question:\n" + data["question"] + "\n" + "A: "
         if len(content) > truncation - len(question):
-            content = content[:truncation - len(question)]
+            content = content[:truncation - len(question) - 1] + '\n'
         content += question
         return content
 
     def answer_post_proc(self, answer_extract: str) -> str:
         return answer_extract
 
     def save_prediction(self, output_path: str, data: dict, answer: str) -> None:
         if not os.path.isfile(output_path):
             with open(output_path, 'w') as file:
                 json.dump([], file)
         output_data = {
             "uid": data["id"],
             "predicted_program": [],
             "predicted_ans": answer
-            }
+        }
         with open(output_path, 'r+') as file:
             file_data = json.load(file)
             file_data.append(output_data)
             file.seek(0)
             json.dump(file_data, file, indent=4)
```

### Comparing `ttqakit-0.0.2/src/ttqakit/icl/utils.py` & `ttqakit-0.1.0/TableQAKit/icl/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     max_length: int = field(default=256)
     api_time_interval: float = field(default=1.0)
     temperature: float = field(default=0.1)
     logging_dir: str = field(default='./log')
     output_path: str = field(default='./data/test_predictions.json')
     use_table_markdown: bool = field(default=True)
     use_table_flatten: bool = field(default=False)
-    truncation: int = field(default=4000)
+    truncation: int = field(default=3000)
 
 
 class Logger(object):
     def __init__(self, logging_path, stream=io.TextIOWrapper(sys.stdout.buffer, encoding='utf8')):
         self.terminal = stream
         self.log = open(logging_path, 'a', encoding='utf-8')
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/data_collator.py` & `ttqakit-0.1.0/TableQAKit/llama/data_collator.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import torch
-
-from typing import Dict, Optional, Sequence, Union
-
-from transformers import DataCollatorWithPadding, BatchEncoding
-from transformers.tokenization_utils import PreTrainedTokenizer
-
-from .utils import IGNORE_INDEX
-
-
-class DynamicDataCollatorWithPadding(DataCollatorWithPadding):
-    r"""
-    Inherits DataCollatorWithPadding. It is capable of dynamically padding for batched data.
-    """
-    def __init__(
-            self,
-            tokenizer: PreTrainedTokenizer,
-            ignore_pad_token_for_loss: Optional[bool] = False
-    ):
-        super().__init__(tokenizer, padding=True)
-        self.label_pad_token_id = IGNORE_INDEX if ignore_pad_token_for_loss else tokenizer.pad_token_id
-
-    def get_attention_masks(self, input_ids: torch.Tensor, device: torch.device) -> torch.Tensor:
-        r"""
-        Generates attention masks for left-padded sequences.
-        """
-        batch_size, seq_length = input_ids.size()
-        attention_mask = torch.ones((batch_size, seq_length), device=device)
-
-        for i, seq in enumerate(input_ids):
-            attention_mask[i, :(seq != self.tokenizer.pad_token_id).nonzero()[0].item()] = 0 # padding
-
-        attention_mask = attention_mask.bool()
-        return attention_mask
-
-    def __call__(self, features: Sequence[Dict[str, Union[torch.Tensor, Sequence[int]]]]) -> BatchEncoding:
-        r"""
-        Pads batched data to the longest sequence in the batch.
-
-        We adopt left-padding in both training and evaluation.
-        """
-        if isinstance(features[0]["input_ids"], torch.Tensor):
-            input_ids = [feature["input_ids"].clone().detach().flip(0) for feature in features]
-        else:
-            input_ids = [torch.tensor(feature["input_ids"]).flip(0) for feature in features]
-
-        if "labels" in features[0]:
-            if isinstance(features[0]["labels"], torch.Tensor):
-                labels = [feature["labels"].clone().detach().flip(0) for feature in features]
-            else:
-                labels = [torch.tensor(feature["labels"]).flip(0) for feature in features]
-            input_ids = input_ids + labels # pad them to the same length
-
-        input_ids = torch.nn.utils.rnn.pad_sequence(
-            input_ids,
-            batch_first=True,
-            padding_value=self.tokenizer.pad_token_id
-        ).flip(-1)
-
-        batch = {}
-
-        if "labels" in features[0]:
-            input_ids, labels = input_ids.split(len(features), dim=0)
-            labels = torch.where(labels != self.tokenizer.pad_token_id, labels, self.label_pad_token_id)
-            batch["labels"] = labels
-
-        batch["input_ids"] = input_ids
-        batch["attention_mask"] = self.get_attention_masks(input_ids, device=input_ids.device)
-
-        return BatchEncoding(batch)
-
+import torch
+
+from typing import Dict, Optional, Sequence, Union
+
+from transformers import DataCollatorWithPadding, BatchEncoding
+from transformers.tokenization_utils import PreTrainedTokenizer
+
+from .utils import IGNORE_INDEX
+
+
+class DynamicDataCollatorWithPadding(DataCollatorWithPadding):
+    r"""
+    Inherits DataCollatorWithPadding. It is capable of dynamically padding for batched data.
+    """
+    def __init__(
+            self,
+            tokenizer: PreTrainedTokenizer,
+            ignore_pad_token_for_loss: Optional[bool] = False
+    ):
+        super().__init__(tokenizer, padding=True)
+        self.label_pad_token_id = IGNORE_INDEX if ignore_pad_token_for_loss else tokenizer.pad_token_id
+
+    def get_attention_masks(self, input_ids: torch.Tensor, device: torch.device) -> torch.Tensor:
+        r"""
+        Generates attention masks for left-padded sequences.
+        """
+        batch_size, seq_length = input_ids.size()
+        attention_mask = torch.ones((batch_size, seq_length), device=device)
+
+        for i, seq in enumerate(input_ids):
+            attention_mask[i, :(seq != self.tokenizer.pad_token_id).nonzero()[0].item()] = 0 # padding
+
+        attention_mask = attention_mask.bool()
+        return attention_mask
+
+    def __call__(self, features: Sequence[Dict[str, Union[torch.Tensor, Sequence[int]]]]) -> BatchEncoding:
+        r"""
+        Pads batched data to the longest sequence in the batch.
+
+        We adopt left-padding in both training and evaluation.
+        """
+        if isinstance(features[0]["input_ids"], torch.Tensor):
+            input_ids = [feature["input_ids"].clone().detach().flip(0) for feature in features]
+        else:
+            input_ids = [torch.tensor(feature["input_ids"]).flip(0) for feature in features]
+
+        if "labels" in features[0]:
+            if isinstance(features[0]["labels"], torch.Tensor):
+                labels = [feature["labels"].clone().detach().flip(0) for feature in features]
+            else:
+                labels = [torch.tensor(feature["labels"]).flip(0) for feature in features]
+            input_ids = input_ids + labels # pad them to the same length
+
+        input_ids = torch.nn.utils.rnn.pad_sequence(
+            input_ids,
+            batch_first=True,
+            padding_value=self.tokenizer.pad_token_id
+        ).flip(-1)
+
+        batch = {}
+
+        if "labels" in features[0]:
+            input_ids, labels = input_ids.split(len(features), dim=0)
+            labels = torch.where(labels != self.tokenizer.pad_token_id, labels, self.label_pad_token_id)
+            batch["labels"] = labels
+
+        batch["input_ids"] = input_ids
+        batch["attention_mask"] = self.get_attention_masks(input_ids, device=input_ids.device)
+
+        return BatchEncoding(batch)
+
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/dataset.py` & `ttqakit-0.1.0/TableQAKit/llama/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -149,7 +149,40 @@
 
         for data_sample in dataset:
             for column_name in column_names:
                 huggingface_data[column_name].append(data_sample[column_name])
 
         hf_dataset = Dataset.from_dict(huggingface_data)
         return hf_dataset
+
+
+class CompAQT(LLaMaDataset):
+    def __read_data_to_huggingface_dataset__(self, data_path: str) -> Dataset:
+        column_names = ["prefix", "prompt", "query", "response", "history"]
+        data = json.load(
+            open(data_path, 'r', encoding='utf-8')
+        )
+        dataset = []
+        for one in data:
+            texts = "paragraphs: \n"
+            tables = "table descriptions: \n"
+            for k, v in one["qa"]["gold_inds"].items():
+                if "text" in k:
+                    texts += (v + "\n")
+                if "table" in k:
+                    tables += (v + "\n")
+            dataset.append({
+                "prefix": None,
+                "prompt": "According to the paragraphs and table descriptions, try your best to answer the question: " + one["qa"]["question"],
+                "query": texts + tables,
+                "response": one["qa"]["program"],
+                "history": None
+            })
+
+        huggingface_data = {column_name: [] for column_name in column_names}
+
+        for data_sample in dataset:
+            for column_name in column_names:
+                huggingface_data[column_name].append(data_sample[column_name])
+
+        hf_dataset = Dataset.from_dict(huggingface_data)
+        return hf_dataset
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/model.py` & `ttqakit-0.1.0/TableQAKit/llama/model.py`

 * *Files identical despite different names*

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/peft_trainer.py` & `ttqakit-0.1.0/TableQAKit/llama/peft_trainer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import os
-import json
-import time
-import torch
-from typing import Dict, Optional
-from datetime import timedelta
-
-from transformers import (
-    Seq2SeqTrainer,
-    TrainerCallback,
-    TrainerControl,
-    TrainerState,
-    TrainingArguments
-)
-
-from transformers.trainer import TRAINING_ARGS_NAME
-from transformers.modeling_utils import unwrap_model
-
-from .utils import (
-    get_logger,
-    FinetuningArguments,
-    FINETUNING_ARGS_NAME,
-    VALUE_HEAD_FILE_NAME
-)
-
-from .model import (
-    get_state_dict,
-    load_trainable_params,
-    load_valuehead_params
-)
-
-
-logger = get_logger(__name__)
-
-
-class LogCallback(TrainerCallback):
-    r"""
-    TrainerCallback includes the state function during training, for more details refer to the TrainerCallback class.
-    The on_log function primarily collects process parameters during training, such as training loss, learning rate,
-    and training epochs, as well as progress parameters like the current percentage progress and estimated remaining
-    time. Every time a log is triggered, a new record is appended to the file "messages.log" for dynamic visualization
-    purposes.
-    """
-
-    def __init__(self):
-        self.start_time = time.time()
-
-    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
-        r"""
-        Event called after logging the last logs.
-        """
-        if "loss" not in state.log_history[-1]:
-            return
-        cur_time = time.time()
-        cur_steps = state.log_history[-1].get("step")
-        elapsed_time = cur_time - self.start_time
-        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
-        remaining_steps = state.max_steps - cur_steps
-        remaining_time = remaining_steps * avg_time_per_step
-        log_dict = {
-            "current_steps": cur_steps,
-            "total_steps": state.max_steps,
-            "loss": state.log_history[-1].get("loss", None),
-            "reward": state.log_history[-1].get("reward", None),
-            "learning_rate": state.log_history[-1].get("learning_rate", None),
-            "epoch": state.log_history[-1].get("epoch", None),
-            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
-            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
-            "remaining_time": str(timedelta(seconds=int(remaining_time)))
-        }
-        os.makedirs(args.output_dir, exist_ok=True)
-        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a") as f:
-            f.write(json.dumps(log_dict) + "\n")
-
-
-class PeftTrainer(Seq2SeqTrainer):
-    r"""
-    Inherits Seq2SeqTrainer to support parameter-efficient checkpoints.
-    """
-
-    def __init__(self, finetuning_args: FinetuningArguments, **kwargs):
-        super().__init__(**kwargs)
-        self.finetuning_args = finetuning_args
-        if self.is_world_process_zero() and os.path.exists(os.path.join(self.args.output_dir, "trainer_log.jsonl")):
-            logger.warning("Previous log file in this folder will be deleted.")
-            os.remove(os.path.join(self.args.output_dir, "trainer_log.jsonl"))
-
-    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, torch.Tensor]] = None) -> None:
-        r"""
-        Saves trainable parameters as model checkpoint.
-
-        This function will only be executed at the process zero.
-
-        Subclass and override to inject custom behavior. It should not be directly used by external scripts.
-        """
-        output_dir = output_dir if output_dir is not None else self.args.output_dir
-        os.makedirs(output_dir, exist_ok=True)
-        logger.info(f"Saving model checkpoint to {output_dir}")
-        model = unwrap_model(self.model)
-
-        if hasattr(model, "pretrained_model"): # for models with valuehead (currently using LoRA only)
-            backbone_model = getattr(model, "pretrained_model")
-            torch.save(get_state_dict(getattr(model, "v_head")), os.path.join(output_dir, VALUE_HEAD_FILE_NAME))
-        else:
-            backbone_model = model
-
-        if self.finetuning_args.finetuning_type == "lora":
-            backbone_model.save_pretrained(output_dir, state_dict=get_state_dict(backbone_model))
-        else: # freeze/full tuning
-            backbone_model.save_pretrained(
-                output_dir,
-                state_dict=get_state_dict(backbone_model),
-                safe_serialization=self.args.save_safetensors
-            )
-            if self.tokenizer is not None:
-                self.tokenizer.save_pretrained(output_dir)
-
-        with open(os.path.join(output_dir, TRAINING_ARGS_NAME), "w", encoding="utf-8") as f:
-            f.write(self.args.to_json_string() + "\n")
-        self.finetuning_args.save_to_json(os.path.join(output_dir, FINETUNING_ARGS_NAME))
-
-    def _load_best_model(self):
-        r"""
-        Loads trainable parameters from model checkpoint.
-
-        Subclass and override to inject custom behavior. It should not be directly used by external scripts.
-        """
-        logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
-
-        model = unwrap_model(self.model)
-        backbone_model = getattr(model, "pretrained_model") if hasattr(model, "pretrained_model") else model
-
-        if self.finetuning_args.finetuning_type == "lora":
-            backbone_model.load_adapter(self.state.best_model_checkpoint, getattr(backbone_model, "active_adapter"))
-            if hasattr(model, "v_head") and load_valuehead_params(model, self.state.best_model_checkpoint):
-                model.v_head.load_state_dict({
-                    "summary.weight": getattr(model, "reward_head_weight"),
-                    "summary.bias": getattr(model, "reward_head_bias")
-                })
-        else: # freeze/full-tuning
-            load_trainable_params(backbone_model, self.state.best_model_checkpoint)
+import os
+import json
+import time
+import torch
+from typing import Dict, Optional
+from datetime import timedelta
+
+from transformers import (
+    Seq2SeqTrainer,
+    TrainerCallback,
+    TrainerControl,
+    TrainerState,
+    TrainingArguments
+)
+
+from transformers.trainer import TRAINING_ARGS_NAME
+from transformers.modeling_utils import unwrap_model
+
+from .utils import (
+    get_logger,
+    FinetuningArguments,
+    FINETUNING_ARGS_NAME,
+    VALUE_HEAD_FILE_NAME
+)
+
+from .model import (
+    get_state_dict,
+    load_trainable_params,
+    load_valuehead_params
+)
+
+
+logger = get_logger(__name__)
+
+
+class LogCallback(TrainerCallback):
+    r"""
+    TrainerCallback includes the state function during training, for more details refer to the TrainerCallback class.
+    The on_log function primarily collects process parameters during training, such as training loss, learning rate,
+    and training epochs, as well as progress parameters like the current percentage progress and estimated remaining
+    time. Every time a log is triggered, a new record is appended to the file "messages.log" for dynamic visualization
+    purposes.
+    """
+
+    def __init__(self):
+        self.start_time = time.time()
+
+    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
+        r"""
+        Event called after logging the last logs.
+        """
+        if "loss" not in state.log_history[-1]:
+            return
+        cur_time = time.time()
+        cur_steps = state.log_history[-1].get("step")
+        elapsed_time = cur_time - self.start_time
+        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
+        remaining_steps = state.max_steps - cur_steps
+        remaining_time = remaining_steps * avg_time_per_step
+        log_dict = {
+            "current_steps": cur_steps,
+            "total_steps": state.max_steps,
+            "loss": state.log_history[-1].get("loss", None),
+            "reward": state.log_history[-1].get("reward", None),
+            "learning_rate": state.log_history[-1].get("learning_rate", None),
+            "epoch": state.log_history[-1].get("epoch", None),
+            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
+            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
+            "remaining_time": str(timedelta(seconds=int(remaining_time)))
+        }
+        os.makedirs(args.output_dir, exist_ok=True)
+        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a") as f:
+            f.write(json.dumps(log_dict) + "\n")
+
+
+class PeftTrainer(Seq2SeqTrainer):
+    r"""
+    Inherits Seq2SeqTrainer to support parameter-efficient checkpoints.
+    """
+
+    def __init__(self, finetuning_args: FinetuningArguments, **kwargs):
+        super().__init__(**kwargs)
+        self.finetuning_args = finetuning_args
+        if self.is_world_process_zero() and os.path.exists(os.path.join(self.args.output_dir, "trainer_log.jsonl")):
+            logger.warning("Previous log file in this folder will be deleted.")
+            os.remove(os.path.join(self.args.output_dir, "trainer_log.jsonl"))
+
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, torch.Tensor]] = None) -> None:
+        r"""
+        Saves trainable parameters as model checkpoint.
+
+        This function will only be executed at the process zero.
+
+        Subclass and override to inject custom behavior. It should not be directly used by external scripts.
+        """
+        output_dir = output_dir if output_dir is not None else self.args.output_dir
+        os.makedirs(output_dir, exist_ok=True)
+        logger.info(f"Saving model checkpoint to {output_dir}")
+        model = unwrap_model(self.model)
+
+        if hasattr(model, "pretrained_model"): # for models with valuehead (currently using LoRA only)
+            backbone_model = getattr(model, "pretrained_model")
+            torch.save(get_state_dict(getattr(model, "v_head")), os.path.join(output_dir, VALUE_HEAD_FILE_NAME))
+        else:
+            backbone_model = model
+
+        if self.finetuning_args.finetuning_type == "lora":
+            backbone_model.save_pretrained(output_dir, state_dict=get_state_dict(backbone_model))
+        else: # freeze/full tuning
+            backbone_model.save_pretrained(
+                output_dir,
+                state_dict=get_state_dict(backbone_model),
+                safe_serialization=self.args.save_safetensors
+            )
+            if self.tokenizer is not None:
+                self.tokenizer.save_pretrained(output_dir)
+
+        with open(os.path.join(output_dir, TRAINING_ARGS_NAME), "w", encoding="utf-8") as f:
+            f.write(self.args.to_json_string() + "\n")
+        self.finetuning_args.save_to_json(os.path.join(output_dir, FINETUNING_ARGS_NAME))
+
+    def _load_best_model(self):
+        r"""
+        Loads trainable parameters from model checkpoint.
+
+        Subclass and override to inject custom behavior. It should not be directly used by external scripts.
+        """
+        logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
+
+        model = unwrap_model(self.model)
+        backbone_model = getattr(model, "pretrained_model") if hasattr(model, "pretrained_model") else model
+
+        if self.finetuning_args.finetuning_type == "lora":
+            backbone_model.load_adapter(self.state.best_model_checkpoint, getattr(backbone_model, "active_adapter"))
+            if hasattr(model, "v_head") and load_valuehead_params(model, self.state.best_model_checkpoint):
+                model.v_head.load_state_dict({
+                    "summary.weight": getattr(model, "reward_head_weight"),
+                    "summary.bias": getattr(model, "reward_head_bias")
+                })
+        else: # freeze/full-tuning
+            load_trainable_params(backbone_model, self.state.best_model_checkpoint)
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/seq2seq.py` & `ttqakit-0.1.0/TableQAKit/llama/seq2seq.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import os
-import json
-import numpy as np
-from dataclasses import dataclass
-from typing import Dict, List, Sequence, Tuple, Union
-
-from transformers.trainer import PredictionOutput
-from transformers.tokenization_utils import PreTrainedTokenizer
-import jieba
-from rouge_chinese import Rouge
-from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
-from .peft_trainer import PeftTrainer
-from .utils import get_logger, IGNORE_INDEX
-
-
-logger = get_logger(__name__)
-
-
-@dataclass
-class ComputeMetrics:
-    r"""
-    Wraps the tokenizer into metric functions, used in Seq2SeqPeftTrainer.
-    """
-
-    tokenizer: PreTrainedTokenizer
-
-    def __call__(self, eval_preds: Sequence[Union[np.ndarray, Tuple[np.ndarray]]]) -> Dict[str, float]:
-        r"""
-        Uses the model predictions to compute metrics.
-        """
-        preds, labels = eval_preds
-        score_dict = {"rouge-1": [], "rouge-2": [], "rouge-l": [], "bleu-4": []}
-
-        for pred, label in zip(preds, labels):
-            pred_pad_len, label_pad_len = np.sum(pred == IGNORE_INDEX), np.sum(label == IGNORE_INDEX)
-            pred = pred[len(label) - label_pad_len : len(pred) - pred_pad_len] # remove prompts
-            label = label[:len(label) - label_pad_len]
-
-            hypothesis = list(jieba.cut(self.tokenizer.decode(pred, skip_special_tokens=True)))
-            reference = list(jieba.cut(self.tokenizer.decode(label, skip_special_tokens=True)))
-
-            if len(" ".join(hypothesis).split()) == 0:
-                result = {"rouge-1": {"f": 0.0}, "rouge-2": {"f": 0.0}, "rouge-l": {"f": 0.0}}
-            else:
-                rouge = Rouge()
-                scores = rouge.get_scores(" ".join(hypothesis), " ".join(reference))
-                result = scores[0]
-
-            for k, v in result.items():
-                score_dict[k].append(round(v["f"] * 100, 4))
-
-            bleu_score = sentence_bleu([list(label)], list(pred), smoothing_function=SmoothingFunction().method3)
-            score_dict["bleu-4"].append(round(bleu_score * 100, 4))
-
-        return {k: float(np.mean(v)) for k, v in score_dict.items()}
-
-
-class Seq2SeqPeftTrainer(PeftTrainer):
-    r"""
-    Inherits PeftTrainer to compute generative metrics such as BLEU and ROUGE.
-    """
-
-    def save_predictions(
-            self,
-            predict_results: PredictionOutput
-    ) -> None:
-        r"""
-        Saves model predictions to `output_dir`.
-
-        A custom behavior that not contained in Seq2SeqTrainer.
-        """
-        if not self.is_world_process_zero():
-            return
-
-        output_prediction_file = os.path.join(self.args.output_dir, "generated_predictions.jsonl")
-        logger.info(f"Saving prediction results to {output_prediction_file}")
-        with open(output_prediction_file, "w", encoding="utf-8") as writer:
-            res: List[str] = []
-            for pred, label in zip(predict_results.predictions, predict_results.label_ids):
-                pred_pad_len, label_pad_len = np.sum(pred == IGNORE_INDEX), np.sum(label == IGNORE_INDEX)
-                pred = pred[len(label) - label_pad_len : len(pred) - pred_pad_len] # remove prompts
-                label = label[:len(label) - label_pad_len]
-
-                pred = self.tokenizer.decode(pred, skip_special_tokens=True)
-                label = self.tokenizer.decode(label, skip_special_tokens=True)
-
-                res.append(json.dumps({"label": label, "predict": pred}, ensure_ascii=False))
-
-            writer.write("\n".join(res))
+import os
+import json
+import numpy as np
+from dataclasses import dataclass
+from typing import Dict, List, Sequence, Tuple, Union
+
+from transformers.trainer import PredictionOutput
+from transformers.tokenization_utils import PreTrainedTokenizer
+import jieba
+from rouge_chinese import Rouge
+from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
+from .peft_trainer import PeftTrainer
+from .utils import get_logger, IGNORE_INDEX
+
+
+logger = get_logger(__name__)
+
+
+@dataclass
+class ComputeMetrics:
+    r"""
+    Wraps the tokenizer into metric functions, used in Seq2SeqPeftTrainer.
+    """
+
+    tokenizer: PreTrainedTokenizer
+
+    def __call__(self, eval_preds: Sequence[Union[np.ndarray, Tuple[np.ndarray]]]) -> Dict[str, float]:
+        r"""
+        Uses the model predictions to compute metrics.
+        """
+        preds, labels = eval_preds
+        score_dict = {"rouge-1": [], "rouge-2": [], "rouge-l": [], "bleu-4": []}
+
+        for pred, label in zip(preds, labels):
+            pred_pad_len, label_pad_len = np.sum(pred == IGNORE_INDEX), np.sum(label == IGNORE_INDEX)
+            pred = pred[len(label) - label_pad_len : len(pred) - pred_pad_len] # remove prompts
+            label = label[:len(label) - label_pad_len]
+
+            hypothesis = list(jieba.cut(self.tokenizer.decode(pred, skip_special_tokens=True)))
+            reference = list(jieba.cut(self.tokenizer.decode(label, skip_special_tokens=True)))
+
+            if len(" ".join(hypothesis).split()) == 0:
+                result = {"rouge-1": {"f": 0.0}, "rouge-2": {"f": 0.0}, "rouge-l": {"f": 0.0}}
+            else:
+                rouge = Rouge()
+                scores = rouge.get_scores(" ".join(hypothesis), " ".join(reference))
+                result = scores[0]
+
+            for k, v in result.items():
+                score_dict[k].append(round(v["f"] * 100, 4))
+
+            bleu_score = sentence_bleu([list(label)], list(pred), smoothing_function=SmoothingFunction().method3)
+            score_dict["bleu-4"].append(round(bleu_score * 100, 4))
+
+        return {k: float(np.mean(v)) for k, v in score_dict.items()}
+
+
+class Seq2SeqPeftTrainer(PeftTrainer):
+    r"""
+    Inherits PeftTrainer to compute generative metrics such as BLEU and ROUGE.
+    """
+
+    def save_predictions(
+            self,
+            predict_results: PredictionOutput
+    ) -> None:
+        r"""
+        Saves model predictions to `output_dir`.
+
+        A custom behavior that not contained in Seq2SeqTrainer.
+        """
+        if not self.is_world_process_zero():
+            return
+
+        output_prediction_file = os.path.join(self.args.output_dir, "generated_predictions.jsonl")
+        logger.info(f"Saving prediction results to {output_prediction_file}")
+        with open(output_prediction_file, "w", encoding="utf-8") as writer:
+            res: List[str] = []
+            for pred, label in zip(predict_results.predictions, predict_results.label_ids):
+                pred_pad_len, label_pad_len = np.sum(pred == IGNORE_INDEX), np.sum(label == IGNORE_INDEX)
+                pred = pred[len(label) - label_pad_len : len(pred) - pred_pad_len] # remove prompts
+                label = label[:len(label) - label_pad_len]
+
+                pred = self.tokenizer.decode(pred, skip_special_tokens=True)
+                label = self.tokenizer.decode(label, skip_special_tokens=True)
+
+                res.append(json.dumps({"label": label, "predict": pred}, ensure_ascii=False))
+
+            writer.write("\n".join(res))
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/template.py` & `ttqakit-0.1.0/TableQAKit/llama/template.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import List, Optional
-from dataclasses import dataclass
-from abc import abstractmethod, ABC
-
-
-@dataclass
-class Template(ABC):
-    @abstractmethod
-    def __post_init__(self) -> None:
-        """
-        call the self._register_template to define the template like:
-        self._register_template(
-            prefix="the prefix if the dataset's prefix is not defined",
-            prompt="the model input with {query}",
-            sep="\n",
-            use_history=False
-        )
-        :return: NoneType
-        """
-        pass
-
-    def get_prompt(self, query: str, history: Optional[list] = None, prefix: Optional[str] = "") -> str:
-        r"""
-        Returns a string containing prompt without response.
-        """
-        return "".join(self._format_example(query, history, prefix))
-
-    def get_dialog(self, query: str, resp: str, history: Optional[list] = None, prefix: Optional[str] = "") -> List[str]:
-        r"""
-        Returns a list containing 2 * n elements where the 2k-th is a query and the (2k+1)-th is a response.
-        """
-        return self._format_example(query, history, prefix) + [resp]
-
-    def _register_template(self, prefix: str, prompt: str, sep: str, use_history: Optional[bool] = True) -> None:
-        self.prefix = prefix
-        self.prompt = prompt
-        self.sep = sep
-        self.use_history = use_history
-
-    def _format_example(self, query: str, history: Optional[list] = None, prefix: Optional[str] = "") -> List[str]:
-        prefix = prefix if prefix else self.prefix  # use prefix if provided
-        prefix = prefix + self.sep if prefix else ""  # add separator for non-empty prefix
-        history = history if (history and self.use_history) else []
-        history = history + [(query, "<dummy>")]
-        convs = []
-        for turn_idx, (user_query, bot_resp) in enumerate(history):
-            if turn_idx == 0:
-                convs.append(prefix + self.prompt.format(query=user_query))
-                convs.append(bot_resp)
-            else:
-                convs.append(self.sep + self.prompt.format(query=user_query))
-                convs.append(bot_resp)
-        return convs[:-1]  # drop last
-
-
-class defaultTemplate(Template):
-    def __post_init__(self):
-        """
-        Default template.
-        """
-        self._register_template(
-            prefix="A chat between a curious user and an artificial intelligence assistant. "
-                   "The assistant gives helpful, detailed, and polite answers to the user's questions.",
-            prompt="Human: {query}\nAssistant: ",
-            sep="\n",
-            use_history=False
-        )
+from typing import List, Optional
+from dataclasses import dataclass
+from abc import abstractmethod, ABC
+
+
+@dataclass
+class Template(ABC):
+    @abstractmethod
+    def __post_init__(self) -> None:
+        """
+        call the self._register_template to define the template like:
+        self._register_template(
+            prefix="the prefix if the dataset's prefix is not defined",
+            prompt="the model input with {query}",
+            sep="\n",
+            use_history=False
+        )
+        :return: NoneType
+        """
+        pass
+
+    def get_prompt(self, query: str, history: Optional[list] = None, prefix: Optional[str] = "") -> str:
+        r"""
+        Returns a string containing prompt without response.
+        """
+        return "".join(self._format_example(query, history, prefix))
+
+    def get_dialog(self, query: str, resp: str, history: Optional[list] = None, prefix: Optional[str] = "") -> List[str]:
+        r"""
+        Returns a list containing 2 * n elements where the 2k-th is a query and the (2k+1)-th is a response.
+        """
+        return self._format_example(query, history, prefix) + [resp]
+
+    def _register_template(self, prefix: str, prompt: str, sep: str, use_history: Optional[bool] = True) -> None:
+        self.prefix = prefix
+        self.prompt = prompt
+        self.sep = sep
+        self.use_history = use_history
+
+    def _format_example(self, query: str, history: Optional[list] = None, prefix: Optional[str] = "") -> List[str]:
+        prefix = prefix if prefix else self.prefix  # use prefix if provided
+        prefix = prefix + self.sep if prefix else ""  # add separator for non-empty prefix
+        history = history if (history and self.use_history) else []
+        history = history + [(query, "<dummy>")]
+        convs = []
+        for turn_idx, (user_query, bot_resp) in enumerate(history):
+            if turn_idx == 0:
+                convs.append(prefix + self.prompt.format(query=user_query))
+                convs.append(bot_resp)
+            else:
+                convs.append(self.sep + self.prompt.format(query=user_query))
+                convs.append(bot_resp)
+        return convs[:-1]  # drop last
+
+
+class defaultTemplate(Template):
+    def __post_init__(self):
+        """
+        Default template.
+        """
+        self._register_template(
+            prefix="A chat between a curious user and an artificial intelligence assistant. "
+                   "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+            prompt="Human: {query}\nAssistant: ",
+            sep="\n",
+            use_history=False
+        )
```

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/trainer.py` & `ttqakit-0.1.0/TableQAKit/llama/Trainer.py`

 * *Files identical despite different names*

### Comparing `ttqakit-0.0.2/src/ttqakit/llama/utils.py` & `ttqakit-0.1.0/TableQAKit/llama/utils.py`

 * *Files identical despite different names*

### Comparing `ttqakit-0.0.2/src/ttqakit/retriever/dataset.py` & `ttqakit-0.1.0/TableQAKit/numerical/retriever/dataset.py`

 * *Files identical despite different names*

### Comparing `ttqakit-0.0.2/src/ttqakit/retriever/model.py` & `ttqakit-0.1.0/TableQAKit/numerical/retriever/model.py`

 * *Files identical despite different names*

### Comparing `ttqakit-0.0.2/src/ttqakit/retriever/utils.py` & `ttqakit-0.1.0/TableQAKit/numerical/retriever/utils.py`

 * *Files identical despite different names*

