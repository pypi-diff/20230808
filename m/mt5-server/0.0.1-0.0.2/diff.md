# Comparing `tmp/mt5-server-0.0.1.tar.gz` & `tmp/mt5-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mt5-server-0.0.1.tar", last modified: Tue Aug  8 01:35:20 2023, max compression
+gzip compressed data, was "mt5-server-0.0.2.tar", last modified: Tue Aug  8 02:11:51 2023, max compression
```

## Comparing `mt5-server-0.0.1.tar` & `mt5-server-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:35:20.506832 mt5-server-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:35:10.000000 mt5-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 01:35:10.000000 mt5-server-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 01:35:20.506832 mt5-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-08 01:35:10.000000 mt5-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:35:20.506832 mt5-server-0.0.1/mt5_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 01:35:20.000000 mt5-server-0.0.1/mt5_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-08 01:35:20.000000 mt5-server-0.0.1/mt5_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:35:20.000000 mt5-server-0.0.1/mt5_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 01:35:20.000000 mt5-server-0.0.1/mt5_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:35:20.000000 mt5-server-0.0.1/mt5_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:35:20.506832 mt5-server-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-08 01:35:10.000000 mt5-server-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:35:20.506832 mt5-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 01:35:10.000000 mt5-server-0.0.1/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:51.194053 mt5-server-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 02:11:40.000000 mt5-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 02:11:40.000000 mt5-server-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 02:11:51.194053 mt5-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 02:11:40.000000 mt5-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:51.190053 mt5-server-0.0.2/mt5_server/
+-rw-r--r--   0 runner    (1001) docker     (123)   167923 2023-08-08 02:11:40.000000 mt5-server-0.0.2/mt5_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 02:11:40.000000 mt5-server-0.0.2/mt5_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-08 02:11:40.000000 mt5-server-0.0.2/mt5_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:51.190053 mt5-server-0.0.2/mt5_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 02:11:51.000000 mt5-server-0.0.2/mt5_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 02:11:51.000000 mt5-server-0.0.2/mt5_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:11:51.000000 mt5-server-0.0.2/mt5_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 02:11:51.000000 mt5-server-0.0.2/mt5_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 02:11:51.000000 mt5-server-0.0.2/mt5_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:11:51.194053 mt5-server-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-08 02:11:40.000000 mt5-server-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:11:51.194053 mt5-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 02:11:40.000000 mt5-server-0.0.2/tests/test_01.py
```

### Comparing `mt5-server-0.0.1/LICENSE` & `mt5-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.1/LICENSE.txt` & `mt5-server-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.1/setup.py` & `mt5-server-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
 
-VERSION = (0, 0, 1)
+VERSION = (0, 0, 2)
 __version__ = '.'.join(map(str, VERSION))
 
 
 setup(
     name='mt5-server',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
     description='Servidor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/michelmetran/mt5_server',
-    keywords='python, dados espaciais, geoprocessamento',
+    keywords='python, metatrader',
     # Python and Packages
     python_requires='>=3',
     install_requires=requirements,
     # Entry
     # Our packages live under src but src is not a package itself
     # package_dir={'': 'sp_ff_apa_corumbatai'},
     # Quando são diversos módulos...
-    packages=find_packages('mt5_server', exclude=['test']),
-    # packages=find_packages(),
+    packages=find_packages('.', exclude=['tests']),
+    #packages=find_packages(),
     # Dados
     # include_package_data=True,
     # package_data={'': ['data/output/geo/*.7z']},
     # Classificação
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

