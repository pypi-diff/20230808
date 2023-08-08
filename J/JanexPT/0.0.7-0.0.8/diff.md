# Comparing `tmp/JanexPT-0.0.7.tar.gz` & `tmp/JanexPT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.7.tar", last modified: Mon Aug  7 19:59:46 2023, max compression
+gzip compressed data, was "JanexPT-0.0.8.tar", last modified: Tue Aug  8 19:19:17 2023, max compression
```

## Comparing `JanexPT-0.0.7.tar` & `JanexPT-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.349858 JanexPT-0.0.7/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3861 2023-08-07 19:59:22.000000 JanexPT-0.0.7/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.7/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:59:46.353858 JanexPT-0.0.7/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 19:52:47.000000 JanexPT-0.0.7/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-07 19:59:46.353858 JanexPT-0.0.7/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-07 19:59:34.000000 JanexPT-0.0.7/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.409964 JanexPT-0.0.8/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4411 2023-08-07 22:19:53.000000 JanexPT-0.0.8/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-08 19:19:17.000000 JanexPT-0.0.8/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       17 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.8/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:19:17.425964 JanexPT-0.0.8/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 22:20:23.000000 JanexPT-0.0.8/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-08 19:19:17.425964 JanexPT-0.0.8/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1320 2023-08-08 19:19:09.000000 JanexPT-0.0.8/setup.py
```

### Comparing `JanexPT-0.0.7/JanexPT/main.py` & `JanexPT-0.0.8/JanexPT/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,22 @@
 import random
 import json
 
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset, DataLoader
 
+IM = IntentMatcher("intents.json", "thesaurus.json")
+
+def tokenize(sentence):
+    input_string = sentence
+    return IM.tokenize(input_string)
 
 def stem(word):
-    return stemmer.stem(word.lower())
+    return IM.stem(word.lower())
 
 def bag_of_words(tokenized_sentence, words):
     # stem each word
     sentence_words = [stem(word) for word in tokenized_sentence]
     # initialize bag with 0 for each word
     bag = np.zeros(len(words), dtype=np.float32)
     for idx, w in enumerate(words):
@@ -64,15 +69,25 @@
         return self.n_samples
 
 class JanexPT:
     def __init__(self, intents_file_path, thesaurus_file_path, UIName):
         self.intents_file_path = intents_file_path
         self.thesaurus_file_path = thesaurus_file_path
         self.FILE = "data.pth"
-        self.data = torch.load(self.FILE)
+        self.model = NeuralNet(self.input_size, self.hidden_size, self.output_size).to(self.device)
+        self.UIName = UIName
+        self.IntentMatcher = IntentMatcher(intents_file_path, thesaurus_file_path)
+        self.intents = self.IntentMatcher.train()
+
+    def SayToAI(self, input_string, user):
+        try:
+            self.data = torch.load(self.FILE)
+        except:
+            self.trainpt()
+            self.data = torch.load(self.FILE)
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.input_size = self.data["input_size"]
         self.hidden_size = self.data["hidden_size"]
         self.output_size = self.data["output_size"]
         self.all_words = self.data['all_words']
         self.tags = self.data['tags']
         self.model_state = self.data["model_state"]
```

### Comparing `JanexPT-0.0.7/JanexPT/train.py` & `JanexPT-0.0.8/JanexPT/train.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.7/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.8/JanexPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -26,21 +26,21 @@
 from JanexPT import *
 ```
 
 Next, create an instance of the JanexPT class and define the path to your intents, thesaurus, and the name you wish to give to your AI.
 ```
 intents_file_path, thesaurus_file_path, UIName = "intents.json", "thesaurus.json", "May" # Use whichever name you like.
 
-JanexPT = JanexPT(intents_file_path, thesaurus_file_path, UIName)
+janexpt = JanexPT(intents_file_path, thesaurus_file_path, UIName)
 
 ```
 
 Then, you will need to train your intents data into a pth file. If you do not have a training program, it will curl install the pre-built one from this repo.
 ```
-JanexPT.trainpt()
+janexpt.trainpt()
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
```

### Comparing `JanexPT-0.0.7/LICENSE` & `JanexPT-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.7/PKG-INFO` & `JanexPT-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -26,21 +26,21 @@
 from JanexPT import *
 ```
 
 Next, create an instance of the JanexPT class and define the path to your intents, thesaurus, and the name you wish to give to your AI.
 ```
 intents_file_path, thesaurus_file_path, UIName = "intents.json", "thesaurus.json", "May" # Use whichever name you like.
 
-JanexPT = JanexPT(intents_file_path, thesaurus_file_path, UIName)
+janexpt = JanexPT(intents_file_path, thesaurus_file_path, UIName)
 
 ```
 
 Then, you will need to train your intents data into a pth file. If you do not have a training program, it will curl install the pre-built one from this repo.
 ```
-JanexPT.trainpt()
+janexpt.trainpt()
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
```

### Comparing `JanexPT-0.0.7/README.md` & `JanexPT-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from JanexPT import *
 ```
 
 Next, create an instance of the JanexPT class and define the path to your intents, thesaurus, and the name you wish to give to your AI.
 ```
 intents_file_path, thesaurus_file_path, UIName = "intents.json", "thesaurus.json", "May" # Use whichever name you like.
 
-JanexPT = JanexPT(intents_file_path, thesaurus_file_path, UIName)
+janexpt = JanexPT(intents_file_path, thesaurus_file_path, UIName)
 
 ```
 
 Then, you will need to train your intents data into a pth file. If you do not have a training program, it will curl install the pre-built one from this repo.
 ```
-JanexPT.trainpt()
+janexpt.trainpt()
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
```

### Comparing `JanexPT-0.0.7/setup.py` & `JanexPT-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.7",
+    version="0.0.8",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
@@ -33,16 +33,17 @@
     packages=setuptools.find_packages(),
 
 
     #if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-        "CipherProgram",
+        "Janex",
         "torch",
+        "nltk",
         ],
 
 
     license="Lily 1.0",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
```

