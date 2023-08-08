# Comparing `tmp/hezar-0.21.2.tar.gz` & `tmp/hezar-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.21.2.tar", max compression
+gzip compressed data, was "hezar-0.21.3.tar", max compression
```

## Comparing `hezar-0.21.2.tar` & `hezar-0.21.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1065 2023-08-07 05:55:55.828773 hezar-0.21.2/LICENSE
--rw-r--r--   0        0        0     4750 2023-08-07 05:55:55.828773 hezar-0.21.2/README.md
--rw-r--r--   0        0        0      260 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/builders.py
--rw-r--r--   0        0        0    11587 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/data_collators.py
--rw-r--r--   0        0        0      320 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1771 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4545 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3653 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3581 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0       26 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     5129 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     4810 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     4864 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     2743 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     2161 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     2743 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11774 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/model.py
--rw-r--r--   0        0        0     1528 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/model_outputs.py
--rw-r--r--   0        0        0      152 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     4094 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     2802 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0     1642 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/sequence_labeling.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     2948 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0     1088 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/text2text.py
--rw-r--r--   0        0        0      240 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3377 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2853 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3437 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0     1733 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/text_classification.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      155 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     4494 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     3652 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      324 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19486 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2282 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    18229 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      190 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5615 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/core_utils.py
--rw-r--r--   0        0        0      531 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     3666 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-07 05:55:55.832773 hezar-0.21.2/pyproject.toml
--rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 11:11:34.399887 hezar-0.21.3/LICENSE
+-rw-r--r--   0        0        0     7090 2023-08-07 11:11:34.399887 hezar-0.21.3/README.md
+-rw-r--r--   0        0        0      260 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/builders.py
+-rw-r--r--   0        0        0    11587 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1771 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     5129 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     4810 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     4864 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2161 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11774 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/model.py
+-rw-r--r--   0        0        0     1528 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0      152 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     4094 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2802 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0     1642 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/sequence_labeling/sequence_labeling.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     2948 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0     1088 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text2text/text2text.py
+-rw-r--r--   0        0        0      240 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3377 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3437 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0     1733 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_classification/text_classification.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4494 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3652 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19486 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    18504 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      190 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5615 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0      531 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     3666 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-07 11:11:34.403887 hezar-0.21.3/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-07 11:11:34.403887 hezar-0.21.3/pyproject.toml
+-rw-r--r--   0        0        0     9572 1970-01-01 00:00:00.000000 hezar-0.21.3/PKG-INFO
```

### Comparing `hezar-0.21.2/LICENSE` & `hezar-0.21.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/builders.py` & `hezar-0.21.3/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/configs.py` & `hezar-0.21.3/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/constants.py` & `hezar-0.21.3/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/data_collators.py` & `hezar-0.21.3/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/datasets/dataset.py` & `hezar-0.21.3/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.21.3/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.21.3/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.21.3/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/data/utils/data_utils.py` & `hezar-0.21.3/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/embeddings/embedding.py` & `hezar-0.21.3/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/embeddings/fasttext.py` & `hezar-0.21.3/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/embeddings/word2vec.py` & `hezar-0.21.3/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/metrics/f1.py` & `hezar-0.21.3/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/metrics/metric.py` & `hezar-0.21.3/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/metrics/recall.py` & `hezar-0.21.3/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/metrics/seqeval.py` & `hezar-0.21.3/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.21.3/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.21.3/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.21.3/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.21.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.21.3/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.21.3/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/model.py` & `hezar-0.21.3/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/model_outputs.py` & `hezar-0.21.3/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.21.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.21.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.21.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.21.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/sequence_labeling/sequence_labeling.py` & `hezar-0.21.3/hezar/models/sequence_labeling/sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text2text/t5/t5_text2text.py` & `hezar-0.21.3/hezar/models/text2text/t5/t5_text2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.21.3/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text2text/text2text.py` & `hezar-0.21.3/hezar/models/text2text/text2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.21.3/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.21.3/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.21.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.21.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.21.3/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.21.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/models/text_classification/text_classification.py` & `hezar-0.21.3/hezar/models/text_classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/preprocessor.py` & `hezar-0.21.3/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/text_normalizer.py` & `hezar-0.21.3/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.21.3/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.21.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.21.3/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.21.3/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.21.3/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/registry.py` & `hezar-0.21.3/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.21.3/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.21.3/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/trainers/trainer.py` & `hezar-0.21.3/hezar/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,22 @@
             optimizer: If None do nothing and return it, otherwise build it using the train config
             lr_scheduler: If None do nothing and return it, otherwise build it using the train config
 
         Returns:
             Optimizer and scheduler
         """
         if optimizer is None:
-            optimizer_config = self.config.optimizer
+            if self.config.optimizer is None:
+                optimizer_config = OptimizerConfig(
+                    name="adamw",
+                    lr=2e-5,
+                    scheduler=LRSchedulerConfig(name="reduce_on_plateau")
+                )
+            else:
+                optimizer_config = self.config.optimizer
 
             # convert to dict so that we can pop some values
             if isinstance(optimizer_config, OptimizerConfig):
                 optimizer_config = optimizer_config.dict()
 
             optimizer_name = optimizer_config.pop("name")
             scheduler_config = optimizer_config.pop("scheduler")
```

### Comparing `hezar-0.21.2/hezar/trainers/trainer_utils.py` & `hezar-0.21.3/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/utils/common_utils.py` & `hezar-0.21.3/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/utils/core_utils.py` & `hezar-0.21.3/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/utils/file_utils.py` & `hezar-0.21.3/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/utils/hub_utils.py` & `hezar-0.21.3/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/hezar/utils/registry_utils.py` & `hezar-0.21.3/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.2/pyproject.toml` & `hezar-0.21.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.21.2"
+version = "0.21.3"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

