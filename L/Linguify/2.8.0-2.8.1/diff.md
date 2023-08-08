# Comparing `tmp/Linguify-2.8.0.tar.gz` & `tmp/Linguify-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Linguify-2.8.0.tar", last modified: Tue Aug  8 03:33:52 2023, max compression
+gzip compressed data, was "Linguify-2.8.1.tar", last modified: Tue Aug  8 04:04:31 2023, max compression
```

## Comparing `Linguify-2.8.0.tar` & `Linguify-2.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 03:33:52.748128 Linguify-2.8.0/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)     1073 2023-08-01 04:06:37.000000 Linguify-2.8.0/LICENSE
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 03:33:52.747115 Linguify-2.8.0/Linguify.egg-info/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/PKG-INFO
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      269 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/SOURCES.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/dependency_links.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       44 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/entry_points.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      100 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/requires.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-08-08 03:33:52.000000 Linguify-2.8.0/Linguify.egg-info/top_level.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-08 03:33:52.748012 Linguify-2.8.0/PKG-INFO
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 03:33:52.747827 Linguify-2.8.0/linguify/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       71 2023-08-02 05:33:49.000000 Linguify-2.8.0/linguify/__init__.py
--rwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)    23729 2023-08-08 01:27:07.000000 Linguify-2.8.0/linguify/linguify.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    23713 2023-08-08 03:31:24.000000 Linguify-2.8.0/linguify/main.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-08-08 03:33:52.748174 Linguify-2.8.0/setup.cfg
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      599 2023-08-08 03:21:20.000000 Linguify-2.8.0/setup.py
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 04:04:31.648604 Linguify-2.8.1/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)     1073 2023-08-01 04:06:37.000000 Linguify-2.8.1/LICENSE
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 04:04:31.647079 Linguify-2.8.1/Linguify.egg-info/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/PKG-INFO
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      269 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/SOURCES.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/dependency_links.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       44 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/entry_points.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      100 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/requires.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-08-08 04:04:31.000000 Linguify-2.8.1/Linguify.egg-info/top_level.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-08 04:04:31.648498 Linguify-2.8.1/PKG-INFO
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-08 04:04:31.648052 Linguify-2.8.1/linguify/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       71 2023-08-02 05:33:49.000000 Linguify-2.8.1/linguify/__init__.py
+-rwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)    23745 2023-08-08 04:03:51.000000 Linguify-2.8.1/linguify/linguify.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    23728 2023-08-08 04:03:17.000000 Linguify-2.8.1/linguify/main.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-08-08 04:04:31.648642 Linguify-2.8.1/setup.cfg
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      599 2023-08-08 04:03:57.000000 Linguify-2.8.1/setup.py
```

### Comparing `Linguify-2.8.0/LICENSE` & `Linguify-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Linguify-2.8.0/linguify/linguify.py` & `Linguify-2.8.1/linguify/linguify.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,15 @@
             openai.Model.list()
             correct = True
         except:
             os.remove(config_path)
             print('Incorrect OpenAI API key.')
 
     # Processing the voicemail
+    print(file)
     audio_file = open(file, "rb")
     transcript = openai.Audio.transcribe(
         model="whisper-1", 
         file=audio_file, 
         prompt='Format it in point form.'
         )
     transcript=transcript['text']
```

### Comparing `Linguify-2.8.0/linguify/main.py` & `Linguify-2.8.1/linguify/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
             openai.api_key,config_path = get_api_key()  
             openai.Model.list()
             correct = True
         except:
             os.remove(config_path)
             print('Incorrect OpenAI API key.')
     
-
+    print(file)
     # Processing the voicemail
     audio_file = open(file, "rb")
     transcript = openai.Audio.transcribe(
         model="whisper-1", 
         file=audio_file, 
         prompt='Format it in point form.'
         )
```

### Comparing `Linguify-2.8.0/setup.py` & `Linguify-2.8.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Linguify',
-    version='2.8.0',
+    version='2.8.1',
     packages=find_packages(),
     package_data={'linguify': ['credentials.json']},
     install_requires=[
     "openai>=0.27.8",
     "python-docx",
     "google-api-python-client",
     "google-auth-httplib2",
```

