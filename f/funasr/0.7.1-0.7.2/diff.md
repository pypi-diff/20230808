# Comparing `tmp/funasr-0.7.1.tar.gz` & `tmp/funasr-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.7.1.tar", last modified: Mon Jul 24 10:53:51 2023, max compression
+gzip compressed data, was "funasr-0.7.2.tar", last modified: Tue Aug  8 14:01:31 2023, max compression
```

## Comparing `funasr-0.7.1.tar` & `funasr-0.7.2.tar`

### file list

```diff
@@ -1,460 +1,468 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.161891 funasr-0.7.1/
--rw-r--r--   0 zhifu      (502) staff       (20)     8016 2023-07-24 10:53:51.161639 funasr-0.7.1/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7039 2023-07-24 05:54:34.000000 funasr-0.7.1/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.722039 funasr-0.7.1/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.744846 funasr-0.7.1/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72259 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6109 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12386 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    18267 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12181 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.771938 funasr-0.7.1/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.7.1/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18908 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_model_from_file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_streaming_iterator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_sv_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.780536 funasr-0.7.1/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.789547 funasr-0.7.1/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3795 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.812804 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.819080 funasr-0.7.1/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3114 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32729 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.828678 funasr-0.7.1/funasr/datasets/small_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/datasets/small_datasets/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.836788 funasr-0.7.1/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5045 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/export_conformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.844622 funasr-0.7.1/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1724 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.849379 funasr-0.7.1/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4105 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/decoder/xformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2454 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/e2e_asr_conformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.852017 funasr-0.7.1/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.7.1/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.869598 funasr-0.7.1/funasr/export/models/language_models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14582 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/embed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2590 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/seq_rnn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5481 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3907 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.871805 funasr-0.7.1/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.872516 funasr-0.7.1/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.874588 funasr-0.7.1/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.7.1/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.875352 funasr-0.7.1/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.878238 funasr-0.7.1/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.900590 funasr-0.7.1/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.940229 funasr-0.7.1/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.940802 funasr-0.7.1/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.7.1/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.944544 funasr-0.7.1/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.959535 funasr-0.7.1/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.965712 funasr-0.7.1/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75537 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_bat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100274 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.974893 funasr-0.7.1/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20694 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/branchformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17014 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/e_branchformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.976805 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56561 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.982167 funasr-0.7.1/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.983725 funasr-0.7.1/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.984555 funasr-0.7.1/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.7.1/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.986770 funasr-0.7.1/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.987498 funasr-0.7.1/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.989842 funasr-0.7.1/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.990895 funasr-0.7.1/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.009528 funasr-0.7.1/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40008 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.039857 funasr-0.7.1/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3480 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/cgmlp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.042750 funasr-0.7.1/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.7.1/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.043471 funasr-0.7.1/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.045489 funasr-0.7.1/funasr/modules/eend_ola/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/report.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/embedding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5282 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/fastformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.053949 funasr-0.7.1/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/lightconv2d.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.054805 funasr-0.7.1/funasr/modules/lora/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12553 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/layers.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1839 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.7.1/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4283 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.060990 funasr-0.7.1/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.062427 funasr-0.7.1/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.063865 funasr-0.7.1/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/subsampling_without_posenc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2782 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/vgg2l.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.064995 funasr-0.7.1/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.065261 funasr-0.7.1/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.065568 funasr-0.7.1/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.066509 funasr-0.7.1/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.7.1/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.067258 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.069802 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.072269 funasr-0.7.1/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.073602 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.078128 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.080498 funasr-0.7.1/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.081596 funasr-0.7.1/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.094409 funasr-0.7.1/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73020 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    62140 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.133998 funasr-0.7.1/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.138709 funasr-0.7.1/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.148461 funasr-0.7.1/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.7.1/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38500 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.158716 funasr-0.7.1/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.7.1/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/runtime_sdk_download_tool.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13725 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-24 10:52:35.000000 funasr-0.7.1/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.724327 funasr-0.7.1/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8016 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    14670 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      763 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-24 10:53:51.161961 funasr-0.7.1/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     3648 2023-07-21 03:47:46.000000 funasr-0.7.1/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.160660 funasr-0.7.1/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.7.1/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.7.1/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.612938 funasr-0.7.2/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8648 2023-08-08 14:01:31.612629 funasr-0.7.2/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7671 2023-08-08 12:04:47.000000 funasr-0.7.2/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.451181 funasr-0.7.2/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.461401 funasr-0.7.2/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72198 2023-07-31 03:29:36.000000 funasr-0.7.2/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6109 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17729 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12386 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18267 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12181 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.467168 funasr-0.7.2/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.7.2/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4350 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18908 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1396 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10503 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3110 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.468456 funasr-0.7.2/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6276 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.469437 funasr-0.7.2/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3795 2023-07-31 03:29:41.000000 funasr-0.7.2/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.470677 funasr-0.7.2/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.7.2/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.472550 funasr-0.7.2/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3114 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32716 2023-07-26 06:54:17.000000 funasr-0.7.2/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.474053 funasr-0.7.2/funasr/datasets/small_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/small_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/small_datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/small_datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/small_datasets/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/datasets/small_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7443 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/datasets/small_datasets/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.474619 funasr-0.7.2/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5045 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/export_conformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11402 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.476669 funasr-0.7.2/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.7.2/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.478015 funasr-0.7.2/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12635 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.7.2/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4105 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/decoder/xformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2454 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/e2e_asr_conformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13111 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.479026 funasr-0.7.2/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.7.2/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7756 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.480705 funasr-0.7.2/funasr/export/models/language_models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/language_models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14582 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/language_models/embed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2590 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/language_models/seq_rnn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5481 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/language_models/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3907 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/export/models/language_models/transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.500029 funasr-0.7.2/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.7.2/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8690 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.500541 funasr-0.7.2/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10140 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.503951 funasr-0.7.2/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.7.2/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.7.2/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.505056 funasr-0.7.2/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.7.2/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.508455 funasr-0.7.2/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.510175 funasr-0.7.2/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.514480 funasr-0.7.2/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3313 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.514947 funasr-0.7.2/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4350 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.516462 funasr-0.7.2/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.534103 funasr-0.7.2/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5211 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.537791 funasr-0.7.2/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75537 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr_bat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100274 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9564 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23607 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.544281 funasr-0.7.2/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20694 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17014 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/e_branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.7.2/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.7.2/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.7.2/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.546061 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56561 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.549317 funasr-0.7.2/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20384 2023-07-31 03:29:36.000000 funasr-0.7.2/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.550183 funasr-0.7.2/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.7.2/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.7.2/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.550746 funasr-0.7.2/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.7.2/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.551900 funasr-0.7.2/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.552345 funasr-0.7.2/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.553643 funasr-0.7.2/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.555012 funasr-0.7.2/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      670 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/models/specaug/abs_profileaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6156 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/models/specaug/profileaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.7.2/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.560931 funasr-0.7.2/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40008 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.562623 funasr-0.7.2/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.7.2/funasr/modules/beam_search/beam_search_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3480 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/cgmlp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.564985 funasr-0.7.2/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.7.2/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.565989 funasr-0.7.2/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.7.2/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1875 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/modules/eend_ola/eend_ola_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4794 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/modules/eend_ola/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.567375 funasr-0.7.2/funasr/modules/eend_ola/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9352 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5232 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/kaldi_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1447 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/eend_ola/utils/report.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/embedding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5282 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/fastformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.569052 funasr-0.7.2/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/lightconv2d.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.569851 funasr-0.7.2/funasr/modules/lora/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/modules/lora/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12553 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/modules/lora/layers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1839 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/modules/lora/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.7.2/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.7.2/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24246 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4283 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.571660 funasr-0.7.2/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.572670 funasr-0.7.2/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.573719 funasr-0.7.2/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21865 2023-08-02 10:49:51.000000 funasr-0.7.2/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/modules/subsampling_without_posenc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2782 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/modules/vgg2l.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.574390 funasr-0.7.2/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.7.2/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.574660 funasr-0.7.2/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.2/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.574812 funasr-0.7.2/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.2/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.575401 funasr-0.7.2/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.7.2/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.576107 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.578086 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.580439 funasr-0.7.2/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_paraformer_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      795 2023-07-26 06:54:17.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.581962 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13639 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_online_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13466 2023-07-26 06:54:17.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.583884 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16830 2023-08-08 05:38:01.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10989 2023-08-08 11:57:07.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.585638 funasr-0.7.2/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.586548 funasr-0.7.2/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.590283 funasr-0.7.2/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73020 2023-07-21 07:26:44.000000 funasr-0.7.2/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    62140 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23867 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.594220 funasr-0.7.2/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.599142 funasr-0.7.2/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.7.2/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.600879 funasr-0.7.2/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.7.2/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38500 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.610363 funasr-0.7.2/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.7.2/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      309 2023-08-04 12:22:25.000000 funasr-0.7.2/funasr/utils/hinter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.7.2/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.7.2/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.7.2/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10339 2023-08-07 08:54:41.000000 funasr-0.7.2/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/runtime_sdk_download_tool.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13725 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.7.2/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-07-21 03:47:46.000000 funasr-0.7.2/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.7.2/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-08-08 11:00:18.000000 funasr-0.7.2/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.452059 funasr-0.7.2/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8648 2023-08-08 14:01:31.000000 funasr-0.7.2/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    15032 2023-08-08 14:01:31.000000 funasr-0.7.2/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-08-08 14:01:31.000000 funasr-0.7.2/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      763 2023-08-08 14:01:31.000000 funasr-0.7.2/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-08-08 14:01:31.000000 funasr-0.7.2/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-08-08 14:01:31.613038 funasr-0.7.2/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3648 2023-07-21 03:47:46.000000 funasr-0.7.2/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:01:31.612283 funasr-0.7.2/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-21 03:47:46.000000 funasr-0.7.2/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-07-21 03:47:46.000000 funasr-0.7.2/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.7.2/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.7.2/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-07-21 03:47:46.000000 funasr-0.7.2/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-21 03:47:46.000000 funasr-0.7.2/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-07-21 03:47:46.000000 funasr-0.7.2/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.7.1/PKG-INFO` & `funasr-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.7.1
+Version: 0.7.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -49,17 +49,17 @@
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker Diarization and multi-talker ASR. FunASR provides convenient scripts and tutorials, supporting inference and fine-tuning of pre-trained models.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition model, has the advantages of high accuracy, high efficiency, and convenient deployment, supporting the rapid construction of speech recognition services. For more details on service deployment, please refer to the [service deployment document](funasr/runtime/readme_cn.md). 
 
 
 <a name="whats-new"></a>
 ## What's new: 
-
+- 2023/08/07: The real-time transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial_online.md)).
 - 2023/07/17: BAT is released, which is a low-latency and low-memory-consumption RNN-T model. For more details, please refer to ([BAT](egs/aishell/bat)).
-- 2023/07/03: The CPU version of the Chinese offline file transcription service has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
+- 2023/07/03: The offline file transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
 - 2023/06/26: ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0 completed the competition and announced the results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 
 <a name="Installation"></a>
 ## Installation
 
 Please ref to [installation docs](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
@@ -67,14 +67,16 @@
 ## Deployment Service
 
 FunASR supports pre-trained or further fine-tuned models for deployment as a service. The CPU version of the Chinese offline file conversion service has been released, details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More detailed information about service deployment can be found in the [deployment roadmap](funasr/runtime/readme_cn.md).
 
 
 <a name="quick-start"></a>
 ## Quick Start
+Quick start for new users（[tutorial](https://alibaba-damo-academy.github.io/FunASR/en/funasr/quick_start_zh.html)）
+
 
 FunASR supports inference and fine-tuning of models trained on industrial datasets of tens of thousands of hours. For more details, please refer to ([modelscope_egs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also supports training and fine-tuning of models on academic standard datasets. For more details, please refer to([egs](https://alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The models include speech recognition (ASR), speech activity detection (VAD), punctuation recovery, language model, speaker verification, speaker separation, and multi-party conversation speech recognition. For a detailed list of models, please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md):
 
 <a name="Community Communication"></a>
 ## Community Communication
 If you encounter problems in use, you can directly raise Issues on the github page.
 
@@ -82,16 +84,16 @@
 
 |DingTalk group |                     WeChat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> | <img src="docs/images/XVERSE.png" width="250"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:------------------------------------------------------:|
 
 The contributors can be found in [contributors list]((./Acknowledge))
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
@@ -106,14 +108,20 @@
 }
 @inproceedings{An2023bat,
   author={Keyu An and Xian Shi and Shiliang Zhang},
   title={BAT: Boundary aware transducer for memory-efficient and low-latency ASR},
   year={2023},
   booktitle={INTERSPEECH},
 }
+@inproceedings{wang2023told,
+  author={Jiaming Wang and Zhihao Du and Shiliang Zhang},
+  title={{TOLD:} {A} Novel Two-Stage Overlap-Aware Framework for Speaker Diarization},
+  year={2023},
+  booktitle={ICASSP},
+}
 @inproceedings{gao22b_interspeech,
   author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
   title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
   year=2022,
   booktitle={Proc. Interspeech 2022},
   pages={2063--2067},
   doi={10.21437/Interspeech.2022-9996}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.7.1 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.7.2 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -39,66 +39,73 @@
 [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
 model_zoo/modelscope_models.md). The representative [Paraformer-large](https://
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition
 model, has the advantages of high accuracy, high efficiency, and convenient
 deployment, supporting the rapid construction of speech recognition services.
 For more details on service deployment, please refer to the [service deployment
-document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/07/17: BAT is
-released, which is a low-latency and low-memory-consumption RNN-T model. For
-more details, please refer to ([BAT](egs/aishell/bat)). - 2023/07/03: The CPU
-version of the Chinese offline file transcription service has been released.
-For more details, please refer to ([Deployment documentation](funasr/runtime/
-docs/SDK_tutorial.md)). - 2023/06/26: ASRU2023 Multi-Channel Multi-Party
-Meeting Transcription Challenge 2.0 completed the competition and announced the
-results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)).  ## Installation Please ref to
-[installation docs](https://alibaba-damo-academy.github.io/FunASR/en/
-installation/installation.html) ## Deployment Service FunASR supports pre-
-trained or further fine-tuned models for deployment as a service. The CPU
-version of the Chinese offline file conversion service has been released,
-details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More
-detailed information about service deployment can be found in the [deployment
-roadmap](funasr/runtime/readme_cn.md).  ## Quick Start FunASR supports
-inference and fine-tuning of models trained on industrial datasets of tens of
-thousands of hours. For more details, please refer to ([modelscope_egs](https:/
-/alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html)). It also supports training and fine-tuning of models on
-academic standard datasets. For more details, please refer to([egs](https://
-alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The
-models include speech recognition (ASR), speech activity detection (VAD),
-punctuation recovery, language model, speaker verification, speaker separation,
-and multi-party conversation speech recognition. For a detailed list of models,
-please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/
-blob/main/docs/model_zoo/modelscope_models.md):  ## Community Communication If
-you encounter problems in use, you can directly raise Issues on the github
-page. You can also scan the following DingTalk group or WeChat group QR code to
-join the community group for communication and discussion. |DingTalk group |
-WeChat group | |:---:|:-----------------------------------------------------:
-| |
+document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/08/07: The real-
+time transcription service (CPU) of Mandarin has been released. For more
+details, please refer to ([Deployment documentation](funasr/runtime/docs/
+SDK_tutorial_online.md)). - 2023/07/17: BAT is released, which is a low-latency
+and low-memory-consumption RNN-T model. For more details, please refer to (
+[BAT](egs/aishell/bat)). - 2023/07/03: The offline file transcription service
+(CPU) of Mandarin has been released. For more details, please refer to (
+[Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)). - 2023/06/26:
+ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0
+completed the competition and announced the results. For more details, please
+refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/
+index.html)).  ## Installation Please ref to [installation docs](https://
+alibaba-damo-academy.github.io/FunASR/en/installation/installation.html) ##
+Deployment Service FunASR supports pre-trained or further fine-tuned models for
+deployment as a service. The CPU version of the Chinese offline file conversion
+service has been released, details can be found in [docs](funasr/runtime/docs/
+SDK_tutorial.md). More detailed information about service deployment can be
+found in the [deployment roadmap](funasr/runtime/readme_cn.md).  ## Quick Start
+Quick start for new usersï¼[tutorial](https://alibaba-damo-academy.github.io/
+FunASR/en/funasr/quick_start_zh.html)ï¼ FunASR supports inference and fine-
+tuning of models trained on industrial datasets of tens of thousands of hours.
+For more details, please refer to ([modelscope_egs](https://alibaba-damo-
+academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also
+supports training and fine-tuning of models on academic standard datasets. For
+more details, please refer to([egs](https://alibaba-damo-academy.github.io/
+FunASR/en/academic_recipe/asr_recipe.html)). The models include speech
+recognition (ASR), speech activity detection (VAD), punctuation recovery,
+language model, speaker verification, speaker separation, and multi-party
+conversation speech recognition. For a detailed list of models, please refer to
+the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+model_zoo/modelscope_models.md):  ## Community Communication If you encounter
+problems in use, you can directly raise Issues on the github page. You can also
+scan the following DingTalk group or WeChat group QR code to join the community
+group for communication and discussion. |DingTalk group | WeChat group | |:---:
+|:-----------------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
+| [docs/images/XVERSE.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:| The contributors can be found in [contributors list]((./Acknowledge)) ##
-License This project is licensed under the [The MIT License](https://
-opensource.org/licenses/MIT). FunASR also contains various third-party
-components and some code modified from other repos under other open source
-licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
-Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{An2023bat,
-author={Keyu An and Xian Shi and Shiliang Zhang}, title={BAT: Boundary aware
-transducer for memory-efficient and low-latency ASR}, year={2023}, booktitle=
-{INTERSPEECH}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
+--:|:------------------------------------------------------:| The contributors
+can be found in [contributors list]((./Acknowledge)) ## License This project is
+licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{An2023bat, author={Keyu An and Xian Shi and Shiliang Zhang},
+title={BAT: Boundary aware transducer for memory-efficient and low-latency
+ASR}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{wang2023told,
+author={Jiaming Wang and Zhihao Du and Shiliang Zhang}, title={{TOLD:} {A}
+Novel Two-Stage Overlap-Aware Framework for Speaker Diarization}, year={2023},
+booktitle={ICASSP}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
 ShiLiang Zhang and Ian McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and
 Accurate Parallel Transformer for Non-autoregressive End-to-End Speech
 Recognition}}, year=2022, booktitle={Proc. Interspeech 2022}, pages={2063--
 2067}, doi={10.21437/Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.7.1/README.md` & `funasr-0.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker Diarization and multi-talker ASR. FunASR provides convenient scripts and tutorials, supporting inference and fine-tuning of pre-trained models.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition model, has the advantages of high accuracy, high efficiency, and convenient deployment, supporting the rapid construction of speech recognition services. For more details on service deployment, please refer to the [service deployment document](funasr/runtime/readme_cn.md). 
 
 
 <a name="whats-new"></a>
 ## What's new: 
-
+- 2023/08/07: The real-time transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial_online.md)).
 - 2023/07/17: BAT is released, which is a low-latency and low-memory-consumption RNN-T model. For more details, please refer to ([BAT](egs/aishell/bat)).
-- 2023/07/03: The CPU version of the Chinese offline file transcription service has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
+- 2023/07/03: The offline file transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
 - 2023/06/26: ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0 completed the competition and announced the results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 
 <a name="Installation"></a>
 ## Installation
 
 Please ref to [installation docs](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
@@ -42,14 +42,16 @@
 ## Deployment Service
 
 FunASR supports pre-trained or further fine-tuned models for deployment as a service. The CPU version of the Chinese offline file conversion service has been released, details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More detailed information about service deployment can be found in the [deployment roadmap](funasr/runtime/readme_cn.md).
 
 
 <a name="quick-start"></a>
 ## Quick Start
+Quick start for new users（[tutorial](https://alibaba-damo-academy.github.io/FunASR/en/funasr/quick_start_zh.html)）
+
 
 FunASR supports inference and fine-tuning of models trained on industrial datasets of tens of thousands of hours. For more details, please refer to ([modelscope_egs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also supports training and fine-tuning of models on academic standard datasets. For more details, please refer to([egs](https://alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The models include speech recognition (ASR), speech activity detection (VAD), punctuation recovery, language model, speaker verification, speaker separation, and multi-party conversation speech recognition. For a detailed list of models, please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md):
 
 <a name="Community Communication"></a>
 ## Community Communication
 If you encounter problems in use, you can directly raise Issues on the github page.
 
@@ -57,16 +59,16 @@
 
 |DingTalk group |                     WeChat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> | <img src="docs/images/XVERSE.png" width="250"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:------------------------------------------------------:|
 
 The contributors can be found in [contributors list]((./Acknowledge))
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
@@ -81,14 +83,20 @@
 }
 @inproceedings{An2023bat,
   author={Keyu An and Xian Shi and Shiliang Zhang},
   title={BAT: Boundary aware transducer for memory-efficient and low-latency ASR},
   year={2023},
   booktitle={INTERSPEECH},
 }
+@inproceedings{wang2023told,
+  author={Jiaming Wang and Zhihao Du and Shiliang Zhang},
+  title={{TOLD:} {A} Novel Two-Stage Overlap-Aware Framework for Speaker Diarization},
+  year={2023},
+  booktitle={ICASSP},
+}
 @inproceedings{gao22b_interspeech,
   author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
   title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
   year=2022,
   booktitle={Proc. Interspeech 2022},
   pages={2063--2067},
   doi={10.21437/Interspeech.2022-9996}
```

#### html2text {}

```diff
@@ -26,66 +26,73 @@
 [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
 model_zoo/modelscope_models.md). The representative [Paraformer-large](https://
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition
 model, has the advantages of high accuracy, high efficiency, and convenient
 deployment, supporting the rapid construction of speech recognition services.
 For more details on service deployment, please refer to the [service deployment
-document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/07/17: BAT is
-released, which is a low-latency and low-memory-consumption RNN-T model. For
-more details, please refer to ([BAT](egs/aishell/bat)). - 2023/07/03: The CPU
-version of the Chinese offline file transcription service has been released.
-For more details, please refer to ([Deployment documentation](funasr/runtime/
-docs/SDK_tutorial.md)). - 2023/06/26: ASRU2023 Multi-Channel Multi-Party
-Meeting Transcription Challenge 2.0 completed the competition and announced the
-results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)).  ## Installation Please ref to
-[installation docs](https://alibaba-damo-academy.github.io/FunASR/en/
-installation/installation.html) ## Deployment Service FunASR supports pre-
-trained or further fine-tuned models for deployment as a service. The CPU
-version of the Chinese offline file conversion service has been released,
-details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More
-detailed information about service deployment can be found in the [deployment
-roadmap](funasr/runtime/readme_cn.md).  ## Quick Start FunASR supports
-inference and fine-tuning of models trained on industrial datasets of tens of
-thousands of hours. For more details, please refer to ([modelscope_egs](https:/
-/alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html)). It also supports training and fine-tuning of models on
-academic standard datasets. For more details, please refer to([egs](https://
-alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The
-models include speech recognition (ASR), speech activity detection (VAD),
-punctuation recovery, language model, speaker verification, speaker separation,
-and multi-party conversation speech recognition. For a detailed list of models,
-please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/
-blob/main/docs/model_zoo/modelscope_models.md):  ## Community Communication If
-you encounter problems in use, you can directly raise Issues on the github
-page. You can also scan the following DingTalk group or WeChat group QR code to
-join the community group for communication and discussion. |DingTalk group |
-WeChat group | |:---:|:-----------------------------------------------------:
-| |
+document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/08/07: The real-
+time transcription service (CPU) of Mandarin has been released. For more
+details, please refer to ([Deployment documentation](funasr/runtime/docs/
+SDK_tutorial_online.md)). - 2023/07/17: BAT is released, which is a low-latency
+and low-memory-consumption RNN-T model. For more details, please refer to (
+[BAT](egs/aishell/bat)). - 2023/07/03: The offline file transcription service
+(CPU) of Mandarin has been released. For more details, please refer to (
+[Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)). - 2023/06/26:
+ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0
+completed the competition and announced the results. For more details, please
+refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/
+index.html)).  ## Installation Please ref to [installation docs](https://
+alibaba-damo-academy.github.io/FunASR/en/installation/installation.html) ##
+Deployment Service FunASR supports pre-trained or further fine-tuned models for
+deployment as a service. The CPU version of the Chinese offline file conversion
+service has been released, details can be found in [docs](funasr/runtime/docs/
+SDK_tutorial.md). More detailed information about service deployment can be
+found in the [deployment roadmap](funasr/runtime/readme_cn.md).  ## Quick Start
+Quick start for new usersï¼[tutorial](https://alibaba-damo-academy.github.io/
+FunASR/en/funasr/quick_start_zh.html)ï¼ FunASR supports inference and fine-
+tuning of models trained on industrial datasets of tens of thousands of hours.
+For more details, please refer to ([modelscope_egs](https://alibaba-damo-
+academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also
+supports training and fine-tuning of models on academic standard datasets. For
+more details, please refer to([egs](https://alibaba-damo-academy.github.io/
+FunASR/en/academic_recipe/asr_recipe.html)). The models include speech
+recognition (ASR), speech activity detection (VAD), punctuation recovery,
+language model, speaker verification, speaker separation, and multi-party
+conversation speech recognition. For a detailed list of models, please refer to
+the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+model_zoo/modelscope_models.md):  ## Community Communication If you encounter
+problems in use, you can directly raise Issues on the github page. You can also
+scan the following DingTalk group or WeChat group QR code to join the community
+group for communication and discussion. |DingTalk group | WeChat group | |:---:
+|:-----------------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
+| [docs/images/XVERSE.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:| The contributors can be found in [contributors list]((./Acknowledge)) ##
-License This project is licensed under the [The MIT License](https://
-opensource.org/licenses/MIT). FunASR also contains various third-party
-components and some code modified from other repos under other open source
-licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
-Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{An2023bat,
-author={Keyu An and Xian Shi and Shiliang Zhang}, title={BAT: Boundary aware
-transducer for memory-efficient and low-latency ASR}, year={2023}, booktitle=
-{INTERSPEECH}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
+--:|:------------------------------------------------------:| The contributors
+can be found in [contributors list]((./Acknowledge)) ## License This project is
+licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{An2023bat, author={Keyu An and Xian Shi and Shiliang Zhang},
+title={BAT: Boundary aware transducer for memory-efficient and low-latency
+ASR}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{wang2023told,
+author={Jiaming Wang and Zhihao Du and Shiliang Zhang}, title={{TOLD:} {A}
+Novel Two-Stage Overlap-Aware Framework for Speaker Diarization}, year={2023},
+booktitle={ICASSP}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
 ShiLiang Zhang and Ian McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and
 Accurate Parallel Transformer for Non-autoregressive End-to-End Speech
 Recognition}}, year=2022, booktitle={Proc. Interspeech 2022}, pages={2063--
 2067}, doi={10.21437/Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.7.1/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.7.2/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/asr_infer.py` & `funasr-0.7.2/funasr/bin/asr_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/asr_inference_launch.py` & `funasr-0.7.2/funasr/bin/asr_inference_launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,16 +256,14 @@
         hotword_list_or_file = param_dict.get('hotword')
         export_mode = param_dict.get("export_mode", False)
         clas_scale = param_dict.get('clas_scale', 1.0)
     else:
         hotword_list_or_file = None
         clas_scale = 1.0
 
-    if kwargs.get("device", None) == "cpu":
-        ngpu = 0
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
         batch_size = 1
 
     # 1. Set random-seed
```

### Comparing `funasr-0.7.1/funasr/bin/asr_train.py` & `funasr-0.7.2/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/build_trainer.py` & `funasr-0.7.2/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/data2vec_train.py` & `funasr-0.7.2/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/diar_infer.py` & `funasr-0.7.2/funasr/bin/diar_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/diar_inference_launch.py` & `funasr-0.7.2/funasr/bin/diar_inference_launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,19 +449,25 @@
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
     group.add_argument(
-        "--diar_smooth_size",
+        "--smooth_size",
         type=int,
         default=121,
         help="The smoothing size for post-processing"
     )
+    group.add_argument(
+        "--dur_threshold",
+        type=int,
+        default=10,
+        help="The threshold of minimum duration"
+    )
 
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
```

### Comparing `funasr-0.7.1/funasr/bin/diar_train.py` & `funasr-0.7.2/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/lm_inference_launch.py` & `funasr-0.7.2/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/lm_train.py` & `funasr-0.7.2/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/punc_infer.py` & `funasr-0.7.2/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/punc_inference_launch.py` & `funasr-0.7.2/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/punc_train.py` & `funasr-0.7.2/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/sa_asr_train.py` & `funasr-0.7.2/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/sv_infer.py` & `funasr-0.7.2/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/sv_inference_launch.py` & `funasr-0.7.2/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/tokenize_text.py` & `funasr-0.7.2/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/tp_infer.py` & `funasr-0.7.2/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/tp_inference_launch.py` & `funasr-0.7.2/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/train.py` & `funasr-0.7.2/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/vad_infer.py` & `funasr-0.7.2/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/bin/vad_inference_launch.py` & `funasr-0.7.2/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_args.py` & `funasr-0.7.2/funasr/build_utils/build_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,20 @@
             class_choices.add_arguments(task_parser)
         task_parser.add_argument(
             "--input_size",
             type=int_or_none,
             default=None,
             help="The number of input dimension of the feature",
         )
+        task_parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The path of cmvn file.",
+        )
 
     elif args.task_name == "lm":
         from funasr.build_utils.build_lm_model import class_choices_list
         for class_choices in class_choices_list:
             class_choices.add_arguments(task_parser)
 
     elif args.task_name == "punc":
@@ -82,14 +88,20 @@
             help="The path of cmvn file.",
         )
 
     elif args.task_name == "diar":
         from funasr.build_utils.build_diar_model import class_choices_list
         for class_choices in class_choices_list:
             class_choices.add_arguments(task_parser)
+        task_parser.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
 
     elif args.task_name == "sv":
         from funasr.build_utils.build_sv_model import class_choices_list
         for class_choices in class_choices_list:
             class_choices.add_arguments(task_parser)
         task_parser.add_argument(
             "--input_size",
```

### Comparing `funasr-0.7.1/funasr/build_utils/build_asr_model.py` & `funasr-0.7.2/funasr/build_utils/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_diar_model.py` & `funasr-0.7.2/funasr/build_utils/build_diar_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 import torch
 
 from funasr.layers.global_mvn import GlobalMVN
-from funasr.layers.label_aggregation import LabelAggregate
+from funasr.layers.label_aggregation import LabelAggregate, LabelAggregateMaxPooling
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.e2e_diar_eend_ola import DiarEENDOLAModel
 from funasr.models.e2e_diar_sond import DiarSondModel
 from funasr.models.encoder.conformer_encoder import ConformerEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.ecapa_tdnn_encoder import ECAPA_TDNN
 from funasr.models.encoder.opennmt_encoders.ci_scorers import DotScorer, CosScorer
@@ -22,14 +22,16 @@
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.models.frontend.windowing import SlidingWindow
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
+from funasr.models.specaug.abs_profileaug import AbsProfileAug
+from funasr.models.specaug.profileaug import ProfileAug
 from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
 from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 
 frontend_choices = ClassChoices(
     name="frontend",
@@ -48,27 +50,37 @@
     classes=dict(
         specaug=SpecAug,
         specaug_lfr=SpecAugLFR,
     ),
     default=None,
     optional=True,
 )
+profileaug_choices = ClassChoices(
+    name="profileaug",
+    classes=dict(
+        profileaug=ProfileAug,
+    ),
+    type_check=AbsProfileAug,
+    default=None,
+    optional=True,
+)
 normalize_choices = ClassChoices(
     "normalize",
     classes=dict(
         global_mvn=GlobalMVN,
         utterance_mvn=UtteranceMVN,
     ),
     default=None,
     optional=True,
 )
 label_aggregator_choices = ClassChoices(
     "label_aggregator",
     classes=dict(
-        label_aggregator=LabelAggregate
+        label_aggregator=LabelAggregate,
+        label_aggregator_max_pool=LabelAggregateMaxPooling,
     ),
     default=None,
     optional=True,
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
@@ -151,14 +163,16 @@
     default="eda",
 )
 class_choices_list = [
     # --frontend and --frontend_conf
     frontend_choices,
     # --specaug and --specaug_conf
     specaug_choices,
+    # --profileaug and --profileaug_conf
+    profileaug_choices,
     # --normalize and --normalize_conf
     normalize_choices,
     # --label_aggregator and --label_aggregator_conf
     label_aggregator_choices,
     # --model and --model_conf
     model_choices,
     # --encoder and --encoder_conf
@@ -174,53 +188,62 @@
     # --eda and --eda_conf
     encoder_decoder_attractor_choices,
 ]
 
 
 def build_diar_model(args):
     # token_list
-    if isinstance(args.token_list, str):
-        with open(args.token_list, encoding="utf-8") as f:
-            token_list = [line.rstrip() for line in f]
-
-        # Overwriting token_list to keep it as "portable".
-        args.token_list = list(token_list)
-    elif isinstance(args.token_list, (tuple, list)):
-        token_list = list(args.token_list)
+    if args.token_list is not None:
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = list(token_list)
+        elif isinstance(args.token_list, (tuple, list)):
+            token_list = list(args.token_list)
+        else:
+            raise RuntimeError("token_list must be str or list")
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
     else:
-        raise RuntimeError("token_list must be str or list")
-    vocab_size = len(token_list)
-    logging.info(f"Vocabulary size: {vocab_size}")
+        token_list = None
+        vocab_size = None
 
     # frontend
     if args.input_size is None:
         frontend_class = frontend_choices.get_class(args.frontend)
         if args.frontend == 'wav_frontend':
             frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
         else:
             frontend = frontend_class(**args.frontend_conf)
-        input_size = frontend.output_size()
     else:
         args.frontend = None
         args.frontend_conf = {}
         frontend = None
-        input_size = args.input_size
 
     # encoder
     encoder_class = encoder_choices.get_class(args.encoder)
-    encoder = encoder_class(input_size=input_size, **args.encoder_conf)
+    encoder = encoder_class(**args.encoder_conf)
 
     if args.model == "sond":
         # data augmentation for spectrogram
         if args.specaug is not None:
             specaug_class = specaug_choices.get_class(args.specaug)
             specaug = specaug_class(**args.specaug_conf)
         else:
             specaug = None
 
+        # Data augmentation for Profiles
+        if hasattr(args, "profileaug") and args.profileaug is not None:
+            profileaug_class = profileaug_choices.get_class(args.profileaug)
+            profileaug = profileaug_class(**args.profileaug_conf)
+        else:
+            profileaug = None
+
         # normalization layer
         if args.normalize is not None:
             normalize_class = normalize_choices.get_class(args.normalize)
             normalize = normalize_class(**args.normalize_conf)
         else:
             normalize = None
 
@@ -257,26 +280,27 @@
             label_aggregator = None
 
         model_class = model_choices.get_class(args.model)
         model = model_class(
             vocab_size=vocab_size,
             frontend=frontend,
             specaug=specaug,
+            profileaug=profileaug,
             normalize=normalize,
             label_aggregator=label_aggregator,
             encoder=encoder,
             speaker_encoder=speaker_encoder,
             ci_scorer=ci_scorer,
             cd_scorer=cd_scorer,
             decoder=decoder,
             token_list=token_list,
             **args.model_conf,
         )
 
-    elif args.model_name == "eend_ola":
+    elif args.model == "eend_ola":
         # encoder-decoder attractor
         encoder_decoder_attractor_class = encoder_decoder_attractor_choices.get_class(args.encoder_decoder_attractor)
         encoder_decoder_attractor = encoder_decoder_attractor_class(**args.encoder_decoder_attractor_conf)
 
         # 9. Build model
         model_class = model_choices.get_class(args.model)
         model = model_class(
```

### Comparing `funasr-0.7.1/funasr/build_utils/build_distributed.py` & `funasr-0.7.2/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_lm_model.py` & `funasr-0.7.2/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_model.py` & `funasr-0.7.2/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_model_from_file.py` & `funasr-0.7.2/funasr/build_utils/build_model_from_file.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_optimizer.py` & `funasr-0.7.2/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_pretrain_model.py` & `funasr-0.7.2/funasr/build_utils/build_pretrain_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.data2vec import Data2VecPretrainModel
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.specaug.specaug import SpecAug
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 
 frontend_choices = ClassChoices(
     name="frontend",
-    classes=dict(default=DefaultFrontend, sliding_window=SlidingWindow),
+    classes=dict(
+        default=DefaultFrontend,
+        sliding_window=SlidingWindow,
+        wav_frontend=WavFrontend,
+    ),
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
     classes=dict(specaug=SpecAug),
     default=None,
     optional=True,
```

### Comparing `funasr-0.7.1/funasr/build_utils/build_punc_model.py` & `funasr-0.7.2/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_scheduler.py` & `funasr-0.7.2/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_streaming_iterator.py` & `funasr-0.7.2/funasr/build_utils/build_streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_sv_model.py` & `funasr-0.7.2/funasr/build_utils/build_sv_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_trainer.py` & `funasr-0.7.2/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/build_utils/build_vad_model.py` & `funasr-0.7.2/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/collate_fn.py` & `funasr-0.7.2/funasr/datasets/small_datasets/collate_fn.py`

 * *Files 20% similar despite different names*

```diff
@@ -81,48 +81,8 @@
     size = len(feature)
     diff = size - target_size
     if diff <= 0:
         return feature
 
     start = np.random.randint(0, diff + 1)
     end = size - diff + start
-    return feature[start:end]
-
-
-def clipping_collate_fn(
-        data: Collection[Tuple[str, Dict[str, np.ndarray]]],
-        max_sample_size=None,
-        not_sequence: Collection[str] = (),
-) -> Tuple[List[str], Dict[str, torch.Tensor]]:
-    # mainly for pre-training
-    uttids = [u for u, _ in data]
-    data = [d for _, d in data]
-
-    assert all(set(data[0]) == set(d) for d in data), "dict-keys mismatching"
-    assert all(
-        not k.endswith("_lengths") for k in data[0]
-    ), f"*_lengths is reserved: {list(data[0])}"
-
-    output = {}
-    for key in data[0]:
-        array_list = [d[key] for d in data]
-        tensor_list = [torch.from_numpy(a) for a in array_list]
-        sizes = [len(s) for s in tensor_list]
-        if max_sample_size is None:
-            target_size = min(sizes)
-        else:
-            target_size = min(min(sizes), max_sample_size)
-        tensor = tensor_list[0].new_zeros(len(tensor_list), target_size, tensor_list[0].shape[1])
-        for i, (source, size) in enumerate(zip(tensor_list, sizes)):
-            diff = size - target_size
-            if diff == 0:
-                tensor[i] = source
-            else:
-                tensor[i] = crop_to_max_size(source, target_size)
-        output[key] = tensor
-
-        if key not in not_sequence:
-            lens = torch.tensor([source.shape[0] for source in tensor], dtype=torch.long)
-            output[key + "_lengths"] = lens
-
-    output = (uttids, output)
-    return output
+    return feature[start:end]
```

### Comparing `funasr-0.7.1/funasr/datasets/dataset.py` & `funasr-0.7.2/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/iterable_dataset.py` & `funasr-0.7.2/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.7.2/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.7.2/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.7.2/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/dataset.py` & `funasr-0.7.2/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.7.2/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/ms_dataset.py` & `funasr-0.7.2/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/preprocessor.py` & `funasr-0.7.2/funasr/datasets/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import numpy as np
 import scipy.signal
 import soundfile
-
+import jieba
 
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.cleaner import TextCleaner
 from funasr.text.token_id_converter import TokenIDConverter
 
 
 class AbsPreprocessor(ABC):
@@ -655,15 +655,14 @@
             split_with_space=split_with_space,
             seg_dict_file=seg_dict_file,
         )
         # The data field name for split text.
         self.split_text_name = split_text_name
         self.seg_jieba = seg_jieba
         if self.seg_jieba:
-            import jieba
             jieba.load_userdict(seg_dict_file)
 
     @classmethod
     def split_words(cls, text: str):
         words = []
         segs = text.split()
         for seg in segs:
```

### Comparing `funasr-0.7.1/funasr/datasets/small_datasets/dataset.py` & `funasr-0.7.2/funasr/datasets/small_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/small_datasets/length_batch_sampler.py` & `funasr-0.7.2/funasr/datasets/small_datasets/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/small_datasets/preprocessor.py` & `funasr-0.7.2/funasr/datasets/small_datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/datasets/small_datasets/sequence_iter_factory.py` & `funasr-0.7.2/funasr/datasets/small_datasets/sequence_iter_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             shape_files = args.valid_shape_file
         else:
             raise NotImplementedError(f"mode={mode}")
         dataset = ESPnetDataset(
             data_path_and_name_and_type,
             preprocess=preprocess_fn,
             dest_sample_rate=dest_sample_rate,
-            speed_perturb=args.speed_perturb if mode=="train" else None,
+            speed_perturb=args.speed_perturb if mode == "train" else None,
         )
 
         # sampler
         dataset_conf = args.dataset_conf
         batch_sampler = LengthBatchSampler(
             batch_bins=dataset_conf["batch_conf"]["batch_size"] * args.ngpu,
             shape_files=shape_files,
@@ -80,15 +80,15 @@
             f"mean={np.mean(bs_list):.1f}, min={np.min(bs_list)}, max={np.max(bs_list)}"
         )
 
         if args.scheduler == "tri_stage" and mode == "train":
             args.max_update = len(bs_list) * args.max_epoch
             logging.info("Max update: {}".format(args.max_update))
 
-        if args.distributed and mode=="train":
+        if args.distributed and mode == "train":
             world_size = torch.distributed.get_world_size()
             rank = torch.distributed.get_rank()
             for batch in batches:
                 if len(batch) < world_size:
                     raise RuntimeError(
                         f"The batch-size must be equal or more than world_size: "
                         f"{len(batch)} < {world_size}"
```

### Comparing `funasr-0.7.1/funasr/export/export_conformer.py` & `funasr-0.7.2/funasr/export/export_conformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/export_model.py` & `funasr-0.7.2/funasr/export/export_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,29 @@
     ):
 
         export_dir = self.cache_dir
         os.makedirs(export_dir, exist_ok=True)
 
         # export encoder1
         self.export_config["model_name"] = "model"
-        model = get_model(
+        models = get_model(
             model,
             self.export_config,
         )
-        model.eval()
-        # self._export_onnx(model, verbose, export_dir)
-        if self.onnx:
-            self._export_onnx(model, verbose, export_dir)
-        else:
-            self._export_torchscripts(model, verbose, export_dir)
-
-        print("output dir: {}".format(export_dir))
+        if not isinstance(models, tuple):
+            models = (models,)
+            
+        for i, model in enumerate(models):
+            model.eval()
+            if self.onnx:
+                self._export_onnx(model, verbose, export_dir)
+            else:
+                self._export_torchscripts(model, verbose, export_dir)
+    
+            print("output dir: {}".format(export_dir))
 
 
     def _torch_quantize(self, model):
         def _run_calibration_data(m):
             # using dummy inputs for a example
             if self.audio_in is not None:
                 feats, feats_len = self.load_feats(self.audio_in)
```

### Comparing `funasr-0.7.1/funasr/export/models/CT_Transformer.py` & `funasr-0.7.2/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/__init__.py` & `funasr-0.7.2/funasr/export/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from funasr.models.e2e_asr_paraformer import Paraformer, BiCifParaformer
+from funasr.models.e2e_asr_paraformer import Paraformer, BiCifParaformer, ParaformerOnline
 from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 from funasr.export.models.e2e_asr_paraformer import BiCifParaformer as BiCifParaformer_export
 from funasr.export.models.e2e_asr_conformer import Conformer as Conformer_export
 
 from funasr.models.e2e_vad import E2EVadModel
 from funasr.export.models.e2e_vad import E2EVadModel as E2EVadModel_export
 from funasr.models.target_delay_transformer import TargetDelayTransformer
 from funasr.export.models.CT_Transformer import CT_Transformer as CT_Transformer_export
 from funasr.train.abs_model import PunctuationModel
 from funasr.models.vad_realtime_transformer import VadRealtimeTransformer
 from funasr.export.models.CT_Transformer import CT_Transformer_VadRealtime as CT_Transformer_VadRealtime_export
+from funasr.export.models.e2e_asr_paraformer import ParaformerOnline_encoder_predictor as ParaformerOnline_encoder_predictor_export
+from funasr.export.models.e2e_asr_paraformer import ParaformerOnline_decoder as ParaformerOnline_decoder_export
 
 def get_model(model, export_config=None):
     if isinstance(model, BiCifParaformer):
         return BiCifParaformer_export(model, **export_config)
+    elif isinstance(model, ParaformerOnline):
+        return (ParaformerOnline_encoder_predictor_export(model, model_name="model"),
+                ParaformerOnline_decoder_export(model, model_name="decoder"))
     elif isinstance(model, Paraformer):
         return Paraformer_export(model, **export_config)
     elif isinstance(model, Conformer_export):
         return Conformer_export(model, **export_config)
     elif isinstance(model, E2EVadModel):
         return E2EVadModel_export(model, **export_config)
     elif isinstance(model, PunctuationModel):
```

### Comparing `funasr-0.7.1/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.7.2/funasr/export/models/decoder/transformer_decoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
+from funasr.export import models
 
 import torch
 import torch.nn as nn
 
 
 from funasr.export.utils.torch_function import MakePadMask
 from funasr.export.utils.torch_function import sequence_mask
 
 from funasr.modules.attention import MultiHeadedAttentionSANMDecoder
 from funasr.export.models.modules.multihead_att import MultiHeadedAttentionSANMDecoder as MultiHeadedAttentionSANMDecoder_export
-from funasr.modules.attention import MultiHeadedAttentionCrossAtt
+from funasr.modules.attention import MultiHeadedAttentionCrossAtt, MultiHeadedAttention
 from funasr.export.models.modules.multihead_att import MultiHeadedAttentionCrossAtt as MultiHeadedAttentionCrossAtt_export
+from funasr.export.models.modules.multihead_att import OnnxMultiHeadedAttention
 from funasr.modules.positionwise_feed_forward import PositionwiseFeedForwardDecoderSANM
 from funasr.export.models.modules.feedforward import PositionwiseFeedForwardDecoderSANM as PositionwiseFeedForwardDecoderSANM_export
-from funasr.export.models.modules.decoder_layer import DecoderLayerSANM as DecoderLayerSANM_export
+from funasr.export.models.modules.decoder_layer import DecoderLayer as DecoderLayer_export
 
 
-class ParaformerSANMDecoder(nn.Module):
+class ParaformerDecoderSAN(nn.Module):
     def __init__(self, model,
                  max_seq_len=512,
                  model_name='decoder',
                  onnx: bool = True,):
         super().__init__()
         # self.embed = model.embed #Embedding(model.embed, max_seq_len)
         self.model = model
@@ -30,30 +32,19 @@
             self.make_pad_mask = sequence_mask(max_seq_len, flip=False)
 
         for i, d in enumerate(self.model.decoders):
             if isinstance(d.feed_forward, PositionwiseFeedForwardDecoderSANM):
                 d.feed_forward = PositionwiseFeedForwardDecoderSANM_export(d.feed_forward)
             if isinstance(d.self_attn, MultiHeadedAttentionSANMDecoder):
                 d.self_attn = MultiHeadedAttentionSANMDecoder_export(d.self_attn)
-            if isinstance(d.src_attn, MultiHeadedAttentionCrossAtt):
-                d.src_attn = MultiHeadedAttentionCrossAtt_export(d.src_attn)
-            self.model.decoders[i] = DecoderLayerSANM_export(d)
-
-        if self.model.decoders2 is not None:
-            for i, d in enumerate(self.model.decoders2):
-                if isinstance(d.feed_forward, PositionwiseFeedForwardDecoderSANM):
-                    d.feed_forward = PositionwiseFeedForwardDecoderSANM_export(d.feed_forward)
-                if isinstance(d.self_attn, MultiHeadedAttentionSANMDecoder):
-                    d.self_attn = MultiHeadedAttentionSANMDecoder_export(d.self_attn)
-                self.model.decoders2[i] = DecoderLayerSANM_export(d)
-
-        for i, d in enumerate(self.model.decoders3):
-            if isinstance(d.feed_forward, PositionwiseFeedForwardDecoderSANM):
-                d.feed_forward = PositionwiseFeedForwardDecoderSANM_export(d.feed_forward)
-            self.model.decoders3[i] = DecoderLayerSANM_export(d)
+            # if isinstance(d.src_attn, MultiHeadedAttentionCrossAtt):
+            #     d.src_attn = MultiHeadedAttentionCrossAtt_export(d.src_attn)
+            if isinstance(d.src_attn, MultiHeadedAttention):
+                d.src_attn = OnnxMultiHeadedAttention(d.src_attn)
+            self.model.decoders[i] = DecoderLayer_export(d)
         
         self.output_layer = model.output_layer
         self.after_norm = model.after_norm
         self.model_name = model_name
         
 
     def prepare_mask(self, mask):
@@ -81,22 +72,15 @@
 
         memory = hs_pad
         memory_mask = self.make_pad_mask(hlens)
         _, memory_mask = self.prepare_mask(memory_mask)
         # memory_mask = myutils.sequence_mask(hlens, device=memory.device)[:, None, :]
 
         x = tgt
-        x, tgt_mask, memory, memory_mask, _ = self.model.decoders(
-            x, tgt_mask, memory, memory_mask
-        )
-        if self.model.decoders2 is not None:
-            x, tgt_mask, memory, memory_mask, _ = self.model.decoders2(
-                x, tgt_mask, memory, memory_mask
-            )
-        x, tgt_mask, memory, memory_mask, _ = self.model.decoders3(
+        x, tgt_mask, memory, memory_mask = self.model.decoders(
             x, tgt_mask, memory, memory_mask
         )
         x = self.after_norm(x)
         x = self.output_layer(x)
 
         return x, ys_in_lens
 
@@ -152,8 +136,8 @@
 
     def get_model_config(self, path):
         return {
             "dec_type": "XformerDecoder",
             "model_path": os.path.join(path, f'{self.model_name}.onnx'),
             "n_layers": len(self.model.decoders) + len(self.model.decoders2),
             "odim": self.model.decoders[0].size
-        }
+        }
```

### Comparing `funasr-0.7.1/funasr/export/models/decoder/xformer_decoder.py` & `funasr-0.7.2/funasr/export/models/decoder/xformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/e2e_asr_conformer.py` & `funasr-0.7.2/funasr/export/models/e2e_asr_conformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.7.2/funasr/export/models/e2e_asr_paraformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import torch
 import torch.nn as nn
 
 from funasr.export.utils.torch_function import MakePadMask
 from funasr.export.utils.torch_function import sequence_mask
-from funasr.models.encoder.sanm_encoder import SANMEncoder
+from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.conformer_encoder import ConformerEncoder
 from funasr.export.models.encoder.sanm_encoder import SANMEncoder as SANMEncoder_export
 from funasr.export.models.encoder.conformer_encoder import ConformerEncoder as ConformerEncoder_export
 from funasr.models.predictor.cif import CifPredictorV2, CifPredictorV3
 from funasr.export.models.predictor.cif import CifPredictorV2 as CifPredictorV2_export
 from funasr.export.models.predictor.cif import CifPredictorV3 as CifPredictorV3_export
 from funasr.models.decoder.sanm_decoder import ParaformerSANMDecoder
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.export.models.decoder.sanm_decoder import ParaformerSANMDecoder as ParaformerSANMDecoder_export
 from funasr.export.models.decoder.transformer_decoder import ParaformerDecoderSAN as ParaformerDecoderSAN_export
+from funasr.export.models.decoder.sanm_decoder import ParaformerSANMDecoderOnline as ParaformerSANMDecoderOnline_export
 
 
 class Paraformer(nn.Module):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
@@ -212,8 +213,154 @@
                 0: 'batch_size',
                 1: 'alphas_length'
             },
             'us_cif_peak': {
                 0: 'batch_size',
                 1: 'alphas_length'
             },
-        }
+        }
+
+
+class ParaformerOnline_encoder_predictor(nn.Module):
+    """
+    Author: Speech Lab, Alibaba Group, China
+    Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
+    https://arxiv.org/abs/2206.08317
+    """
+    
+    def __init__(
+        self,
+        model,
+        max_seq_len=512,
+        feats_dim=560,
+        model_name='model',
+        **kwargs,
+    ):
+        super().__init__()
+        onnx = False
+        if "onnx" in kwargs:
+            onnx = kwargs["onnx"]
+        if isinstance(model.encoder, SANMEncoder) or isinstance(model.encoder, SANMEncoderChunkOpt):
+            self.encoder = SANMEncoder_export(model.encoder, onnx=onnx)
+        elif isinstance(model.encoder, ConformerEncoder):
+            self.encoder = ConformerEncoder_export(model.encoder, onnx=onnx)
+        if isinstance(model.predictor, CifPredictorV2):
+            self.predictor = CifPredictorV2_export(model.predictor)
+        
+        self.feats_dim = feats_dim
+        self.model_name = model_name
+        
+        if onnx:
+            self.make_pad_mask = MakePadMask(max_seq_len, flip=False)
+        else:
+            self.make_pad_mask = sequence_mask(max_seq_len, flip=False)
+    
+    def forward(
+        self,
+        speech: torch.Tensor,
+        speech_lengths: torch.Tensor,
+    ):
+        # a. To device
+        batch = {"speech": speech, "speech_lengths": speech_lengths, "online": True}
+        # batch = to_device(batch, device=self.device)
+        
+        enc, enc_len = self.encoder(**batch)
+        mask = self.make_pad_mask(enc_len)[:, None, :]
+        alphas, _ = self.predictor.forward_cnn(enc, mask)
+        
+        return enc, enc_len, alphas
+    
+    def get_dummy_inputs(self):
+        speech = torch.randn(2, 30, self.feats_dim)
+        speech_lengths = torch.tensor([6, 30], dtype=torch.int32)
+        return (speech, speech_lengths)
+    
+    def get_input_names(self):
+        return ['speech', 'speech_lengths']
+    
+    def get_output_names(self):
+        return ['enc', 'enc_len', 'alphas']
+    
+    def get_dynamic_axes(self):
+        return {
+            'speech': {
+                0: 'batch_size',
+                1: 'feats_length'
+            },
+            'speech_lengths': {
+                0: 'batch_size',
+            },
+            'enc': {
+                0: 'batch_size',
+                1: 'feats_length'
+            },
+            'enc_len': {
+                0: 'batch_size',
+            },
+            'alphas': {
+                0: 'batch_size',
+                1: 'feats_length'
+            },
+        }
+
+
+class ParaformerOnline_decoder(nn.Module):
+    """
+    Author: Speech Lab, Alibaba Group, China
+    Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
+    https://arxiv.org/abs/2206.08317
+    """
+    
+    def __init__(
+        self,
+        model,
+        max_seq_len=512,
+        feats_dim=560,
+        model_name='model',
+        **kwargs,
+    ):
+        super().__init__()
+        onnx = False
+        if "onnx" in kwargs:
+            onnx = kwargs["onnx"]
+
+        if isinstance(model.decoder, ParaformerDecoderSAN):
+            self.decoder = ParaformerDecoderSAN_export(model.decoder, onnx=onnx)
+        elif isinstance(model.decoder, ParaformerSANMDecoder):
+            self.decoder = ParaformerSANMDecoderOnline_export(model.decoder, onnx=onnx)
+        
+        self.feats_dim = feats_dim
+        self.model_name = model_name
+        self.enc_size = model.encoder._output_size
+        
+        if onnx:
+            self.make_pad_mask = MakePadMask(max_seq_len, flip=False)
+        else:
+            self.make_pad_mask = sequence_mask(max_seq_len, flip=False)
+    
+    def forward(
+        self,
+        enc: torch.Tensor,
+        enc_len: torch.Tensor,
+        acoustic_embeds: torch.Tensor,
+        acoustic_embeds_len: torch.Tensor,
+        *args,
+    ):
+        decoder_out, out_caches = self.decoder(enc, enc_len, acoustic_embeds, acoustic_embeds_len, *args)
+        sample_ids = decoder_out.argmax(dim=-1)
+        
+        return decoder_out, sample_ids, out_caches
+    
+    def get_dummy_inputs(self, ):
+        dummy_inputs = self.decoder.get_dummy_inputs(enc_size=self.enc_size)
+        return dummy_inputs
+
+    def get_input_names(self):
+        
+        return self.decoder.get_input_names()
+
+    def get_output_names(self):
+        
+        return self.decoder.get_output_names()
+
+    def get_dynamic_axes(self):
+        return self.decoder.get_dynamic_axes()
```

### Comparing `funasr-0.7.1/funasr/export/models/e2e_vad.py` & `funasr-0.7.2/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.7.2/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.7.2/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.7.2/funasr/export/models/encoder/sanm_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 from funasr.export.utils.torch_function import MakePadMask
 from funasr.export.utils.torch_function import sequence_mask
 from funasr.modules.attention import MultiHeadedAttentionSANM
 from funasr.export.models.modules.multihead_att import MultiHeadedAttentionSANM as MultiHeadedAttentionSANM_export
 from funasr.export.models.modules.encoder_layer import EncoderLayerSANM as EncoderLayerSANM_export
 from funasr.modules.positionwise_feed_forward import PositionwiseFeedForward
 from funasr.export.models.modules.feedforward import PositionwiseFeedForward as PositionwiseFeedForward_export
+from funasr.modules.embedding import StreamSinusoidalPositionEncoder
 
 
 class SANMEncoder(nn.Module):
     def __init__(
         self,
         model,
         max_seq_len=512,
         feats_dim=560,
         model_name='encoder',
         onnx: bool = True,
     ):
         super().__init__()
         self.embed = model.embed
+        if isinstance(self.embed, StreamSinusoidalPositionEncoder):
+            self.embed = None
         self.model = model
         self.feats_dim = feats_dim
         self._output_size = model._output_size
 
         if onnx:
             self.make_pad_mask = MakePadMask(max_seq_len, flip=False)
         else:
@@ -59,16 +62,18 @@
         mask_4d_bhlt = mask_4d_bhlt * -10000.0
         
         return mask_3d_btd, mask_4d_bhlt
 
     def forward(self,
                 speech: torch.Tensor,
                 speech_lengths: torch.Tensor,
+                online: bool = False 
                 ):
-        speech = speech * self._output_size ** 0.5
+        if not online:
+            speech = speech * self._output_size ** 0.5
         mask = self.make_pad_mask(speech_lengths)
         mask = self.prepare_mask(mask)
         if self.embed is None:
             xs_pad = speech
         else:
             xs_pad = self.embed(speech)
```

### Comparing `funasr-0.7.1/funasr/export/models/language_models/embed.py` & `funasr-0.7.2/funasr/export/models/language_models/embed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/language_models/seq_rnn.py` & `funasr-0.7.2/funasr/export/models/language_models/seq_rnn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/language_models/subsampling.py` & `funasr-0.7.2/funasr/export/models/language_models/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/language_models/transformer.py` & `funasr-0.7.2/funasr/export/models/language_models/transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/modules/decoder_layer.py` & `funasr-0.7.2/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/modules/encoder_layer.py` & `funasr-0.7.2/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/modules/feedforward.py` & `funasr-0.7.2/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/models/modules/multihead_att.py` & `funasr-0.7.2/funasr/export/models/modules/multihead_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 
         context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
         new_context_layer_shape = context_layer.size()[:-2] + (self.all_head_size,)
         context_layer = context_layer.view(new_context_layer_shape)
         return self.linear_out(context_layer)  # (batch, time1, d_model)
 
 
-def preprocess_for_attn(x, mask, cache, pad_fn):
+def preprocess_for_attn(x, mask, cache, pad_fn, kernel_size):
     x = x * mask
     x = x.transpose(1, 2)
     if cache is None:
         x = pad_fn(x)
     else:
-        x = torch.cat((cache[:, :, 1:], x), dim=2)
-        cache = x
+        x = torch.cat((cache, x), dim=2)
+        cache = x[:, :, -(kernel_size-1):]
     return x, cache
 
 
 torch_version = tuple([int(i) for i in torch.__version__.split(".")[:2]])
 if torch_version >= (1, 8):
     import torch.fx
     torch.fx.wrap('preprocess_for_attn')
@@ -86,15 +86,15 @@
         super().__init__()
         self.fsmn_block = model.fsmn_block
         self.pad_fn = model.pad_fn
         self.kernel_size = model.kernel_size
         self.attn = None
 
     def forward(self, inputs, mask, cache=None):
-        x, cache = preprocess_for_attn(inputs, mask, cache, self.pad_fn)
+        x, cache = preprocess_for_attn(inputs, mask, cache, self.pad_fn, self.kernel_size)
         x = self.fsmn_block(x)
         x = x.transpose(1, 2)
 
         x = x + inputs
         x = x * mask
         return x, cache
```

### Comparing `funasr-0.7.1/funasr/export/models/predictor/cif.py` & `funasr-0.7.2/funasr/export/models/predictor/cif.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,33 +32,40 @@
 		self.smooth_factor = model.smooth_factor
 		self.noise_threshold = model.noise_threshold
 		self.tail_threshold = model.tail_threshold
 	
 	def forward(self, hidden: torch.Tensor,
 	            mask: torch.Tensor,
 	            ):
+		alphas, token_num = self.forward_cnn(hidden, mask)
+		mask = mask.transpose(-1, -2).float()
+		mask = mask.squeeze(-1)
+		hidden, alphas, token_num = self.tail_process_fn(hidden, alphas, mask=mask)
+		acoustic_embeds, cif_peak = cif(hidden, alphas, self.threshold)
+		
+		return acoustic_embeds, token_num, alphas, cif_peak
+	
+	def forward_cnn(self, hidden: torch.Tensor,
+	            mask: torch.Tensor,
+	            ):
 		h = hidden
 		context = h.transpose(1, 2)
 		queries = self.pad(context)
 		output = torch.relu(self.cif_conv1d(queries))
 		output = output.transpose(1, 2)
 		
 		output = self.cif_output(output)
 		alphas = torch.sigmoid(output)
 		alphas = torch.nn.functional.relu(alphas * self.smooth_factor - self.noise_threshold)
 		mask = mask.transpose(-1, -2).float()
 		alphas = alphas * mask
 		alphas = alphas.squeeze(-1)
 		token_num = alphas.sum(-1)
-		
-		mask = mask.squeeze(-1)
-		hidden, alphas, token_num = self.tail_process_fn(hidden, alphas, mask=mask)
-		acoustic_embeds, cif_peak = cif(hidden, alphas, self.threshold)
-		
-		return acoustic_embeds, token_num, alphas, cif_peak
+
+		return alphas, token_num
 	
 	def tail_process_fn(self, hidden, alphas, token_num=None, mask=None):
 		b, t, d = hidden.size()
 		tail_threshold = self.tail_threshold
 		
 		zeros_t = torch.zeros((b, 1), dtype=torch.float32, device=alphas.device)
 		ones_t = torch.ones_like(zeros_t)
@@ -281,8 +288,8 @@
 
         fire_place = integrate >= threshold
         integrate = torch.where(fire_place,
                                 integrate - torch.ones([batch_size], device=alphas.device),
                                 integrate)
 
     fires = torch.stack(list_fires, 1)
-    return fires
+    return fires
```

### Comparing `funasr-0.7.1/funasr/export/test/test_onnx.py` & `funasr-0.7.2/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/test/test_onnx_punc.py` & `funasr-0.7.2/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.7.2/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/test/test_onnx_vad.py` & `funasr-0.7.2/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/export/utils/torch_function.py` & `funasr-0.7.2/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/fileio/datadir_writer.py` & `funasr-0.7.2/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/fileio/npy_scp.py` & `funasr-0.7.2/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/fileio/rand_gen_dataset.py` & `funasr-0.7.2/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/fileio/read_text.py` & `funasr-0.7.2/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/fileio/sound_scp.py` & `funasr-0.7.2/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/iterators/chunk_iter_factory.py` & `funasr-0.7.2/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/iterators/multiple_iter_factory.py` & `funasr-0.7.2/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/iterators/sequence_iter_factory.py` & `funasr-0.7.2/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/complex_utils.py` & `funasr-0.7.2/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/global_mvn.py` & `funasr-0.7.2/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/label_aggregation.py` & `funasr-0.7.2/funasr/layers/label_aggregation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from typing import Optional
 from typing import Tuple
-
+from torch.nn import functional as F
 from funasr.modules.nets_utils import make_pad_mask
 
 
 class LabelAggregate(torch.nn.Module):
     def __init__(
         self,
         win_length: int = 512,
@@ -74,7 +74,40 @@
 
             olens = (ilens - self.win_length) // self.hop_length + 1
             output.masked_fill_(make_pad_mask(olens, output, 1), 0.0)
         else:
             olens = None
 
         return output.to(input.dtype), olens
+
+
+class LabelAggregateMaxPooling(torch.nn.Module):
+    def __init__(
+        self,
+        hop_length: int = 8,
+    ):
+        super().__init__()
+
+        self.hop_length = hop_length
+
+    def extra_repr(self):
+        return (
+            f"hop_length={self.hop_length}, "
+        )
+
+    def forward(
+        self, input: torch.Tensor, ilens: torch.Tensor = None
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
+        """LabelAggregate forward function.
+
+        Args:
+            input: (Batch, Nsamples, Label_dim)
+            ilens: (Batch)
+        Returns:
+            output: (Batch, Frames, Label_dim)
+
+        """
+
+        output = F.max_pool1d(input.transpose(1, 2), self.hop_length, self.hop_length).transpose(1, 2)
+        olens = ilens // self.hop_length
+
+        return output.to(input.dtype), olens
```

### Comparing `funasr-0.7.1/funasr/layers/log_mel.py` & `funasr-0.7.2/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/mask_along_axis.py` & `funasr-0.7.2/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/sinc_conv.py` & `funasr-0.7.2/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/stft.py` & `funasr-0.7.2/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/time_warp.py` & `funasr-0.7.2/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/layers/utterance_mvn.py` & `funasr-0.7.2/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/losses/label_smoothing_loss.py` & `funasr-0.7.2/funasr/losses/label_smoothing_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,18 @@
             criterion=nn.BCEWithLogitsLoss(reduction="none")
     ):
         super().__init__()
         self.normalize_length = normalize_length
         self.criterion = criterion
 
     def forward(self, pred, label, lengths):
-        pad_mask = make_pad_mask(lengths, maxlen=pred.shape[1])
+        pad_mask = make_pad_mask(lengths, maxlen=pred.shape[1]).to(pred.device)
         loss = self.criterion(pred, label)
         denom = (~pad_mask).sum() if self.normalize_length else pred.shape[0]
-        return loss.masked_fill(pad_mask, 0).sum() / denom
+        return loss.masked_fill(pad_mask.unsqueeze(-1), 0).sum() / denom
 
 
 class NllLoss(nn.Module):
     """Nll loss.
 
     :param int size: the number of class
     :param int padding_idx: ignored class id
```

### Comparing `funasr-0.7.1/funasr/main_funcs/average_nbest_models.py` & `funasr-0.7.2/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.7.2/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/main_funcs/collect_stats.py` & `funasr-0.7.2/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/main_funcs/pack_funcs.py` & `funasr-0.7.2/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/ctc.py` & `funasr-0.7.2/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/data2vec.py` & `funasr-0.7.2/funasr/models/data2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
 
 from funasr.layers.abs_normalize import AbsNormalize
+from funasr.models.base_model import FunASRModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
@@ -32,16 +32,16 @@
     """Data2Vec Pretrain model"""
 
     def __init__(
             self,
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
+            preencoder: Optional[AbsPreEncoder] = None,
     ):
 
         super().__init__()
 
         self.frontend = frontend
         self.specaug = specaug
         self.normalize = normalize
```

### Comparing `funasr-0.7.1/funasr/models/decoder/contextual_decoder.py` & `funasr-0.7.2/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/decoder/rnn_decoder.py` & `funasr-0.7.2/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.7.2/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/decoder/sanm_decoder.py` & `funasr-0.7.2/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/decoder/sv_decoder.py` & `funasr-0.7.2/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/decoder/transformer_decoder.py` & `funasr-0.7.2/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr.py` & `funasr-0.7.2/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_bat.py` & `funasr-0.7.2/funasr/models/e2e_asr_bat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_common.py` & `funasr-0.7.2/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.7.2/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_mfcca.py` & `funasr-0.7.2/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_paraformer.py` & `funasr-0.7.2/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_asr_transducer.py` & `funasr-0.7.2/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.7.2/funasr/models/e2e_diar_eend_ola.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
-
 from contextlib import contextmanager
 from distutils.version import LooseVersion
-from typing import Dict
-from typing import Tuple
+from typing import Dict, List, Tuple, Optional
 
 import numpy as np
 import torch
 import torch.nn as  nn
+import torch.nn.functional as F
 
+from funasr.models.base_model import FunASRModel
 from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
 from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
+from funasr.modules.eend_ola.utils.losses import standard_loss, cal_power_loss, fast_batch_pit_n_speaker_loss
+from funasr.modules.eend_ola.utils.power import create_powerlabel
 from funasr.modules.eend_ola.utils.power import generate_mapping_dict
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     pass
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
@@ -29,33 +28,55 @@
 def pad_attractor(att, max_n_speakers):
     C, D = att.shape
     if C < max_n_speakers:
         att = torch.cat([att, torch.zeros(max_n_speakers - C, D).to(torch.float32).to(att.device)], dim=0)
     return att
 
 
+def pad_labels(ts, out_size):
+    for i, t in enumerate(ts):
+        if t.shape[1] < out_size:
+            ts[i] = F.pad(
+                t,
+                (0, out_size - t.shape[1], 0, 0),
+                mode='constant',
+                value=0.
+            )
+    return ts
+
+
+def pad_results(ys, out_size):
+    ys_padded = []
+    for i, y in enumerate(ys):
+        if y.shape[1] < out_size:
+            ys_padded.append(
+                torch.cat([y, torch.zeros(y.shape[0], out_size - y.shape[1]).to(torch.float32).to(y.device)], dim=1))
+        else:
+            ys_padded.append(y)
+    return ys_padded
+
+
 class DiarEENDOLAModel(FunASRModel):
     """EEND-OLA diarization model"""
 
     def __init__(
             self,
-            frontend: WavFrontendMel23,
+            frontend: Optional[WavFrontendMel23],
             encoder: EENDOLATransformerEncoder,
             encoder_decoder_attractor: EncoderDecoderAttractor,
             n_units: int = 256,
             max_n_speaker: int = 8,
             attractor_loss_weight: float = 1.0,
             mapping_dict=None,
             **kwargs,
     ):
-
         super().__init__()
         self.frontend = frontend
         self.enc = encoder
-        self.eda = encoder_decoder_attractor
+        self.encoder_decoder_attractor = encoder_decoder_attractor
         self.attractor_loss_weight = attractor_loss_weight
         self.max_n_speaker = max_n_speaker
         if mapping_dict is None:
             mapping_dict = generate_mapping_dict(max_speaker_num=self.max_n_speaker)
             self.mapping_dict = mapping_dict
         # PostNet
         self.postnet = nn.LSTM(self.max_n_speaker, n_units, 1, batch_first=True)
@@ -70,137 +91,87 @@
         emb = torch.split(emb.view(pad_shape[0], pad_shape[1], -1), 1, dim=0)
         emb = [e[0][:ilen] for e, ilen in zip(emb, ilens)]
         return emb
 
     def forward_post_net(self, logits, ilens):
         maxlen = torch.max(ilens).to(torch.int).item()
         logits = nn.utils.rnn.pad_sequence(logits, batch_first=True, padding_value=-1)
-        logits = nn.utils.rnn.pack_padded_sequence(logits, ilens.cpu().to(torch.int64), batch_first=True, enforce_sorted=False)
+        logits = nn.utils.rnn.pack_padded_sequence(logits, ilens.cpu().to(torch.int64), batch_first=True,
+                                                   enforce_sorted=False)
         outputs, (_, _) = self.postnet(logits)
         outputs = nn.utils.rnn.pad_packed_sequence(outputs, batch_first=True, padding_value=-1, total_length=maxlen)[0]
         outputs = [output[:ilens[i].to(torch.int).item()] for i, output in enumerate(outputs)]
         outputs = [self.output_layer(output) for output in outputs]
         return outputs
 
     def forward(
             self,
-            speech: torch.Tensor,
-            speech_lengths: torch.Tensor,
-            text: torch.Tensor,
-            text_lengths: torch.Tensor,
+            speech: List[torch.Tensor],
+            speaker_labels: List[torch.Tensor],
+            orders: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
-        """Frontend + Encoder + Decoder + Calc loss
-        Args:
-            speech: (Batch, Length, ...)
-            speech_lengths: (Batch, )
-            text: (Batch, Length)
-            text_lengths: (Batch,)
-        """
-        assert text_lengths.dim() == 1, text_lengths.shape
-        # Check that batch_size is unified
-        assert (
-                speech.shape[0]
-                == speech_lengths.shape[0]
-                == text.shape[0]
-                == text_lengths.shape[0]
-        ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
-        batch_size = speech.shape[0]
-
-        # for data-parallel
-        text = text[:, : text_lengths.max()]
-
-        # 1. Encoder
-        encoder_out, encoder_out_lens = self.enc(speech, speech_lengths)
-        intermediate_outs = None
-        if isinstance(encoder_out, tuple):
-            intermediate_outs = encoder_out[1]
-            encoder_out = encoder_out[0]
-
-        loss_att, acc_att, cer_att, wer_att = None, None, None, None
-        loss_ctc, cer_ctc = None, None
-        stats = dict()
-
-        # 1. CTC branch
-        if self.ctc_weight != 0.0:
-            loss_ctc, cer_ctc = self._calc_ctc_loss(
-                encoder_out, encoder_out_lens, text, text_lengths
-            )
 
-            # Collect CTC branch stats
-            stats["loss_ctc"] = loss_ctc.detach() if loss_ctc is not None else None
-            stats["cer_ctc"] = cer_ctc
-
-        # Intermediate CTC (optional)
-        loss_interctc = 0.0
-        if self.interctc_weight != 0.0 and intermediate_outs is not None:
-            for layer_idx, intermediate_out in intermediate_outs:
-                # we assume intermediate_out has the same length & padding
-                # as those of encoder_out
-                loss_ic, cer_ic = self._calc_ctc_loss(
-                    intermediate_out, encoder_out_lens, text, text_lengths
-                )
-                loss_interctc = loss_interctc + loss_ic
-
-                # Collect Intermedaite CTC stats
-                stats["loss_interctc_layer{}".format(layer_idx)] = (
-                    loss_ic.detach() if loss_ic is not None else None
-                )
-                stats["cer_interctc_layer{}".format(layer_idx)] = cer_ic
-
-            loss_interctc = loss_interctc / len(intermediate_outs)
-
-            # calculate whole encoder loss
-            loss_ctc = (
-                               1 - self.interctc_weight
-                       ) * loss_ctc + self.interctc_weight * loss_interctc
-
-        # 2b. Attention decoder branch
-        if self.ctc_weight != 1.0:
-            loss_att, acc_att, cer_att, wer_att = self._calc_att_loss(
-                encoder_out, encoder_out_lens, text, text_lengths
-            )
+        # Check that batch_size is unified
+        assert (len(speech) == len(speaker_labels)), (len(speech), len(speaker_labels))
+        speech_lengths = torch.tensor([len(sph) for sph in speech]).to(torch.int64)
+        speaker_labels_lengths = torch.tensor([spk.shape[-1] for spk in speaker_labels]).to(torch.int64)
+        batch_size = len(speech)
+
+        # Encoder
+        encoder_out = self.forward_encoder(speech, speech_lengths)
+
+        # Encoder-decoder attractor
+        attractor_loss, attractors = self.encoder_decoder_attractor([e[order] for e, order in zip(encoder_out, orders)],
+                                                                    speaker_labels_lengths)
+        speaker_logits = [torch.matmul(e, att.permute(1, 0)) for e, att in zip(encoder_out, attractors)]
+
+        # pit loss
+        pit_speaker_labels = fast_batch_pit_n_speaker_loss(speaker_logits, speaker_labels)
+        pit_loss = standard_loss(speaker_logits, pit_speaker_labels)
+
+        # pse loss
+        with torch.no_grad():
+            power_ts = [create_powerlabel(label.cpu().numpy(), self.mapping_dict, self.max_n_speaker).
+                            to(encoder_out[0].device, non_blocking=True) for label in pit_speaker_labels]
+        pad_attractors = [pad_attractor(att, self.max_n_speaker) for att in attractors]
+        pse_speaker_logits = [torch.matmul(e, pad_att.permute(1, 0)) for e, pad_att in zip(encoder_out, pad_attractors)]
+        pse_speaker_logits = self.forward_post_net(pse_speaker_logits, speech_lengths)
+        pse_loss = cal_power_loss(pse_speaker_logits, power_ts)
 
-        # 3. CTC-Att loss definition
-        if self.ctc_weight == 0.0:
-            loss = loss_att
-        elif self.ctc_weight == 1.0:
-            loss = loss_ctc
-        else:
-            loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att
+        loss = pse_loss + pit_loss + self.attractor_loss_weight * attractor_loss
 
-        # Collect Attn branch stats
-        stats["loss_att"] = loss_att.detach() if loss_att is not None else None
-        stats["acc"] = acc_att
-        stats["cer"] = cer_att
-        stats["wer"] = wer_att
+        stats = dict()
+        stats["pse_loss"] = pse_loss.detach()
+        stats["pit_loss"] = pit_loss.detach()
+        stats["attractor_loss"] = attractor_loss.detach()
+        stats["batch_size"] = batch_size
 
         # Collect total loss stats
         stats["loss"] = torch.clone(loss.detach())
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
     def estimate_sequential(self,
                             speech: torch.Tensor,
-                            speech_lengths: torch.Tensor,
                             n_speakers: int = None,
                             shuffle: bool = True,
                             threshold: float = 0.5,
                             **kwargs):
-        speech = [s[:s_len] for s, s_len in zip(speech, speech_lengths)]
+        speech_lengths = torch.tensor([len(sph) for sph in speech]).to(torch.int64)
         emb = self.forward_encoder(speech, speech_lengths)
         if shuffle:
             orders = [np.arange(e.shape[0]) for e in emb]
             for order in orders:
                 np.random.shuffle(order)
-            attractors, probs = self.eda.estimate(
+            attractors, probs = self.encoder_decoder_attractor.estimate(
                 [e[torch.from_numpy(order).to(torch.long).to(speech[0].device)] for e, order in zip(emb, orders)])
         else:
-            attractors, probs = self.eda.estimate(emb)
+            attractors, probs = self.encoder_decoder_attractor.estimate(emb)
         attractors_active = []
         for p, att, e in zip(probs, attractors, emb):
             if n_speakers and n_speakers >= 0:
                 att = att[:n_speakers, ]
                 attractors_active.append(att)
             elif threshold is not None:
                 silence = torch.nonzero(p < threshold)[0]
```

### Comparing `funasr-0.7.1/funasr/models/e2e_diar_sond.py` & `funasr-0.7.2/funasr/models/e2e_diar_sond.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
-
+import logging
+import random
 from contextlib import contextmanager
 from distutils.version import LooseVersion
 from itertools import permutations
 from typing import Dict
 from typing import Optional
 from typing import Tuple, List
 
@@ -15,43 +16,42 @@
 
 from funasr.modules.nets_utils import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.specaug.abs_specaug import AbsSpecAug
+from funasr.models.specaug.abs_profileaug import AbsProfileAug
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.models.base_model import FunASRModel
 from funasr.losses.label_smoothing_loss import LabelSmoothingLoss, SequenceBinaryCrossEntropy
 from funasr.utils.misc import int2vec
+from funasr.utils.hinter import hint_once
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
 class DiarSondModel(FunASRModel):
-    """
-    Author: Speech Lab, Alibaba Group, China
-    SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
-    https://arxiv.org/abs/2211.10243
-    TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
-    https://arxiv.org/abs/2303.05397
+    """Speaker overlap-aware neural diarization model
+    reference: https://arxiv.org/abs/2211.10243
     """
 
     def __init__(
         self,
         vocab_size: int,
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
+        profileaug: Optional[AbsProfileAug],
         normalize: Optional[AbsNormalize],
         encoder: torch.nn.Module,
         speaker_encoder: Optional[torch.nn.Module],
         ci_scorer: torch.nn.Module,
         cd_scorer: Optional[torch.nn.Module],
         decoder: torch.nn.Module,
         token_list: list,
@@ -60,100 +60,155 @@
         max_spk_num: int = 16,
         label_aggregator: Optional[torch.nn.Module] = None,
         normalize_speech_speaker: bool = False,
         ignore_id: int = -1,
         speaker_discrimination_loss_weight: float = 1.0,
         inter_score_loss_weight: float = 0.0,
         inputs_type: str = "raw",
+        model_regularizer_weight: float = 0.0,
+        freeze_encoder: bool = False,
+        onfly_shuffle_speaker: bool = True,
     ):
 
         super().__init__()
 
         self.encoder = encoder
         self.speaker_encoder = speaker_encoder
         self.ci_scorer = ci_scorer
         self.cd_scorer = cd_scorer
         self.normalize = normalize
         self.frontend = frontend
         self.specaug = specaug
+        self.profileaug = profileaug
         self.label_aggregator = label_aggregator
         self.decoder = decoder
         self.token_list = token_list
         self.max_spk_num = max_spk_num
         self.normalize_speech_speaker = normalize_speech_speaker
         self.ignore_id = ignore_id
+        self.model_regularizer_weight = model_regularizer_weight
+        self.freeze_encoder = freeze_encoder
+        self.onfly_shuffle_speaker = onfly_shuffle_speaker
         self.criterion_diar = LabelSmoothingLoss(
             size=vocab_size,
             padding_idx=ignore_id,
             smoothing=lsm_weight,
             normalize_length=length_normalized_loss,
         )
         self.criterion_bce = SequenceBinaryCrossEntropy(normalize_length=length_normalized_loss)
         self.pse_embedding = self.generate_pse_embedding()
         self.power_weight = torch.from_numpy(2 ** np.arange(max_spk_num)[np.newaxis, np.newaxis, :]).float()
         self.int_token_arr = torch.from_numpy(np.array(self.token_list).astype(int)[np.newaxis, np.newaxis, :]).int()
         self.speaker_discrimination_loss_weight = speaker_discrimination_loss_weight
         self.inter_score_loss_weight = inter_score_loss_weight
         self.forward_steps = 0
         self.inputs_type = inputs_type
+        self.to_regularize_parameters = None
+
+    def get_regularize_parameters(self):
+        to_regularize_parameters, normal_parameters = [], []
+        for name, param in self.named_parameters():
+            if ("encoder" in name and "weight" in name and "bn" not in name and
+                ("conv2" in name or "conv1" in name or "conv_sc" in name or "dense" in name)
+            ):
+                to_regularize_parameters.append((name, param))
+            else:
+                normal_parameters.append((name, param))
+        self.to_regularize_parameters = to_regularize_parameters
+        return to_regularize_parameters, normal_parameters
 
     def generate_pse_embedding(self):
-        embedding = np.zeros((len(self.token_list), self.max_spk_num), dtype=np.float)
+        embedding = np.zeros((len(self.token_list), self.max_spk_num), dtype=np.float32)
         for idx, pse_label in enumerate(self.token_list):
-            emb = int2vec(int(pse_label), vec_dim=self.max_spk_num, dtype=np.float)
+            emb = int2vec(int(pse_label), vec_dim=self.max_spk_num, dtype=np.float32)
             embedding[idx] = emb
         return torch.from_numpy(embedding)
 
+    def rand_permute_speaker(self, raw_profile, raw_binary_labels):
+        """
+        raw_profile: B, N, D
+        raw_binary_labels: B, T, N
+        """
+        assert raw_profile.shape[1] == raw_binary_labels.shape[2], \
+            "Num profile: {}, Num label: {}".format(raw_profile.shape[1], raw_binary_labels.shape[-1])
+        profile = torch.clone(raw_profile)
+        binary_labels = torch.clone(raw_binary_labels)
+        bsz, num_spk = profile.shape[0], profile.shape[1]
+        for i in range(bsz):
+            idx = list(range(num_spk))
+            random.shuffle(idx)
+            profile[i] = profile[i][idx, :]
+            binary_labels[i] = binary_labels[i][:, idx]
+
+        return profile, binary_labels
+
     def forward(
         self,
         speech: torch.Tensor,
         speech_lengths: torch.Tensor = None,
         profile: torch.Tensor = None,
         profile_lengths: torch.Tensor = None,
         binary_labels: torch.Tensor = None,
         binary_labels_lengths: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Speaker Encoder + CI Scorer + CD Scorer + Decoder + Calc loss
+
         Args:
             speech: (Batch, samples) or (Batch, frames, input_size)
             speech_lengths: (Batch,) default None for chunk interator,
                                      because the chunk-iterator does not
                                      have the speech_lengths returned.
                                      see in
                                      espnet2/iterators/chunk_iter_factory.py
             profile: (Batch, N_spk, dim)
             profile_lengths: (Batch,)
             binary_labels: (Batch, frames, max_spk_num)
             binary_labels_lengths: (Batch,)
         """
         assert speech.shape[0] <= binary_labels.shape[0], (speech.shape, binary_labels.shape)
         batch_size = speech.shape[0]
+        if self.freeze_encoder:
+            hint_once("Freeze encoder", "freeze_encoder", rank=0)
+            self.encoder.eval()
         self.forward_steps = self.forward_steps + 1
         if self.pse_embedding.device != speech.device:
             self.pse_embedding = self.pse_embedding.to(speech.device)
             self.power_weight = self.power_weight.to(speech.device)
             self.int_token_arr = self.int_token_arr.to(speech.device)
 
-        # 1. Network forward
-        pred, inter_outputs = self.prediction_forward(
-            speech, speech_lengths,
-            profile, profile_lengths,
-            return_inter_outputs=True
-        )
-        (speech, speech_lengths), (profile, profile_lengths), (ci_score, cd_score) = inter_outputs
+        if self.onfly_shuffle_speaker:
+            hint_once("On-the-fly shuffle speaker permutation.", "onfly_shuffle_speaker", rank=0)
+            profile, binary_labels = self.rand_permute_speaker(profile, binary_labels)
 
-        # 2. Aggregate time-domain labels to match forward outputs
+        # 0a. Aggregate time-domain labels to match forward outputs
         if self.label_aggregator is not None:
             binary_labels, binary_labels_lengths = self.label_aggregator(
                 binary_labels, binary_labels_lengths
             )
-        # 2. Calculate power-set encoding (PSE) labels
-        raw_pse_labels = torch.sum(binary_labels * self.power_weight, dim=2, keepdim=True)
+        # 0b. augment profiles
+        if self.profileaug is not None and self.training:
+            speech, profile, binary_labels = self.profileaug(
+                speech, speech_lengths,
+                profile, profile_lengths,
+                binary_labels, binary_labels_lengths
+            )
+
+        # 1. Calculate power-set encoding (PSE) labels
+        pad_bin_labels = F.pad(binary_labels, (0, self.max_spk_num - binary_labels.shape[2]), "constant", 0.0)
+        raw_pse_labels = torch.sum(pad_bin_labels * self.power_weight, dim=2, keepdim=True)
         pse_labels = torch.argmax((raw_pse_labels.int() == self.int_token_arr).float(), dim=2)
 
+        # 2. Network forward
+        pred, inter_outputs = self.prediction_forward(
+            speech, speech_lengths,
+            profile, profile_lengths,
+            return_inter_outputs=True
+        )
+        (speech, speech_lengths), (profile, profile_lengths), (ci_score, cd_score) = inter_outputs
+
         # If encoder uses conv* as input_layer (i.e., subsampling),
         # the sequence length of 'pred' might be slightly less than the
         # length of 'spk_labels'. Here we force them to be equal.
         length_diff_tolerance = 2
         length_diff = abs(pse_labels.shape[1] - pred.shape[1])
         if length_diff <= length_diff_tolerance:
             min_len = min(pred.shape[1], pse_labels.shape[1])
@@ -161,17 +216,22 @@
             pred = pred[:, :min_len]
             cd_score = cd_score[:, :min_len]
             ci_score = ci_score[:, :min_len]
 
         loss_diar = self.classification_loss(pred, pse_labels, binary_labels_lengths)
         loss_spk_dis = self.speaker_discrimination_loss(profile, profile_lengths)
         loss_inter_ci, loss_inter_cd = self.internal_score_loss(cd_score, ci_score, pse_labels, binary_labels_lengths)
+        regularizer_loss = None
+        if self.model_regularizer_weight > 0 and self.to_regularize_parameters is not None:
+            regularizer_loss = self.calculate_regularizer_loss()
         label_mask = make_pad_mask(binary_labels_lengths, maxlen=pse_labels.shape[1]).to(pse_labels.device)
         loss = (loss_diar + self.speaker_discrimination_loss_weight * loss_spk_dis
                 + self.inter_score_loss_weight * (loss_inter_ci + loss_inter_cd))
+        # if regularizer_loss is not None:
+        #     loss = loss + regularizer_loss * self.model_regularizer_weight
 
         (
             correct,
             num_frames,
             speech_scored,
             speech_miss,
             speech_falarm,
@@ -200,27 +260,34 @@
 
         stats = dict(
             loss=loss.detach(),
             loss_diar=loss_diar.detach() if loss_diar is not None else None,
             loss_spk_dis=loss_spk_dis.detach() if loss_spk_dis is not None else None,
             loss_inter_ci=loss_inter_ci.detach() if loss_inter_ci is not None else None,
             loss_inter_cd=loss_inter_cd.detach() if loss_inter_cd is not None else None,
+            regularizer_loss=regularizer_loss.detach() if regularizer_loss is not None else None,
             sad_mr=sad_mr,
             sad_fr=sad_fr,
             mi=mi,
             fa=fa,
             cf=cf,
             acc=acc,
             der=der,
             forward_steps=self.forward_steps,
         )
 
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
+    def calculate_regularizer_loss(self):
+        regularizer_loss = 0.0
+        for name, param in self.to_regularize_parameters:
+            regularizer_loss = regularizer_loss + torch.norm(param, p=2)
+        return regularizer_loss
+
     def classification_loss(
             self,
             predictions: torch.Tensor,
             labels: torch.Tensor,
             prediction_lengths: torch.Tensor
     ) -> torch.Tensor:
         mask = make_pad_mask(prediction_lengths, maxlen=labels.shape[1])
@@ -384,14 +451,15 @@
             return logits, [(speech, speech_lengths), (profile, profile_lengths), (ci_simi, cd_simi)]
         return logits
 
     def encode(
         self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder
+
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch,)
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -483,8 +551,8 @@
             speech_scored,
             speech_miss,
             speech_falarm,
             speaker_scored,
             speaker_miss,
             speaker_falarm,
             speaker_error,
-        )
+        )
```

### Comparing `funasr-0.7.1/funasr/models/e2e_sa_asr.py` & `funasr-0.7.2/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_sv.py` & `funasr-0.7.2/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_tp.py` & `funasr-0.7.2/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_uni_asr.py` & `funasr-0.7.2/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/e2e_vad.py` & `funasr-0.7.2/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/branchformer_encoder.py` & `funasr-0.7.2/funasr/models/encoder/branchformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/conformer_encoder.py` & `funasr-0.7.2/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.7.2/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/e_branchformer_encoder.py` & `funasr-0.7.2/funasr/models/encoder/e_branchformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.7.2/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.7.2/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.7.2/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.7.2/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.7.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.7.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.7.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.7.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.7.2/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/rnn_encoder.py` & `funasr-0.7.2/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/sanm_encoder.py` & `funasr-0.7.2/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/encoder/transformer_encoder.py` & `funasr-0.7.2/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/default.py` & `funasr-0.7.2/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.7.2/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/fused.py` & `funasr-0.7.2/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/s3prl.py` & `funasr-0.7.2/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/wav_frontend.py` & `funasr-0.7.2/funasr/models/frontend/wav_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
                 continue
         elif line_item[0] == '<Rescale>':
             line_item = lines[i + 1].split()
             if line_item[0] == '<LearnRateCoef>':
                 rescale_line = line_item[3:(len(line_item) - 1)]
                 vars_list = list(rescale_line)
                 continue
-    means = np.array(means_list).astype(np.float)
-    vars = np.array(vars_list).astype(np.float)
+    means = np.array(means_list).astype(np.float32)
+    vars = np.array(vars_list).astype(np.float32)
     cmvn = np.array([means, vars])
     cmvn = torch.as_tensor(cmvn, dtype=torch.float32)
     return cmvn
 
 
 def apply_cmvn(inputs, cmvn):  # noqa
     """
```

### Comparing `funasr-0.7.1/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.7.2/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/frontend/windowing.py` & `funasr-0.7.2/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/joint_net/joint_network.py` & `funasr-0.7.2/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/pooling/statistic_pooling.py` & `funasr-0.7.2/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.7.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/predictor/cif.py` & `funasr-0.7.2/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/preencoder/linear.py` & `funasr-0.7.2/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/preencoder/sinc.py` & `funasr-0.7.2/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/seq_rnn_lm.py` & `funasr-0.7.2/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/specaug/specaug.py` & `funasr-0.7.2/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/target_delay_transformer.py` & `funasr-0.7.2/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/transformer_lm.py` & `funasr-0.7.2/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/models/vad_realtime_transformer.py` & `funasr-0.7.2/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/add_sos_eos.py` & `funasr-0.7.2/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/attention.py` & `funasr-0.7.2/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.7.2/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.7.2/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/beam_search/beam_search.py` & `funasr-0.7.2/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.7.2/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.7.2/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/cgmlp.py` & `funasr-0.7.2/funasr/modules/cgmlp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/data_utils.py` & `funasr-0.7.2/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/ema_module.py` & `funasr-0.7.2/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.7.2/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/quant_noise.py` & `funasr-0.7.2/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/utils.py` & `funasr-0.7.2/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.7.2/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/dynamic_conv.py` & `funasr-0.7.2/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/dynamic_conv2d.py` & `funasr-0.7.2/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/e2e_asr_common.py` & `funasr-0.7.2/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/eend_ola/encoder.py` & `funasr-0.7.2/funasr/modules/eend_ola/encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,47 +87,33 @@
                  n_layers: int,
                  n_units: int,
                  e_units: int = 2048,
                  h: int = 4,
                  dropout_rate: float = 0.1,
                  use_pos_emb: bool = False):
         super(EENDOLATransformerEncoder, self).__init__()
+        self.linear_in = nn.Linear(idim, n_units)
         self.lnorm_in = nn.LayerNorm(n_units)
         self.n_layers = n_layers
         self.dropout = nn.Dropout(dropout_rate)
         for i in range(n_layers):
             setattr(self, '{}{:d}'.format("lnorm1_", i),
                     nn.LayerNorm(n_units))
             setattr(self, '{}{:d}'.format("self_att_", i),
                     MultiHeadSelfAttention(n_units, h))
             setattr(self, '{}{:d}'.format("lnorm2_", i),
                     nn.LayerNorm(n_units))
             setattr(self, '{}{:d}'.format("ff_", i),
                     PositionwiseFeedForward(n_units, e_units, dropout_rate))
         self.lnorm_out = nn.LayerNorm(n_units)
-        if use_pos_emb:
-            self.pos_enc = torch.nn.Sequential(
-                torch.nn.Linear(idim, n_units),
-                torch.nn.LayerNorm(n_units),
-                torch.nn.Dropout(dropout_rate),
-                torch.nn.ReLU(),
-                PositionalEncoding(n_units, dropout_rate),
-            )
-        else:
-            self.linear_in = nn.Linear(idim, n_units)
-            self.pos_enc = None
 
     def __call__(self, x, x_mask=None):
         BT_size = x.shape[0] * x.shape[1]
-        if self.pos_enc is not None:
-            e = self.pos_enc(x)
-            e = e.view(BT_size, -1)
-        else:
-            e = self.linear_in(x.reshape(BT_size, -1))
+        e = self.linear_in(x.reshape(BT_size, -1))
         for i in range(self.n_layers):
             e = getattr(self, '{}{:d}'.format("lnorm1_", i))(e)
             s = getattr(self, '{}{:d}'.format("self_att_", i))(e, x.shape[0], x_mask)
             e = e + self.dropout(s)
             e = getattr(self, '{}{:d}'.format("lnorm2_", i))(e)
             s = getattr(self, '{}{:d}'.format("ff_", i))(e)
             e = e + self.dropout(s)
-        return self.lnorm_out(e)
+        return self.lnorm_out(e)
```

### Comparing `funasr-0.7.1/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.7.2/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/eend_ola/utils/power.py` & `funasr-0.7.2/funasr/modules/eend_ola/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/eend_ola/utils/report.py` & `funasr-0.7.2/funasr/modules/eend_ola/utils/report.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/embedding.py` & `funasr-0.7.2/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/fastformer.py` & `funasr-0.7.2/funasr/modules/fastformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/beamformer.py` & `funasr-0.7.2/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.7.2/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.7.2/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/feature_transform.py` & `funasr-0.7.2/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/frontend.py` & `funasr-0.7.2/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/frontends/mask_estimator.py` & `funasr-0.7.2/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/layer_norm.py` & `funasr-0.7.2/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/lightconv.py` & `funasr-0.7.2/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/lightconv2d.py` & `funasr-0.7.2/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/lora/layers.py` & `funasr-0.7.2/funasr/modules/lora/layers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/lora/utils.py` & `funasr-0.7.2/funasr/modules/lora/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/mask.py` & `funasr-0.7.2/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/multi_layer_conv.py` & `funasr-0.7.2/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/nets_utils.py` & `funasr-0.7.2/funasr/modules/nets_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,56 @@
 
     for i in range(n_batch):
         pad[i, : xs[i].size(0)] = xs[i]
 
     return pad
 
 
+def pad_list_all_dim(xs, pad_value):
+    """Perform padding for the list of tensors.
+
+    Args:
+        xs (List): List of Tensors [(T_1, `*`), (T_2, `*`), ..., (T_B, `*`)].
+        pad_value (float): Value for padding.
+
+    Returns:
+        Tensor: Padded tensor (B, Tmax, `*`).
+
+    Examples:
+        >>> x = [torch.ones(4), torch.ones(2), torch.ones(1)]
+        >>> x
+        [tensor([1., 1., 1., 1.]), tensor([1., 1.]), tensor([1.])]
+        >>> pad_list(x, 0)
+        tensor([[1., 1., 1., 1.],
+                [1., 1., 0., 0.],
+                [1., 0., 0., 0.]])
+
+    """
+    n_batch = len(xs)
+    num_dim = len(xs[0].shape)
+    max_len_all_dim = []
+    for i in range(num_dim):
+        max_len_all_dim.append(max(x.size(i) for x in xs))
+    pad = xs[0].new(n_batch, *max_len_all_dim).fill_(pad_value)
+
+    for i in range(n_batch):
+        if num_dim == 1:
+            pad[i, : xs[i].size(0)] = xs[i]
+        elif num_dim == 2:
+            pad[i, : xs[i].size(0), : xs[i].size(1)] = xs[i]
+        elif num_dim == 3:
+            pad[i, : xs[i].size(0), : xs[i].size(1), : xs[i].size(2)] = xs[i]
+        else:
+            raise ValueError(
+                "pad_list_all_dim only support 1-D, 2-D and 3-D tensors, not {}-D.".format(num_dim)
+            )
+
+    return pad
+
+
 def make_pad_mask(lengths, xs=None, length_dim=-1, maxlen=None):
     """Make mask tensor containing indices of padded part.
 
     Args:
         lengths (LongTensor or List): Batch of lengths (B,).
         xs (Tensor, optional): The reference tensor.
             If set, masks will be the same shape as this tensor.
```

### Comparing `funasr-0.7.1/funasr/modules/positionwise_feed_forward.py` & `funasr-0.7.2/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/repeat.py` & `funasr-0.7.2/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/rnn/argument.py` & `funasr-0.7.2/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/rnn/attentions.py` & `funasr-0.7.2/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/rnn/decoders.py` & `funasr-0.7.2/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/rnn/encoders.py` & `funasr-0.7.2/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/scorers/ctc.py` & `funasr-0.7.2/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.7.2/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/scorers/length_bonus.py` & `funasr-0.7.2/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/scorers/scorer_interface.py` & `funasr-0.7.2/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.7.2/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.7.2/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/streaming_utils/utils.py` & `funasr-0.7.2/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/subsampling.py` & `funasr-0.7.2/funasr/modules/subsampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,16 @@
 
     def forward(self, x, x_len):
         """Subsample x.
 
         """
         x = x.transpose(1, 2)  # (b, d ,t)
         x = self.pad_fn(x)
-        x = F.relu(self.conv(x))
+        #x = F.relu(self.conv(x))
+        x = F.leaky_relu(self.conv(x), negative_slope=0.)
         x = x.transpose(1, 2)  # (b, t ,d)
 
         if x_len is None:
 
             return x, None
         x_len = (x_len - 1) // self.stride + 1
         return x, x_len
```

### Comparing `funasr-0.7.1/funasr/modules/subsampling_without_posenc.py` & `funasr-0.7.2/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/modules/vgg2l.py` & `funasr-0.7.2/funasr/modules/vgg2l.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/optimizers/fairseq_adam.py` & `funasr-0.7.2/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/optimizers/sgd.py` & `funasr-0.7.2/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/demo.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/libtorch/setup.py` & `funasr-0.7.2/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from funasr_onnx import CT_Transformer
 
-model_dir = "damo/punc_ct-transformer_zh-cn-common-vocab272727-pytorch"
+#model_dir = "damo/punc_ct-transformer_zh-cn-common-vocab272727-pytorch"
+model_dir = "damo/punc_ct-transformer_cn-en-common-vocab471067-large"
 model = CT_Transformer(model_dir)
 
 text_in="跨境河流是养育沿岸人民的生命之源长期以来为帮助下游地区防灾减灾中方技术人员在上游地区极为恶劣的自然条件下克服巨大困难甚至冒着生命危险向印方提供汛期水文资料处理紧急事件中方重视印方在跨境河流问题上的关切愿意进一步完善双方联合工作机制凡是中方能做的我们都会去做而且会做得更好我请印度朋友们放心中国在上游的任何开发利用都会经过科学规划和论证兼顾上下游的利益"
 result = model(text_in)
 print(result[0])
```

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import List, Union, Tuple
 import numpy as np
 
 from .utils.utils import (ONNXRuntimeError,
                           OrtInferSession, get_logger,
                           read_yaml)
-from .utils.utils import (TokenIDConverter, split_to_mini_sentence,code_mix_split_words)
+from .utils.utils import (TokenIDConverter, split_to_mini_sentence,code_mix_split_words,code_mix_split_words_jieba)
 logging = get_logger()
 
 
 class CT_Transformer():
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
@@ -61,17 +61,26 @@
         for i in range(len(self.punc_list)):
             if self.punc_list[i] == ",":
                 self.punc_list[i] = "，"
             elif self.punc_list[i] == "?":
                 self.punc_list[i] = "？"
             elif self.punc_list[i] == "。":
                 self.period = i
+        if "seg_jieba" in config:
+            self.seg_jieba = True
+            self.jieba_usr_dict_path = os.path.join(model_dir, 'jieba_usr_dict')
+            self.code_mix_split_words_jieba = code_mix_split_words_jieba(self.jieba_usr_dict_path)
+        else:
+            self.seg_jieba = False
 
     def __call__(self, text: Union[list, str], split_size=20):
-        split_text = code_mix_split_words(text)
+        if self.seg_jieba:
+            split_text = self.code_mix_split_words_jieba(text)
+        else:
+            split_text = code_mix_split_words(text)
         split_text_id = self.converter.tokens2ids(split_text)
         mini_sentences = split_to_mini_sentence(split_text, split_size)
         mini_sentences_id = split_to_mini_sentence(split_text_id, split_size)
         assert len(mini_sentences) == len(mini_sentences_id)
         cache_sent = []
         cache_sent_id = []
         new_mini_sentence = ""
```

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files 6% similar despite different names*

```diff
@@ -345,14 +345,36 @@
     i = np.iinfo(middle_data.dtype)
     abs_max = 2 ** (i.bits - 1)
     offset = i.min + abs_max
     array = np.frombuffer((middle_data.astype(dtype) - offset) / abs_max, dtype=np.float32)
     return array
 
 
+class SinusoidalPositionEncoderOnline():
+    '''Streaming Positional encoding.
+    '''
+
+    def encode(self, positions: np.ndarray = None, depth: int = None, dtype: np.dtype = np.float32):
+        batch_size = positions.shape[0]
+        positions = positions.astype(dtype)
+        log_timescale_increment = np.log(np.array([10000], dtype=dtype)) / (depth / 2 - 1)
+        inv_timescales = np.exp(np.arange(depth / 2).astype(dtype) * (-log_timescale_increment))
+        inv_timescales = np.reshape(inv_timescales, [batch_size, -1])
+        scaled_time = np.reshape(positions, [1, -1, 1]) * np.reshape(inv_timescales, [1, 1, -1])
+        encoding = np.concatenate((np.sin(scaled_time), np.cos(scaled_time)), axis=2)
+        return encoding.astype(dtype)
+
+    def forward(self, x, start_idx=0):
+        batch_size, timesteps, input_dim = x.shape
+        positions = np.arange(1, timesteps+1+start_idx)[None, :]
+        position_encoding = self.encode(positions, input_dim, x.dtype)
+
+        return x + position_encoding[:, start_idx: start_idx + timesteps]
+
+
 def test():
     path = "/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav"
     import librosa
     cmvn_file = "/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/am.mvn"
     config_file = "/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/config.yaml"
     from funasr.runtime.python.onnxruntime.rapid_paraformer.utils.utils import read_yaml
     config = read_yaml(config_file)
```

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 
 import functools
 import logging
 import pickle
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
+import re
 import numpy as np
 import yaml
-from onnxruntime import (GraphOptimizationLevel, InferenceSession,
-                         SessionOptions, get_available_providers, get_device)
-
+try:
+    from onnxruntime import (GraphOptimizationLevel, InferenceSession,
+                             SessionOptions, get_available_providers, get_device)
+except:
+    print("please pip3 install onnxruntime")
+import jieba
 import warnings
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
@@ -226,14 +230,72 @@
                     words.append(current_word)
                     current_word = ""
                 words.append(c)
         if len(current_word) > 0:
             words.append(current_word)
     return words
 
+def isEnglish(text:str):
+    if re.search('^[a-zA-Z\']+$', text):
+        return True
+    else:
+        return False
+
+def join_chinese_and_english(input_list):
+    line = ''
+    for token in input_list:
+        if isEnglish(token):
+            line = line + ' ' + token
+        else:
+            line = line + token
+
+    line = line.strip()
+    return line
+
+def code_mix_split_words_jieba(seg_dict_file: str):
+    jieba.load_userdict(seg_dict_file)
+
+    def _fn(text: str):
+        input_list = text.split()
+        token_list_all = []
+        langauge_list = []
+        token_list_tmp = []
+        language_flag = None
+        for token in input_list:
+            if isEnglish(token) and language_flag == 'Chinese':
+                token_list_all.append(token_list_tmp)
+                langauge_list.append('Chinese')
+                token_list_tmp = []
+            elif not isEnglish(token) and language_flag == 'English':
+                token_list_all.append(token_list_tmp)
+                langauge_list.append('English')
+                token_list_tmp = []
+    
+            token_list_tmp.append(token)
+    
+            if isEnglish(token):
+                language_flag = 'English'
+            else:
+                language_flag = 'Chinese'
+    
+        if token_list_tmp:
+            token_list_all.append(token_list_tmp)
+            langauge_list.append(language_flag)
+    
+        result_list = []
+        for token_list_tmp, language_flag in zip(token_list_all, langauge_list):
+            if language_flag == 'English':
+                result_list.extend(token_list_tmp)
+            else:
+                seg_list = jieba.cut(join_chinese_and_english(token_list_tmp), HMM=False)
+                result_list.extend(seg_list)
+    
+        return result_list
+    return _fn
+
 def read_yaml(yaml_path: Union[str, Path]) -> Dict:
     if not Path(yaml_path).exists():
         raise FileExistsError(f'The {yaml_path} does not exist.')
 
     with open(str(yaml_path), 'rb') as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
```

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.7.2/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/build_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/folded_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/length_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.7.2/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/schedulers/abs_scheduler.py` & `funasr-0.7.2/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/schedulers/noam_lr.py` & `funasr-0.7.2/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.7.2/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/schedulers/warmup_lr.py` & `funasr-0.7.2/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/abs_task.py` & `funasr-0.7.2/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/asr.py` & `funasr-0.7.2/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/data2vec.py` & `funasr-0.7.2/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/diar.py` & `funasr-0.7.2/funasr/tasks/diar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-Author: Speech Lab, Alibaba Group, China
-SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
-https://arxiv.org/abs/2211.10243
-TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
-https://arxiv.org/abs/2303.05397
-"""
-
 import argparse
 import logging
 import os
 from pathlib import Path
 from typing import Callable
 from typing import Collection
 from typing import Dict
@@ -18,49 +10,54 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
 
-from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.collate_fn import DiarCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
-from funasr.layers.label_aggregation import LabelAggregate
 from funasr.layers.utterance_mvn import UtteranceMVN
-from funasr.models.e2e_diar_sond import DiarSondModel
-from funasr.models.e2e_diar_eend_ola import DiarEENDOLAModel
-from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.models.encoder.conformer_encoder import ConformerEncoder
-from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.layers.label_aggregation import LabelAggregate, LabelAggregateMaxPooling
+from funasr.models.ctc import CTC
+from funasr.models.encoder.resnet34_encoder import ResNet34Diar, ResNet34SpL2RegDiar
 from funasr.models.encoder.ecapa_tdnn_encoder import ECAPA_TDNN
-from funasr.models.encoder.opennmt_encoders.ci_scorers import DotScorer, CosScorer
 from funasr.models.encoder.opennmt_encoders.conv_encoder import ConvEncoder
 from funasr.models.encoder.opennmt_encoders.fsmn_encoder import FsmnEncoder
 from funasr.models.encoder.opennmt_encoders.self_attention_encoder import SelfAttentionEncoder
-from funasr.models.encoder.resnet34_encoder import ResNet34Diar, ResNet34SpL2RegDiar
+from funasr.models.encoder.opennmt_encoders.ci_scorers import DotScorer, CosScorer
+from funasr.models.e2e_diar_sond import DiarSondModel
+from funasr.models.encoder.abs_encoder import AbsEncoder
+from funasr.models.encoder.conformer_encoder import ConformerEncoder
+from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
+from funasr.models.postencoder.hugging_face_transformers_postencoder import (
+    HuggingFaceTransformersPostEncoder,  # noqa: H301
+)
+from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
+from funasr.models.preencoder.linear import LinearProjection
+from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
-from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
-from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
+from funasr.models.specaug.abs_profileaug import AbsProfileAug
+from funasr.models.specaug.profileaug import ProfileAug
 from funasr.tasks.abs_task import AbsTask
 from funasr.torch_utils.initialize import initialize
-from funasr.models.base_model import FunASRModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
 
@@ -68,55 +65,63 @@
     name="frontend",
     classes=dict(
         default=DefaultFrontend,
         sliding_window=SlidingWindow,
         s3prl=S3prlFrontend,
         fused=FusedFrontends,
         wav_frontend=WavFrontend,
-        wav_frontend_mel23=WavFrontendMel23,
     ),
     type_check=AbsFrontend,
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
     classes=dict(
         specaug=SpecAug,
         specaug_lfr=SpecAugLFR,
     ),
     type_check=AbsSpecAug,
     default=None,
     optional=True,
 )
+profileaug_choices = ClassChoices(
+    name="profileaug",
+    classes=dict(
+        profileaug=ProfileAug,
+    ),
+    type_check=AbsProfileAug,
+    default=None,
+    optional=True,
+)
 normalize_choices = ClassChoices(
     "normalize",
     classes=dict(
         global_mvn=GlobalMVN,
         utterance_mvn=UtteranceMVN,
     ),
     type_check=AbsNormalize,
     default=None,
     optional=True,
 )
 label_aggregator_choices = ClassChoices(
     "label_aggregator",
     classes=dict(
-        label_aggregator=LabelAggregate
+        label_aggregator=LabelAggregate,
+        label_aggregator_max_pool=LabelAggregateMaxPooling,
     ),
     type_check=torch.nn.Module,
     default=None,
     optional=True,
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
         sond=DiarSondModel,
-        eend_ola=DiarEENDOLAModel,
     ),
-    type_check=FunASRModel,
+    type_check=torch.nn.Module,
     default="sond",
 )
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
         conformer=ConformerEncoder,
         transformer=TransformerEncoder,
@@ -126,15 +131,14 @@
         fsmn=FsmnEncoder,
         conv=ConvEncoder,
         resnet34=ResNet34Diar,
         resnet34_sp_l2reg=ResNet34SpL2RegDiar,
         sanm_chunk_opt=SANMEncoderChunkOpt,
         data2vec_encoder=Data2VecEncoder,
         ecapa_tdnn=ECAPA_TDNN,
-        eend_ola_transformer=EENDOLATransformerEncoder,
     ),
     type_check=torch.nn.Module,
     default="resnet34",
 )
 speaker_encoder_choices = ClassChoices(
     "speaker_encoder",
     classes=dict(
@@ -178,35 +182,28 @@
     classes=dict(
         rnn=RNNEncoder,
         fsmn=FsmnEncoder,
     ),
     type_check=torch.nn.Module,
     default="fsmn",
 )
-# encoder_decoder_attractor is used for EEND-OLA
-encoder_decoder_attractor_choices = ClassChoices(
-    "encoder_decoder_attractor",
-    classes=dict(
-        eda=EncoderDecoderAttractor,
-    ),
-    type_check=torch.nn.Module,
-    default="eda",
-)
 
 
 class DiarTask(AbsTask):
     # If you need more than 1 optimizer, change this value
     num_optimizers: int = 1
 
     # Add variable objects configurations
     class_choices_list = [
         # --frontend and --frontend_conf
         frontend_choices,
         # --specaug and --specaug_conf
         specaug_choices,
+        # --profileaug and --profileaug_conf
+        profileaug_choices,
         # --normalize and --normalize_conf
         normalize_choices,
         # --label_aggregator and --label_aggregator_conf
         label_aggregator_choices,
         # --model and --model_conf
         model_choices,
         # --encoder and --encoder_conf
@@ -339,15 +336,15 @@
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
-        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
+        return DiarCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
         if args.use_preprocessor:
             retval = CommonPreprocessor(
@@ -395,14 +392,49 @@
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         return retval
 
     @classmethod
+    def build_optimizers(
+            cls,
+            args: argparse.Namespace,
+            model: torch.nn.Module,
+    ) -> List[torch.optim.Optimizer]:
+        if cls.num_optimizers != 1:
+            raise RuntimeError(
+                "build_optimizers() must be overridden if num_optimizers != 1"
+            )
+        from funasr.tasks.abs_task import optim_classes
+        optim_class = optim_classes.get(args.optim)
+        if optim_class is None:
+            raise ValueError(f"must be one of {list(optim_classes)}: {args.optim}")
+        else:
+            if (hasattr(model, "model_regularizer_weight") and
+                model.model_regularizer_weight > 0.0 and
+                hasattr(model, "get_regularize_parameters")
+            ):
+                to_regularize_parameters, normal_parameters = model.get_regularize_parameters()
+                logging.info(f"Set weight decay {model.model_regularizer_weight} for parameters: "
+                             f"{[name for name, value in to_regularize_parameters]}")
+                module_optim_config = [
+                    {"params": [value for name, value in to_regularize_parameters],
+                     "weight_decay": model.model_regularizer_weight},
+                    {"params": [value for name, value in normal_parameters],
+                     "weight_decay": 0.0}
+                ]
+                optim = optim_class(module_optim_config, **args.optim_conf)
+            else:
+                optim = optim_class(model.parameters(), **args.optim_conf)
+
+        optimizers = [optim]
+        return optimizers
+
+    @classmethod
     def build_model(cls, args: argparse.Namespace):
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
@@ -432,14 +464,21 @@
         # 2. Data augmentation for spectrogram
         if args.specaug is not None:
             specaug_class = specaug_choices.get_class(args.specaug)
             specaug = specaug_class(**args.specaug_conf)
         else:
             specaug = None
 
+        # 2b. Data augmentation for Profiles
+        if hasattr(args, "profileaug") and args.profileaug is not None:
+            profileaug_class = profileaug_choices.get_class(args.profileaug)
+            profileaug = profileaug_class(**args.profileaug_conf)
+        else:
+            profileaug = None
+
         # 3. Normalization layer
         if args.normalize is not None:
             normalize_class = normalize_choices.get_class(args.normalize)
             normalize = normalize_class(**args.normalize_conf)
         else:
             normalize = None
 
@@ -479,28 +518,30 @@
 
         # 9. Build model
         model_class = model_choices.get_class(args.model)
         model = model_class(
             vocab_size=vocab_size,
             frontend=frontend,
             specaug=specaug,
+            profileaug=profileaug,
             normalize=normalize,
             label_aggregator=label_aggregator,
             encoder=encoder,
             speaker_encoder=speaker_encoder,
             ci_scorer=ci_scorer,
             cd_scorer=cd_scorer,
             decoder=decoder,
             token_list=token_list,
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
+            logging.info(f"Init model parameters with {args.init}.")
 
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
@@ -531,38 +572,38 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, FunASRModel):
+        if not isinstance(model, torch.nn.Module):
             raise RuntimeError(
-                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
+                f"model must inherit {torch.nn.Module.__name__}, but got {type(model)}"
             )
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
             if device == "cuda":
                 device = f"cuda:{torch.cuda.current_device()}"
             model_dir = os.path.dirname(model_file)
             model_name = os.path.basename(model_file)
             if "model.ckpt-" in model_name or ".bin" in model_name:
                 if ".bin" in model_name:
                     model_name_pth = os.path.join(model_dir, model_name.replace('.bin', '.pb'))
                 else:
-                    model_name_pth = os.path.join(model_dir, "{}.pb".format(model_name))
+                    model_name_pth = os.path.join(model_dir, "{}.pth".format(model_name))
                 if os.path.exists(model_name_pth):
                     logging.info("model_file is load from pth: {}".format(model_name_pth))
                     model_dict = torch.load(model_name_pth, map_location=device)
                 else:
                     model_dict = cls.convert_tf2torch(model, model_file)
-                model.load_state_dict(model_dict)
+                # model.load_state_dict(model_dict)
             else:
                 model_dict = torch.load(model_file, map_location=device)
         model_dict = cls.fileter_model_dict(model_dict, model.state_dict())
         model.load_state_dict(model_dict)
         if model_name_pth is not None and not os.path.exists(model_name_pth):
             torch.save(model_dict, model_name_pth)
             logging.info("model_file is saved to pth: {}".format(model_name_pth))
@@ -612,291 +653,7 @@
             var_dict_torch_update.update(var_dict_torch_update_local)
         # decoder
         if model.decoder is not None:
             var_dict_torch_update_local = model.decoder.convert_tf2torch(var_dict_tf, var_dict_torch)
             var_dict_torch_update.update(var_dict_torch_update_local)
 
         return var_dict_torch_update
-
-
-class EENDOLADiarTask(AbsTask):
-    # If you need more than 1 optimizer, change this value
-    num_optimizers: int = 1
-
-    # Add variable objects configurations
-    class_choices_list = [
-        # --frontend and --frontend_conf
-        frontend_choices,
-        # --specaug and --specaug_conf
-        model_choices,
-        # --encoder and --encoder_conf
-        encoder_choices,
-        # --speaker_encoder and --speaker_encoder_conf
-        encoder_decoder_attractor_choices,
-    ]
-
-    # If you need to modify train() or eval() procedures, change Trainer class here
-    trainer = Trainer
-
-    @classmethod
-    def add_task_arguments(cls, parser: argparse.ArgumentParser):
-        group = parser.add_argument_group(description="Task related")
-
-        # NOTE(kamo): add_arguments(..., required=True) can't be used
-        # to provide --print_config mode. Instead of it, do as
-        # required = parser.get_default("required")
-        # required += ["token_list"]
-
-        group.add_argument(
-            "--token_list",
-            type=str_or_none,
-            default=None,
-            help="A text mapping int-id to token",
-        )
-        group.add_argument(
-            "--split_with_space",
-            type=str2bool,
-            default=True,
-            help="whether to split text using <space>",
-        )
-        group.add_argument(
-            "--seg_dict_file",
-            type=str,
-            default=None,
-            help="seg_dict_file for text processing",
-        )
-        group.add_argument(
-            "--init",
-            type=lambda x: str_or_none(x.lower()),
-            default=None,
-            help="The initialization method",
-            choices=[
-                "chainer",
-                "xavier_uniform",
-                "xavier_normal",
-                "kaiming_uniform",
-                "kaiming_normal",
-                None,
-            ],
-        )
-
-        group.add_argument(
-            "--input_size",
-            type=int_or_none,
-            default=None,
-            help="The number of input dimension of the feature",
-        )
-
-        group = parser.add_argument_group(description="Preprocess related")
-        group.add_argument(
-            "--use_preprocessor",
-            type=str2bool,
-            default=True,
-            help="Apply preprocessing to data or not",
-        )
-        group.add_argument(
-            "--token_type",
-            type=str,
-            default="char",
-            choices=["char"],
-            help="The text will be tokenized in the specified level token",
-        )
-        parser.add_argument(
-            "--speech_volume_normalize",
-            type=float_or_none,
-            default=None,
-            help="Scale the maximum amplitude to the given value.",
-        )
-        parser.add_argument(
-            "--rir_scp",
-            type=str_or_none,
-            default=None,
-            help="The file path of rir scp file.",
-        )
-        parser.add_argument(
-            "--rir_apply_prob",
-            type=float,
-            default=1.0,
-            help="THe probability for applying RIR convolution.",
-        )
-        parser.add_argument(
-            "--cmvn_file",
-            type=str_or_none,
-            default=None,
-            help="The file path of noise scp file.",
-        )
-        parser.add_argument(
-            "--noise_scp",
-            type=str_or_none,
-            default=None,
-            help="The file path of noise scp file.",
-        )
-        parser.add_argument(
-            "--noise_apply_prob",
-            type=float,
-            default=1.0,
-            help="The probability applying Noise adding.",
-        )
-        parser.add_argument(
-            "--noise_db_range",
-            type=str,
-            default="13_15",
-            help="The range of noise decibel level.",
-        )
-
-        for class_choices in cls.class_choices_list:
-            # Append --<name> and --<name>_conf.
-            # e.g. --encoder and --encoder_conf
-            class_choices.add_arguments(group)
-
-    @classmethod
-    def build_collate_fn(
-            cls, args: argparse.Namespace, train: bool
-    ) -> Callable[
-        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
-        Tuple[List[str], Dict[str, torch.Tensor]],
-    ]:
-        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
-        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
-
-    @classmethod
-    def build_preprocess_fn(
-            cls, args: argparse.Namespace, train: bool
-    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        # if args.use_preprocessor:
-        #     retval = CommonPreprocessor(
-        #         train=train,
-        #         token_type=args.token_type,
-        #         token_list=args.token_list,
-        #         bpemodel=None,
-        #         non_linguistic_symbols=None,
-        #         text_cleaner=None,
-        #         g2p_type=None,
-        #         split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
-        #         seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
-        #         # NOTE(kamo): Check attribute existence for backward compatibility
-        #         rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
-        #         rir_apply_prob=args.rir_apply_prob
-        #         if hasattr(args, "rir_apply_prob")
-        #         else 1.0,
-        #         noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
-        #         noise_apply_prob=args.noise_apply_prob
-        #         if hasattr(args, "noise_apply_prob")
-        #         else 1.0,
-        #         noise_db_range=args.noise_db_range
-        #         if hasattr(args, "noise_db_range")
-        #         else "13_15",
-        #         speech_volume_normalize=args.speech_volume_normalize
-        #         if hasattr(args, "rir_scp")
-        #         else None,
-        #     )
-        # else:
-        #     retval = None
-        return None
-
-    @classmethod
-    def required_data_names(
-            cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        if not inference:
-            retval = ("speech", )
-        else:
-            # Recognition mode
-            retval = ("speech", )
-        return retval
-
-    @classmethod
-    def optional_data_names(
-            cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        retval = ()
-        return retval
-
-    @classmethod
-    def build_model(cls, args: argparse.Namespace):
-
-        # 1. frontend
-        if args.input_size is None or args.frontend == "wav_frontend_mel23":
-            # Extract features in the model
-            frontend_class = frontend_choices.get_class(args.frontend)
-            if args.frontend == 'wav_frontend':
-                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
-            else:
-                frontend = frontend_class(**args.frontend_conf)
-            input_size = frontend.output_size()
-        else:
-            # Give features from data-loader
-            args.frontend = None
-            args.frontend_conf = {}
-            frontend = None
-            input_size = args.input_size
-
-        # 2. Encoder
-        encoder_class = encoder_choices.get_class(args.encoder)
-        encoder = encoder_class(**args.encoder_conf)
-
-        # 3. EncoderDecoderAttractor
-        encoder_decoder_attractor_class = encoder_decoder_attractor_choices.get_class(args.encoder_decoder_attractor)
-        encoder_decoder_attractor = encoder_decoder_attractor_class(**args.encoder_decoder_attractor_conf)
-
-        # 9. Build model
-        model_class = model_choices.get_class(args.model)
-        model = model_class(
-            frontend=frontend,
-            encoder=encoder,
-            encoder_decoder_attractor=encoder_decoder_attractor,
-            **args.model_conf,
-        )
-
-        # 10. Initialize
-        if args.init is not None:
-            initialize(model, args.init)
-
-        return model
-
-    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
-    @classmethod
-    def build_model_from_file(
-            cls,
-            config_file: Union[Path, str] = None,
-            model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            device: str = "cpu",
-    ):
-        """Build model from the files.
-
-        This method is used for inference or fine-tuning.
-
-        Args:
-            config_file: The yaml file saved when training.
-            model_file: The model file saved when training.
-            cmvn_file: The cmvn file for front-end
-            device: Device type, "cpu", "cuda", or "cuda:N".
-
-        """
-        if config_file is None:
-            assert model_file is not None, (
-                "The argument 'model_file' must be provided "
-                "if the argument 'config_file' is not specified."
-            )
-            config_file = Path(model_file).parent / "config.yaml"
-        else:
-            config_file = Path(config_file)
-
-        with config_file.open("r", encoding="utf-8") as f:
-            args = yaml.safe_load(f)
-        args = argparse.Namespace(**args)
-        model = cls.build_model(args)
-        if not isinstance(model, FunASRModel):
-            raise RuntimeError(
-                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
-            )
-        if model_file is not None:
-            if device == "cuda":
-                device = f"cuda:{torch.cuda.current_device()}"
-            checkpoint = torch.load(model_file, map_location=device)
-            if "state_dict" in checkpoint.keys():
-                model.load_state_dict(checkpoint["state_dict"])
-            else:
-                model.load_state_dict(checkpoint)
-        model.to(device)
-        return model, args
```

### Comparing `funasr-0.7.1/funasr/tasks/lm.py` & `funasr-0.7.2/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/punctuation.py` & `funasr-0.7.2/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/sa_asr.py` & `funasr-0.7.2/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/sv.py` & `funasr-0.7.2/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/tasks/vad.py` & `funasr-0.7.2/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/build_tokenizer.py` & `funasr-0.7.2/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/char_tokenizer.py` & `funasr-0.7.2/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/cleaner.py` & `funasr-0.7.2/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/korean_cleaner.py` & `funasr-0.7.2/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/phoneme_tokenizer.py` & `funasr-0.7.2/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.7.2/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/token_id_converter.py` & `funasr-0.7.2/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/text/word_tokenizer.py` & `funasr-0.7.2/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.7.2/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/device_funcs.py` & `funasr-0.7.2/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/forward_adaptor.py` & `funasr-0.7.2/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/initialize.py` & `funasr-0.7.2/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.7.2/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/model_summary.py` & `funasr-0.7.2/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/torch_utils/recursive_op.py` & `funasr-0.7.2/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/train/abs_model.py` & `funasr-0.7.2/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/train/class_choices.py` & `funasr-0.7.2/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/train/distributed_utils.py` & `funasr-0.7.2/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/train/reporter.py` & `funasr-0.7.2/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/train/trainer.py` & `funasr-0.7.2/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/asr_env_checking.py` & `funasr-0.7.2/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/asr_utils.py` & `funasr-0.7.2/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/cli_utils.py` & `funasr-0.7.2/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/compute_eer.py` & `funasr-0.7.2/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/compute_min_dcf.py` & `funasr-0.7.2/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/compute_wer.py` & `funasr-0.7.2/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/config_argparse.py` & `funasr-0.7.2/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/get_default_kwargs.py` & `funasr-0.7.2/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/griffin_lim.py` & `funasr-0.7.2/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/job_runner.py` & `funasr-0.7.2/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/misc.py` & `funasr-0.7.2/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/modelscope_param.py` & `funasr-0.7.2/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/modelscope_utils.py` & `funasr-0.7.2/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/nested_dict_action.py` & `funasr-0.7.2/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/postprocess_utils.py` & `funasr-0.7.2/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/prepare_data.py` & `funasr-0.7.2/funasr/utils/prepare_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,30 +192,31 @@
             for file_name in file_names:
                 path = path + " " + os.path.join(split_path, str(i + 1), file_name)
             f_data.write(path + "\n")
 
 
 def prepare_data(args, distributed_option):
     distributed = distributed_option.distributed
+    data_names = args.dataset_conf.get("data_names", "speech,text").split(",")
+    data_types = args.dataset_conf.get("data_types", "sound,text").split(",")
+    file_names = args.data_file_names.split(",")
+    batch_type = args.dataset_conf["batch_conf"]["batch_type"]
     if not distributed or distributed_option.dist_rank == 0:
         if hasattr(args, "filter_input") and args.filter_input:
             filter_wav_text(args.data_dir, args.train_set)
             filter_wav_text(args.data_dir, args.valid_set)
 
-        if args.dataset_type == "small":
+        if args.dataset_type == "small" and batch_type != "unsorted":
             calc_shape(args, args.train_set)
             calc_shape(args, args.valid_set)
 
         if args.dataset_type == "large":
             generate_data_list(args, args.data_dir, args.train_set)
             generate_data_list(args, args.data_dir, args.valid_set)
 
-    data_names = args.dataset_conf.get("data_names", "speech,text").split(",")
-    data_types = args.dataset_conf.get("data_types", "sound,text").split(",")
-    file_names = args.data_file_names.split(",")
     print("data_names: {}, data_types: {}, file_names: {}".format(data_names, data_types, file_names))
     assert len(data_names) == len(data_types) == len(file_names)
     if args.dataset_type == "small":
         args.train_shape_file = [os.path.join(args.data_dir, args.train_set, "{}_shape".format(data_names[0]))]
         args.valid_shape_file = [os.path.join(args.data_dir, args.valid_set, "{}_shape".format(data_names[0]))]
         args.train_data_path_and_name_and_type, args.valid_data_path_and_name_and_type = [], []
         for file_name, data_name, data_type in zip(file_names, data_names, data_types):
```

### Comparing `funasr-0.7.1/funasr/utils/runtime_sdk_download_tool.py` & `funasr-0.7.2/funasr/utils/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/sized_dict.py` & `funasr-0.7.2/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/timestamp_tools.py` & `funasr-0.7.2/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/types.py` & `funasr-0.7.2/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/vad_utils.py` & `funasr-0.7.2/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr/utils/wav_utils.py` & `funasr-0.7.2/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/funasr.egg-info/PKG-INFO` & `funasr-0.7.2/funasr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.7.1
+Version: 0.7.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -49,17 +49,17 @@
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker Diarization and multi-talker ASR. FunASR provides convenient scripts and tutorials, supporting inference and fine-tuning of pre-trained models.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition model, has the advantages of high accuracy, high efficiency, and convenient deployment, supporting the rapid construction of speech recognition services. For more details on service deployment, please refer to the [service deployment document](funasr/runtime/readme_cn.md). 
 
 
 <a name="whats-new"></a>
 ## What's new: 
-
+- 2023/08/07: The real-time transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial_online.md)).
 - 2023/07/17: BAT is released, which is a low-latency and low-memory-consumption RNN-T model. For more details, please refer to ([BAT](egs/aishell/bat)).
-- 2023/07/03: The CPU version of the Chinese offline file transcription service has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
+- 2023/07/03: The offline file transcription service (CPU) of Mandarin has been released. For more details, please refer to ([Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)).
 - 2023/06/26: ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0 completed the competition and announced the results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 
 <a name="Installation"></a>
 ## Installation
 
 Please ref to [installation docs](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
@@ -67,14 +67,16 @@
 ## Deployment Service
 
 FunASR supports pre-trained or further fine-tuned models for deployment as a service. The CPU version of the Chinese offline file conversion service has been released, details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More detailed information about service deployment can be found in the [deployment roadmap](funasr/runtime/readme_cn.md).
 
 
 <a name="quick-start"></a>
 ## Quick Start
+Quick start for new users（[tutorial](https://alibaba-damo-academy.github.io/FunASR/en/funasr/quick_start_zh.html)）
+
 
 FunASR supports inference and fine-tuning of models trained on industrial datasets of tens of thousands of hours. For more details, please refer to ([modelscope_egs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also supports training and fine-tuning of models on academic standard datasets. For more details, please refer to([egs](https://alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The models include speech recognition (ASR), speech activity detection (VAD), punctuation recovery, language model, speaker verification, speaker separation, and multi-party conversation speech recognition. For a detailed list of models, please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md):
 
 <a name="Community Communication"></a>
 ## Community Communication
 If you encounter problems in use, you can directly raise Issues on the github page.
 
@@ -82,16 +84,16 @@
 
 |DingTalk group |                     WeChat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> | <img src="docs/images/XVERSE.png" width="250"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:------------------------------------------------------:|
 
 The contributors can be found in [contributors list]((./Acknowledge))
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
@@ -106,14 +108,20 @@
 }
 @inproceedings{An2023bat,
   author={Keyu An and Xian Shi and Shiliang Zhang},
   title={BAT: Boundary aware transducer for memory-efficient and low-latency ASR},
   year={2023},
   booktitle={INTERSPEECH},
 }
+@inproceedings{wang2023told,
+  author={Jiaming Wang and Zhihao Du and Shiliang Zhang},
+  title={{TOLD:} {A} Novel Two-Stage Overlap-Aware Framework for Speaker Diarization},
+  year={2023},
+  booktitle={ICASSP},
+}
 @inproceedings{gao22b_interspeech,
   author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
   title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
   year=2022,
   booktitle={Proc. Interspeech 2022},
   pages={2063--2067},
   doi={10.21437/Interspeech.2022-9996}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.7.1 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.7.2 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -39,66 +39,73 @@
 [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
 model_zoo/modelscope_models.md). The representative [Paraformer-large](https://
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary), a non-autoregressive end-to-end speech recognition
 model, has the advantages of high accuracy, high efficiency, and convenient
 deployment, supporting the rapid construction of speech recognition services.
 For more details on service deployment, please refer to the [service deployment
-document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/07/17: BAT is
-released, which is a low-latency and low-memory-consumption RNN-T model. For
-more details, please refer to ([BAT](egs/aishell/bat)). - 2023/07/03: The CPU
-version of the Chinese offline file transcription service has been released.
-For more details, please refer to ([Deployment documentation](funasr/runtime/
-docs/SDK_tutorial.md)). - 2023/06/26: ASRU2023 Multi-Channel Multi-Party
-Meeting Transcription Challenge 2.0 completed the competition and announced the
-results. For more details, please refer to ([M2MeT2.0](https://alibaba-damo-
-academy.github.io/FunASR/m2met2/index.html)).  ## Installation Please ref to
-[installation docs](https://alibaba-damo-academy.github.io/FunASR/en/
-installation/installation.html) ## Deployment Service FunASR supports pre-
-trained or further fine-tuned models for deployment as a service. The CPU
-version of the Chinese offline file conversion service has been released,
-details can be found in [docs](funasr/runtime/docs/SDK_tutorial.md). More
-detailed information about service deployment can be found in the [deployment
-roadmap](funasr/runtime/readme_cn.md).  ## Quick Start FunASR supports
-inference and fine-tuning of models trained on industrial datasets of tens of
-thousands of hours. For more details, please refer to ([modelscope_egs](https:/
-/alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html)). It also supports training and fine-tuning of models on
-academic standard datasets. For more details, please refer to([egs](https://
-alibaba-damo-academy.github.io/FunASR/en/academic_recipe/asr_recipe.html)). The
-models include speech recognition (ASR), speech activity detection (VAD),
-punctuation recovery, language model, speaker verification, speaker separation,
-and multi-party conversation speech recognition. For a detailed list of models,
-please refer to the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/
-blob/main/docs/model_zoo/modelscope_models.md):  ## Community Communication If
-you encounter problems in use, you can directly raise Issues on the github
-page. You can also scan the following DingTalk group or WeChat group QR code to
-join the community group for communication and discussion. |DingTalk group |
-WeChat group | |:---:|:-----------------------------------------------------:
-| |
+document](funasr/runtime/readme_cn.md).  ## What's new: - 2023/08/07: The real-
+time transcription service (CPU) of Mandarin has been released. For more
+details, please refer to ([Deployment documentation](funasr/runtime/docs/
+SDK_tutorial_online.md)). - 2023/07/17: BAT is released, which is a low-latency
+and low-memory-consumption RNN-T model. For more details, please refer to (
+[BAT](egs/aishell/bat)). - 2023/07/03: The offline file transcription service
+(CPU) of Mandarin has been released. For more details, please refer to (
+[Deployment documentation](funasr/runtime/docs/SDK_tutorial.md)). - 2023/06/26:
+ASRU2023 Multi-Channel Multi-Party Meeting Transcription Challenge 2.0
+completed the competition and announced the results. For more details, please
+refer to ([M2MeT2.0](https://alibaba-damo-academy.github.io/FunASR/m2met2/
+index.html)).  ## Installation Please ref to [installation docs](https://
+alibaba-damo-academy.github.io/FunASR/en/installation/installation.html) ##
+Deployment Service FunASR supports pre-trained or further fine-tuned models for
+deployment as a service. The CPU version of the Chinese offline file conversion
+service has been released, details can be found in [docs](funasr/runtime/docs/
+SDK_tutorial.md). More detailed information about service deployment can be
+found in the [deployment roadmap](funasr/runtime/readme_cn.md).  ## Quick Start
+Quick start for new usersï¼[tutorial](https://alibaba-damo-academy.github.io/
+FunASR/en/funasr/quick_start_zh.html)ï¼ FunASR supports inference and fine-
+tuning of models trained on industrial datasets of tens of thousands of hours.
+For more details, please refer to ([modelscope_egs](https://alibaba-damo-
+academy.github.io/FunASR/en/modelscope_pipeline/quick_start.html)). It also
+supports training and fine-tuning of models on academic standard datasets. For
+more details, please refer to([egs](https://alibaba-damo-academy.github.io/
+FunASR/en/academic_recipe/asr_recipe.html)). The models include speech
+recognition (ASR), speech activity detection (VAD), punctuation recovery,
+language model, speaker verification, speaker separation, and multi-party
+conversation speech recognition. For a detailed list of models, please refer to
+the [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+model_zoo/modelscope_models.md):  ## Community Communication If you encounter
+problems in use, you can directly raise Issues on the github page. You can also
+scan the following DingTalk group or WeChat group QR code to join the community
+group for communication and discussion. |DingTalk group | WeChat group | |:---:
+|:-----------------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
+| [docs/images/XVERSE.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:| The contributors can be found in [contributors list]((./Acknowledge)) ##
-License This project is licensed under the [The MIT License](https://
-opensource.org/licenses/MIT). FunASR also contains various third-party
-components and some code modified from other repos under other open source
-licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
-Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{An2023bat,
-author={Keyu An and Xian Shi and Shiliang Zhang}, title={BAT: Boundary aware
-transducer for memory-efficient and low-latency ASR}, year={2023}, booktitle=
-{INTERSPEECH}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
+--:|:------------------------------------------------------:| The contributors
+can be found in [contributors list]((./Acknowledge)) ## License This project is
+licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. The use of pretraining model is
+subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{An2023bat, author={Keyu An and Xian Shi and Shiliang Zhang},
+title={BAT: Boundary aware transducer for memory-efficient and low-latency
+ASR}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings{wang2023told,
+author={Jiaming Wang and Zhihao Du and Shiliang Zhang}, title={{TOLD:} {A}
+Novel Two-Stage Overlap-Aware Framework for Speaker Diarization}, year={2023},
+booktitle={ICASSP}, } @inproceedings{gao22b_interspeech, author={Zhifu Gao and
 ShiLiang Zhang and Ian McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and
 Accurate Parallel Transformer for Non-autoregressive End-to-End Speech
 Recognition}}, year=2022, booktitle={Proc. Interspeech 2022}, pages={2063--
 2067}, doi={10.21437/Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.7.1/funasr.egg-info/SOURCES.txt` & `funasr-0.7.2/funasr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,17 @@
 funasr/models/predictor/__init__.py
 funasr/models/predictor/cif.py
 funasr/models/preencoder/__init__.py
 funasr/models/preencoder/abs_preencoder.py
 funasr/models/preencoder/linear.py
 funasr/models/preencoder/sinc.py
 funasr/models/specaug/__init__.py
+funasr/models/specaug/abs_profileaug.py
 funasr/models/specaug/abs_specaug.py
+funasr/models/specaug/profileaug.py
 funasr/models/specaug/specaug.py
 funasr/modules/__init__.py
 funasr/modules/add_sos_eos.py
 funasr/modules/attention.py
 funasr/modules/cgmlp.py
 funasr/modules/dynamic_conv.py
 funasr/modules/dynamic_conv2d.py
@@ -245,17 +247,20 @@
 funasr/modules/data2vec/ema_module.py
 funasr/modules/data2vec/grad_multiply.py
 funasr/modules/data2vec/multihead_attention.py
 funasr/modules/data2vec/quant_noise.py
 funasr/modules/data2vec/utils.py
 funasr/modules/data2vec/wav2vec2.py
 funasr/modules/eend_ola/__init__.py
+funasr/modules/eend_ola/eend_ola_dataloader.py
 funasr/modules/eend_ola/encoder.py
 funasr/modules/eend_ola/encoder_decoder_attractor.py
 funasr/modules/eend_ola/utils/__init__.py
+funasr/modules/eend_ola/utils/feature.py
+funasr/modules/eend_ola/utils/kaldi_data.py
 funasr/modules/eend_ola/utils/losses.py
 funasr/modules/eend_ola/utils/power.py
 funasr/modules/eend_ola/utils/report.py
 funasr/modules/frontends/__init__.py
 funasr/modules/frontends/beamformer.py
 funasr/modules/frontends/dnn_beamformer.py
 funasr/modules/frontends/dnn_wpe.py
@@ -293,21 +298,23 @@
 funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
 funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
 funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
 funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
 funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
 funasr/runtime/python/onnxruntime/__init__.py
 funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+funasr/runtime/python/onnxruntime/demo_paraformer_online.py
 funasr/runtime/python/onnxruntime/demo_punc_offline.py
 funasr/runtime/python/onnxruntime/demo_punc_online.py
 funasr/runtime/python/onnxruntime/demo_vad_offline.py
 funasr/runtime/python/onnxruntime/demo_vad_online.py
 funasr/runtime/python/onnxruntime/setup.py
 funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
 funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_online_bin.py
 funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
 funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
@@ -368,14 +375,15 @@
 funasr/utils/cli_utils.py
 funasr/utils/compute_eer.py
 funasr/utils/compute_min_dcf.py
 funasr/utils/compute_wer.py
 funasr/utils/config_argparse.py
 funasr/utils/get_default_kwargs.py
 funasr/utils/griffin_lim.py
+funasr/utils/hinter.py
 funasr/utils/job_runner.py
 funasr/utils/kwargs2args.py
 funasr/utils/misc.py
 funasr/utils/modelscope_param.py
 funasr/utils/modelscope_utils.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
```

### Comparing `funasr-0.7.1/funasr.egg-info/requires.txt` & `funasr-0.7.2/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/setup.py` & `funasr-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_asr_inference_pipeline.py` & `funasr-0.7.2/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.7.2/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_lm_pipeline.py` & `funasr-0.7.2/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_punctuation_pipeline.py` & `funasr-0.7.2/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_sv_inference_pipeline.py` & `funasr-0.7.2/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_tp_pipeline.py` & `funasr-0.7.2/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.1/tests/test_vad_inference_pipeline.py` & `funasr-0.7.2/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

