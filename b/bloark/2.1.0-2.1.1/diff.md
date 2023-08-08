# Comparing `tmp/bloark-2.1.0.tar.gz` & `tmp/bloark-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloark-2.1.0.tar", max compression
+gzip compressed data, was "bloark-2.1.1.tar", max compression
```

## Comparing `bloark-2.1.0.tar` & `bloark-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 bloark-2.1.0/LICENSE
--rw-r--r--   0        0        0     1542 2023-07-15 23:37:34.226075 bloark-2.1.0/README.md
--rw-r--r--   0        0        0      137 2023-07-16 19:42:54.285250 bloark-2.1.0/bloark/__init__.py
--rw-r--r--   0        0        0    18571 2023-08-08 01:55:27.457106 bloark-2.1.0/bloark/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 bloark-2.1.0/bloark/builder_helpers.py
--rw-r--r--   0        0        0     2977 2023-07-16 21:18:37.433442 bloark-2.1.0/bloark/decorators.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 bloark-2.1.0/bloark/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 bloark-2.1.0/bloark/logger_init.py
--rw-r--r--   0        0        0    16600 2023-07-16 21:23:43.884492 bloark-2.1.0/bloark/modifier.py
--rw-r--r--   0        0        0     8978 2023-07-16 21:36:29.042415 bloark-2.1.0/bloark/reader.py
--rw-r--r--   0        0        0     7755 2023-07-16 20:23:09.560453 bloark-2.1.0/bloark/utils.py
--rw-r--r--   0        0        0     5234 2023-07-16 05:25:20.174851 bloark-2.1.0/bloark/warehouse.py
--rw-r--r--   0        0        0      979 2023-08-08 01:48:56.219807 bloark-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 bloark-2.1.0/setup.py
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 bloark-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 bloark-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1542 2023-07-15 23:37:34.226075 bloark-2.1.1/README.md
+-rw-r--r--   0        0        0      137 2023-07-16 19:42:54.285250 bloark-2.1.1/bloark/__init__.py
+-rw-r--r--   0        0        0    18575 2023-08-08 14:29:20.405162 bloark-2.1.1/bloark/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 bloark-2.1.1/bloark/builder_helpers.py
+-rw-r--r--   0        0        0     2977 2023-07-16 21:18:37.433442 bloark-2.1.1/bloark/decorators.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 bloark-2.1.1/bloark/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 bloark-2.1.1/bloark/logger_init.py
+-rw-r--r--   0        0        0    16600 2023-07-16 21:23:43.884492 bloark-2.1.1/bloark/modifier.py
+-rw-r--r--   0        0        0     8978 2023-07-16 21:36:29.042415 bloark-2.1.1/bloark/reader.py
+-rw-r--r--   0        0        0     7755 2023-07-16 20:23:09.560453 bloark-2.1.1/bloark/utils.py
+-rw-r--r--   0        0        0     5234 2023-07-16 05:25:20.174851 bloark-2.1.1/bloark/warehouse.py
+-rw-r--r--   0        0        0      979 2023-08-08 14:29:45.543862 bloark-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 bloark-2.1.1/setup.py
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 bloark-2.1.1/PKG-INFO
```

### Comparing `bloark-2.1.0/LICENSE` & `bloark-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/README.md` & `bloark-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/builder.py` & `bloark-2.1.1/bloark/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         try:
             start_time = time.time()
             if file_path.endswith('.7z'):
                 with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
                     z.extractall(path=decompressed_dir_path)
             elif file_path.endswith('.bz2'):
-                decompressed_filename = os.path.join(decompressed_dir_path, file_path.replace('.bz2', '').split('/')[-1])
+                decompressed_filename = os.path.join(decompressed_dir_path, os.path.split(file_path.replace('.bz2', ''))[-1])
                 with bz2.open(file_path, 'rb') as f_in, open(decompressed_filename, 'wb') as f_out:
                     for data in iter(lambda: f_in.read(500 * 1024), b''):  # Read in 500KB chunks once.
                         f_out.write(data)
             else:
                 logging.error(f'Unsupported file format: {archive_filename}')
                 return []
             end_time = time.time()
```

### Comparing `bloark-2.1.0/bloark/decorators.py` & `bloark-2.1.1/bloark/decorators.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/logger.py` & `bloark-2.1.1/bloark/logger.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/logger_init.py` & `bloark-2.1.1/bloark/logger_init.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/modifier.py` & `bloark-2.1.1/bloark/modifier.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/reader.py` & `bloark-2.1.1/bloark/reader.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/utils.py` & `bloark-2.1.1/bloark/utils.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/bloark/warehouse.py` & `bloark-2.1.1/bloark/warehouse.py`

 * *Files identical despite different names*

### Comparing `bloark-2.1.0/pyproject.toml` & `bloark-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bloark"
-version = "2.1.0"
+version = "2.1.1"
 description = "Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "bloark" },
 ]
```

### Comparing `bloark-2.1.0/setup.py` & `bloark-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'zstandard>=0.21.0,<0.22.0']
 
 entry_points = \
 {'console_scripts': ['benchmark = tests.benchmark:main']}
 
 setup_kwargs = {
     'name': 'bloark',
-    'version': '2.1.0',
+    'version': '2.1.1',
     'description': 'Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/b4d5d2b0-860c-4d73-02f0-104d77223800/Ultra" alt="BloArk" />\n\n# Blocks Architecture (BloArk)\n\nBlocks Architecture (BloArk) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install bloark\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bloark.lingxi.li/',
```

### Comparing `bloark-2.1.0/PKG-INFO` & `bloark-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloark
-Version: 2.1.0
+Version: 2.1.1
 Summary: Blocks Architecture (BloArk): A unified tool for processing revision-based data efficiently.
 Home-page: https://bloark.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

