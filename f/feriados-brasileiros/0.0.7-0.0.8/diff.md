# Comparing `tmp/feriados_brasileiros-0.0.7.tar.gz` & `tmp/feriados_brasileiros-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feriados_brasileiros-0.0.7.tar", last modified: Thu Jul 27 00:37:43 2023, max compression
+gzip compressed data, was "feriados_brasileiros-0.0.8.tar", last modified: Tue Aug  8 01:28:19 2023, max compression
```

## Comparing `feriados_brasileiros-0.0.7.tar` & `feriados_brasileiros-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.954950 feriados_brasileiros-0.0.7/feriados_brasileiros/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/feriados_brasileiros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/feriados_brasileiros/datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:28:19.509073 feriados_brasileiros-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-08 01:28:19.509073 feriados_brasileiros-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:28:19.509073 feriados_brasileiros-0.0.8/feriados_brasileiros/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/feriados_brasileiros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/feriados_brasileiros/datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:28:19.509073 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-08 01:28:19.000000 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 01:28:19.000000 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:28:19.000000 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 01:28:19.000000 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:28:19.000000 feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:28:19.509073 feriados_brasileiros-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-08 01:28:08.000000 feriados_brasileiros-0.0.8/setup.py
```

### Comparing `feriados_brasileiros-0.0.7/LICENSE` & `feriados_brasileiros-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.7/MANIFEST.in` & `feriados_brasileiros-0.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.7/PKG-INFO` & `feriados_brasileiros-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feriados_brasileiros
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,datas,feriados
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Feriados Brasileiros
 
 [PyPI](https://pypi.org/project/feriados-brasileiros) | [GitHub](https://github.com/michelmetran/feriados)
 
+
+
 <br>
 
 > _Adoro um feriado! Quem não gosta?!_
 
 Com objetivo de listar os feriados brasileiros, criei o pacote **feriados-brasileiros**, que permite criar uma tabela contendo todos os feriados de um determinado ano, bem como ajustar atributos conforme a necessidade.
 
 A opção por ajustar atributos se deve ao fato de que, nem sempre, um feriado em uma instituição também é feriado n'outra! Feriado de endoeças, por exemplo, é feriado em instituições do meio jurídico, enquanto muitos nem sabem que feriado é esse!
```

### Comparing `feriados_brasileiros-0.0.7/README.md` & `feriados_brasileiros-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Feriados Brasileiros
 
 [PyPI](https://pypi.org/project/feriados-brasileiros) | [GitHub](https://github.com/michelmetran/feriados)
 
+
+
 <br>
 
 > _Adoro um feriado! Quem não gosta?!_
 
 Com objetivo de listar os feriados brasileiros, criei o pacote **feriados-brasileiros**, que permite criar uma tabela contendo todos os feriados de um determinado ano, bem como ajustar atributos conforme a necessidade.
 
 A opção por ajustar atributos se deve ao fato de que, nem sempre, um feriado em uma instituição também é feriado n'outra! Feriado de endoeças, por exemplo, é feriado em instituições do meio jurídico, enquanto muitos nem sabem que feriado é esse!
```

### Comparing `feriados_brasileiros-0.0.7/feriados_brasileiros/datas.py` & `feriados_brasileiros-0.0.8/feriados_brasileiros/datas.py`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/PKG-INFO` & `feriados_brasileiros-0.0.8/feriados_brasileiros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feriados-brasileiros
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,datas,feriados
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Feriados Brasileiros
 
 [PyPI](https://pypi.org/project/feriados-brasileiros) | [GitHub](https://github.com/michelmetran/feriados)
 
+
+
 <br>
 
 > _Adoro um feriado! Quem não gosta?!_
 
 Com objetivo de listar os feriados brasileiros, criei o pacote **feriados-brasileiros**, que permite criar uma tabela contendo todos os feriados de um determinado ano, bem como ajustar atributos conforme a necessidade.
 
 A opção por ajustar atributos se deve ao fato de que, nem sempre, um feriado em uma instituição também é feriado n'outra! Feriado de endoeças, por exemplo, é feriado em instituições do meio jurídico, enquanto muitos nem sabem que feriado é esse!
```

### Comparing `feriados_brasileiros-0.0.7/setup.py` & `feriados_brasileiros-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
-VERSION = (0, 0, 7)
+VERSION = (0, 0, 8)
 __version__ = '.'.join(map(str, VERSION))
 
 setup(
     name='feriados_brasileiros',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
```

