# Comparing `tmp/lenio-ai-prompt-engineer-1.2.0.tar.gz` & `tmp/lenio-ai-prompt-engineer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenio-ai-prompt-engineer-1.2.0.tar", last modified: Mon Aug  7 20:30:24 2023, max compression
+gzip compressed data, was "lenio-ai-prompt-engineer-1.2.1.tar", last modified: Mon Aug  7 21:44:05 2023, max compression
```

## Comparing `lenio-ai-prompt-engineer-1.2.0.tar` & `lenio-ai-prompt-engineer-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.540533 lenio-ai-prompt-engineer-1.2.0/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 20:30:24.539865 lenio-ai-prompt-engineer-1.2.0/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     2955 2023-08-07 20:24:36.000000 lenio-ai-prompt-engineer-1.2.0/README.md
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.522242 lenio-ai-prompt-engineer-1.2.0/cli/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.2.0/cli/__init__.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.525510 lenio-ai-prompt-engineer-1.2.0/cli/evals/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4015 2023-08-07 16:39:39.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/classification.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7920 2023-08-07 19:35:22.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/elovalue.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3867 2023-08-07 15:30:35.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/equal.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3810 2023-08-07 18:54:01.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/includes.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1402 2023-08-07 02:29:30.000000 lenio-ai-prompt-engineer-1.2.0/cli/generation.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3039 2023-08-07 19:25:44.000000 lenio-ai-prompt-engineer-1.2.0/cli/iteration.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     9535 2023-08-07 20:01:14.000000 lenio-ai-prompt-engineer-1.2.0/cli/main.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.533419 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/grammatical_errors.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_lowercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_uppercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_uppercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/synonymous_prompt.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/uppercase.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.538866 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      808 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/requires.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-07 20:30:24.541365 lenio-ai-prompt-engineer-1.2.0/setup.cfg
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-07 20:30:11.000000 lenio-ai-prompt-engineer-1.2.0/setup.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 21:44:05.679238 lenio-ai-prompt-engineer-1.2.1/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 21:44:05.678338 lenio-ai-prompt-engineer-1.2.1/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     2955 2023-08-07 20:24:36.000000 lenio-ai-prompt-engineer-1.2.1/README.md
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 21:44:05.657586 lenio-ai-prompt-engineer-1.2.1/cli/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.2.1/cli/__init__.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 21:44:05.663261 lenio-ai-prompt-engineer-1.2.1/cli/evals/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.2.1/cli/evals/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4015 2023-08-07 16:39:39.000000 lenio-ai-prompt-engineer-1.2.1/cli/evals/classification.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7920 2023-08-07 19:35:22.000000 lenio-ai-prompt-engineer-1.2.1/cli/evals/elovalue.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3867 2023-08-07 15:30:35.000000 lenio-ai-prompt-engineer-1.2.1/cli/evals/equal.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3810 2023-08-07 18:54:01.000000 lenio-ai-prompt-engineer-1.2.1/cli/evals/includes.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1402 2023-08-07 02:29:30.000000 lenio-ai-prompt-engineer-1.2.1/cli/generation.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3039 2023-08-07 19:25:44.000000 lenio-ai-prompt-engineer-1.2.1/cli/iteration.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     9682 2023-08-07 21:36:33.000000 lenio-ai-prompt-engineer-1.2.1/cli/main.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 21:44:05.671262 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/grammatical_errors.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/random_lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/random_lowercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/random_uppercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/random_uppercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/synonymous_prompt.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.2.1/cli/promptChange/uppercase.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 21:44:05.676942 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      808 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/requires.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-07 21:44:05.000000 lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-07 21:44:05.679552 lenio-ai-prompt-engineer-1.2.1/setup.cfg
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-07 21:43:46.000000 lenio-ai-prompt-engineer-1.2.1/setup.py
```

### Comparing `lenio-ai-prompt-engineer-1.2.0/README.md` & `lenio-ai-prompt-engineer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/evals/classification.py` & `lenio-ai-prompt-engineer-1.2.1/cli/evals/classification.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/evals/elovalue.py` & `lenio-ai-prompt-engineer-1.2.1/cli/evals/elovalue.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/evals/equal.py` & `lenio-ai-prompt-engineer-1.2.1/cli/evals/equal.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/evals/includes.py` & `lenio-ai-prompt-engineer-1.2.1/cli/evals/includes.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/generation.py` & `lenio-ai-prompt-engineer-1.2.1/cli/generation.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/iteration.py` & `lenio-ai-prompt-engineer-1.2.1/cli/iteration.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/main.py` & `lenio-ai-prompt-engineer-1.2.1/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 from .promptChange import uppercase, lowercase, random_uppercase, random_lowercase, random_lowercase_word, random_uppercase_word, synonymous_prompt, grammatical_errors
 import yaml
 import textwrap
 import numpy as np
 from collections import defaultdict
 from dotenv import load_dotenv
 load_dotenv()
+openai.api_base = os.getenv("OPENAI_API_BASE")
 openai.api_key = os.getenv("OPENAI_API_KEY")
+openai.api_type = os.getenv("OPENAI_API_TYPE")
+openai.api_version = os.getenv("OPENAI_API_VERSION")
 
 # It loads and reads the content of a given YAML file and returns its content as a Python dictionary or list.
 def read_yaml(file_name):
     with open(file_name, 'r') as file:
         content = yaml.safe_load(file)
     return content
```

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/promptChange/grammatical_errors.py` & `lenio-ai-prompt-engineer-1.2.1/cli/promptChange/grammatical_errors.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/cli/promptChange/synonymous_prompt.py` & `lenio-ai-prompt-engineer-1.2.1/cli/promptChange/synonymous_prompt.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt` & `lenio-ai-prompt-engineer-1.2.1/lenio_ai_prompt_engineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

