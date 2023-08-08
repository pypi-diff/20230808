# Comparing `tmp/omniinfer_client-0.3.0.tar.gz` & `tmp/omniinfer_client-0.3.1.tar.gz`

## Comparing `omniinfer_client-0.3.0.tar` & `omniinfer_client-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/.python-version
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/Makefile
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/requirements.lock
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/Makefile
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/conf.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/make.bat
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/modules.rst
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/docs/omniinfer_client.rst
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/controlnet_qrcode.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/model_search.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/txt2img_with_hiresfix.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/txt2img_with_lora.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/exceptions.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/omni.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/serializer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/settings.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/src/omniinfer_client/version.py
--rw-r--r--   0        0        0     8790 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/tests/test_basics.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/tests/test_model.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/LICENSE
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 omniinfer_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/.python-version
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/Makefile
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/requirements.lock
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/modules.rst
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/docs/omniinfer_client.rst
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/examples/controlnet_qrcode.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/examples/model_search.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/examples/txt2img_with_hiresfix.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/examples/txt2img_with_lora.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/exceptions.py
+-rw-r--r--   0        0        0    10314 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/omni.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/serializer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/settings.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/src/omniinfer_client/version.py
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/tests/test_basics.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/tests/test_model.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 omniinfer_client-0.3.1/PKG-INFO
```

### Comparing `omniinfer_client-0.3.0/requirements-dev.lock` & `omniinfer_client-0.3.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/docs/Makefile` & `omniinfer_client-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/docs/conf.py` & `omniinfer_client-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/docs/make.bat` & `omniinfer_client-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/docs/omniinfer_client.rst` & `omniinfer_client-0.3.1/docs/omniinfer_client.rst`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/examples/controlnet_qrcode.py` & `omniinfer_client-0.3.1/examples/controlnet_qrcode.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/examples/model_search.py` & `omniinfer_client-0.3.1/examples/model_search.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/examples/txt2img_with_hiresfix.py` & `omniinfer_client-0.3.1/examples/txt2img_with_hiresfix.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/examples/txt2img_with_lora.py` & `omniinfer_client-0.3.1/examples/txt2img_with_lora.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/examples/fixtures/qrcode.png` & `omniinfer_client-0.3.1/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/src/omniinfer_client/omni.py` & `omniinfer_client-0.3.1/src/omniinfer_client/omni.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,28 @@
         self.session = requests.Session()
 
         if not self.api_key:
             raise ValueError("OMNI_API_KEY environment variable not set")
 
         # eg: {"all": [proto.ModelInfo], "checkpoint": [proto.ModelInfo], "lora": [proto.ModelInfo]}
         self._model_list_cache = None
+        self._extra_headers = {}
+
+    def set_extra_headers(self, headers: dict):
+        self._extra_headers = headers
 
     def _get(self, api_path, params=None) -> dict:
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json',
             'X-Omni-Key': self.api_key,
             'User-Agent': "omniinfer-python-sdk/{}".format(__version__),
             'Accept-Encoding': 'gzip, deflate',
         }
+        headers.update(self._extra_headers)
 
         logger.debug(f"[GET] params: {params}")
 
         response = self.session.get(
             self.base_url + api_path,
             headers=headers,
             params=params,
@@ -61,14 +66,15 @@
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json',
             'X-Omni-Key': self.api_key,
             'User-Agent': "omniinfer-python-sdk/{}".format(__version__),
             'Accept-Encoding': 'gzip, deflate',
         }
+        headers.update(self._extra_headers)
 
         logger.debug(f"[POST] data: {data}")
 
         response = self.session.post(
             self.base_url + api_path,
             headers=headers,
             json=data,
@@ -199,15 +205,15 @@
         if response.data is None:
             raise OmniResponseError(f"Image to Image generation failed with response {response.msg}, code: {response.code}")
 
         res = self.wait_for_task(response.data.task_id)
         if download_images:
             res.download_images()
         return res
-    
+
     def sync_upscale(self, request: UpscaleRequest, download_images=True) -> ProgressResponse:
         """Syncronously upscale image from request, optionally download images
 
         Args:
             request (UpscaleRequest): _description_
             download_images (bool, optional): _description_. Defaults to True.
 
@@ -235,16 +241,14 @@
         Returns:
             UpscaleResponse: An object containing the task status and the URL of the upscaled image.
         """
         response = self._post('/upscale', request.to_dict())
 
         return UpscaleResponse.from_dict(response)
 
-
-
     def models(self, refresh=False) -> ModelList:
         """Get list of models
 
         This method retrieves a list of models available in the Omni API. If the list has already been retrieved and
         `refresh` is False, the cached list will be returned. Otherwise, a new request will be made to the API to
         retrieve the list.
```

### Comparing `omniinfer_client-0.3.0/src/omniinfer_client/proto.py` & `omniinfer_client-0.3.1/src/omniinfer_client/proto.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/src/omniinfer_client/utils.py` & `omniinfer_client-0.3.1/src/omniinfer_client/utils.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/tests/test_basics.py` & `omniinfer_client-0.3.1/tests/test_basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     )
     upscale_res = client.sync_upscale(upscale_req)
     assert (upscale_res.data.status == ProgressResponseStatusCode.SUCCESSFUL)
     assert (len(upscale_res.data.imgs_bytes) == 1)
     img = Image.open(io.BytesIO(upscale_res.data.imgs_bytes[0]))
     assert img.size == (768, 768)
 
+
 def test_upscale_multiple_upscaler():
     client = OmniClient(os.getenv('OMNI_API_KEY'))
     res = client.sync_img2img(Img2ImgRequest(
         model_name='dreamshaper_8_93211.safetensors',
         prompt='a dog flying in the sky',
         width=512,
         height=512,
@@ -260,8 +261,26 @@
         upscaler_2='Nearest',
         gfpgan_visibility=1,
     )
     upscale_res = client.sync_upscale(upscale_req)
     assert (upscale_res.data.status == ProgressResponseStatusCode.SUCCESSFUL)
     assert (len(upscale_res.data.imgs_bytes) == 1)
     img = Image.open(io.BytesIO(upscale_res.data.imgs_bytes[0]))
-    assert img.size == (768, 768)
+    assert img.size == (768, 768)
+
+
+def test_txt2img_custom_headers():
+    client = OmniClient(os.getenv('OMNI_API_KEY'))
+    client.set_extra_headers({"User-Agent": "test-custom-user-agent"})
+
+    res = client.sync_img2img(Img2ImgRequest(
+        model_name='dreamshaper_8_93211.safetensors',
+        prompt='a dog flying in the sky',
+        width=512,
+        height=512,
+        batch_size=1,
+        cfg_scale=7.5,
+        sampler_name=Samplers.EULER_A,
+    ))
+
+    assert (res.data.status == ProgressResponseStatusCode.SUCCESSFUL)
+    assert (len(res.data.imgs_bytes) == 1)
```

### Comparing `omniinfer_client-0.3.0/tests/test_model.py` & `omniinfer_client-0.3.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/.gitignore` & `omniinfer_client-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/LICENSE` & `omniinfer_client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/README.md` & `omniinfer_client-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.3.0/pyproject.toml` & `omniinfer_client-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omniinfer_client"
-version = "0.3.0"
+version = "0.3.1"
 description = "Omniinfer SDK for Python"
 authors = [
     { name = "Omniinfer", email = "omniinfer@gmail.com" }
 ]
 
 
 dependencies = [
```

### Comparing `omniinfer_client-0.3.0/PKG-INFO` & `omniinfer_client-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniinfer_client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Omniinfer SDK for Python
 Project-URL: Homepage, https://github.com/omniinfer/python-sdk
 Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: Omniinfer <omniinfer@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 omniinfer.io
```

