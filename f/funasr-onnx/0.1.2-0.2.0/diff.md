# Comparing `tmp/funasr_onnx-0.1.2.tar.gz` & `tmp/funasr_onnx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr_onnx-0.1.2.tar", last modified: Thu Jul  6 08:03:22 2023, max compression
+gzip compressed data, was "funasr_onnx-0.2.0.tar", last modified: Tue Aug  8 14:03:35 2023, max compression
```

## Comparing `funasr_onnx-0.1.2.tar` & `funasr_onnx-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.243365 funasr_onnx-0.1.2/
--rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-07-06 08:03:22.243059 funasr_onnx-0.1.2/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     8039 2023-05-12 03:33:34.000000 funasr_onnx-0.1.2/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.238876 funasr_onnx-0.1.2/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.1.2/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr_onnx-0.1.2/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr_onnx-0.1.2/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.242623 funasr_onnx-0.1.2/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.1.2/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr_onnx-0.1.2/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr_onnx-0.1.2/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr_onnx-0.1.2/funasr_onnx/vad_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.240099 funasr_onnx-0.1.2/funasr_onnx.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      103 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-06 08:03:22.243437 funasr_onnx-0.1.2/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr_onnx-0.1.2/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:03:35.651335 funasr_onnx-0.2.0/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-08-08 14:03:35.651026 funasr_onnx-0.2.0/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     8039 2023-05-12 03:33:34.000000 funasr_onnx-0.2.0/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:03:35.647430 funasr_onnx-0.2.0/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.2.0/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr_onnx-0.2.0/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13639 2023-08-08 05:38:01.000000 funasr_onnx-0.2.0/funasr_onnx/paraformer_online_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13466 2023-07-26 06:54:17.000000 funasr_onnx-0.2.0/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:03:35.650621 funasr_onnx-0.2.0/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.2.0/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.2.0/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16830 2023-08-08 05:38:01.000000 funasr_onnx-0.2.0/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.2.0/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.2.0/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10989 2023-08-08 11:57:07.000000 funasr_onnx-0.2.0/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr_onnx-0.2.0/funasr_onnx/vad_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-08-08 14:03:35.648564 funasr_onnx-0.2.0/funasr_onnx.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-08-08 14:03:35.000000 funasr_onnx-0.2.0/funasr_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)      522 2023-08-08 14:03:35.000000 funasr_onnx-0.2.0/funasr_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-08-08 14:03:35.000000 funasr_onnx-0.2.0/funasr_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      103 2023-08-08 14:03:35.000000 funasr_onnx-0.2.0/funasr_onnx.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-08-08 14:03:35.000000 funasr_onnx-0.2.0/funasr_onnx.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-08-08 14:03:35.651408 funasr_onnx-0.2.0/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-08-08 14:03:25.000000 funasr_onnx-0.2.0/setup.py
```

### Comparing `funasr_onnx-0.1.2/PKG-INFO` & `funasr_onnx-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr_onnx
-Version: 0.1.2
+Version: 0.2.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.1.2/README.md` & `funasr_onnx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.2.0/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx/punc_bin.py` & `funasr_onnx-0.2.0/funasr_onnx/punc_bin.py`

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

### Comparing `funasr_onnx-0.1.2/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.2.0/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.2.0/funasr_onnx/utils/frontend.py`

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

### Comparing `funasr_onnx-0.1.2/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.2.0/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.2.0/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx/utils/utils.py` & `funasr_onnx-0.2.0/funasr_onnx/utils/utils.py`

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

### Comparing `funasr_onnx-0.1.2/funasr_onnx/vad_bin.py` & `funasr_onnx-0.2.0/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.2/funasr_onnx.egg-info/PKG-INFO` & `funasr_onnx-0.2.0/funasr_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr-onnx
-Version: 0.1.2
+Version: 0.2.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.1.2/setup.py` & `funasr_onnx-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.1.2'
+VERSION_NUM = '0.2.0'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
```

