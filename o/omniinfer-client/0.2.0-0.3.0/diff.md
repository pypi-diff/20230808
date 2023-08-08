# Comparing `tmp/omniinfer_client-0.2.0.tar.gz` & `tmp/omniinfer_client-0.3.0.tar.gz`

## Comparing `omniinfer_client-0.2.0.tar` & `omniinfer_client-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/.python-version
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/Makefile
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/requirements.lock
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/modules.rst
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/omniinfer_client.rst
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/controlnet_qrcode.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/model_search.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/txt2img_with_lora.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/exceptions.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/omni.py
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/serializer.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/settings.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/version.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/tests/test_basics.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/tests/test_model.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/.python-version
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/Makefile
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/requirements.lock
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/modules.rst
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/omniinfer_client.rst
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/controlnet_qrcode.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/model_search.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/txt2img_with_hiresfix.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/txt2img_with_lora.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/exceptions.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/omni.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/serializer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/settings.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/version.py
+-rw-r--r--   0        0        0     8790 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/tests/test_basics.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/tests/test_model.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/PKG-INFO
```

### Comparing `omniinfer_client-0.2.0/requirements-dev.lock` & `omniinfer_client-0.3.0/requirements-dev.lock`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 jaraco-classes==3.2.3
 jeepney==0.8.0
 keyring==24.1.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 packaging==23.1
+pillow==9.5.0
 pkginfo==1.9.6
 pluggy==1.2.0
 pycparser==2.21
 pygments==2.16.0
 pyproject-hooks==1.0.0
 pytest==7.4.0
 pytest-dependency==0.5.1
```

### Comparing `omniinfer_client-0.2.0/docs/Makefile` & `omniinfer_client-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/docs/conf.py` & `omniinfer_client-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/docs/make.bat` & `omniinfer_client-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/docs/omniinfer_client.rst` & `omniinfer_client-0.3.0/docs/omniinfer_client.rst`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/examples/controlnet_qrcode.py` & `omniinfer_client-0.3.0/examples/controlnet_qrcode.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/examples/model_search.py` & `omniinfer_client-0.3.0/examples/model_search.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/examples/txt2img_with_lora.py` & `omniinfer_client-0.3.0/examples/txt2img_with_lora.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/examples/fixtures/qrcode.png` & `omniinfer_client-0.3.0/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/src/omniinfer_client/proto.py` & `omniinfer_client-0.3.0/src/omniinfer_client/proto.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,18 +132,24 @@
     n_iter: int = 1
     steps: int = 20
     cfg_scale: float = 7
     height: int = 512
     width: int = 512
     seed: Optional[int] = -1
     restore_faces: Optional[bool] = False
-    sd_vae: Optional[str] = "Automatic"
+    sd_vae: Optional[str] = None
     clip_skip: Optional[int] = 1
     controlnet_units: Optional[List[ControlnetUnit]] = None
 
+    enable_hr: Optional[bool] = False
+    hr_upscaler: Optional[str] = 'R-ESRGAN 4x+'
+    hr_scale: Optional[float] = 2.0
+    hr_resize_x: Optional[int] = None
+    hr_resize_y: Optional[int] = None
+
 
 class Txt2ImgResponseCode(Enum):
     NORMAL = 0
     INTERNAL_ERROR = -1
     INVALID_JSON = 1
     MODEL_NOT_EXISTS = 2
     TASK_ID_NOT_EXISTS = 3
@@ -197,15 +203,15 @@
     negative_prompt: Optional[str] = None
     batch_size: Optional[int] = 1
     n_iter: Optional[int] = 1
     steps: Optional[int] = 20
     width: Optional[int] = 1024
     height: Optional[int] = 1024
     restore_faces: Optional[bool] = False
-    sd_vae: Optional[str] = "Automatic"
+    sd_vae: Optional[str] = None
     clip_skip: Optional[int] = 1
     controlnet_units: Optional[List[ControlnetUnit]] = None
 
 
 class Img2ImgResponseCode(Enum):
     NORMAL = 0
     INTERNAL_ERROR = -1
@@ -300,14 +306,70 @@
     data: ProgressData
     msg: Optional[str] = ""
 
     def download_images(self):
         if self.data.imgs is not None and len(self.data.imgs) > 0:
             self.data.imgs_bytes = batch_download_images(self.data.imgs)
 
+# --------------- Upscale ---------------
+
+
+class UpscaleResizeMode(Enum):
+    SCALE = 0
+    SIZE = 1
+
+@dataclass
+class UpscaleRequest(JSONe):
+    image: str
+    upscaler_1: Optional[str] = 'R-ESRGAN 4x+'
+    resize_mode: Optional[UpscaleResizeMode] = UpscaleResizeMode.SCALE
+    upscaling_resize: Optional[float] = 2.0
+    upscaling_resize_w: Optional[int] = None
+    upscaling_resize_h: Optional[int] = None
+    upscaling_crop: Optional[bool] = False
+
+    upscaler_2: Optional[str] = None
+    extras_upscaler_2_visibility: Optional[float] = None
+    gfpgan_visibility: Optional[float] = None
+    codeformer_visibility: Optional[float] = None
+    codeformer_weight: Optional[float] = None
+
+
+class UpscaleResponseCode(Enum):
+    NORMAL = 0
+    INTERNAL_ERROR = -1
+    INVALID_JSON = 1
+    MODEL_NOT_EXISTS = 2
+    TASK_ID_NOT_EXISTS = 3
+    INVALID_AUTH = 4
+    HOST_UNAVAILABLE = 5
+    PARAM_RANGE_ERROR = 6
+    COST_BALANCE_ERROR = 7
+    SAMPLER_NOT_EXISTS = 8
+    TIMEOUT = 9
+
+    UNKNOWN = 100
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
+
+
+@dataclass
+class UpscaleResponseData(JSONe):
+    task_id: str
+    warn: Optional[str] = None
+
+
+@dataclass
+class UpscaleResponse(JSONe):
+    code: UpscaleResponseCode
+    msg: str
+    data: Optional[UpscaleResponseData] = None
+
 
 # --------------- Model ---------------
 
 
 class ModelType(Enum):
     CHECKPOINT = "checkpoint"
     LORA = "lora"
```

### Comparing `omniinfer_client-0.2.0/src/omniinfer_client/utils.py` & `omniinfer_client-0.3.0/src/omniinfer_client/utils.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/tests/test_model.py` & `omniinfer_client-0.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/.gitignore` & `omniinfer_client-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/LICENSE` & `omniinfer_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.2.0/README.md` & `omniinfer_client-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -146,14 +146,44 @@
 if res.data.status != ProgressResponseStatusCode.SUCCESSFUL:
     raise Exception('Failed to generate image with error: ' +
                     res.data.failed_reason)
 
 save_image(res.data.imgs_bytes[0], "qrcode-art.png")
 ```
 
+### Txt2Img with Hires.Fix
+
+[txt2img_with_hiresfix.py](./examples/txt2img_with_hiresfix.py)
+
+```python
+import os
+
+from omniinfer_client import *
+
+client = OmniClient(os.getenv('OMNI_API_KEY'))
+req = Txt2ImgRequest(
+    model_name='dreamshaper_8_93211.safetensors',
+    prompt='a dog flying in the sky',
+    width=512,
+    height=512,
+    batch_size=1,
+    cfg_scale=7.5,
+    sampler_name=Samplers.EULER_A,
+    enable_hr=True,
+    hr_scale=2.0
+)
+
+res = client.sync_txt2img(req)
+if res.data.status != ProgressResponseStatusCode.SUCCESSFUL:
+    raise Exception('Failed to generate image with error: ' +
+                    res.data.failed_reason)
+
+save_image(res.data.imgs_bytes[0], "txt2img-hiresfix-1024.png")
+```
+
 
 ## Testing
 
 ```
 export OMNI_API_KEY=<YOUR_API_KEY>
 
 python -m pytest
```

### Comparing `omniinfer_client-0.2.0/pyproject.toml` & `omniinfer_client-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omniinfer_client"
-version = "0.2.0"
+version = "0.3.0"
 description = "Omniinfer SDK for Python"
 authors = [
     { name = "Omniinfer", email = "omniinfer@gmail.com" }
 ]
 
 
 dependencies = [
@@ -34,11 +34,12 @@
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pytest>=7.0.1",
     "pytest-dependency>=0.5.1",
     "build>=0.9.0",
     "twine>=3.8.0",
+    "pillow>=8.4.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `omniinfer_client-0.2.0/PKG-INFO` & `omniinfer_client-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniinfer_client
-Version: 0.2.0
+Version: 0.3.0
 Summary: Omniinfer SDK for Python
 Project-URL: Homepage, https://github.com/omniinfer/python-sdk
 Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: Omniinfer <omniinfer@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 omniinfer.io
@@ -183,14 +183,44 @@
 if res.data.status != ProgressResponseStatusCode.SUCCESSFUL:
     raise Exception('Failed to generate image with error: ' +
                     res.data.failed_reason)
 
 save_image(res.data.imgs_bytes[0], "qrcode-art.png")
 ```
 
+### Txt2Img with Hires.Fix
+
+[txt2img_with_hiresfix.py](./examples/txt2img_with_hiresfix.py)
+
+```python
+import os
+
+from omniinfer_client import *
+
+client = OmniClient(os.getenv('OMNI_API_KEY'))
+req = Txt2ImgRequest(
+    model_name='dreamshaper_8_93211.safetensors',
+    prompt='a dog flying in the sky',
+    width=512,
+    height=512,
+    batch_size=1,
+    cfg_scale=7.5,
+    sampler_name=Samplers.EULER_A,
+    enable_hr=True,
+    hr_scale=2.0
+)
+
+res = client.sync_txt2img(req)
+if res.data.status != ProgressResponseStatusCode.SUCCESSFUL:
+    raise Exception('Failed to generate image with error: ' +
+                    res.data.failed_reason)
+
+save_image(res.data.imgs_bytes[0], "txt2img-hiresfix-1024.png")
+```
+
 
 ## Testing
 
 ```
 export OMNI_API_KEY=<YOUR_API_KEY>
 
 python -m pytest
```

