# Comparing `tmp/AudioLoader-0.1.3.tar.gz` & `tmp/AudioLoader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AudioLoader-0.1.3.tar", last modified: Wed Oct 26 11:52:36 2022, max compression
+gzip compressed data, was "AudioLoader-0.1.4.tar", last modified: Tue Aug  8 09:54:34 2023, max compression
```

## Comparing `AudioLoader-0.1.3.tar` & `AudioLoader-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.409154 AudioLoader-0.1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.357154 AudioLoader-0.1.3/AudioLoader/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-26 11:51:52.000000 AudioLoader-0.1.3/AudioLoader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.373154 AudioLoader-0.1.3/AudioLoader/music/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/music/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45837 2022-10-26 11:31:16.000000 AudioLoader-0.1.3/AudioLoader/music/amt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.389154 AudioLoader-0.1.3/AudioLoader/music/mss/
--rw-r--r--   0 root         (0) root         (0)       61 2022-05-06 04:47:40.000000 AudioLoader-0.1.3/AudioLoader/music/mss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6082 2022-05-06 04:27:48.000000 AudioLoader-0.1.3/AudioLoader/music/mss/fastmusdb.py
--rw-r--r--   0 root         (0) root         (0)    13674 2022-09-03 05:23:42.000000 AudioLoader-0.1.3/AudioLoader/music/mss/musdbhq.py
--rw-r--r--   0 root         (0) root         (0)      972 2022-09-03 07:00:34.000000 AudioLoader-0.1.3/AudioLoader/music/overlapping.pkl
--rw-r--r--   0 root         (0) root         (0)     5914 2022-10-26 07:18:02.000000 AudioLoader-0.1.3/AudioLoader/music/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.409154 AudioLoader-0.1.3/AudioLoader/speech/
--rw-r--r--   0 root         (0) root         (0)      112 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19472 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/speech/mls.py
--rw-r--r--   0 root         (0) root         (0)     9468 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/speech/speechcommands.py
--rw-r--r--   0 root         (0) root         (0)     7568 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/speech/timit.py
--rw-r--r--   0 root         (0) root         (0)     2165 2022-06-29 06:23:41.000000 AudioLoader-0.1.3/AudioLoader/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 11:52:36.373154 AudioLoader-0.1.3/AudioLoader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1906 2022-10-26 11:52:36.000000 AudioLoader-0.1.3/AudioLoader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      555 2022-10-26 11:52:36.000000 AudioLoader-0.1.3/AudioLoader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-26 11:52:36.000000 AudioLoader-0.1.3/AudioLoader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-10-26 11:52:36.000000 AudioLoader-0.1.3/AudioLoader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-09-03 08:47:12.000000 AudioLoader-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1906 2022-10-26 11:52:36.409154 AudioLoader-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1410 2022-06-29 06:31:09.000000 AudioLoader-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-26 11:52:36.409154 AudioLoader-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1298 2022-09-03 08:35:46.000000 AudioLoader-0.1.3/setup.py
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/AudioLoader/
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)       21 2023-08-08 09:50:46.000000 AudioLoader-0.1.4/AudioLoader/__init__.py
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/AudioLoader/music/
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/__init__.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    45842 2023-08-08 09:11:57.000000 AudioLoader-0.1.4/AudioLoader/music/amt.py
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/AudioLoader/music/mss/
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     1930 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/MIDI_program_map.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)       96 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/__init__.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     6001 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/fastmusdb.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     1237 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/moisedb23_preprocessing.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     9831 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/moisesdb23.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    13676 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/musdbhq.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    28164 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/slakh.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    12930 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/mss/utils.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)      972 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/overlapping.pkl
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     5914 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/music/utils.py
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/AudioLoader/speech/
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)      112 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/speech/__init__.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    19472 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/speech/mls.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)    10080 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/speech/speechcommands.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     7568 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/speech/timit.py
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     8400 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/AudioLoader/utils.py
+drwxrwxr-x   0 kinwai    (1013) kinwai    (1013)        0 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/AudioLoader.egg-info/
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     2558 2023-08-08 09:54:34.000000 AudioLoader-0.1.4/AudioLoader.egg-info/PKG-INFO
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)      744 2023-08-08 09:54:34.000000 AudioLoader-0.1.4/AudioLoader.egg-info/SOURCES.txt
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)        1 2023-08-08 09:54:34.000000 AudioLoader-0.1.4/AudioLoader.egg-info/dependency_links.txt
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)       12 2023-08-08 09:54:34.000000 AudioLoader-0.1.4/AudioLoader.egg-info/top_level.txt
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)       42 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/MANIFEST.in
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     2558 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/PKG-INFO
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     2062 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/README.md
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)       38 2023-08-08 09:54:34.437853 AudioLoader-0.1.4/setup.cfg
+-rw-rw-r--   0 kinwai    (1013) kinwai    (1013)     1298 2023-08-08 09:01:17.000000 AudioLoader-0.1.4/setup.py
```

### Comparing `AudioLoader-0.1.3/AudioLoader/music/amt.py` & `AudioLoader-0.1.4/AudioLoader/music/amt.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         self.ext_archive = '.zip'
         self.name_archive = 'MAPS'
         self.original_ext = '.wav'        
         self.data_type = data_type
         self.sampling_rate = sampling_rate
         self.dataset = 'MAPS'
              
-        self.groups = groups if isinstance(groups, list) else self.available_groups(groups)
+        self.groups = self.available_groups(groups) if isinstance(groups, str) else list(groups)
         
         print(f"========={self.download=}=========")
         if self.download:
             # Check if MAPS folder exists
             if not os.path.isdir(os.path.join(root, self.name_archive)):
                 os.makedirs(os.path.join(root, self.name_archive))
```

### Comparing `AudioLoader-0.1.3/AudioLoader/music/mss/fastmusdb.py` & `AudioLoader-0.1.4/AudioLoader/music/mss/fastmusdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 # import soundfile
 from tqdm import tqdm
 import torch
 import torch.nn.functional as F
 from torch.utils.data import Dataset
 import torchaudio
 import hashlib
-from torchaudio.datasets.utils import (
-    download_url,
-    extract_archive,
-)
 
 from collections import OrderedDict
 import math
 
 class FastMUSDB(Dataset):
     def __init__(self,
                  root=None,
```

### Comparing `AudioLoader-0.1.3/AudioLoader/music/mss/musdbhq.py` & `AudioLoader-0.1.4/AudioLoader/music/mss/musdbhq.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 import musdb
 import torch
 import torch.nn.functional as F
 from torch.utils.data import Dataset
 import torchaudio
 from torchaudio.compliance import kaldi # for downsampling
 import hashlib
-from torchaudio.datasets.utils import (
+from AudioLoader.utils import (
     download_url,
     extract_archive,
 )
 
+
 from collections import OrderedDict
 import math
 
 metadata= './metadata'
 MIXTURE = 'mixture'
 EXT = '.wav'
 
@@ -53,14 +54,15 @@
             samplerate (int): target sample rate. if the file sample rate
                 is different, it will be resampled on the fly.
             channels (int): target nb of channels. if different, will be
                 changed onthe fly.
             ext (str): extension for audio files (default is .wav).
         samplerate and channels are converted on the fly.
         """
+        
  
          # Getting audio path
         ext_archive = '.zip'
         archive_name = 'musdb18hq'
 
         download_path = Path(root)
         self.download_path = download_path
```

### Comparing `AudioLoader-0.1.3/AudioLoader/music/overlapping.pkl` & `AudioLoader-0.1.4/AudioLoader/music/overlapping.pkl`

 * *Files identical despite different names*

### Comparing `AudioLoader-0.1.3/AudioLoader/music/utils.py` & `AudioLoader-0.1.4/AudioLoader/music/utils.py`

 * *Files identical despite different names*

### Comparing `AudioLoader-0.1.3/AudioLoader/speech/mls.py` & `AudioLoader-0.1.4/AudioLoader/speech/mls.py`

 * *Files identical despite different names*

### Comparing `AudioLoader-0.1.3/AudioLoader/speech/speechcommands.py` & `AudioLoader-0.1.4/AudioLoader/speech/speechcommands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 from torch.utils.data import Dataset
 import torchaudio
 from pathlib import Path
-from typing import Tuple, Union
+from typing import Tuple, Optional, Callable, Any
 from torch import Tensor
-import torch
 import os
-import time
 import tqdm
-import shutil
-import glob
-import multiprocessing as mp
-import warnings
-from distutils.dir_util import copy_tree
-from torchaudio.compliance import kaldi # for downsampling
 from torchaudio.datasets.utils import (
     download_url,
     extract_archive,
 )
-import hashlib
 import torch.nn.functional as F            
 
 #start for speechcommands 12 classes code
 SAMPLE_RATE = 16000
 FOLDER_IN_ARCHIVE = "SpeechCommands"
 URL = "speech_commands_v0.02"
 HASH_DIVIDER = "_nohash_"
@@ -139,30 +130,30 @@
             audio_samples = F.pad(audio_samples, (0,pad_length)) # pad the end of the audio until 1 second
             # (1, 16000)
         cache.append((audio_samples, rate, name2idx[label], speaker_id, utterance_number)) 
     
     
     # include silence
     if subset=='training':
-        slience_clips = [
+        silence_clips = [
             'dude_miaowing.wav',
             'white_noise.wav',
             'exercise_bike.wav',
             'doing_the_dishes.wav',
             'pink_noise.wav'
         ]
     elif subset=='validation':
-        slience_clips = [
+        silence_clips = [
             'running_tap.wav'
         ]
     else:
-        slience_clips = []
+        silence_clips = []
         
         
-    for i in slience_clips: 
+    for i in silence_clips: 
         audio_samples, rate = torchaudio.load(os.path.join(path, '_background_noise_', i))
         for start in range(0,
                            audio_samples.shape[1] - SAMPLE_RATE,
                            SAMPLE_RATE//2):
             audio_segment = audio_samples[0, start:start + SAMPLE_RATE]
             cache.append((audio_segment.unsqueeze(0), rate, name2idx['_silence_'], '00000000', -1))        
         
@@ -183,22 +174,28 @@
         subset (str or None, optional):
             Select a subset of the dataset [None, "training", "validation", "testing"]. None means
             the whole dataset. "validation" and "testing" are defined in "validation_list.txt" and
             "testing_list.txt", respectively, and "training" is the rest. Details for the files
             "validation_list.txt" and "testing_list.txt" are explained in the README of the dataset
             and in the introduction of Section 7 of the original paper and its reference 12. The
             original paper can be found `here <https://arxiv.org/pdf/1804.03209.pdf>`_. (Default: ``None``)
+        transform (callable, optional): A function/transform that takes in an a torch Tensor of audio and
+            returns a transformed version.
+        target_transform (callable, optional): A function/transform that takes in the target (sample_rate,
+            label, speaker_id, utterance_number) and transforms it
     """
 
     def __init__(self,
-                 root,
-                 url,
-                 folder_in_archive,
-                 download,
-                 subset,
+                 root: str,
+                 url: str,
+                 folder_in_archive: str,
+                 download: bool,
+                 subset: str,
+                 transform: Optional[Callable[[Tensor], Any]] = None,
+                 target_transform: Optional[Callable[[int, str, str, int], Any]] = None,
                  ):
 
         assert subset is None or subset in ["training", "validation", "testing"], (
             "When `subset` not None, it must take a value from "
             + "{'training', 'validation', 'testing'}."
         )
 
@@ -249,24 +246,32 @@
             ]
             self._data = caching_data(self._walker, self._path, subset)
             
         else:
             walker = sorted(str(p) for p in Path(self._path).glob('*/*.wav'))
             self._walker = [w for w in walker if HASH_DIVIDER in w and EXCEPT_FOLDER not in w]
 
-    def __getitem__(self, n: int) -> Tuple[Tensor, int, str, str, int]:
+        self.transform = transform
+        self.target_transform = target_transform
+
+    def __getitem__(self, n: int) -> Tuple[Any, Any]:
         """Load the n-th sample from the dataset.
         Args:
             n (int): The index of the sample to be loaded
         Returns:
-            (Tensor, int, str, str, int):
-            ``(waveform, sample_rate, label, speaker_id, utterance_number)``
+            (Any, Any): (transformed) waveform and corresponding (transformed) label
         """
-        return self._data[n]
-
+        data = self._data[n]
 
-    def __len__(self) -> int:
-        return len(self._data)       
+        waveform = data[0]
+        label = data[1:]
 
+        if self.transform is not None:
+            waveform = self.transform(waveform)
 
+        if self.target_transform is not None:
+            label = self.target_transform(*label)
 
+        return waveform, label
 
+    def __len__(self) -> int:
+        return len(self._data)
```

### Comparing `AudioLoader-0.1.3/AudioLoader/speech/timit.py` & `AudioLoader-0.1.4/AudioLoader/speech/timit.py`

 * *Files identical despite different names*

### Comparing `AudioLoader-0.1.3/AudioLoader.egg-info/PKG-INFO` & `AudioLoader-0.1.4/AudioLoader.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 Metadata-Version: 2.1
 Name: AudioLoader
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of PyTorch audio datasets for speech and music applications
 Home-page: https://github.com/KinWaiCheuk/AudioLoader
 Author: KinWaiCheuk
 Author-email: u3500684@connect.hku.hk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # AudioLoader
-This will be a collection of PyTorch audio dataset loaders that are not available in the official PyTorch dataset and torchaudio dataset yet. I am building various one-click-ready audio datasets for my research, and I hope it will also benefit other people. 
+AudioLoader is a PyTorch dataset based on [torchaudio](https://pytorch.org/audio/stable/datasets.html). It contains a collection of datasets that are not available in [torchaudio](https://pytorch.org/audio/stable/datasets.html) yet.
 
 **Currently supported datasets:**
 1. [Speech](./AudioLoader/speech/speech_README.md#Speech)
     1. [Multilingual LibriSpeech (MLS)](./AudioLoader/speech/speech_README.md#Multilingual-LibriSpeech)
     1. [TIMIT](./AudioLoader/speech/speech_README.md#TIMIT)
     1. [SpeechCommands v2 (12 classes)](./AudioLoader/speech/speech_README.md#SpeechCommandsv2)
 1. [Automatic Music Transcription (AMT)](./AudioLoader/music/amt_README.md#Automatic-Music-Transcription)
     1. [MAPS](./AudioLoader/music/amt_README.md#maps)
     1. [MusicNet](./AudioLoader/music/amt_README.md#musicnet)
     1. [MAESTRO](./AudioLoader/music/amt_README.md#maestro)
 1. [Music Source Separation (MSS)](./AudioLoader/music/mss/mss_README.md#Music-Source-Separation)
     1. [FastMUSDB](./AudioLoader/music/mss/mss_README.md#FastMUSDB)
     1. [MusdbHQ](./AudioLoader/music/mss/mss_README.md#MusdbHQ)
+    
+## Example code
+A complete example code is available in this [repository](https://github.com/KinWaiCheuk/pytorch_template). The following pseudo  code shows the general idea of how to apply AudioLoader to your existing code.
+
+```python
+from AudioLoader.speech import TIMIT
+from torch.utils.data import DataLoader
+
+# AudioLoader helps you to set up supported datasets
+dataset = TIMIT('./YourFolder',
+                split='train',
+                groups='all',
+                download=True)
+train_loader = DataLoader(dataset,
+                          batch_size=4)
+
+# Pass the dataset to you 
+model = MyModel()
+trainer = pl.Trainer()
+trainer.fit(model, train_loader)
+
+```
 
 ## Installation
 `pip install git+https://github.com/KinWaiCheuk/AudioLoader.git`
 
 ## News & Changelog
 **version 0.0.3** (10 Sep 2021): 
 1. Replace broken links with a working links for `MAPS` and `TIMIT`
```

### Comparing `AudioLoader-0.1.3/AudioLoader.egg-info/SOURCES.txt` & `AudioLoader-0.1.4/AudioLoader.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 AudioLoader.egg-info/SOURCES.txt
 AudioLoader.egg-info/dependency_links.txt
 AudioLoader.egg-info/top_level.txt
 AudioLoader/music/__init__.py
 AudioLoader/music/amt.py
 AudioLoader/music/overlapping.pkl
 AudioLoader/music/utils.py
+AudioLoader/music/mss/MIDI_program_map.py
 AudioLoader/music/mss/__init__.py
 AudioLoader/music/mss/fastmusdb.py
+AudioLoader/music/mss/moisedb23_preprocessing.py
+AudioLoader/music/mss/moisesdb23.py
 AudioLoader/music/mss/musdbhq.py
+AudioLoader/music/mss/slakh.py
+AudioLoader/music/mss/utils.py
 AudioLoader/speech/__init__.py
 AudioLoader/speech/mls.py
 AudioLoader/speech/speechcommands.py
 AudioLoader/speech/timit.py
```

### Comparing `AudioLoader-0.1.3/PKG-INFO` & `AudioLoader-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 Metadata-Version: 2.1
 Name: AudioLoader
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of PyTorch audio datasets for speech and music applications
 Home-page: https://github.com/KinWaiCheuk/AudioLoader
 Author: KinWaiCheuk
 Author-email: u3500684@connect.hku.hk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # AudioLoader
-This will be a collection of PyTorch audio dataset loaders that are not available in the official PyTorch dataset and torchaudio dataset yet. I am building various one-click-ready audio datasets for my research, and I hope it will also benefit other people. 
+AudioLoader is a PyTorch dataset based on [torchaudio](https://pytorch.org/audio/stable/datasets.html). It contains a collection of datasets that are not available in [torchaudio](https://pytorch.org/audio/stable/datasets.html) yet.
 
 **Currently supported datasets:**
 1. [Speech](./AudioLoader/speech/speech_README.md#Speech)
     1. [Multilingual LibriSpeech (MLS)](./AudioLoader/speech/speech_README.md#Multilingual-LibriSpeech)
     1. [TIMIT](./AudioLoader/speech/speech_README.md#TIMIT)
     1. [SpeechCommands v2 (12 classes)](./AudioLoader/speech/speech_README.md#SpeechCommandsv2)
 1. [Automatic Music Transcription (AMT)](./AudioLoader/music/amt_README.md#Automatic-Music-Transcription)
     1. [MAPS](./AudioLoader/music/amt_README.md#maps)
     1. [MusicNet](./AudioLoader/music/amt_README.md#musicnet)
     1. [MAESTRO](./AudioLoader/music/amt_README.md#maestro)
 1. [Music Source Separation (MSS)](./AudioLoader/music/mss/mss_README.md#Music-Source-Separation)
     1. [FastMUSDB](./AudioLoader/music/mss/mss_README.md#FastMUSDB)
     1. [MusdbHQ](./AudioLoader/music/mss/mss_README.md#MusdbHQ)
+    
+## Example code
+A complete example code is available in this [repository](https://github.com/KinWaiCheuk/pytorch_template). The following pseudo  code shows the general idea of how to apply AudioLoader to your existing code.
+
+```python
+from AudioLoader.speech import TIMIT
+from torch.utils.data import DataLoader
+
+# AudioLoader helps you to set up supported datasets
+dataset = TIMIT('./YourFolder',
+                split='train',
+                groups='all',
+                download=True)
+train_loader = DataLoader(dataset,
+                          batch_size=4)
+
+# Pass the dataset to you 
+model = MyModel()
+trainer = pl.Trainer()
+trainer.fit(model, train_loader)
+
+```
 
 ## Installation
 `pip install git+https://github.com/KinWaiCheuk/AudioLoader.git`
 
 ## News & Changelog
 **version 0.0.3** (10 Sep 2021): 
 1. Replace broken links with a working links for `MAPS` and `TIMIT`
```

### Comparing `AudioLoader-0.1.3/setup.py` & `AudioLoader-0.1.4/setup.py`

 * *Files identical despite different names*

