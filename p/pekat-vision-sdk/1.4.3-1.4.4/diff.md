# Comparing `tmp/pekat_vision_sdk-1.4.3.tar.gz` & `tmp/pekat_vision_sdk-1.4.4.tar.gz`

## Comparing `pekat_vision_sdk-1.4.3.tar` & `pekat_vision_sdk-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/__init__.py
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/pekat_vision_instance.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/LICENSE
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/PekatVisionSDK/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/PekatVisionSDK/__init__.py
+-rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/PekatVisionSDK/pekat_vision_instance.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/LICENSE
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.4/PKG-INFO
```

### Comparing `pekat_vision_sdk-1.4.3/PekatVisionSDK/pekat_vision_instance.py` & `pekat_vision_sdk-1.4.4/PekatVisionSDK/pekat_vision_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         :return: results of recognition based on response_type
         :rtype: (NDArray[np.uint8], dict) | dict
         """
         image_path = None
         numpy_image = None
 
         if sys.version_info < (3, 10):
+            global StrOrPathLike
             StrOrPathLike = (str, os.PathLike)
 
         if isinstance(image, StrOrPathLike):
             image_path = Path(image)
         elif isinstance(image, np.ndarray):
             numpy_image = image
         else:
```

### Comparing `pekat_vision_sdk-1.4.3/LICENSE` & `pekat_vision_sdk-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.3/README.md` & `pekat_vision_sdk-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.3/pyproject.toml` & `pekat_vision_sdk-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.3/PKG-INFO` & `pekat_vision_sdk-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pekat-vision-sdk
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python module for communication with PEKAT VISION
 Project-URL: Homepage, https://github.com/pekat-vision/pekat-vision-sdk-python
 Project-URL: repository, https://github.com/pekat-vision/pekat-vision-sdk-python.git
 Author-email: developers@pekatvision.com
 Maintainer-email: developers@pekatvision.com
 License-Expression: MIT
 License-File: LICENSE
```

