# Comparing `tmp/ppacls-0.3.3-py3-none-any.whl.zip` & `tmp/ppacls-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,30 @@
-Zip file size: 51507 bytes, number of entries: 36
--rw-rw-rw-  2.0 fat      131 b- defN 23-Mar-21 11:35 ppacls/__init__.py
--rw-rw-rw-  2.0 fat     8528 b- defN 23-Mar-21 13:02 ppacls/predict.py
--rw-rw-rw-  2.0 fat    23680 b- defN 23-Mar-21 13:02 ppacls/trainer.py
+Zip file size: 48784 bytes, number of entries: 28
+-rw-rw-rw-  2.0 fat      154 b- defN 23-Aug-08 12:36 ppacls/__init__.py
+-rw-rw-rw-  2.0 fat     8971 b- defN 23-Aug-07 14:51 ppacls/predict.py
+-rw-rw-rw-  2.0 fat    25444 b- defN 23-Aug-08 12:30 ppacls/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-04 14:44 ppacls/data_utils/__init__.py
--rw-rw-rw-  2.0 fat    22814 b- defN 23-Mar-22 11:01 ppacls/data_utils/audio.py
--rw-rw-rw-  2.0 fat     2307 b- defN 23-Mar-01 04:34 ppacls/data_utils/featurizer.py
--rw-rw-rw-  2.0 fat     2813 b- defN 23-Jan-30 12:36 ppacls/data_utils/reader.py
--rw-rw-rw-  2.0 fat     4337 b- defN 23-Mar-22 11:00 ppacls/data_utils/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-04 14:44 ppacls/data_utils/augmentor/__init__.py
--rw-rw-rw-  2.0 fat     5105 b- defN 23-Feb-20 10:10 ppacls/data_utils/augmentor/augmentation.py
--rw-rw-rw-  2.0 fat      965 b- defN 22-Nov-04 14:44 ppacls/data_utils/augmentor/base.py
--rw-rw-rw-  2.0 fat     2026 b- defN 22-Nov-05 14:37 ppacls/data_utils/augmentor/noise_perturb.py
--rw-rw-rw-  2.0 fat      979 b- defN 22-Nov-05 14:37 ppacls/data_utils/augmentor/resample.py
--rw-rw-rw-  2.0 fat     1009 b- defN 22-Nov-05 14:37 ppacls/data_utils/augmentor/shift_perturb.py
--rw-rw-rw-  2.0 fat     5015 b- defN 22-Nov-04 14:44 ppacls/data_utils/augmentor/spec_augment.py
--rw-rw-rw-  2.0 fat     1138 b- defN 22-Nov-04 14:44 ppacls/data_utils/augmentor/spec_sub.py
--rw-rw-rw-  2.0 fat     1980 b- defN 22-Nov-05 14:37 ppacls/data_utils/augmentor/speed_perturb.py
--rw-rw-rw-  2.0 fat     1140 b- defN 22-Nov-05 14:37 ppacls/data_utils/augmentor/volume_perturb.py
+-rw-rw-rw-  2.0 fat    22288 b- defN 23-Aug-06 15:46 ppacls/data_utils/audio.py
+-rw-rw-rw-  2.0 fat      909 b- defN 23-Feb-15 13:35 ppacls/data_utils/collate_fn.py
+-rw-rw-rw-  2.0 fat     3771 b- defN 23-Aug-07 14:51 ppacls/data_utils/featurizer.py
+-rw-rw-rw-  2.0 fat     5517 b- defN 23-Aug-06 15:48 ppacls/data_utils/reader.py
+-rw-rw-rw-  2.0 fat     1581 b- defN 23-Aug-07 14:51 ppacls/data_utils/spec_aug.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-Mar-28 11:56 ppacls/data_utils/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-05 11:08 ppacls/models/__init__.py
--rw-rw-rw-  2.0 fat    11101 b- defN 23-Mar-21 11:44 ppacls/models/ecapa_tdnn.py
--rw-rw-rw-  2.0 fat     9884 b- defN 23-Mar-21 11:38 ppacls/models/panns.py
+-rw-rw-rw-  2.0 fat    11191 b- defN 23-Aug-07 14:51 ppacls/models/ecapa_tdnn.py
+-rw-rw-rw-  2.0 fat     9863 b- defN 23-Aug-07 14:51 ppacls/models/panns.py
 -rw-rw-rw-  2.0 fat     4539 b- defN 23-Mar-21 11:44 ppacls/models/pooling.py
--rw-rw-rw-  2.0 fat     6841 b- defN 23-Mar-21 11:47 ppacls/models/res2net.py
--rw-rw-rw-  2.0 fat     6713 b- defN 23-Mar-21 11:47 ppacls/models/resnet_se.py
--rw-rw-rw-  2.0 fat     3571 b- defN 23-Mar-21 11:47 ppacls/models/tdnn.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-Aug-07 14:51 ppacls/models/res2net.py
+-rw-rw-rw-  2.0 fat     6699 b- defN 23-Aug-07 14:51 ppacls/models/resnet_se.py
+-rw-rw-rw-  2.0 fat     3557 b- defN 23-Aug-07 14:51 ppacls/models/tdnn.py
 -rw-rw-rw-  2.0 fat     5049 b- defN 23-Mar-18 10:41 ppacls/models/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-04 14:44 ppacls/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2839 b- defN 22-Nov-04 14:44 ppacls/utils/logger.py
--rw-rw-rw-  2.0 fat     1028 b- defN 22-Nov-08 10:02 ppacls/utils/lr.py
--rw-rw-rw-  2.0 fat     1594 b- defN 23-Mar-21 13:10 ppacls/utils/record.py
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Mar-23 11:45 ppacls/utils/record.py
+-rw-rw-rw-  2.0 fat     3399 b- defN 23-Aug-05 12:19 ppacls/utils/scheduler.py
 -rw-rw-rw-  2.0 fat     3365 b- defN 23-Feb-20 12:50 ppacls/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Mar-22 11:18 ppacls-0.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6462 b- defN 23-Mar-22 11:18 ppacls-0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-22 11:18 ppacls-0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-22 11:18 ppacls-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3040 b- defN 23-Mar-22 11:18 ppacls-0.3.3.dist-info/RECORD
-36 files, 161650 bytes uncompressed, 46633 bytes compressed:  71.2%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-08 14:08 ppacls-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    18452 b- defN 23-Aug-08 14:08 ppacls-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-08 14:08 ppacls-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-08 14:08 ppacls-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2241 b- defN 23-Aug-08 14:08 ppacls-0.4.0.dist-info/RECORD
+28 files, 164018 bytes uncompressed, 45214 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -9,51 +9,27 @@
 
 Filename: ppacls/data_utils/__init__.py
 Comment: 
 
 Filename: ppacls/data_utils/audio.py
 Comment: 
 
-Filename: ppacls/data_utils/featurizer.py
-Comment: 
-
-Filename: ppacls/data_utils/reader.py
-Comment: 
-
-Filename: ppacls/data_utils/utils.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/__init__.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/augmentation.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/base.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/noise_perturb.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/resample.py
-Comment: 
-
-Filename: ppacls/data_utils/augmentor/shift_perturb.py
+Filename: ppacls/data_utils/collate_fn.py
 Comment: 
 
-Filename: ppacls/data_utils/augmentor/spec_augment.py
+Filename: ppacls/data_utils/featurizer.py
 Comment: 
 
-Filename: ppacls/data_utils/augmentor/spec_sub.py
+Filename: ppacls/data_utils/reader.py
 Comment: 
 
-Filename: ppacls/data_utils/augmentor/speed_perturb.py
+Filename: ppacls/data_utils/spec_aug.py
 Comment: 
 
-Filename: ppacls/data_utils/augmentor/volume_perturb.py
+Filename: ppacls/data_utils/utils.py
 Comment: 
 
 Filename: ppacls/models/__init__.py
 Comment: 
 
 Filename: ppacls/models/ecapa_tdnn.py
 Comment: 
@@ -78,32 +54,32 @@
 
 Filename: ppacls/utils/__init__.py
 Comment: 
 
 Filename: ppacls/utils/logger.py
 Comment: 
 
-Filename: ppacls/utils/lr.py
+Filename: ppacls/utils/record.py
 Comment: 
 
-Filename: ppacls/utils/record.py
+Filename: ppacls/utils/scheduler.py
 Comment: 
 
 Filename: ppacls/utils/utils.py
 Comment: 
 
-Filename: ppacls-0.3.3.dist-info/LICENSE
+Filename: ppacls-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: ppacls-0.3.3.dist-info/METADATA
+Filename: ppacls-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: ppacls-0.3.3.dist-info/WHEEL
+Filename: ppacls-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: ppacls-0.3.3.dist-info/top_level.txt
+Filename: ppacls-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ppacls-0.3.3.dist-info/RECORD
+Filename: ppacls-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ppacls/__init__.py

```diff
@@ -1,2 +1,3 @@
+__version__ = "0.4.0"
 # 项目支持的模型
 SUPPORT_MODEL = ['EcapaTdnn', 'PANNS_CNN6', 'PANNS_CNN10', 'PANNS_CNN14', 'Res2Net', 'ResNetSE', 'TDNN']
```

## ppacls/predict.py

```diff
@@ -1,8 +1,9 @@
 import os
+from io import BufferedReader
 
 import numpy as np
 import paddle
 import yaml
 
 from ppacls import SUPPORT_MODEL
 from ppacls.data_utils.audio import AudioSegment
@@ -17,15 +18,15 @@
 
 logger = setup_logger(__name__)
 
 
 class PPAClsPredictor:
     def __init__(self,
                  configs,
-                 model_path='models/EcapaTdnn_MelSpectrogram/best_model/',
+                 model_path='models/EcapaTdnn_Fbank/best_model/',
                  use_gpu=True):
         """
         声音分类预测工具
         :param configs: 配置参数
         :param model_path: 导出的预测模型文件夹路径
         :param use_gpu: 是否使用GPU预测
         """
@@ -38,128 +39,136 @@
         # 读取配置文件
         if isinstance(configs, str):
             with open(configs, 'r', encoding='utf-8') as f:
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
-        self.audio_featurizer = AudioFeaturizer(feature_conf=self.configs.feature_conf, **self.configs.preprocess_conf)
+        self._audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
         # 创建模型
         if not os.path.exists(model_path):
             raise Exception("模型文件不存在，请检查{}是否存在！".format(model_path))
         # 获取模型
         if self.configs.use_model == 'EcapaTdnn':
-            self.predictor = EcapaTdnn(input_size=self.audio_featurizer.feature_dim,
-                                       num_class=self.configs.dataset_conf.num_class,
-                                       **self.configs.model_conf)
+            self.predictor = EcapaTdnn(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN6':
-            self.predictor = PANNS_CNN6(input_size=self.audio_featurizer.feature_dim,
-                                        num_class=self.configs.dataset_conf.num_class,
-                                        **self.configs.model_conf)
+            self.predictor = PANNS_CNN6(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN10':
-            self.predictor = PANNS_CNN10(input_size=self.audio_featurizer.feature_dim,
-                                         num_class=self.configs.dataset_conf.num_class,
-                                         **self.configs.model_conf)
+            self.predictor = PANNS_CNN10(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN14':
-            self.predictor = PANNS_CNN14(input_size=self.audio_featurizer.feature_dim,
-                                         num_class=self.configs.dataset_conf.num_class,
-                                         **self.configs.model_conf)
+            self.predictor = PANNS_CNN14(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'Res2Net':
-            self.predictor = Res2Net(input_size=self.audio_featurizer.feature_dim,
-                                     num_class=self.configs.dataset_conf.num_class,
-                                     **self.configs.model_conf)
+            self.predictor = Res2Net(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'ResNetSE':
-            self.predictor = ResNetSE(input_size=self.audio_featurizer.feature_dim,
-                                      num_class=self.configs.dataset_conf.num_class,
-                                      **self.configs.model_conf)
+            self.predictor = ResNetSE(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         elif self.configs.use_model == 'TDNN':
-            self.predictor = TDNN(input_size=self.audio_featurizer.feature_dim,
-                                  num_class=self.configs.dataset_conf.num_class,
-                                  **self.configs.model_conf)
+            self.predictor = TDNN(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         else:
             raise Exception(f'{self.configs.use_model} 模型不存在！')
         # 加载模型
         if os.path.isdir(model_path):
             model_path = os.path.join(model_path, 'model.pdparams')
         assert os.path.exists(model_path), f"{model_path} 模型不存在！"
         self.predictor.set_state_dict(paddle.load(model_path))
         print(f"成功加载模型参数：{model_path}")
         self.predictor.eval()
         # 获取分类标签
         with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
             lines = f.readlines()
         self.class_labels = [l.replace('\n', '') for l in lines]
-        # 获取特征器
-        self.audio_featurizer = AudioFeaturizer(feature_conf=self.configs.feature_conf, **self.configs.preprocess_conf)
 
-    # 预测一个音频的特征
-    def predict(self,
-                audio_data,
-                sample_rate=16000):
-        """预测一个音频
-
-        :param audio_data: 需要识别的数据，支持文件路径，字节，numpy
+    def _load_audio(self, audio_data, sample_rate=16000):
+        """加载音频
+        :param audio_data: 需要识别的数据，支持文件路径，文件对象，字节，numpy。如果是字节的话，必须是完整的字节文件
         :param sample_rate: 如果传入的事numpy数据，需要指定采样率
-        :return: 结果标签和对应的得分
+        :return: 识别的文本结果和解码的得分数
         """
         # 加载音频文件，并进行预处理
         if isinstance(audio_data, str):
-            input_data = AudioSegment.from_file(audio_data)
+            audio_segment = AudioSegment.from_file(audio_data)
+        elif isinstance(audio_data, BufferedReader):
+            audio_segment = AudioSegment.from_file(audio_data)
         elif isinstance(audio_data, np.ndarray):
-            input_data = AudioSegment.from_ndarray(audio_data, sample_rate)
+            audio_segment = AudioSegment.from_ndarray(audio_data, sample_rate)
         elif isinstance(audio_data, bytes):
-            input_data = AudioSegment.from_wave_bytes(audio_data)
+            audio_segment = AudioSegment.from_bytes(audio_data)
         else:
             raise Exception(f'不支持该数据类型，当前数据类型为：{type(audio_data)}')
         # 重采样
-        if input_data.sample_rate != self.configs.dataset_conf.sample_rate:
-            input_data.resample(self.configs.dataset_conf.sample_rate)
+        if audio_segment.sample_rate != self.configs.dataset_conf.sample_rate:
+            audio_segment.resample(self.configs.dataset_conf.sample_rate)
         # decibel normalization
         if self.configs.dataset_conf.use_dB_normalization:
-            input_data.normalize(target_db=self.configs.dataset_conf.target_dB)
-        if 'panns' in self.configs.use_model:
-            # 对小于训练长度的复制补充
-            num_chunk_samples = int(self.configs.dataset_conf.chunk_duration * input_data.sample_rate)
-            if input_data.num_samples < num_chunk_samples:
-                shortage = num_chunk_samples - input_data.num_samples
-                input_data.pad_silence(duration=float(shortage / input_data.sample_rate * 1.1), sides='end')
-            # 裁剪需要的数据
-            input_data.crop(duration=self.configs.dataset_conf.chunk_duration)
+            audio_segment.normalize(target_db=self.configs.dataset_conf.target_dB)
+        return audio_segment
+
+    # 预测一个音频的特征
+    def predict(self,
+                audio_data,
+                sample_rate=16000):
+        """预测一个音频
+
+        :param audio_data: 需要识别的数据，支持文件路径，文件对象，字节，numpy。如果是字节的话，必须是完整并带格式的字节文件
+        :param sample_rate: 如果传入的事numpy数据，需要指定采样率
+        :return: 结果标签和对应的得分
+        """
+        # 加载音频文件，并进行预处理
+        input_data = self._load_audio(audio_data=audio_data, sample_rate=sample_rate)
+        assert input_data.duration >= self.configs.dataset_conf.min_duration, \
+            f'音频太短，最小应该为{self.configs.dataset_conf.min_duration}s，当前音频为{input_data.duration}s'
         input_data = paddle.to_tensor(input_data.samples, dtype=paddle.float32).unsqueeze(0)
-        audio_feature = self.audio_featurizer(input_data)
-        data_length = paddle.to_tensor([audio_feature.shape[1]], dtype=paddle.int64)
+        input_len_ratio = paddle.to_tensor([1], dtype=paddle.float32)
+        audio_feature, _ = self._audio_featurizer(input_data, input_len_ratio)
         # 执行预测
-        output = self.predictor(audio_feature, data_length)
+        if self.configs.use_model == 'EcapaTdnn':
+            output = self.predictor([audio_feature, input_len_ratio])
+        else:
+            output = self.predictor(audio_feature)
         result = paddle.nn.functional.softmax(output).numpy()[0]
         # 最大概率的label
         lab = np.argsort(result)[-1]
         score = result[lab]
         return self.class_labels[lab], round(float(score), 5)
 
-    def predict_batch(self, audios_data):
-        """预测一批音频
+    def predict_batch(self, audios_data, sample_rate=16000):
+        """预测一批音频的特征
 
-        :param audios_data: 经过预处理的一批数据
+        :param audios_data: 需要预测音频的路径
+        :param sample_rate: 如果传入的事numpy数据，需要指定采样率
         :return: 结果标签和对应的得分
         """
-        data_length = paddle.to_tensor([a.shape[0] for a in audios_data], dtype=paddle.int64)
+        audios_data1, data_length = [], []
+        for audio_data in audios_data:
+            # 加载音频文件，并进行预处理
+            input_data = self._load_audio(audio_data=audio_data, sample_rate=sample_rate)
+            audios_data1.append(input_data.samples)
+            data_length.append(input_data.num_samples)
         # 找出音频长度最长的
-        batch = sorted(audios_data, key=lambda a: a.shape[0], reverse=True)
-        freq_size = batch[0].shape[1]
+        batch = sorted(audios_data1, key=lambda a: a.shape[0], reverse=True)
         max_audio_length = batch[0].shape[0]
         batch_size = len(batch)
         # 以最大的长度创建0张量
-        inputs = np.zeros((batch_size, max_audio_length, freq_size), dtype=np.float32)
-        for i, sample in enumerate(batch):
-            seq_length = sample.shape[0]
+        inputs = np.zeros((batch_size, max_audio_length), dtype='float32')
+        input_lens_ratio = []
+        for x in range(batch_size):
+            tensor = audios_data1[x]
+            seq_length = tensor.shape[0]
             # 将数据插入都0张量中，实现了padding
-            inputs[i, :seq_length, :] = sample[:, :]
-        audios_data = paddle.to_tensor(inputs, dtype=paddle.float32)
+            inputs[x, :seq_length] = tensor[:]
+            input_lens_ratio.append(seq_length / max_audio_length)
+        input_lens_ratio = paddle.to_tensor(input_lens_ratio, dtype=paddle.float32)
+        inputs = paddle.to_tensor(inputs, dtype=paddle.float32)
+        audio_feature = self._audio_featurizer(inputs)
+        data_length = paddle.to_tensor([audio_feature.shape[1]], dtype=paddle.int64)
         # 执行预测
-        output = self.predictor(audios_data, data_length)
+        if self.configs.use_model == 'EcapaTdnn':
+            output = self.predictor([audio_feature, data_length])
+        else:
+            output = self.predictor(audio_feature)
         results = paddle.nn.functional.softmax(output).numpy()
         labels, scores = [], []
         for result in results:
             lab = np.argsort(result)[-1]
             score = result[lab]
             labels.append(self.class_labels[lab])
             scores.append(round(float(score), 5))
```

## ppacls/trainer.py

```diff
@@ -1,33 +1,37 @@
-import io
 import json
 import os
+import platform
 import shutil
 import time
 from datetime import timedelta
 
 import paddle
 import yaml
+from paddle import summary
 from paddle.distributed import fleet
-from paddle.io import DataLoader
+from paddle.io import DataLoader, DistributedBatchSampler
 from paddle.metric import accuracy
+from paddle.optimizer.lr import CosineAnnealingDecay
 from sklearn.metrics import confusion_matrix
 from tqdm import tqdm
 from visualdl import LogWriter
 
-from ppacls import SUPPORT_MODEL
+from ppacls import SUPPORT_MODEL, __version__
+from ppacls.data_utils.collate_fn import collate_fn
 from ppacls.data_utils.featurizer import AudioFeaturizer
 from ppacls.data_utils.reader import CustomDataset
+from ppacls.data_utils.spec_aug import SpecAug
 from ppacls.models.ecapa_tdnn import EcapaTdnn
 from ppacls.models.panns import PANNS_CNN6, PANNS_CNN10, PANNS_CNN14
 from ppacls.models.res2net import Res2Net
 from ppacls.models.resnet_se import ResNetSE
 from ppacls.models.tdnn import TDNN
 from ppacls.utils.logger import setup_logger
-from ppacls.utils.lr import cosine_decay_with_warmup
+from ppacls.utils.scheduler import cosine_decay_with_warmup
 from ppacls.utils.utils import dict_to_object, plot_confusion_matrix, print_arguments
 
 logger = setup_logger(__name__)
 
 
 class PPAClsTrainer(object):
     def __init__(self, configs, use_gpu=True):
@@ -48,99 +52,102 @@
             with open(configs, 'r', encoding='utf-8') as f:
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         self.model = None
         self.test_loader = None
+        self.amp_scaler = None
         # 获取分类标签
         with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
             lines = f.readlines()
         self.class_labels = [l.replace('\n', '') for l in lines]
         # 获取特征器
-        self.audio_featurizer = AudioFeaturizer(feature_conf=self.configs.feature_conf, **self.configs.preprocess_conf)
+        self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
+        self.spec_aug = SpecAug(**self.configs.dataset_conf.get('spec_aug_args', {}))
+        if platform.system().lower() == 'windows':
+            self.configs.dataset_conf.dataLoader.num_workers = 0
+            logger.warning('Windows系统不支持多线程读取数据，已自动关闭！')
 
-    def __setup_dataloader(self, augment_conf_path=None, is_train=False):
-        # 获取训练数据
-        if augment_conf_path is not None and os.path.exists(augment_conf_path) and is_train:
-            augmentation_config = io.open(augment_conf_path, mode='r', encoding='utf8').read()
-        else:
-            if augment_conf_path is not None and not os.path.exists(augment_conf_path):
-                logger.info('数据增强配置文件{}不存在'.format(augment_conf_path))
-            augmentation_config = '{}'
+    def __setup_dataloader(self, is_train=False):
         if is_train:
             self.train_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.train_list,
                                                do_vad=self.configs.dataset_conf.do_vad,
-                                               chunk_duration=self.configs.dataset_conf.chunk_duration,
+                                               max_duration=self.configs.dataset_conf.max_duration,
                                                min_duration=self.configs.dataset_conf.min_duration,
-                                               augmentation_config=augmentation_config,
+                                               aug_conf=self.configs.dataset_conf.aug_conf,
                                                sample_rate=self.configs.dataset_conf.sample_rate,
                                                use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
                                                target_dB=self.configs.dataset_conf.target_dB,
                                                mode='train')
             # 设置支持多卡训练
-            self.train_batch_sampler = paddle.io.DistributedBatchSampler(dataset=self.train_dataset,
-                                                                         batch_size=self.configs.dataset_conf.batch_size,
-                                                                         shuffle=True)
+            train_sampler = None
+            if paddle.distributed.get_world_size() > 1:
+                # 设置支持多卡训练
+                train_sampler = DistributedBatchSampler(dataset=self.train_dataset,
+                                                        batch_size=self.configs.dataset_conf.dataLoader.batch_size,
+                                                        shuffle=True)
             self.train_loader = DataLoader(dataset=self.train_dataset,
-                                           batch_sampler=self.train_batch_sampler,
-                                           num_workers=self.configs.dataset_conf.num_workers)
+                                           collate_fn=collate_fn,
+                                           shuffle=(train_sampler is None),
+                                           batch_sampler=train_sampler,
+                                           **self.configs.dataset_conf.dataLoader)
         # 获取测试数据
         self.test_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.test_list,
                                           do_vad=self.configs.dataset_conf.do_vad,
-                                          chunk_duration=self.configs.dataset_conf.chunk_duration,
+                                          max_duration=self.configs.dataset_conf.eval_conf.max_duration,
                                           min_duration=self.configs.dataset_conf.min_duration,
                                           sample_rate=self.configs.dataset_conf.sample_rate,
                                           use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
                                           target_dB=self.configs.dataset_conf.target_dB,
                                           mode='eval')
         self.test_loader = DataLoader(dataset=self.test_dataset,
-                                      batch_size=self.configs.dataset_conf.batch_size,
-                                      num_workers=self.configs.dataset_conf.num_workers)
+                                      collate_fn=collate_fn,
+                                      batch_size=self.configs.dataset_conf.eval_conf.batch_size,
+                                      num_workers=self.configs.dataset_conf.dataLoader.num_workers)
 
     def __setup_model(self, input_size, is_train=False):
         # 获取模型
         if self.configs.use_model == 'EcapaTdnn':
-            self.model = EcapaTdnn(input_size=input_size,
-                                   num_class=self.configs.dataset_conf.num_class,
-                                   **self.configs.model_conf)
+            self.model = EcapaTdnn(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN6':
-            self.model = PANNS_CNN6(input_size=input_size,
-                                    num_class=self.configs.dataset_conf.num_class,
-                                    **self.configs.model_conf)
+            self.model = PANNS_CNN6(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN10':
-            self.model = PANNS_CNN10(input_size=input_size,
-                                     num_class=self.configs.dataset_conf.num_class,
-                                     **self.configs.model_conf)
+            self.model = PANNS_CNN10(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'PANNS_CNN14':
-            self.model = PANNS_CNN14(input_size=input_size,
-                                     num_class=self.configs.dataset_conf.num_class,
-                                     **self.configs.model_conf)
+            self.model = PANNS_CNN14(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'Res2Net':
-            self.model = Res2Net(input_size=input_size,
-                                 num_class=self.configs.dataset_conf.num_class,
-                                 **self.configs.model_conf)
+            self.model = Res2Net(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'ResNetSE':
-            self.model = ResNetSE(input_size=input_size,
-                                  num_class=self.configs.dataset_conf.num_class,
-                                  **self.configs.model_conf)
+            self.model = ResNetSE(input_size=input_size, **self.configs.model_conf)
         elif self.configs.use_model == 'TDNN':
-            self.model = TDNN(input_size=input_size,
-                              num_class=self.configs.dataset_conf.num_class,
-                              **self.configs.model_conf)
+            self.model = TDNN(input_size=input_size, **self.configs.model_conf)
         else:
             raise Exception(f'{self.configs.use_model} 模型不存在！')
+        summary(self.model, (1, 98, self.audio_featurizer.feature_dim))
         # print(self.model)
         # 获取损失函数
         self.loss = paddle.nn.CrossEntropyLoss()
         if is_train:
-            # 学习率衰减
-            self.scheduler = cosine_decay_with_warmup(learning_rate=float(self.configs.optimizer_conf.learning_rate),
-                                                      max_epochs=int(self.configs.train_conf.max_epoch * 1.2),
-                                                      step_per_epoch=len(self.train_loader))
+            if self.configs.train_conf.enable_amp:
+                # 自动混合精度训练，逻辑2，定义GradScaler
+                self.amp_scaler = paddle.amp.GradScaler(init_loss_scaling=1024)
+            # 学习率衰减函数
+            scheduler_args = self.configs.optimizer_conf.get('scheduler_args', {}) \
+                if self.configs.optimizer_conf.get('scheduler_args', {}) is not None else {}
+            if self.configs.optimizer_conf.scheduler == 'CosineAnnealingLR':
+                max_step = int(self.configs.train_conf.max_epoch * 1.2) * len(self.train_loader)
+                self.scheduler = CosineAnnealingDecay(T_max=max_step,
+                                                      **scheduler_args)
+            elif self.configs.optimizer_conf.scheduler == 'WarmupCosineSchedulerLR':
+                self.scheduler = cosine_decay_with_warmup(step_per_epoch=len(self.train_loader),
+                                                          **scheduler_args)
+            else:
+                raise Exception(f'不支持学习率衰减函数：{self.configs.optimizer_conf.scheduler}')
             # 获取优化方法
             optimizer = self.configs.optimizer_conf.optimizer
             if optimizer == 'Adam':
                 self.optimizer = paddle.optimizer.Adam(parameters=self.model.parameters(),
                                                        learning_rate=self.scheduler,
                                                        weight_decay=float(self.configs.optimizer_conf.weight_decay))
             elif optimizer == 'AdamW':
@@ -151,15 +158,14 @@
                 self.optimizer = paddle.optimizer.Momentum(parameters=self.model.parameters(),
                                                            momentum=self.configs.optimizer_conf.momentum,
                                                            learning_rate=self.scheduler,
                                                            weight_decay=float(self.configs.optimizer_conf.weight_decay))
             else:
                 raise Exception(f'不支持优化方法：{optimizer}')
 
-
     def __load_pretrained(self, pretrained_model):
         # 加载预训练模型
         if pretrained_model is not None:
             if os.path.isdir(pretrained_model):
                 pretrained_model = os.path.join(pretrained_model, 'model.pdparams')
             assert os.path.exists(pretrained_model), f"{pretrained_model} 模型不存在！"
             model_dict = self.model.state_dict()
@@ -186,14 +192,17 @@
                                         and os.path.exists(os.path.join(last_model_dir, 'optimizer.pdopt'))):
             # 自动获取最新保存的模型
             if resume_model is None: resume_model = last_model_dir
             assert os.path.exists(os.path.join(resume_model, 'model.pdparams')), "模型参数文件不存在！"
             assert os.path.exists(os.path.join(resume_model, 'optimizer.pdopt')), "优化方法参数文件不存在！"
             self.model.set_state_dict(paddle.load(os.path.join(resume_model, 'model.pdparams')))
             self.optimizer.set_state_dict(paddle.load(os.path.join(resume_model, 'optimizer.pdopt')))
+            # 自动混合精度参数
+            if self.amp_scaler is not None and os.path.exists(os.path.join(resume_model, 'scaler.pdparams')):
+                self.amp_scaler.set_state_dict(paddle.load(os.path.join(resume_model, 'scaler.pdparams')))
             with open(os.path.join(resume_model, 'model.state'), 'r', encoding='utf-8') as f:
                 json_data = json.load(f)
                 last_epoch = json_data['last_epoch'] - 1
                 best_acc = json_data['accuracy']
             logger.info('成功恢复模型参数和优化方法参数：{}'.format(resume_model))
         return last_epoch, best_acc
 
@@ -207,19 +216,23 @@
             model_path = os.path.join(save_model_path,
                                       f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                       'epoch_{}'.format(epoch_id))
         os.makedirs(model_path, exist_ok=True)
         try:
             paddle.save(self.optimizer.state_dict(), os.path.join(model_path, 'optimizer.pdopt'))
             paddle.save(self.model.state_dict(), os.path.join(model_path, 'model.pdparams'))
+            # 自动混合精度参数
+            if self.amp_scaler is not None:
+                paddle.save(self.amp_scaler.state_dict(), os.path.join(model_path, 'scaler.pdparams'))
         except Exception as e:
             logger.error(f'保存模型时出现错误，错误信息：{e}')
             return
         with open(os.path.join(model_path, 'model.state'), 'w', encoding='utf-8') as f:
-            f.write('{"last_epoch": %d, "accuracy": %f}' % (epoch_id, best_acc))
+            data = {"last_epoch": epoch_id, "accuracy": best_acc, "version": __version__}
+            f.write(json.dumps(data))
         if not best_model:
             last_model_path = os.path.join(save_model_path,
                                            f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                            'last_model')
             shutil.rmtree(last_model_path, ignore_errors=True)
             shutil.copytree(model_path, last_model_path)
             # 删除旧的模型
@@ -230,35 +243,54 @@
                 shutil.rmtree(old_model_path)
         logger.info('已保存模型：{}'.format(model_path))
 
     def __train_epoch(self, epoch_id, local_rank, writer):
         train_times, accuracies, loss_sum = [], [], []
         start = time.time()
         sum_batch = len(self.train_loader) * self.configs.train_conf.max_epoch
-        for batch_id, (audio, label) in enumerate(self.train_loader()):
-            features = self.audio_featurizer(audio)
-            audio_lens = [features.shape[1] for _ in range(audio.shape[0])]
-            audio_lens = paddle.to_tensor(audio_lens, dtype=paddle.int64)
-            output = self.model(features, audio_lens)
+        for batch_id, (audio, label, input_lens_ratio) in enumerate(self.train_loader()):
+            features, _ = self.audio_featurizer(audio, input_lens_ratio)
+            # 特征增强
+            if self.configs.dataset_conf.use_spec_aug:
+                features = self.spec_aug(features)
+            # 执行模型计算，是否开启自动混合精度
+            with paddle.amp.auto_cast(enable=self.configs.train_conf.enable_amp, level='O1'):
+                if self.configs.use_model == 'EcapaTdnn':
+                    output = self.model([features, input_lens_ratio])
+                else:
+                    output = self.model(features)
             # 计算损失值
             los = self.loss(output, label)
-            los.backward()
-            self.optimizer.step()
+            # 是否开启自动混合精度
+            if self.configs.train_conf.enable_amp:
+                # loss缩放，乘以系数loss_scaling
+                scaled = self.amp_scaler.scale(los)
+                scaled.backward()
+            else:
+                los.backward()
+            # 是否开启自动混合精度
+            if self.configs.train_conf.enable_amp:
+                # 更新参数（参数梯度先除系数loss_scaling再更新参数）
+                self.amp_scaler.step(self.optimizer)
+                # 基于动态loss_scaling策略更新loss_scaling系数
+                self.amp_scaler.update()
+            else:
+                self.optimizer.step()
             self.optimizer.clear_grad()
             # 计算准确率
             label = paddle.reshape(label, shape=(-1, 1))
             acc = accuracy(input=paddle.nn.functional.softmax(output), label=label)
-            accuracies.append(acc.numpy()[0])
-            loss_sum.append(los.numpy()[0])
+            accuracies.append(float(acc))
+            loss_sum.append(float(los))
             train_times.append((time.time() - start) * 1000)
 
             # 多卡训练只使用一个进程打印
             if batch_id % self.configs.train_conf.log_interval == 0 and local_rank == 0:
                 # 计算每秒训练数据量
-                train_speed = self.configs.dataset_conf.batch_size / (sum(train_times) / len(train_times) / 1000)
+                train_speed = self.configs.dataset_conf.dataLoader.batch_size / (sum(train_times) / len(train_times) / 1000)
                 # 计算剩余时间
                 eta_sec = (sum(train_times) / len(train_times)) * (
                         sum_batch - (epoch_id - 1) * len(self.train_loader) - batch_id)
                 eta_str = str(timedelta(seconds=int(eta_sec / 1000)))
                 logger.info(f'Train epoch: [{epoch_id}/{self.configs.train_conf.max_epoch}], '
                             f'batch: [{batch_id}/{len(self.train_loader)}], '
                             f'loss: {sum(loss_sum) / len(loss_sum):.5f}, '
@@ -273,22 +305,20 @@
                 train_times = []
             self.scheduler.step()
             start = time.time()
 
     def train(self,
               save_model_path='models/',
               resume_model=None,
-              pretrained_model=None,
-              augment_conf_path='configs/augmentation.json'):
+              pretrained_model=None):
         """
         训练模型
         :param save_model_path: 模型保存的路径
         :param resume_model: 恢复训练，当为None则不使用预训练模型
         :param pretrained_model: 预训练模型的路径，当为None则不使用预训练模型
-        :param augment_conf_path: 数据增强的配置文件，为json格式
         """
         paddle.seed(1000)
         # 获取有多少张显卡训练
         nranks = paddle.distributed.get_world_size()
         local_rank = paddle.distributed.get_rank()
         writer = None
         if local_rank == 0:
@@ -297,15 +327,15 @@
 
         if nranks > 1 and self.use_gpu:
             # 初始化Fleet环境
             strategy = fleet.DistributedStrategy()
             fleet.init(is_collective=True, strategy=strategy)
 
         # 获取数据
-        self.__setup_dataloader(augment_conf_path=augment_conf_path, is_train=True)
+        self.__setup_dataloader(is_train=True)
         # 获取模型
         self.__setup_model(input_size=self.audio_featurizer.feature_dim, is_train=True)
 
         # 支持多卡训练
         if nranks > 1 and self.use_gpu:
             self.optimizer = fleet.distributed_optimizer(self.optimizer)
             self.model = fleet.distributed_model(self.model)
@@ -324,15 +354,15 @@
             epoch_id += 1
             start_epoch = time.time()
             # 训练一个epoch
             self.__train_epoch(epoch_id=epoch_id, local_rank=local_rank, writer=writer)
             # 多卡训练只使用一个进程执行评估和保存模型
             if local_rank == 0:
                 logger.info('=' * 70)
-                loss, acc = self.evaluate(resume_model=None)
+                loss, acc = self.evaluate()
                 logger.info('Test epoch: {}, time/epoch: {}, loss: {:.5f}, accuracy: {:.5f}'.format(
                     epoch_id, str(timedelta(seconds=(time.time() - start_epoch))), loss, acc))
                 logger.info('=' * 70)
                 writer.add_scalar('Test/Accuracy', acc, test_step)
                 writer.add_scalar('Test/Loss', loss, test_step)
                 test_step += 1
                 self.model.train()
@@ -340,15 +370,15 @@
                 if acc >= best_acc:
                     best_acc = acc
                     self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=acc,
                                            best_model=True)
                 # 保存模型
                 self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=loss)
 
-    def evaluate(self, resume_model='models/EcapaTdnn_MelSpectrogram/best_model/', save_matrix_path=None):
+    def evaluate(self, resume_model=None, save_matrix_path=None):
         """
         评估模型
         :param resume_model: 所使用的模型
         :param save_matrix_path: 保存混合矩阵的路径
         :return: 评估结果
         """
         if self.test_loader is None:
@@ -366,25 +396,26 @@
         if isinstance(self.model, paddle.DataParallel):
             eval_model = self.model._layers
         else:
             eval_model = self.model
 
         accuracies, losses, preds, labels = [], [], [], []
         with paddle.no_grad():
-            for batch_id, (audio, label) in enumerate(tqdm(self.test_loader())):
-                features = self.audio_featurizer(audio)
-                audio_lens = [features.shape[1] for _ in range(audio.shape[0])]
-                audio_lens = paddle.to_tensor(audio_lens, dtype=paddle.int64)
-                output = eval_model(features, audio_lens)
+            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.test_loader())):
+                features, _ = self.audio_featurizer(audio, input_lens_ratio)
+                if self.configs.use_model == 'EcapaTdnn':
+                    output = eval_model([features, input_lens_ratio])
+                else:
+                    output = eval_model(features)
                 los = self.loss(output, label)
                 # 计算准确率
                 label = paddle.reshape(label, shape=(-1, 1))
                 acc = accuracy(input=paddle.nn.functional.softmax(output), label=label)
-                accuracies.append(acc.numpy()[0])
-                losses.append(los.numpy()[0])
+                accuracies.append(float(acc))
+                losses.append(float(los))
                 # 模型预测标签
                 pred = paddle.argsort(output, descending=True)[:, 0].numpy().tolist()
                 preds.extend(pred)
                 # 真实标签
                 labels.extend(label.numpy().tolist())
         loss = float(sum(losses) / len(losses))
         acc = float(sum(accuracies) / len(accuracies))
@@ -393,15 +424,15 @@
             cm = confusion_matrix(labels, preds)
             plot_confusion_matrix(cm=cm, save_path=os.path.join(save_matrix_path, f'{int(time.time())}.png'),
                                   class_labels=self.class_labels)
 
         self.model.train()
         return loss, acc
 
-    def export(self, save_model_path='models/', resume_model='models/EcapaTdnn_MelSpectrogram/best_model/'):
+    def export(self, save_model_path='models/', resume_model='models/EcapaTdnn_Fbank/best_model/'):
         """
         导出预测模型
         :param save_model_path: 模型保存的路径
         :param resume_model: 准备转换的模型路径
         :return:
         """
         # 获取模型
```

## ppacls/data_utils/audio.py

```diff
@@ -52,15 +52,15 @@
                 "rms=%.2fdB" % (type(self), self.num_samples, self.sample_rate, self.duration, self.rms_db))
 
     @classmethod
     def from_file(cls, file):
         """从音频文件创建音频段
         
         :param file: 文件路径，或者文件对象
-        :type file: str
+        :type file: str, BufferedReader
         :return: 音频片段实例
         :rtype: AudioSegment
         """
         assert os.path.exists(file), f'文件不存在，请检查路径：{file}'
         try:
             samples, sample_rate = soundfile.read(file, dtype='float32')
         except:
@@ -101,38 +101,43 @@
         start_frame = int(start * sample_rate)
         end_frame = int(end * sample_rate)
         sndfile.seek(start_frame)
         data = sndfile.read(frames=end_frame - start_frame, dtype='float32')
         return cls(data, sample_rate)
 
     @classmethod
-    def from_bytes(cls, bytes):
+    def from_bytes(cls, data):
         """从包含音频样本的字节创建音频段
 
-        :param bytes: 包含音频样本的字节
-        :type bytes: bytes
+        :param data: 包含音频样本的字节
+        :type data: bytes
         :return: 音频部分实例
         :rtype: AudioSegment
         """
-        samples, sample_rate = soundfile.read(io.BytesIO(bytes), dtype='float32')
+        samples, sample_rate = soundfile.read(io.BytesIO(data), dtype='float32')
         return cls(samples, sample_rate)
 
     @classmethod
-    def from_wave_bytes(cls, bytes, sample_rate=16000):
-        """从包含音频样本的字节创建音频段，字节的来源是wave.open或者pyaudio.PyAudio()，
-        音频格式nchannels=1, sampwidth=2(PyAudio的是format=pyaudio.paInt16), framerate=16000
+    def from_pcm_bytes(cls, data, channels=1, samp_width=2, sample_rate=16000):
+        """从包含无格式PCM音频的字节创建音频
 
-        :param bytes: 包含音频样本的字节
-        :type bytes: bytes
+        :param data: 包含音频样本的字节
+        :type data: bytes
+        :param channels: 音频的通道数
+        :type channels: int
+        :param samp_width: 音频采样的宽度，如np.int16为2
+        :type samp_width: int
         :param sample_rate: 音频样本采样率
         :type sample_rate: int
         :return: 音频部分实例
         :rtype: AudioSegment
         """
-        samples = buf_to_float(bytes)
+        samples = buf_to_float(data, n_bytes=samp_width)
+        if channels > 1:
+            samples = samples.reshape(-1, channels)
         return cls(samples, sample_rate)
 
     @classmethod
     def from_ndarray(cls, data, sample_rate=16000):
         """从numpy.ndarray创建音频段
 
         :param data: numpy.ndarray类型的音频数据
@@ -406,61 +411,51 @@
                              "than original segment.")
         start_time = random.uniform(0.0, self.duration - subsegment_length)
         self.subsegment(start_time, start_time + subsegment_length)
 
     def add_noise(self,
                   noise,
                   snr_dB,
-                  allow_downsampling=False,
                   max_gain_db=300.0):
         """以特定的信噪比添加给定的噪声段。如果噪声段比该噪声段长，则从该噪声段中采样匹配长度的随机子段。
 
         Note that this is an in-place transformation.
 
         :param noise: Noise signal to add.
         :type noise: AudioSegment
         :param snr_dB: Signal-to-Noise Ratio, in decibels.
         :type snr_dB: float
-        :param allow_downsampling: Whether to allow the noise signal to be
-                                   downsampled to match the base signal sample
-                                   rate.
-        :type allow_downsampling: bool
         :param max_gain_db: Maximum amount of gain to apply to noise signal
                             before adding it in. This is to prevent attempting
                             to apply infinite gain to a zero signal.
         :type max_gain_db: float
         :raises ValueError: If the sample rate does not match between the two
-                            audio segments when downsampling is not allowed, or
-                            if the duration of noise segments is shorter than
-                            original audio segments.
+                            audio segments, or if the duration of noise segments
+                            is shorter than original audio segments.
         """
-        if allow_downsampling and noise.sample_rate > self.sample_rate:
-            noise.resample(self.sample_rate)
         if noise.sample_rate != self.sample_rate:
             raise ValueError("噪声采样率(%d Hz)不等于基信号采样率(%d Hz)" % (noise.sample_rate, self.sample_rate))
         if noise.duration < self.duration:
             raise ValueError("噪声信号(%f秒)必须至少与基信号(%f秒)一样长" % (noise.duration, self.duration))
         noise_gain_db = min(self.rms_db - noise.rms_db - snr_dB, max_gain_db)
         noise_new = copy.deepcopy(noise)
         noise_new.random_subsegment(self.duration)
         noise_new.gain_db(noise_gain_db)
         self.superimpose(noise_new)
 
     def vad(self, top_db=20, overlap=200):
         self._samples = vad(wav=self._samples, top_db=top_db, overlap=overlap)
 
+    # 裁剪音频
     def crop(self, duration, mode='eval'):
-        num_chunk_samples = int(duration * self.sample_rate)
-        if self.num_samples > num_chunk_samples:
+        if self.duration > duration:
             if mode == 'train':
-                start = random.randint(0, self.num_samples - num_chunk_samples - 1)
-                stop = start + num_chunk_samples
-                self._samples = self._samples[start:stop]
+                self.random_subsegment(duration)
             else:
-                self._samples = self._samples[:num_chunk_samples]
+                self.subsegment(end_sec=duration)
 
     @property
     def samples(self):
         """返回音频样本
 
         :return: Audio samples.
         :rtype: ndarray
```

## ppacls/data_utils/featurizer.py

```diff
@@ -1,62 +1,98 @@
 import paddle
 from paddle import nn
+import paddleaudio.compliance.kaldi as Kaldi
 from paddle.audio.features import LogMelSpectrogram, MelSpectrogram, Spectrogram, MFCC
 
 
 class AudioFeaturizer(nn.Layer):
     """音频特征器
 
-    :param feature_conf: 预处理方法的参数
-    :type feature_conf: dict
-    :param sample_rate: 用于训练的音频的采样率
-    :type sample_rate: int
+    :param feature_method: 所使用的预处理方法
+    :type feature_method: str
+    :param method_args: 预处理方法的参数
+    :type method_args: dict
     """
 
-    def __init__(self, feature_method='MelSpectrogram', feature_conf={}):
+    def __init__(self, feature_method='MelSpectrogram', method_args={}):
         super().__init__()
-        self._feature_conf = feature_conf
+        self._method_args = method_args
         self._feature_method = feature_method
         if feature_method == 'LogMelSpectrogram':
-            self.feat_fun = LogMelSpectrogram(**feature_conf)
+            self.feat_fun = LogMelSpectrogram(**method_args)
         elif feature_method == 'MelSpectrogram':
-            self.feat_fun = MelSpectrogram(**feature_conf)
+            self.feat_fun = MelSpectrogram(**method_args)
         elif feature_method == 'Spectrogram':
-            self.feat_fun = Spectrogram(**feature_conf)
+            self.feat_fun = Spectrogram(**method_args)
         elif feature_method == 'MFCC':
-            self.feat_fun = MFCC(**feature_conf)
+            self.feat_fun = MFCC(**method_args)
+        elif feature_method == 'Fbank':
+            self.feat_fun = KaldiFbank(**method_args)
         else:
             raise Exception(f'预处理方法 {self._feature_method} 不存在!')
 
-    def forward(self, waveforms):
+    def forward(self, waveforms, input_lens_ratio):
         """从AudioSegment中提取音频特征
 
         :param waveforms: Audio segment to extract features from.
         :type waveforms: AudioSegment
+        :param input_lens_ratio: input length ratio
+        :type input_lens_ratio: tensor
         :return: Spectrogram audio feature in 2darray.
         :rtype: ndarray
         """
         feature = self.feat_fun(waveforms)
         feature = feature.transpose([0, 2, 1])
         # 归一化
-        mean = paddle.mean(feature, 1, keepdim=True)
-        std = paddle.std(feature, 1, keepdim=True)
-        feature = (feature - mean) / (std + 1e-5)
-        return feature
+        feature = feature - feature.mean(1, keepdim=True)
+        # 对掩码比例进行扩展
+        input_lens = (input_lens_ratio * feature.shape[1]).astype(paddle.int32)
+        mask_lens = input_lens.unsqueeze(1)
+        # 生成掩码张量
+        idxs = paddle.arange(feature.shape[1])
+        idxs = idxs.tile([feature.shape[0], 1])
+        mask = idxs < mask_lens
+        mask = mask.unsqueeze(-1)
+        # 对特征进行掩码操作
+        feature_masked = paddle.where(mask, feature, paddle.zeros_like(feature))
+        return feature_masked, input_lens
 
     @property
     def feature_dim(self):
         """返回特征大小
 
         :return: 特征大小
         :rtype: int
         """
         if self._feature_method == 'LogMelSpectrogram':
-            return self._feature_conf.n_mels
+            return self._method_args.get('n_mels', 128)
         elif self._feature_method == 'MelSpectrogram':
-            return self._feature_conf.n_mels
+            return self._method_args.get('n_mels', 64)
         elif self._feature_method == 'Spectrogram':
-            return self._feature_conf.n_fft // 2 + 1
+            return self._method_args.get('n_fft', 512) // 2 + 1
         elif self._feature_method == 'MFCC':
-            return self._feature_conf.n_mfcc
+            return self._method_args.get('n_mfcc', 40)
+        elif self._feature_method == 'Fbank':
+            return self._method_args.get('n_mels', 23)
         else:
             raise Exception('没有{}预处理方法'.format(self._feature_method))
+
+
+class KaldiFbank(nn.Layer):
+    def __init__(self, **kwargs):
+        super(KaldiFbank, self).__init__()
+        self.kwargs = kwargs
+
+    def forward(self, waveforms):
+        """
+        :param waveforms: [Batch, Length]
+        :return: [Batch, Length, Feature]
+        """
+        log_fbanks = []
+        for waveform in waveforms:
+            if len(waveform.shape) == 1:
+                waveform = waveform.unsqueeze(0)
+            log_fbank = Kaldi.fbank(waveform, **self.kwargs)
+            log_fbank = log_fbank.transpose((1, 0))
+            log_fbanks.append(log_fbank)
+        log_fbank = paddle.stack(log_fbanks)
+        return log_fbank
```

## ppacls/data_utils/reader.py

```diff
@@ -1,66 +1,124 @@
+import os
+import random
+
 import numpy as np
 from paddle.io import Dataset
 
 from ppacls.data_utils.audio import AudioSegment
-from ppacls.data_utils.augmentor.augmentation import AugmentationPipeline
 from ppacls.utils.logger import setup_logger
 
 logger = setup_logger(__name__)
 
 
 # 音频数据加载器
 class CustomDataset(Dataset):
     def __init__(self,
                  data_list_path,
                  do_vad=True,
-                 chunk_duration=3,
+                 max_duration=3,
                  min_duration=0.5,
-                 augmentation_config='{}',
                  mode='train',
                  sample_rate=16000,
+                 aug_conf={},
                  use_dB_normalization=True,
                  target_dB=-20):
+        """音频数据加载器
+
+        Args:
+            data_list_path: 包含音频路径和标签的数据列表文件的路径
+            do_vad: 是否对音频进行语音活动检测（VAD）来裁剪静音部分
+            max_duration: 最长的音频长度，大于这个长度会裁剪掉
+            min_duration: 过滤最短的音频长度
+            aug_conf: 用于指定音频增强的配置
+            mode: 数据集模式。在训练模式下，数据集可能会进行一些数据增强的预处理
+            sample_rate: 采样率
+            use_dB_normalization: 是否对音频进行音量归一化
+            target_dB: 音量归一化的大小
+        """
         super(CustomDataset, self).__init__()
         self.do_vad = do_vad
-        self.chunk_duration = chunk_duration
+        self.max_duration = max_duration
         self.min_duration = min_duration
         self.mode = mode
         self._target_sample_rate = sample_rate
         self._use_dB_normalization = use_dB_normalization
         self._target_dB = target_dB
-        self._augmentation_pipeline = AugmentationPipeline(augmentation_config=augmentation_config)
+        self.aug_conf = aug_conf
+        self.noises_path = None
         # 获取数据列表
         with open(data_list_path, 'r') as f:
             self.lines = f.readlines()
 
     def __getitem__(self, idx):
         # 分割音频路径和标签
         audio_path, label = self.lines[idx].replace('\n', '').split('\t')
         # 读取音频
         audio_segment = AudioSegment.from_file(audio_path)
         # 裁剪静音
         if self.do_vad:
             audio_segment.vad()
         # 数据太短不利于训练
         if self.mode == 'train':
-            if audio_segment.num_samples < int(self.min_duration * audio_segment.sample_rate):
+            if audio_segment.duration < self.min_duration:
                 return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
         # 重采样
         if audio_segment.sample_rate != self._target_sample_rate:
             audio_segment.resample(self._target_sample_rate)
+        # 音频增强
+        if self.mode == 'train':
+            audio_segment = self.augment_audio(audio_segment, **self.aug_conf)
         # decibel normalization
         if self._use_dB_normalization:
             audio_segment.normalize(target_db=self._target_dB)
-        # 音频增强
-        self._augmentation_pipeline.transform_audio(audio_segment)
-        # 对小于训练长度的复制补充
-        num_chunk_samples = int(self.chunk_duration * audio_segment.sample_rate)
-        if audio_segment.num_samples < num_chunk_samples:
-            shortage = num_chunk_samples - audio_segment.num_samples
-            audio_segment.pad_silence(duration=float(shortage / audio_segment.sample_rate * 1.1), sides='end')
         # 裁剪需要的数据
-        audio_segment.crop(duration=self.chunk_duration, mode=self.mode)
+        audio_segment.crop(duration=self.max_duration, mode=self.mode)
         return np.array(audio_segment.samples, dtype=np.float32), np.array(int(label), dtype=np.int64)
 
     def __len__(self):
         return len(self.lines)
+
+    # 音频增强
+    def augment_audio(self,
+                      audio_segment,
+                      speed_perturb=False,
+                      volume_perturb=False,
+                      volume_aug_prob=0.2,
+                      noise_dir=None,
+                      noise_aug_prob=0.2):
+        # 语速增强，注意使用语速增强分类数量会大三倍
+        if speed_perturb:
+            speeds = [1.0, 0.9, 1.1]
+            speed_idx = random.randint(0, 2)
+            speed_rate = speeds[speed_idx]
+            if speed_rate != 1.0:
+                audio_segment.change_speed(speed_rate)
+        # 音量增强
+        if volume_perturb and random.random() < volume_aug_prob:
+            min_gain_dBFS, max_gain_dBFS = -15, 15
+            gain = random.uniform(min_gain_dBFS, max_gain_dBFS)
+            audio_segment.gain_db(gain)
+        # 获取噪声文件
+        if self.noises_path is None and noise_dir is not None:
+            self.noises_path = []
+            if noise_dir is not None and os.path.exists(noise_dir):
+                for file in os.listdir(noise_dir):
+                    self.noises_path.append(os.path.join(noise_dir, file))
+        # 噪声增强
+        if len(self.noises_path) > 0 and random.random() < noise_aug_prob:
+            min_snr_dB, max_snr_dB = 10, 50
+            # 随机选择一个noises_path中的一个
+            noise_path = random.sample(self.noises_path, 1)[0]
+            # 读取噪声音频
+            noise_segment = AudioSegment.slice_from_file(noise_path)
+            # 如果噪声采样率不等于audio_segment的采样率，则重采样
+            if noise_segment.sample_rate != audio_segment.sample_rate:
+                noise_segment.resample(audio_segment.sample_rate)
+            # 随机生成snr_dB的值
+            snr_dB = random.uniform(min_snr_dB, max_snr_dB)
+            # 如果噪声的长度小于audio_segment的长度，则将噪声的前面的部分填充噪声末尾补长
+            if noise_segment.duration < audio_segment.duration:
+                diff_duration = audio_segment.num_samples - noise_segment.num_samples
+                noise_segment._samples = np.pad(noise_segment.samples, (0, diff_duration), 'wrap')
+            # 将噪声添加到audio_segment中，并将snr_dB调整到最小值和最大值之间
+            audio_segment.add_noise(noise_segment, snr_dB)
+        return audio_segment
```

## ppacls/data_utils/utils.py

```diff
@@ -78,28 +78,41 @@
     resampler = av.audio.resampler.AudioResampler(format="s16", layout="mono", rate=sample_rate)
 
     raw_buffer = io.BytesIO()
     dtype = None
 
     with av.open(file, metadata_errors="ignore") as container:
         frames = container.decode(audio=0)
+        frames = _ignore_invalid_frames(frames)
         frames = _group_frames(frames, 500000)
         frames = _resample_frames(frames, resampler)
 
         for frame in frames:
             array = frame.to_ndarray()
             dtype = array.dtype
             raw_buffer.write(array)
 
     audio = np.frombuffer(raw_buffer.getbuffer(), dtype=dtype)
 
     # Convert s16 back to f32.
     return audio.astype(np.float32) / 32768.0
 
 
+def _ignore_invalid_frames(frames):
+    iterator = iter(frames)
+
+    while True:
+        try:
+            yield next(iterator)
+        except StopIteration:
+            break
+        except av.error.InvalidDataError:
+            continue
+
+
 def _group_frames(frames, num_samples=None):
     fifo = av.audio.fifo.AudioFifo()
 
     for frame in frames:
         frame.pts = None  # Ignore timestamp check.
         fifo.write(frame)
```

## ppacls/models/ecapa_tdnn.py

```diff
@@ -241,25 +241,29 @@
                              out_channels=self.emb_size,
                              kernel_size=1)
         else:
             raise Exception(f'没有{pooling_type}池化层！')
 
         self.output = nn.Linear(self.emb_size, num_class)
 
-    def forward(self, x, lengths=None):
+    def forward(self, x):
         """
         Compute embeddings.
 
         Args:
             x (paddle.Tensor): Input data with shape (N, time, freq).
             lengths (paddle.Tensor, optional): Length proportions of batch length with shape (N). Defaults to None.
 
         Returns:
             paddle.Tensor: Output embeddings with shape (N, self.emb_size, 1)
         """
+        if isinstance(x, list):
+            x, lengths = x
+        else:
+            lengths = None
         x = x.transpose([0, 2, 1])
         xl = []
         for layer in self.blocks:
             try:
                 x = layer(x, lengths=lengths)
             except TypeError:
                 x = layer(x)
```

## ppacls/models/panns.py

```diff
@@ -94,15 +94,15 @@
         self.fc1 = nn.Linear(512, self.emb_size)
         self.fc_audioset = nn.Linear(self.emb_size, 527)
         self.extract_embedding = extract_embedding
 
         self.dropout = nn.Dropout(dropout)
         self.fc = nn.Linear(self.emb_size, num_class)
 
-    def forward(self, x, x_len):
+    def forward(self, x):
         x = x.unsqueeze(1)
         x = x.transpose([0, 3, 2, 1])
         x = self.bn0(x)
         x = x.transpose([0, 3, 2, 1])
 
         x = self.conv_block1(x, pool_size=(2, 2), pool_type='avg')
         x = F.dropout(x, p=0.2, training=self.training)
@@ -156,15 +156,15 @@
         self.fc1 = nn.Linear(512, self.emb_size)
         self.fc_audioset = nn.Linear(self.emb_size, 527)
         self.extract_embedding = extract_embedding
 
         self.dropout = nn.Dropout(dropout)
         self.fc = nn.Linear(self.emb_size, num_class)
 
-    def forward(self, x, x_len):
+    def forward(self, x):
         x = x.unsqueeze(1)
         x = x.transpose([0, 3, 2, 1])
         x = self.bn0(x)
         x = x.transpose([0, 3, 2, 1])
 
         x = self.conv_block1(x, pool_size=(2, 2), pool_type='avg')
         x = F.dropout(x, p=0.2, training=self.training)
@@ -220,15 +220,15 @@
         self.fc1 = nn.Linear(2048, self.emb_size)
         self.fc_audioset = nn.Linear(self.emb_size, 527)
         self.extract_embedding = extract_embedding
 
         self.dropout = nn.Dropout(dropout)
         self.fc = nn.Linear(self.emb_size, num_class)
 
-    def forward(self, x, x_len):
+    def forward(self, x):
         x = x.unsqueeze(1)
         x = x.transpose([0, 3, 2, 1])
         x = self.bn0(x)
         x = x.transpose([0, 3, 2, 1])
 
         x = self.conv_block1(x, pool_size=(2, 2), pool_type='avg')
         x = F.dropout(x, p=0.2, training=self.training)
```

## ppacls/models/res2net.py

```diff
@@ -150,15 +150,15 @@
                         stype='stage', baseWidth=self.base_width, scale=self.scale)]
         self.inplanes = planes * block.expansion
         for i in range(1, blocks):
             layers.append(block(self.inplanes, planes, baseWidth=self.base_width, scale=self.scale))
 
         return nn.Sequential(*layers)
 
-    def forward(self, x, lengths=None):
+    def forward(self, x):
         x = x.transpose([0, 2, 1])
         x = x.unsqueeze(1)
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.relu(x)
         x = self.max_pool(x)
```

## ppacls/models/resnet_se.py

```diff
@@ -157,15 +157,15 @@
         layers = [block(self.inplanes, planes, stride, downsample)]
         self.inplanes = planes * block.expansion
         for i in range(1, blocks):
             layers.append(block(self.inplanes, planes))
 
         return nn.Sequential(*layers)
 
-    def forward(self, x, lengths=None):
+    def forward(self, x):
         x = x.transpose([0, 2, 1])
         x = x.unsqueeze(1)
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.relu(x)
 
         x = self.layer1(x)
```

## ppacls/models/tdnn.py

```diff
@@ -49,15 +49,15 @@
                              out_channels=self.emb_size,
                              kernel_size=1)
         else:
             raise Exception(f'没有{pooling_type}池化层！')
 
         self.output = nn.Linear(self.emb_size, num_class)
 
-    def forward(self, x, lengths=None):
+    def forward(self, x):
         """
         Compute embeddings.
 
         Args:
             x (torch.Tensor): Input data with shape (N, time, freq).
 
         Returns:
```

## ppacls/utils/record.py

```diff
@@ -1,50 +1,31 @@
 import os
-import wave
 
-import pyaudio
+import soundcard
+import soundfile
 
 
 class RecordAudio:
-    def __init__(self):
+    def __init__(self, channels=1, sample_rate=16000):
         # 录音参数
-        self.chunk = 1024
-        self.format = pyaudio.paInt16
-        self.channels = 1
-        self.rate = 16000
-
-        # 打开录音
-        self.p = pyaudio.PyAudio()
-        self.stream = self.p.open(format=self.format,
-                                  channels=self.channels,
-                                  rate=self.rate,
-                                  input=True,
-                                  frames_per_buffer=self.chunk)
+        self.channels = channels
+        self.sample_rate = sample_rate
+
+        # 获取麦克风
+        self.default_mic = soundcard.default_microphone()
 
     def record(self, record_seconds=3, save_path=None):
         """录音
 
         :param record_seconds: 录音时间，默认3秒
         :param save_path: 录音保存的路径，后缀名为wav
-        :return: 录音的文件路径
+        :return: 音频的numpy数据
         """
         print("开始录音......")
-        frames = []
-        for i in range(0, int(self.rate / self.chunk * record_seconds)):
-            data = self.stream.read(self.chunk)
-            frames.append(data)
-
+        num_frames = int(record_seconds * self.sample_rate)
+        data = self.default_mic.record(samplerate=self.sample_rate, numframes=num_frames, channels=self.channels)
+        audio_data = data.squeeze()
         print("录音已结束!")
-        audio_data = b''.join(frames)
         if save_path is not None:
             os.makedirs(os.path.dirname(save_path), exist_ok=True)
-            wf = wave.open(save_path, 'wb')
-            wf.setnchannels(self.channels)
-            wf.setsampwidth(self.p.get_sample_size(self.format))
-            wf.setframerate(self.rate)
-            wf.writeframes(b''.join(frames))
-            wf.close()
+            soundfile.write(save_path, data=data, samplerate=self.sample_rate)
         return audio_data
-
-    def close(self):
-        self.stream.close()
-        self.p.close()
```

## Comparing `ppacls-0.3.3.dist-info/LICENSE` & `ppacls-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ppacls-0.3.3.dist-info/RECORD` & `ppacls-0.4.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-ppacls/__init__.py,sha256=VLx9wNuBj0wRvc9G4VOHIKpm4iiFYNufPdWO6SIPP-Q,131
-ppacls/predict.py,sha256=A9hTEhzAdl7ObriPn99c8RDTwkNN-seX-zYezGV-6cw,8528
-ppacls/trainer.py,sha256=84YF7bCONKbaBbWsNPISWYPkHrNQNgL3YmUBdIRoa0Y,23680
+ppacls/__init__.py,sha256=wikLtyqyBTLDjLAsamssDRQMEC8AOKbTbzBPIOlatIM,154
+ppacls/predict.py,sha256=jtpJeJ3FNiIr9NTQinYUwbBUt46B2sOenWGv2Wt07sA,8971
+ppacls/trainer.py,sha256=1NltJ6vUolYDhON5tBJui8lZzfsDqvx8cnsVDTHzal0,25444
 ppacls/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppacls/data_utils/audio.py,sha256=uBqejS9qAfxw9VMVmUNrF8gkXN7jd48S3K2GDUKtm9s,22814
-ppacls/data_utils/featurizer.py,sha256=BNSfSmCrza7UNA95qHD4UG21DxNVHNrD-yKVe97Lio0,2307
-ppacls/data_utils/reader.py,sha256=a1tzFPDFPcK5QPn8UZS-cZDlUkVDChuXezrqPtPjOgA,2813
-ppacls/data_utils/utils.py,sha256=U81Q-hmPQDUK_yc-opzOb8G28dgEWqnOq5ej3jSrk7w,4337
-ppacls/data_utils/augmentor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppacls/data_utils/augmentor/augmentation.py,sha256=V1mOOCuLB7pHGEUulYGd-jPOhNUWkhIMcUKKG8uQDHg,5105
-ppacls/data_utils/augmentor/base.py,sha256=Qw5AsIjpqDkggVkVyfPGTI_IwnfSuIWViRdgo7g2ze0,965
-ppacls/data_utils/augmentor/noise_perturb.py,sha256=XRu-d97toPzOGSN3lNtaheCP3doo0UhOIk-83_-grGI,2026
-ppacls/data_utils/augmentor/resample.py,sha256=dIql7ARk8WKq29oy4TqiI4Txsa7DaZPucOQYtRIZVX0,979
-ppacls/data_utils/augmentor/shift_perturb.py,sha256=0GmZZ10wsbnoziym3DTpGJzp_wJRPHvm4UwO2s5s3JM,1009
-ppacls/data_utils/augmentor/spec_augment.py,sha256=Eg1i0v4JVZYc8Sg7ezGobGvQZd44c6tq-0UjOus0CK4,5015
-ppacls/data_utils/augmentor/spec_sub.py,sha256=sPa5Jvbrhl5zHycSU_wPWkKnyQ2u0JgSOmhWO7ACdJ4,1138
-ppacls/data_utils/augmentor/speed_perturb.py,sha256=bhdcxPbDDfnHXL97oS2hzeoJCZqg4tMKLSxw3r0XkT4,1980
-ppacls/data_utils/augmentor/volume_perturb.py,sha256=jF0MrujL8X0-cL_jNzr-y1BJ7cgVzLRbcnUCYMqjhrw,1140
+ppacls/data_utils/audio.py,sha256=plDqJzokaP18Gm3wNZNcbGlMffjTINUbjBA1xxU-Dck,22288
+ppacls/data_utils/collate_fn.py,sha256=tb5yu7VH69x1nGKxJUBoZ5UNsVgYxZ_zbth2YN52zPw,909
+ppacls/data_utils/featurizer.py,sha256=9j7nEQbe1f5udaxZwFIG6D_erTW3gMKuIZB2cd3-hMI,3771
+ppacls/data_utils/reader.py,sha256=tHSAewEP3bqSzhjkkavzWk-i_BOGuX8q1xopV4kxJkM,5517
+ppacls/data_utils/spec_aug.py,sha256=Qw32xZTw1f8Fk3Kw9aQt_5IKiH8k1giXbCX3XUzU1xw,1581
+ppacls/data_utils/utils.py,sha256=POF5Eyg6bAgOWKnELkM4nOEG82_NLrEK8ooLHiodvVs,4638
 ppacls/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppacls/models/ecapa_tdnn.py,sha256=7nZvcmecZW8kWVARP7tjQHRJyxPAhqoDGgofESZrCNo,11101
-ppacls/models/panns.py,sha256=ypbS0PMAEZ-JuMNrImPgBWt4997nvzDmKRWv44FcAKE,9884
+ppacls/models/ecapa_tdnn.py,sha256=551n7Ux2Q1m08c8oe0CQayFj-e5o1bH5GeaLt7dnmA8,11191
+ppacls/models/panns.py,sha256=4L2JQgaSQyIvWNCmr7zKmU0oiHOwN3nGB1FD5hQbSUM,9863
 ppacls/models/pooling.py,sha256=Zill06JHzPbPiJCKuK3X1sXGF2wzaRMAnnne1dzVBKE,4539
-ppacls/models/res2net.py,sha256=blXV-TwgxJI2y9H1uousq6P8mF5aRI_Djz66KdkNhUI,6841
-ppacls/models/resnet_se.py,sha256=bN4CFWUD_zOrjrfgok9PfVB5yDhIT3DgoVS2WnCopAc,6713
-ppacls/models/tdnn.py,sha256=RHiwFoMAnRp27_Raf6uMBVBzkDOICf8kJNCBxQvRGDA,3571
+ppacls/models/res2net.py,sha256=PPO-9qnkvNNBW55CvC8Ky8EWu4wIgc-IK3yaKzucQ8I,6827
+ppacls/models/resnet_se.py,sha256=8D6zA8PIxPCEIQBsGkUOjAvWJIi06YcLT3yFFRyKoN0,6699
+ppacls/models/tdnn.py,sha256=ndUJdqtAKsY17kSOwQ697-_6Y_krIl-UHMIKDtkP-vI,3557
 ppacls/models/utils.py,sha256=WFaGb66sSLalS-2yr9VIOnICrLjR8rGmiggGaWnZV_Y,5049
 ppacls/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppacls/utils/logger.py,sha256=-ssorx8FlHA_wrd2Eq6f4HkOqaOG2YseBGvYAo8NXN8,2839
-ppacls/utils/lr.py,sha256=Y5miRHlE00rZS6nVMt82d0S8KRoy5XvREc2pnOim2NU,1028
-ppacls/utils/record.py,sha256=GIX3fU9oyIIDmM59TPQ7w1bLOH6JYxMddlW4Hk9fqQA,1594
+ppacls/utils/record.py,sha256=2i4kz5kPDa9KkbAK_Q34sVIXOkD9TroPROIe5QdzqWg,1067
+ppacls/utils/scheduler.py,sha256=IZ1kU6S86hfnuZLfkepflStogDyYvRPEDMP4P_mwGvs,3399
 ppacls/utils/utils.py,sha256=0_GNZXI_2yNcX3AOEltt1p6ZsmvqcU-YyAuXqwlaQdE,3365
-ppacls-0.3.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ppacls-0.3.3.dist-info/METADATA,sha256=1bHjSTyziwkaxLx52bQVn4X9bM2IQiru4xsLc6q4ooc,6462
-ppacls-0.3.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ppacls-0.3.3.dist-info/top_level.txt,sha256=RkvwIMbjgjfhvlagK7GKtMw9ZSfGRMbY4vk2nbLpvrY,7
-ppacls-0.3.3.dist-info/RECORD,,
+ppacls-0.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+ppacls-0.4.0.dist-info/METADATA,sha256=LpJ-qC0FmxTiiXPbVyHCO8KwnbzjpHaA28b41rXIsUU,18452
+ppacls-0.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ppacls-0.4.0.dist-info/top_level.txt,sha256=RkvwIMbjgjfhvlagK7GKtMw9ZSfGRMbY4vk2nbLpvrY,7
+ppacls-0.4.0.dist-info/RECORD,,
```

