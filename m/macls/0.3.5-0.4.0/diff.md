# Comparing `tmp/macls-0.3.5-py3-none-any.whl.zip` & `tmp/macls-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,36 +1,31 @@
-Zip file size: 47647 bytes, number of entries: 34
--rw-rw-rw-  2.0 fat      131 b- defN 23-Mar-21 11:28 macls/__init__.py
--rw-rw-rw-  2.0 fat     8422 b- defN 23-Mar-21 13:03 macls/predict.py
--rw-rw-rw-  2.0 fat    24545 b- defN 23-Mar-21 13:03 macls/trainer.py
+Zip file size: 45341 bytes, number of entries: 29
+-rw-rw-rw-  2.0 fat      154 b- defN 23-Aug-08 12:36 macls/__init__.py
+-rw-rw-rw-  2.0 fat     8970 b- defN 23-Aug-07 14:52 macls/predict.py
+-rw-rw-rw-  2.0 fat    26413 b- defN 23-Aug-08 12:30 macls/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 macls/data_utils/__init__.py
--rw-rw-rw-  2.0 fat    22813 b- defN 23-Mar-22 11:02 macls/data_utils/audio.py
--rw-rw-rw-  2.0 fat     2420 b- defN 23-Mar-01 11:31 macls/data_utils/featurizer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-Jan-30 13:17 macls/data_utils/reader.py
--rw-rw-rw-  2.0 fat     4337 b- defN 23-Mar-22 11:02 macls/data_utils/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/__init__.py
--rw-rw-rw-  2.0 fat     5517 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/augmentation.py
--rw-rw-rw-  2.0 fat      965 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/base.py
--rw-rw-rw-  2.0 fat     2024 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/noise_perturb.py
--rw-rw-rw-  2.0 fat      977 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/resample.py
--rw-rw-rw-  2.0 fat     1007 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/shift_perturb.py
--rw-rw-rw-  2.0 fat     5015 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/spec_augment.py
--rw-rw-rw-  2.0 fat     1138 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/spec_sub.py
--rw-rw-rw-  2.0 fat     1978 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/speed_perturb.py
--rw-rw-rw-  2.0 fat     1138 b- defN 23-Jan-30 13:17 macls/data_utils/augmentor/volume_perturb.py
+-rw-rw-rw-  2.0 fat    22287 b- defN 23-Aug-06 15:13 macls/data_utils/audio.py
+-rw-rw-rw-  2.0 fat      965 b- defN 23-Feb-15 12:59 macls/data_utils/collate_fn.py
+-rw-rw-rw-  2.0 fat     3587 b- defN 23-Aug-06 15:14 macls/data_utils/featurizer.py
+-rw-rw-rw-  2.0 fat     5640 b- defN 23-Aug-06 15:50 macls/data_utils/reader.py
+-rw-rw-rw-  2.0 fat     1572 b- defN 23-Aug-07 14:52 macls/data_utils/spec_aug.py
+-rw-rw-rw-  2.0 fat     5652 b- defN 23-Mar-28 12:05 macls/data_utils/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-16 05:03 macls/metric/__init__.py
+-rw-rw-rw-  2.0 fat      329 b- defN 23-Aug-07 15:15 macls/metric/metrics.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 macls/models/__init__.py
 -rw-rw-rw-  2.0 fat     5378 b- defN 23-Mar-21 11:25 macls/models/ecapa_tdnn.py
 -rw-rw-rw-  2.0 fat     9707 b- defN 23-Mar-21 11:25 macls/models/panns.py
 -rw-rw-rw-  2.0 fat     3000 b- defN 23-Mar-18 06:27 macls/models/pooling.py
 -rw-rw-rw-  2.0 fat     6680 b- defN 23-Mar-21 11:25 macls/models/res2net.py
 -rw-rw-rw-  2.0 fat     6585 b- defN 23-Mar-21 11:25 macls/models/resnet_se.py
 -rw-rw-rw-  2.0 fat     3050 b- defN 23-Mar-21 11:25 macls/models/tdnn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 macls/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2839 b- defN 23-Jan-30 13:17 macls/utils/logger.py
--rw-rw-rw-  2.0 fat     1594 b- defN 23-Mar-21 13:09 macls/utils/record.py
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Mar-23 11:45 macls/utils/record.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 23-Aug-06 15:19 macls/utils/scheduler.py
 -rw-rw-rw-  2.0 fat     3364 b- defN 23-Feb-20 12:41 macls/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Mar-22 11:20 macls-0.3.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6487 b- defN 23-Mar-22 11:20 macls-0.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-22 11:20 macls-0.3.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Mar-22 11:20 macls-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2851 b- defN 23-Mar-22 11:20 macls-0.3.5.dist-info/RECORD
-34 files, 148433 bytes uncompressed, 43073 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-08 14:08 macls-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17396 b- defN 23-Aug-08 14:08 macls-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-08 14:08 macls-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Aug-08 14:08 macls-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2291 b- defN 23-Aug-08 14:08 macls-0.4.0.dist-info/RECORD
+29 files, 150078 bytes uncompressed, 41699 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -9,51 +9,33 @@
 
 Filename: macls/data_utils/__init__.py
 Comment: 
 
 Filename: macls/data_utils/audio.py
 Comment: 
 
-Filename: macls/data_utils/featurizer.py
-Comment: 
-
-Filename: macls/data_utils/reader.py
-Comment: 
-
-Filename: macls/data_utils/utils.py
-Comment: 
-
-Filename: macls/data_utils/augmentor/__init__.py
-Comment: 
-
-Filename: macls/data_utils/augmentor/augmentation.py
-Comment: 
-
-Filename: macls/data_utils/augmentor/base.py
-Comment: 
-
-Filename: macls/data_utils/augmentor/noise_perturb.py
+Filename: macls/data_utils/collate_fn.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/resample.py
+Filename: macls/data_utils/featurizer.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/shift_perturb.py
+Filename: macls/data_utils/reader.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/spec_augment.py
+Filename: macls/data_utils/spec_aug.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/spec_sub.py
+Filename: macls/data_utils/utils.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/speed_perturb.py
+Filename: macls/metric/__init__.py
 Comment: 
 
-Filename: macls/data_utils/augmentor/volume_perturb.py
+Filename: macls/metric/metrics.py
 Comment: 
 
 Filename: macls/models/__init__.py
 Comment: 
 
 Filename: macls/models/ecapa_tdnn.py
 Comment: 
@@ -78,26 +60,29 @@
 
 Filename: macls/utils/logger.py
 Comment: 
 
 Filename: macls/utils/record.py
 Comment: 
 
+Filename: macls/utils/scheduler.py
+Comment: 
+
 Filename: macls/utils/utils.py
 Comment: 
 
-Filename: macls-0.3.5.dist-info/LICENSE
+Filename: macls-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: macls-0.3.5.dist-info/METADATA
+Filename: macls-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: macls-0.3.5.dist-info/WHEEL
+Filename: macls-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: macls-0.3.5.dist-info/top_level.txt
+Filename: macls-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: macls-0.3.5.dist-info/RECORD
+Filename: macls-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## macls/__init__.py

```diff
@@ -1,2 +1,3 @@
+__version__ = "0.4.0"
 # 项目支持的模型
 SUPPORT_MODEL = ['EcapaTdnn', 'PANNS_CNN6', 'PANNS_CNN10', 'PANNS_CNN14', 'Res2Net', 'ResNetSE', 'TDNN']
```

## macls/predict.py

```diff
@@ -1,8 +1,10 @@
 import os
+from io import BufferedReader
+from typing import List
 
 import numpy as np
 import torch
 import yaml
 
 from macls import SUPPORT_MODEL
 from macls.data_utils.audio import AudioSegment
@@ -17,15 +19,15 @@
 
 logger = setup_logger(__name__)
 
 
 class MAClsPredictor:
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
@@ -39,128 +41,132 @@
         if isinstance(configs, str):
             with open(configs, 'r', encoding='utf-8') as f:
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         # 获取特征器
-        self.audio_featurizer = AudioFeaturizer(feature_conf=self.configs.feature_conf, **self.configs.preprocess_conf)
-        self.audio_featurizer.to(self.device)
+        self._audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
+        self._audio_featurizer.to(self.device)
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
         self.predictor.to(self.device)
         # 加载模型
         if os.path.isdir(model_path):
-            model_path = os.path.join(model_path, 'model.pt')
+            model_path = os.path.join(model_path, 'model.pth')
         assert os.path.exists(model_path), f"{model_path} 模型不存在！"
         if torch.cuda.is_available() and use_gpu:
             model_state_dict = torch.load(model_path)
         else:
             model_state_dict = torch.load(model_path, map_location='cpu')
         self.predictor.load_state_dict(model_state_dict)
         print(f"成功加载模型参数：{model_path}")
         self.predictor.eval()
         # 获取分类标签
         with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
             lines = f.readlines()
         self.class_labels = [l.replace('\n', '') for l in lines]
 
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
         input_data = torch.tensor(input_data.samples, dtype=torch.float32, device=self.device).unsqueeze(0)
-        audio_feature = self.audio_featurizer(input_data)
+        input_len_ratio = torch.tensor([1], dtype=torch.float32, device=self.device)
+        audio_feature, _ = self._audio_featurizer(input_data, input_len_ratio)
         # 执行预测
         output = self.predictor(audio_feature)
         result = torch.nn.functional.softmax(output, dim=-1)[0]
         result = result.data.cpu().numpy()
         # 最大概率的label
         lab = np.argsort(result)[-1]
         score = result[lab]
         return self.class_labels[lab], round(float(score), 5)
 
-    def predict_batch(self, audios_data):
-        """预测一批音频
+    def predict_batch(self, audios_data: List, sample_rate=16000):
+        """预测一批音频的特征
 
-        :param audios_data: 经过预处理的一批数据
+        :param audios_data: 需要识别的数据，支持文件路径，文件对象，字节，numpy。如果是字节的话，必须是完整并带格式的字节文件
+        :param sample_rate: 如果传入的事numpy数据，需要指定采样率
         :return: 结果标签和对应的得分
         """
+        audios_data1 = []
+        for audio_data in audios_data:
+            # 加载音频文件，并进行预处理
+            input_data = self._load_audio(audio_data=audio_data, sample_rate=sample_rate)
+            audios_data1.append(input_data.samples)
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
-        audios_data = torch.tensor(inputs, dtype=torch.float32, device=self.device).unsqueeze(0)
+            inputs[x, :seq_length] = tensor[:]
+            input_lens_ratio.append(seq_length / max_audio_length)
+        input_lens_ratio = torch.tensor(input_lens_ratio, dtype=torch.float32, device=self.device)
+        inputs = torch.tensor(inputs, dtype=torch.float32, device=self.device)
+        audio_feature, _ = self._audio_featurizer(inputs, input_lens_ratio)
         # 执行预测
-        output = self.predictor(audios_data)
+        output = self.predictor(audio_feature)
         results = torch.nn.functional.softmax(output, dim=-1)
         results = results.data.cpu().numpy()
         labels, scores = [], []
         for result in results:
             lab = np.argsort(result)[-1]
             score = result[lab]
             labels.append(self.class_labels[lab])
```

## macls/trainer.py

```diff
@@ -14,23 +14,27 @@
 from torch.utils.data.distributed import DistributedSampler
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from torch.utils.data import DataLoader
 from torchinfo import summary
 from tqdm import tqdm
 from visualdl import LogWriter
 
-from macls import SUPPORT_MODEL
+from macls import SUPPORT_MODEL, __version__
+from macls.data_utils.collate_fn import collate_fn
 from macls.data_utils.featurizer import AudioFeaturizer
 from macls.data_utils.reader import CustomDataset
+from macls.data_utils.spec_aug import SpecAug
+from macls.metric.metrics import accuracy
 from macls.models.ecapa_tdnn import EcapaTdnn
 from macls.models.panns import PANNS_CNN6, PANNS_CNN10, PANNS_CNN14
 from macls.models.res2net import Res2Net
 from macls.models.resnet_se import ResNetSE
 from macls.models.tdnn import TDNN
 from macls.utils.logger import setup_logger
+from macls.utils.scheduler import WarmupCosineSchedulerLR
 from macls.utils.utils import dict_to_object, plot_confusion_matrix, print_arguments
 
 logger = setup_logger(__name__)
 
 
 class MAClsTrainer(object):
     def __init__(self, configs, use_gpu=True):
@@ -51,103 +55,95 @@
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
         if platform.system().lower() == 'windows':
-            self.configs.dataset_conf.num_workers = 0
+            self.configs.dataset_conf.dataLoader.num_workers = 0
             logger.warning('Windows系统不支持多线程读取数据，已自动关闭！')
         # 获取特征器
-        self.audio_featurizer = AudioFeaturizer(feature_conf=self.configs.feature_conf, **self.configs.preprocess_conf)
+        self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
+        self.audio_featurizer.to(self.device)
+        # 特征增强
+        self.spec_aug = SpecAug(**self.configs.dataset_conf.get('spec_aug_args', {}))
+        self.spec_aug.to(self.device)
 
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
+            # 设置支持多卡训练
             train_sampler = None
             if torch.cuda.device_count() > 1:
                 # 设置支持多卡训练
                 train_sampler = DistributedSampler(dataset=self.train_dataset)
             self.train_loader = DataLoader(dataset=self.train_dataset,
+                                           collate_fn=collate_fn,
                                            shuffle=(train_sampler is None),
-                                           batch_size=self.configs.dataset_conf.batch_size,
                                            sampler=train_sampler,
-                                           num_workers=self.configs.dataset_conf.num_workers)
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
         self.model.to(self.device)
         self.audio_featurizer.to(self.device)
         summary(self.model, input_size=(1, 98, self.audio_featurizer.feature_dim))
+        # 使用Pytorch2.0的编译器
+        if self.configs.train_conf.use_compile and torch.__version__ >= "2" and platform.system().lower() == 'windows':
+            self.model = torch.compile(self.model, mode="reduce-overhead")
         # print(self.model)
         # 获取损失函数
         self.loss = torch.nn.CrossEntropyLoss()
         if is_train:
+            if self.configs.train_conf.enable_amp:
+                self.amp_scaler = torch.cuda.amp.GradScaler(init_scale=1024)
             # 获取优化方法
             optimizer = self.configs.optimizer_conf.optimizer
             if optimizer == 'Adam':
                 self.optimizer = torch.optim.Adam(params=self.model.parameters(),
                                                   lr=float(self.configs.optimizer_conf.learning_rate),
                                                   weight_decay=float(self.configs.optimizer_conf.weight_decay))
             elif optimizer == 'AdamW':
@@ -158,21 +154,34 @@
                 self.optimizer = torch.optim.SGD(params=self.model.parameters(),
                                                  momentum=self.configs.optimizer_conf.momentum,
                                                  lr=float(self.configs.optimizer_conf.learning_rate),
                                                  weight_decay=float(self.configs.optimizer_conf.weight_decay))
             else:
                 raise Exception(f'不支持优化方法：{optimizer}')
             # 学习率衰减函数
-            self.scheduler = CosineAnnealingLR(self.optimizer, T_max=int(self.configs.train_conf.max_epoch * 1.2))
+            scheduler_args = self.configs.optimizer_conf.get('scheduler_args', {}) \
+                if self.configs.optimizer_conf.get('scheduler_args', {}) is not None else {}
+            if self.configs.optimizer_conf.scheduler == 'CosineAnnealingLR':
+                max_step = int(self.configs.train_conf.max_epoch * 1.2) * len(self.train_loader)
+                self.scheduler = CosineAnnealingLR(optimizer=self.optimizer,
+                                                   T_max=max_step,
+                                                   **scheduler_args)
+            elif self.configs.optimizer_conf.scheduler == 'WarmupCosineSchedulerLR':
+                self.scheduler = WarmupCosineSchedulerLR(optimizer=self.optimizer,
+                                                         fix_epoch=self.configs.train_conf.max_epoch,
+                                                         step_per_epoch=len(self.train_loader),
+                                                         **scheduler_args)
+            else:
+                raise Exception(f'不支持学习率衰减函数：{self.configs.optimizer_conf.scheduler}')
 
     def __load_pretrained(self, pretrained_model):
         # 加载预训练模型
         if pretrained_model is not None:
             if os.path.isdir(pretrained_model):
-                pretrained_model = os.path.join(pretrained_model, 'model.pt')
+                pretrained_model = os.path.join(pretrained_model, 'model.pth')
             assert os.path.exists(pretrained_model), f"{pretrained_model} 模型不存在！"
             if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
                 model_dict = self.model.module.state_dict()
             else:
                 model_dict = self.model.state_dict()
             model_state_dict = torch.load(pretrained_model)
             # 过滤不存在的参数
@@ -192,26 +201,29 @@
 
     def __load_checkpoint(self, save_model_path, resume_model):
         last_epoch = -1
         best_acc = 0
         last_model_dir = os.path.join(save_model_path,
                                       f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                       'last_model')
-        if resume_model is not None or (os.path.exists(os.path.join(last_model_dir, 'model.pt'))
-                                        and os.path.exists(os.path.join(last_model_dir, 'optimizer.pt'))):
+        if resume_model is not None or (os.path.exists(os.path.join(last_model_dir, 'model.pth'))
+                                        and os.path.exists(os.path.join(last_model_dir, 'optimizer.pth'))):
             # 自动获取最新保存的模型
             if resume_model is None: resume_model = last_model_dir
-            assert os.path.exists(os.path.join(resume_model, 'model.pt')), "模型参数文件不存在！"
-            assert os.path.exists(os.path.join(resume_model, 'optimizer.pt')), "优化方法参数文件不存在！"
-            state_dict = torch.load(os.path.join(resume_model, 'model.pt'))
+            assert os.path.exists(os.path.join(resume_model, 'model.pth')), "模型参数文件不存在！"
+            assert os.path.exists(os.path.join(resume_model, 'optimizer.pth')), "优化方法参数文件不存在！"
+            state_dict = torch.load(os.path.join(resume_model, 'model.pth'))
             if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
                 self.model.module.load_state_dict(state_dict)
             else:
                 self.model.load_state_dict(state_dict)
-            self.optimizer.load_state_dict(torch.load(os.path.join(resume_model, 'optimizer.pt')))
+            self.optimizer.load_state_dict(torch.load(os.path.join(resume_model, 'optimizer.pth')))
+            # 自动混合精度参数
+            if self.amp_scaler is not None and os.path.exists(os.path.join(resume_model, 'scaler.pth')):
+                self.amp_scaler.load_state_dict(torch.load(os.path.join(resume_model, 'scaler.pth')))
             with open(os.path.join(resume_model, 'model.state'), 'r', encoding='utf-8') as f:
                 json_data = json.load(f)
                 last_epoch = json_data['last_epoch'] - 1
                 best_acc = json_data['accuracy']
             logger.info('成功恢复模型参数和优化方法参数：{}'.format(resume_model))
         return last_epoch, best_acc
 
@@ -226,18 +238,22 @@
                                       f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                       'best_model')
         else:
             model_path = os.path.join(save_model_path,
                                       f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                       'epoch_{}'.format(epoch_id))
         os.makedirs(model_path, exist_ok=True)
-        torch.save(self.optimizer.state_dict(), os.path.join(model_path, 'optimizer.pt'))
-        torch.save(state_dict, os.path.join(model_path, 'model.pt'))
+        torch.save(self.optimizer.state_dict(), os.path.join(model_path, 'optimizer.pth'))
+        torch.save(state_dict, os.path.join(model_path, 'model.pth'))
+        # 自动混合精度参数
+        if self.amp_scaler is not None:
+            torch.save(self.amp_scaler.state_dict(), os.path.join(model_path, 'scaler.pth'))
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
@@ -248,43 +264,58 @@
                 shutil.rmtree(old_model_path)
         logger.info('已保存模型：{}'.format(model_path))
 
     def __train_epoch(self, epoch_id, local_rank, writer, nranks=0):
         train_times, accuracies, loss_sum = [], [], []
         start = time.time()
         sum_batch = len(self.train_loader) * self.configs.train_conf.max_epoch
-        for batch_id, (audio, label) in enumerate(self.train_loader):
+        for batch_id, (audio, label, input_lens_ratio) in enumerate(self.train_loader):
             if nranks > 1:
                 audio = audio.to(local_rank)
+                input_lens_ratio = input_lens_ratio.to(local_rank)
                 label = label.to(local_rank).long()
             else:
                 audio = audio.to(self.device)
+                input_lens_ratio = input_lens_ratio.to(self.device)
                 label = label.to(self.device).long()
-            features = self.audio_featurizer(audio)
-            output = self.model(features)
+            features, _ = self.audio_featurizer(audio, input_lens_ratio)
+            # 特征增强
+            if self.configs.dataset_conf.use_spec_aug:
+                features = self.spec_aug(features)
+            # 执行模型计算，是否开启自动混合精度
+            with torch.cuda.amp.autocast(enabled=self.configs.train_conf.enable_amp):
+                output = self.model(features)
             # 计算损失值
             los = self.loss(output, label)
+            # 是否开启自动混合精度
+            if self.configs.train_conf.enable_amp:
+                # loss缩放，乘以系数loss_scaling
+                scaled = self.amp_scaler.scale(los)
+                scaled.backward()
+            else:
+                los.backward()
+            # 是否开启自动混合精度
+            if self.configs.train_conf.enable_amp:
+                self.amp_scaler.unscale_(self.optimizer)
+                self.amp_scaler.step(self.optimizer)
+                self.amp_scaler.update()
+            else:
+                self.optimizer.step()
             self.optimizer.zero_grad()
-            los.backward()
-            self.optimizer.step()
 
             # 计算准确率
-            output = torch.nn.functional.softmax(output, dim=-1)
-            output = output.data.cpu().numpy()
-            output = np.argmax(output, axis=1)
-            label = label.data.cpu().numpy()
-            acc = np.mean((output == label).astype(int))
+            acc = accuracy(output, label)
             accuracies.append(acc)
             loss_sum.append(los)
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
@@ -294,27 +325,25 @@
                 writer.add_scalar('Train/Loss', sum(loss_sum) / len(loss_sum), self.train_step)
                 writer.add_scalar('Train/Accuracy', (sum(accuracies) / len(accuracies)), self.train_step)
                 # 记录学习率
                 writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], self.train_step)
                 train_times = []
                 self.train_step += 1
             start = time.time()
-        self.scheduler.step()
+            self.scheduler.step()
 
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
         # 获取有多少张显卡训练
         nranks = torch.cuda.device_count()
         local_rank = 0
         writer = None
         if local_rank == 0:
             # 日志记录器
@@ -322,15 +351,15 @@
 
         if nranks > 1 and self.use_gpu:
             # 初始化NCCL环境
             dist.init_process_group(backend='nccl')
             local_rank = int(os.environ["LOCAL_RANK"])
 
         # 获取数据
-        self.__setup_dataloader(augment_conf_path=augment_conf_path, is_train=True)
+        self.__setup_dataloader(is_train=True)
         # 获取模型
         self.__setup_model(input_size=self.audio_featurizer.feature_dim, is_train=True)
 
         # 支持多卡训练
         if nranks > 1 and self.use_gpu:
             self.model.to(local_rank)
             self.audio_featurizer.to(local_rank)
@@ -350,15 +379,15 @@
             epoch_id += 1
             start_epoch = time.time()
             # 训练一个epoch
             self.__train_epoch(epoch_id=epoch_id, local_rank=local_rank, writer=writer, nranks=nranks)
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
@@ -366,86 +395,86 @@
                 if acc >= best_acc:
                     best_acc = acc
                     self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=acc,
                                            best_model=True)
                 # 保存模型
                 self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=acc)
 
-    def evaluate(self, resume_model='models/EcapaTdnn_MelSpectrogram/best_model/', save_matrix_path=None):
+    def evaluate(self, resume_model=None, save_matrix_path=None):
         """
         评估模型
         :param resume_model: 所使用的模型
         :param save_matrix_path: 保存混合矩阵的路径
         :return: 评估结果
         """
         if self.test_loader is None:
             self.__setup_dataloader()
         if self.model is None:
             self.__setup_model(input_size=self.audio_featurizer.feature_dim)
         if resume_model is not None:
             if os.path.isdir(resume_model):
-                resume_model = os.path.join(resume_model, 'model.pt')
+                resume_model = os.path.join(resume_model, 'model.pth')
             assert os.path.exists(resume_model), f"{resume_model} 模型不存在！"
             model_state_dict = torch.load(resume_model)
             self.model.load_state_dict(model_state_dict)
             logger.info(f'成功加载模型：{resume_model}')
         self.model.eval()
         if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
             eval_model = self.model.module
         else:
             eval_model = self.model
 
         accuracies, losses, preds, labels = [], [], [], []
         with torch.no_grad():
-            for batch_id, (audio, label) in enumerate(tqdm(self.test_loader)):
+            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.test_loader)):
                 audio = audio.to(self.device)
+                input_lens_ratio = input_lens_ratio.to(self.device)
                 label = label.to(self.device).long()
-                features = self.audio_featurizer(audio)
+                features, _ = self.audio_featurizer(audio, input_lens_ratio)
                 output = eval_model(features)
                 los = self.loss(output, label)
+                # 计算准确率
+                acc = accuracy(output, label)
+                accuracies.append(acc)
+                # 模型预测标签
                 label = label.data.cpu().numpy()
                 output = output.data.cpu().numpy()
-                # 模型预测标签
                 pred = np.argmax(output, axis=1)
                 preds.extend(pred.tolist())
                 # 真实标签
                 labels.extend(label.tolist())
-
-                # 计算准确率
-                acc = np.mean((pred == label).astype(int))
-                accuracies.append(acc)
                 losses.append(los.data.cpu().numpy())
         loss = float(sum(losses) / len(losses))
         acc = float(sum(accuracies) / len(accuracies))
         # 保存混合矩阵
         if save_matrix_path is not None:
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
         self.__setup_model(input_size=self.audio_featurizer.feature_dim)
         # 加载预训练模型
         if os.path.isdir(resume_model):
-            resume_model = os.path.join(resume_model, 'model.pt')
+            resume_model = os.path.join(resume_model, 'model.pth')
         assert os.path.exists(resume_model), f"{resume_model} 模型不存在！"
         model_state_dict = torch.load(resume_model)
         self.model.load_state_dict(model_state_dict)
         logger.info('成功恢复模型参数和优化方法参数：{}'.format(resume_model))
         self.model.eval()
         # 获取静态模型
         infer_model = self.model.export()
         infer_model_path = os.path.join(save_model_path,
                                         f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
-                                        'inference.pt')
+                                        'inference.pth')
         os.makedirs(os.path.dirname(infer_model_path), exist_ok=True)
         torch.jit.save(infer_model, infer_model_path)
         logger.info("预测模型已保存：{}".format(infer_model_path))
```

## macls/data_utils/audio.py

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

## macls/data_utils/featurizer.py

```diff
@@ -1,65 +1,95 @@
 import torch
 from torch import nn
+import torchaudio.compliance.kaldi as Kaldi
 from torchaudio.transforms import MelSpectrogram, Spectrogram, MFCC
 
 
 class AudioFeaturizer(nn.Module):
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
         if feature_method == 'MelSpectrogram':
-            self.feat_fun = MelSpectrogram(**feature_conf)
+            self.feat_fun = MelSpectrogram(**method_args)
         elif feature_method == 'Spectrogram':
-            self.feat_fun = Spectrogram(**feature_conf)
+            self.feat_fun = Spectrogram(**method_args)
         elif feature_method == 'MFCC':
-            melkwargs = feature_conf.copy()
-            del melkwargs['sample_rate']
-            del melkwargs['n_mfcc']
-            self.feat_fun = MFCC(sample_rate=self._feature_conf.sample_rate,
-                                 n_mfcc=self._feature_conf.n_mfcc,
-                                 melkwargs=melkwargs)
+            self.feat_fun = MFCC(**method_args)
+        elif feature_method == 'Fbank':
+            self.feat_fun = KaldiFbank(**method_args)
         else:
             raise Exception(f'预处理方法 {self._feature_method} 不存在!')
 
-    def forward(self, waveforms):
-        """从音频中提取音频特征
+    def forward(self, waveforms, input_lens_ratio):
+        """从AudioSegment中提取音频特征
 
-        :param waveforms: Audio to extract features from.
-        :type waveforms: ndarray
+        :param waveforms: Audio segment to extract features from.
+        :type waveforms: AudioSegment
+        :param input_lens_ratio: input length ratio
+        :type input_lens_ratio: tensor
         :return: Spectrogram audio feature in 2darray.
         :rtype: ndarray
         """
         feature = self.feat_fun(waveforms)
         feature = feature.transpose(2, 1)
         # 归一化
-        mean = torch.mean(feature, 1, keepdim=True)
-        std = torch.std(feature, 1, keepdim=True)
-        feature = (feature - mean) / (std + 1e-5)
-        return feature
+        feature = feature - feature.mean(1, keepdim=True)
+        # 对掩码比例进行扩展
+        input_lens = (input_lens_ratio * feature.shape[1])
+        mask_lens = torch.round(input_lens).long()
+        mask_lens = mask_lens.unsqueeze(1)
+        input_lens = input_lens.int()
+        # 生成掩码张量
+        idxs = torch.arange(feature.shape[1], device=feature.device).repeat(feature.shape[0], 1)
+        mask = idxs < mask_lens
+        mask = mask.unsqueeze(-1)
+        # 对特征进行掩码操作
+        feature_masked = torch.where(mask, feature, torch.zeros_like(feature))
+        return feature_masked, input_lens
 
     @property
     def feature_dim(self):
         """返回特征大小
 
         :return: 特征大小
         :rtype: int
         """
-        if self._feature_method == 'LogMelSpectrogram':
-            return self._feature_conf.n_mels
-        elif self._feature_method == 'MelSpectrogram':
-            return self._feature_conf.n_mels
+        if self._feature_method == 'MelSpectrogram':
+            return self._method_args.get('n_mels', 128)
         elif self._feature_method == 'Spectrogram':
-            return self._feature_conf.n_fft // 2 + 1
+            return self._method_args.get('n_fft', 400) // 2 + 1
         elif self._feature_method == 'MFCC':
-            return self._feature_conf.n_mfcc
+            return self._method_args.get('n_mfcc', 40)
+        elif self._feature_method == 'Fbank':
+            return self._method_args.get('num_mel_bins', 23)
         else:
             raise Exception('没有{}预处理方法'.format(self._feature_method))
+
+
+class KaldiFbank(nn.Module):
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
+            log_fbank = log_fbank.transpose(0, 1)
+            log_fbanks.append(log_fbank)
+        log_fbank = torch.stack(log_fbanks)
+        return log_fbank
```

## macls/data_utils/reader.py

```diff
@@ -1,66 +1,126 @@
+import os
+import random
+
 import numpy as np
 from torch.utils.data import Dataset
 
 from macls.data_utils.audio import AudioSegment
-from macls.data_utils.augmentor.augmentation import AugmentationPipeline
 from macls.utils.logger import setup_logger
 
 logger = setup_logger(__name__)
 
 
-# 音频数据加载器
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
+                 num_speakers=1000,
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
+            num_speakers: 总说话人数量
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
+        self.num_speakers = num_speakers
+        self.noises_path = None
         # 获取数据列表
-        with open(data_list_path, 'r') as f:
+        with open(data_list_path, 'r', encoding='utf-8') as f:
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
-                return self.__getitem__(idx+1 if idx < len(self.lines) - 1 else 0)
+            if audio_segment.duration < self.min_duration:
+                return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
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

## macls/data_utils/utils.py

```diff
@@ -1,13 +1,14 @@
 import io
 import itertools
 
 import av
 import librosa
 import numpy as np
+import torch
 
 
 def vad(wav, top_db=20, overlap=200):
     # Split an audio signal into non-silent intervals
     intervals = librosa.effects.split(wav, top_db=top_db)
     if len(intervals) == 0:
         return wav
@@ -78,28 +79,41 @@
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
 
@@ -143,7 +157,36 @@
     scale = 1.0 / float(1 << ((8 * n_bytes) - 1))
 
     # Construct the format string
     fmt = "<i{:d}".format(n_bytes)
 
     # Rescale and format the data buffer
     return scale * np.frombuffer(x, fmt).astype(dtype)
+
+
+def make_pad_mask(lengths: torch.Tensor, max_len: int = 0) -> torch.Tensor:
+    """Make mask tensor containing indices of padded part.
+
+    See description of make_non_pad_mask.
+
+    Args:
+        lengths (torch.Tensor): Batch of lengths (B,).
+    Returns:
+        torch.Tensor: Mask tensor containing indices of padded part.
+
+    Examples:
+        >>> lengths = [5, 3, 2]
+        >>> make_pad_mask(lengths)
+        masks = [[0, 0, 0, 0 ,0],
+                 [0, 0, 0, 1, 1],
+                 [0, 0, 1, 1, 1]]
+    """
+    batch_size = lengths.size(0)
+    max_len = max_len if max_len > 0 else lengths.max().item()
+    seq_range = torch.arange(0,
+                             max_len,
+                             dtype=torch.int64,
+                             device=lengths.device)
+    seq_range_expand = seq_range.unsqueeze(0).expand(batch_size, max_len)
+    seq_length_expand = lengths.unsqueeze(-1)
+    mask = seq_range_expand >= seq_length_expand
+    return mask
```

## macls/utils/record.py

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

## Comparing `macls-0.3.5.dist-info/LICENSE` & `macls-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `macls-0.3.5.dist-info/RECORD` & `macls-0.4.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-macls/__init__.py,sha256=VLx9wNuBj0wRvc9G4VOHIKpm4iiFYNufPdWO6SIPP-Q,131
-macls/predict.py,sha256=qUuakcBkIcE25oSgm7CNq7Amsc3vnM_fq15ytySYbCo,8422
-macls/trainer.py,sha256=1B1K68LqO7HJ37v61PQEyaIHVsgmCKFCCgK882UDtS0,24545
+macls/__init__.py,sha256=wikLtyqyBTLDjLAsamssDRQMEC8AOKbTbzBPIOlatIM,154
+macls/predict.py,sha256=JNpmpAGM3ln08WeWBpVisSk6eK7GvOmB4Po_cU-yU5w,8970
+macls/trainer.py,sha256=uWL3tDOpMSeYbxKUMKulOGvbBGP4hDmy3JrQTlQetBw,26413
 macls/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-macls/data_utils/audio.py,sha256=cG8Jl_fFefOiAQr6NjFmtql-qiQPZxv2uDjAuvWqFAk,22813
-macls/data_utils/featurizer.py,sha256=Qh33BnL7sEMiQV9XJQqdQd4RvU6OP-oDIj1NlYdRXNY,2420
-macls/data_utils/reader.py,sha256=sWvKllizJH1hpsOG3gYub96WlVhPCz-CBFnkq-EE4fQ,2815
-macls/data_utils/utils.py,sha256=U81Q-hmPQDUK_yc-opzOb8G28dgEWqnOq5ej3jSrk7w,4337
-macls/data_utils/augmentor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-macls/data_utils/augmentor/augmentation.py,sha256=os_R4BVejMnBKn2Ap7qLpvezLK5ub8vKigV6AOwKvqs,5517
-macls/data_utils/augmentor/base.py,sha256=Qw5AsIjpqDkggVkVyfPGTI_IwnfSuIWViRdgo7g2ze0,965
-macls/data_utils/augmentor/noise_perturb.py,sha256=xzPQqUR31RNAv5gfNDR68C9XS1ONQaOTsH51NwjvvUg,2024
-macls/data_utils/augmentor/resample.py,sha256=DDhbg3_K4iWS8xuyojvluq_MgNsztjrQi_gEyBFJjKw,977
-macls/data_utils/augmentor/shift_perturb.py,sha256=3LdylfnoVdOqU5YO2Qca3ouhFcwSmuEZk0U-0S9Lm6w,1007
-macls/data_utils/augmentor/spec_augment.py,sha256=Eg1i0v4JVZYc8Sg7ezGobGvQZd44c6tq-0UjOus0CK4,5015
-macls/data_utils/augmentor/spec_sub.py,sha256=sPa5Jvbrhl5zHycSU_wPWkKnyQ2u0JgSOmhWO7ACdJ4,1138
-macls/data_utils/augmentor/speed_perturb.py,sha256=taz1RKZyEQYmCCtJSGZorhKxxeek6FwNdoBqaQBGHy8,1978
-macls/data_utils/augmentor/volume_perturb.py,sha256=-QKbLIp0FleJE4A0ttnRq6MKCqedGhbO6Wb5kBSXUj4,1138
+macls/data_utils/audio.py,sha256=xJWwFXKrtitU7GZZuNmqmXPsq1Bzj-qnYd49naBvVyo,22287
+macls/data_utils/collate_fn.py,sha256=GxqMcZ5Q2ScQxj6crIUWeVygzWxIk9KAbC6GWW6awrQ,965
+macls/data_utils/featurizer.py,sha256=-MAiHLattWuHK7fa4Wr1-7Jqw_AqKuY7hr-73nEqPBk,3587
+macls/data_utils/reader.py,sha256=3wJw3iQum199U2n2CVxWd400e1OUTbyrcO2Ib8YJru4,5640
+macls/data_utils/spec_aug.py,sha256=Sr9-Ss6I7LA3TGMqzML_X-nb_nnMfUxt5KbsA6HJpzM,1572
+macls/data_utils/utils.py,sha256=mNpCY4PcaeKCSjEB6gQWsiyUBRNDvwrY9YizFTRuaww,5652
+macls/metric/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+macls/metric/metrics.py,sha256=Asj6VaDQXxmcB_HRIJt7v4zdRBgLTyn3Q2mDTFPcgEM,329
 macls/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 macls/models/ecapa_tdnn.py,sha256=IGF30mt5io03N666qpOtwh34e0pFDWj6Y2h_JJ6XKzo,5378
 macls/models/panns.py,sha256=Ylg4O5TDv3BoPn5v0HXZD0wASdy9jAvhvTTP9FWDPpo,9707
 macls/models/pooling.py,sha256=z-1Go_Yhiy8FJoaq_UT0lmFYS92qvvMmntmc2AEh-Kk,3000
 macls/models/res2net.py,sha256=70ctRGC6_lZpqkxRU1ZzluOTci4VV_Csqpk6Ns87bcI,6680
 macls/models/resnet_se.py,sha256=qM1YKhrJTWEYQUQ4nP_Awg8YETws2NZRVZlP8UsAUr4,6585
 macls/models/tdnn.py,sha256=foMiLbpQ4loRuo-2G31J6yCRq8ZSu48BSpx7OUy4M50,3050
 macls/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 macls/utils/logger.py,sha256=-ssorx8FlHA_wrd2Eq6f4HkOqaOG2YseBGvYAo8NXN8,2839
-macls/utils/record.py,sha256=GIX3fU9oyIIDmM59TPQ7w1bLOH6JYxMddlW4Hk9fqQA,1594
+macls/utils/record.py,sha256=2i4kz5kPDa9KkbAK_Q34sVIXOkD9TroPROIe5QdzqWg,1067
+macls/utils/scheduler.py,sha256=RXgRf_sntkOjruj30pp6uPE7dqFR06jDa4tRogpl5Us,1496
 macls/utils/utils.py,sha256=-KEdKJYlZ9q3Cjb0re1bNMf3ZVCi6EmpDydGYM9BuJU,3364
-macls-0.3.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-macls-0.3.5.dist-info/METADATA,sha256=K9V2YHdkFvovEroSfMgObolnIJBWVp2oivCkojhrAtA,6487
-macls-0.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-macls-0.3.5.dist-info/top_level.txt,sha256=fmi1Rmptc1CNX_eoWedGPlbhlTSDi3liMSfVFvHYE1Q,6
-macls-0.3.5.dist-info/RECORD,,
+macls-0.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+macls-0.4.0.dist-info/METADATA,sha256=_V4TD7-f_CsM6FOz6MGW7ajXjtEq5mn8OkC_oCakBMs,17396
+macls-0.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+macls-0.4.0.dist-info/top_level.txt,sha256=fmi1Rmptc1CNX_eoWedGPlbhlTSDi3liMSfVFvHYE1Q,6
+macls-0.4.0.dist-info/RECORD,,
```

