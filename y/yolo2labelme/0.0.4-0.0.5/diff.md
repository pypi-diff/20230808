# Comparing `tmp/yolo2labelme-0.0.4.tar.gz` & `tmp/yolo2labelme-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolo2labelme-0.0.4.tar", last modified: Thu Jun  8 17:40:06 2023, max compression
+gzip compressed data, was "yolo2labelme-0.0.5.tar", last modified: Tue Aug  8 19:24:46 2023, max compression
```

## Comparing `yolo2labelme-0.0.4.tar` & `yolo2labelme-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     1069 2023-06-04 14:00:21.000000 yolo2labelme-0.0.4/LICENSE
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     1400 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/PKG-INFO
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      825 2023-06-08 17:33:33.000000 yolo2labelme-0.0.4/README.md
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      647 2023-06-08 17:40:00.000000 yolo2labelme-0.0.4/pyproject.toml
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       38 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/setup.cfg
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      231 2023-06-08 17:39:52.000000 yolo2labelme-0.0.4/setup.py
-drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/yolo2labelme.egg-info/
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     1400 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/PKG-INFO
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      240 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/SOURCES.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)        1 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/dependency_links.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       51 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/entry_points.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       13 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/top_level.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     3184 2023-06-08 17:07:33.000000 yolo2labelme-0.0.4/yolo2labelme.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:24:46.009111 yolo2labelme-0.0.5/
+-rw-rw-rw-   0        0        0     1069 2023-06-04 14:00:20.000000 yolo2labelme-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1972 2023-08-08 19:24:46.008113 yolo2labelme-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2023-08-08 19:19:03.000000 yolo2labelme-0.0.5/README.md
+-rw-rw-rw-   0        0        0      647 2023-08-08 19:24:39.000000 yolo2labelme-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 19:24:46.009111 yolo2labelme-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-08-08 19:24:19.000000 yolo2labelme-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:24:46.005123 yolo2labelme-0.0.5/yolo2labelme.egg-info/
+-rw-rw-rw-   0        0        0     1972 2023-08-08 19:24:45.000000 yolo2labelme-0.0.5/yolo2labelme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-08-08 19:24:45.000000 yolo2labelme-0.0.5/yolo2labelme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 19:24:45.000000 yolo2labelme-0.0.5/yolo2labelme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-08 19:24:45.000000 yolo2labelme-0.0.5/yolo2labelme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-08-08 19:24:45.000000 yolo2labelme-0.0.5/yolo2labelme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3759 2023-08-08 19:14:34.000000 yolo2labelme-0.0.5/yolo2labelme.py
```

### Comparing `yolo2labelme-0.0.4/LICENSE` & `yolo2labelme-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yolo2labelme-0.0.4/PKG-INFO` & `yolo2labelme-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: yolo2labelme
-Version: 0.0.4
-Summary: Tool to convert yolo format dataset to labelme json format.
-Author-email: Kadapalla Nithin Kumar <kadapallanithin@gmail.com>
-Project-URL: Homepage, https://github.com/kadapallaNithin/yolo2labelme
-Project-URL: Bug Tracker, https://github.com/kadapallaNithin/yolo2labelme/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # yolo2labelme
 
 Tool to convert yolo format dataset to labelme json format.
 
 ## Installation
 ```bash
 pip install yolo2labelme
 ```
 ## Usage
+Arguments:
+
+`data` : path to dataset directory
+
+Keyword arguments:
+
+`out` : path to output directory. Default dataset is created at same path as data_dir with name labelmeDataset.
+
+`skip` : action to take if `.txt` file corresponding to image is not found.
+- `False` (default) raises `FileNotFoundError`.
+- `print` prints missing file path to stdout.
+- `True` or any other value skips file silently.
 ### CLI Usage:
 
 Following command creates labelme json dataset directory at `path/to/yolo/labelmeDataset` from `path/to/yolo/dataset` dataset directory.
 ```bash
 yolo2labelme path/to/yolo/dataset
 ```
 
-Specify output directory
+Specify output directory, skip.
 
 ```bash
-yolo2labelme path/to/yoloDataset --out path/to/labelmeJsonDir
+yolo2labelme path/to/yoloDataset --out path/to/labelmeJsonDir --skip print
 ```
 
 ### Python Usage:
 ```python
 from yolo2lableme import yolo2labelme
 yolo2labelme('path/to/yolo/dataset')
 ```
-With output directory
+With output directory and skip action
 ```python
-yolo2labelme('path/to/yolo/dataset','path/to/labelme/dataset')
+yolo2labelme('path/to/yolo/dataset','path/to/labelme/dataset',skip=True)
 ```
 Or simply
 ```python
 from yolo2labelme import y2l
 y2l('path/to/dataset')
 ```
 ## Useful links
 https://github.com/kadapallaNithin/yolo2labelme
 
 https://pypi.org/project/yolo2labelme/
+
+Lableme to yolo : https://pypi.org/project/labelme2yolo/
```

### Comparing `yolo2labelme-0.0.4/pyproject.toml` & `yolo2labelme-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yolo2labelme"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Kadapalla Nithin Kumar", email="kadapallanithin@gmail.com" },
 ]
 description = "Tool to convert yolo format dataset to labelme json format."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yolo2labelme-0.0.4/yolo2labelme.py` & `yolo2labelme-0.0.5/yolo2labelme.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,35 +63,44 @@
     img_filename = os.path.basename(img_path)
     json_path = img_filename_to_ext(img_filename,'.json')
     json_path = os.path.join(out_dir,json_path)
     with open(json_path,'w') as f:
         f.write(json.dumps(result))
     shutil.copyfile(img_path, os.path.join(out_dir, img_filename) )
 
-def yolo2labelme(data_dir, out_dir=None):
-    yaml_path = os.path.join(data_dir,"dataset.yaml")
+def yolo2labelme(data, out=None, skip=False):
+    yaml_path = os.path.join(data,"dataset.yaml")
     with open(yaml_path, 'r') as stream:
         data_loaded = yaml.safe_load(stream)
         class_labels = data_loaded['names']
 
-    if out_dir is None:
-        out_dir = os.path.join(os.path.abspath(data_dir),'..','labelmeDataset')
+    if out is None:
+        out = os.path.join(os.path.abspath(data),'..','labelmeDataset')
     for dir_type in ['test', 'train','val']:
-        dir_path = os.path.join(data_loaded[dir_type])
+        dir_path = os.path.join(data, data_loaded[dir_type])
+        dir_path = os.path.abspath(dir_path)
         for filename in os.listdir(dir_path):
             img_file = os.path.join(dir_path,filename)
             if is_image_file(img_file):
                 txt_file = img_filename_to_ext(img_file.replace('images','labels'), '.txt')
-
-                yolo2labelme_single(txt_file, img_file, class_labels, out_dir)
+                if os.path.exists(txt_file):
+                    yolo2labelme_single(txt_file, img_file, class_labels, out)
+                else:
+                    if skip == False:
+                        raise FileNotFoundError(f"{txt_file} is expected to exist."
+                                                +"Pass skip=True to skip silently.\n"
+                                                +"skip='print' to print missed paths.")
+                    elif skip == 'print':
+                        print(f'Missing {txt_file}')
 
 y2l = yolo2labelme
 
 def main():
     argparser = argparse.ArgumentParser()
     argparser.add_argument('data')
     argparser.add_argument('--out', default=None, required=False)
+    argparser.add_argument('--skip', default=False, required=False)
     args = argparser.parse_args()
-    yolo2labelme(args.data, args.out)
+    yolo2labelme(args.data, args.out, args.skip)
 
 if __name__ == '__main__':
     main()
```

