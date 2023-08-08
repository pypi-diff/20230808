# Comparing `tmp/auto-eval-0.3.6.tar.gz` & `tmp/auto-eval-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.3.6.tar", last modified: Mon Jul 24 03:08:52 2023, max compression
+gzip compressed data, was "auto-eval-0.3.7.tar", last modified: Tue Aug  8 02:39:55 2023, max compression
```

## Comparing `auto-eval-0.3.6.tar` & `auto-eval-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.686622 auto-eval-0.3.6/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.6/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-24 03:08:52.686370 auto-eval-0.3.6/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.6/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.681293 auto-eval-0.3.6/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.681801 auto-eval-0.3.6/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.6/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    15857 2023-07-24 03:05:07.000000 auto-eval-0.3.6/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.683014 auto-eval-0.3.6/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.6/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6171 2023-07-24 02:32:35.000000 auto-eval-0.3.6/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.684405 auto-eval-0.3.6/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.6/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.6/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.6/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.685363 auto-eval-0.3.6/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.6/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.6/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-24 03:08:52.686676 auto-eval-0.3.6/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 10:07:13.000000 auto-eval-0.3.6/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.096855 auto-eval-0.3.7/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.7/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16552 2023-08-08 02:39:55.096661 auto-eval-0.3.7/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16126 2023-08-08 02:35:46.000000 auto-eval-0.3.7/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.094079 auto-eval-0.3.7/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16552 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-08-08 02:39:55.000000 auto-eval-0.3.7/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.094525 auto-eval-0.3.7/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.7/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    15858 2023-07-24 03:15:51.000000 auto-eval-0.3.7/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.094842 auto-eval-0.3.7/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.7/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6171 2023-07-24 02:32:35.000000 auto-eval-0.3.7/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.095775 auto-eval-0.3.7/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.7/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.7/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.7/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-08 02:39:55.096448 auto-eval-0.3.7/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.7/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4378 2023-08-08 02:33:30.000000 auto-eval-0.3.7/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-08 02:39:55.096899 auto-eval-0.3.7/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-08-08 02:34:25.000000 auto-eval-0.3.7/setup.py
```

### Comparing `auto-eval-0.3.6/LICENSE` & `auto-eval-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.6/PKG-INFO` & `auto-eval-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.6
+Version: 0.3.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,14 +50,16 @@
 
 Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
 
 Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
 
 
 ## Installation
+Requirements Python >=3.10
+
 ```sh
 pip install -U auto-eval
 ```
 
 ## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
@@ -67,31 +69,31 @@
 
 ### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
```

### Comparing `auto-eval-0.3.6/README.md` & `auto-eval-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
 
 Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
 
 
 ## Installation
+Requirements Python >=3.10
+
 ```sh
 pip install -U auto-eval
 ```
 
 ## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
@@ -55,31 +57,31 @@
 
 ### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
```

### Comparing `auto-eval-0.3.6/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.3.7/auto_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.6
+Version: 0.3.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,14 +50,16 @@
 
 Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
 
 Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
 
 
 ## Installation
+Requirements Python >=3.10
+
 ```sh
 pip install -U auto-eval
 ```
 
 ## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
@@ -67,31 +69,31 @@
 
 ### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.openai.com/v1",
+    "api_base": "https://api.openai.com/v1",
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Replace with your Azure OpenAI resource's endpoint value.",
+    "api_base": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
 Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "https://api.anthropic.com",
+    "api_base": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
```

### Comparing `auto-eval-0.3.6/eval/auto_llms_eval.py` & `auto-eval-0.3.7/eval/auto_llms_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,19 +266,20 @@
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
     scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.question_column_names, eval_config.answer_column_names, eval_config.sample_num, eval_config.eval_models)
 
     process_num = len(eval_config.api_config_files)
-    if eval_config.engines is not None and len(eval_config.engines) > 1:
-        assert len(eval_config.engines) == process_num, f'Number of engines must be equal to number of api config files when specific multiple engines, but got {len(eval_config.engines)} engines and {process_num} api config files.'
+
+    eval_config.engines = eval_config.engines if eval_config.engines is not None else [''] * process_num
     if eval_config.engines is not None and len(eval_config.engines) == 1:
         eval_config.engines = eval_config.engines * process_num
-    eval_config.engines = eval_config.engines if eval_config.engines is not None else [''] * process_num
+    if eval_config.engines is not None and len(eval_config.engines) > 1:
+        assert len(eval_config.engines) == process_num, f'Number of engines must be equal to number of api config files when specific multiple engines, but got {len(eval_config.engines)} engines and {process_num} api config files.'
 
     # Init api tool and prompter
     if process_num == 1:
         failed_groups = []
         tool = OneAPITool.from_config_file(eval_config.api_config_files[0])
         for group in tqdm(unscored_groups):
             result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engines[0], eval_config.temperature, eval_config.max_new_tokens)
```

### Comparing `auto-eval-0.3.6/eval/commands/auto_eval.py` & `auto-eval-0.3.7/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.6/eval/prompt_template/prompter.py` & `auto-eval-0.3.7/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.6/eval/prompt_template/prompts.py` & `auto-eval-0.3.7/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.6/eval/utils/data_utils.py` & `auto-eval-0.3.7/eval/utils/data_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,42 +3,50 @@
 import os
 import json
 import pandas as pd
 import numpy as np
 from typing import Union, List
 
 
-def df_reader(data_path, header: Union[int, None] = 0, usecols: Union[List[Union[str, int]], None] = None ,sep='\t', sheet_name=0) -> pd.DataFrame:
-    if data_path.endswith('json'):
-        df_data = pd.read_json(data_path)
-    elif data_path.endswith('jsonl'):
-        df_data = pd.read_json(data_path, lines=True)
-    elif data_path.endswith('xlsx'):
-        df_data = pd.read_excel(data_path, header=header, usecols=usecols, sheet_name=sheet_name)
-    elif data_path.endswith('.pkl'):
-        df_data = pd.read_pickle(data_path)
-    elif data_path.endswith('csv'):
-        df_data = pd.read_csv(data_path, header=header, usecols=usecols, sep=sep)
-    elif data_path.endswith('.parquet'):
-        df_data = pd.read_parquet(data_path)
-    else:
-        raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
+def df_reader(data_path, header: int | None = 0, usecols: list[str | int] | None = None ,sep='\t', sheet_name=0) -> pd.DataFrame:
+    extention = data_path.split('.')[-1]
+    match extention:
+        case 'jsonl':
+            df_data = pd.read_json(data_path, lines=True, convert_dates=False)
+        case 'json':
+            df_data = pd.read_json(data_path)
+        case 'xlsx':
+            df_data = pd.read_excel(data_path,header=header, usecols=usecols, sheet_name=sheet_name)
+        case 'csv' | 'tsv':
+            df_data = pd.read_csv(data_path, header=header, usecols=usecols, sep=sep)
+        case 'pkl':
+            df_data = pd.read_pickle(data_path)
+        case 'parquet':
+            df_data = pd.read_parquet(data_path)
+        case _:
+            raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv, parquet, pkl')
     return df_data
-
+    
 def df_saver(df: pd.DataFrame, data_path):
-    if data_path.endswith('json'):
-        df.to_json(data_path, orient='records', force_ascii=False)
-    if data_path.endswith('jsonl'):
-        df.to_json(data_path, orient='records', force_ascii=False, lines=True)
-    elif data_path.endswith('xlsx'):
-        df2xlsx(df, data_path, index=False)
-    elif data_path.endswith('csv'):
-        df.to_csv(data_path)
-    else:
-        raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
+    extention = data_path.split('.')[-1]
+    match extention:
+        case 'jsonl':
+            df.to_json(data_path, orient='records', force_ascii=False, lines=True)
+        case 'json':
+            df.to_json(data_path, orient='records', force_ascii=False)
+        case 'xlsx':
+            df2xlsx(df, data_path, index=False)
+        case 'csv' | 'tsv':
+            df.to_csv(data_path)
+        case 'pkl':
+            df.to_pickle(data_path)
+        case 'parquet':
+            df.to_parquet(data_path)
+        case _:
+            raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
     
 
 def extract_all_json(text, merged_return=True):
     json_strings = re.findall(r'\{[^}]*\}', text)
     json_dicts = [json.loads(j) for j in json_strings]
     if not merged_return:
         return json_dicts
```

### Comparing `auto-eval-0.3.6/setup.py` & `auto-eval-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.3.6",
+    version="0.3.7",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

