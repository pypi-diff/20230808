# Comparing `tmp/ffmpegcv-0.3.5.tar.gz` & `tmp/ffmpegcv-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.3.5.tar", last modified: Tue Jun 27 10:33:37 2023, max compression
+gzip compressed data, was "ffmpegcv-0.3.6.tar", last modified: Tue Aug  8 09:26:16 2023, max compression
```

## Comparing `ffmpegcv-0.3.5.tar` & `ffmpegcv-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12966 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12747 2023-06-27 06:23:38.000000 ffmpegcv-0.3.5/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10510 2023-06-27 05:28:52.000000 ffmpegcv-0.3.5/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      631 2023-06-27 05:41:10.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2513 2023-06-27 10:16:24.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     4128 2023-06-26 16:58:44.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2606 2023-06-27 09:58:14.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.5/ffmpegcv/stream_info.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.5/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12966 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      519 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-27 10:29:42.000000 ffmpegcv-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:26:16.602591 ffmpegcv-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-08 09:26:16.602591 ffmpegcv-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:26:16.602591 ffmpegcv-0.3.6/ffmpegcv/
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_stream_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_writer_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/ffmpeg_writer_stream_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/stream_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/ffmpegcv/video_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:26:16.602591 ffmpegcv-0.3.6/ffmpegcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-08 09:26:16.000000 ffmpegcv-0.3.6/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 09:26:16.000000 ffmpegcv-0.3.6/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:26:16.000000 ffmpegcv-0.3.6/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 09:26:16.000000 ffmpegcv-0.3.6/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 09:26:16.000000 ffmpegcv-0.3.6/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:26:16.602591 ffmpegcv-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-08 09:26:03.000000 ffmpegcv-0.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ffmpegcv-0.3.5/PKG-INFO` & `ffmpegcv-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
```

### Comparing `ffmpegcv-0.3.5/README.md` & `ffmpegcv-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.5/ffmpegcv/__init__.py` & `ffmpegcv-0.3.6/ffmpegcv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from .ffmpeg_reader import FFmpegReader, FFmpegReaderNV
 from .ffmpeg_writer import FFmpegWriter, FFmpegWriterNV
 from .ffmpeg_reader_camera import FFmpegReaderCAM
 from .ffmpeg_reader_stream import FFmpegReaderStream
+from .ffmpeg_reader_stream_realtime import FFmpegReaderStreamRT
+from .ffmpeg_writer_stream_realtime import FFmpegWriterStreamRT
 from .ffmpeg_noblock import noblock
 from .video_info import get_num_NVIDIA_GPUs
 import shutil
 from subprocess import DEVNULL, check_output
 
 
 def _check():
@@ -240,14 +242,18 @@
     """
     `ffmpegcv.VideoWriterNV` is a gpu version for `ffmpegcv.VideoWriter`.
     """
     _check_nvidia()
     return FFmpegWriterNV.VideoWriter(file, codec, fps, frameSize, pix_fmt, gpu)
 
 
+def VideoWriterStreamRT(url, pix_fmt="bgr24", bitrate=None):
+    return FFmpegWriterStreamRT.VideoWriter(url, 'libx264', pix_fmt, bitrate)
+
+
 def VideoCaptureCAM(
     camname,
     pix_fmt="bgr24",
     crop_xywh=None,
     resize=None,
     resize_keepratio=True,
     resize_keepratioalign="center",
@@ -396,7 +402,18 @@
         resize,
         resize_keepratio,
         resize_keepratioalign
     )
 
 
 VideoReaderStream = VideoCaptureStream
+
+
+def VideoCaptureStreamRT(
+    stream_url,
+    pix_fmt="bgr24",
+    camsize_wh=None
+):
+    assert camsize_wh is not None
+    return FFmpegReaderStreamRT.VideoReader(stream_url, pix_fmt, camsize=camsize_wh)
+
+VideoReaderStreamRT = VideoCaptureStreamRT
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_noblock.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_noblock.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     release_process,
 )
 
 
 class FFmpegReader:
     def __init__(self):
         self.iframe = -1
+        self.waitInit = True
+        self.process = None
+        self._isopen = True
 
     def __repr__(self):
         props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
         return f"{self.__class__}\n" + props
 
     def __enter__(self):
         return self
@@ -110,17 +113,15 @@
         else:
             filteropt = ""
 
         vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning "
             f' -vcodec {vid.codec} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
-        )
-
-        vid.process = run_async(vid.ffmpeg_cmd)
+        )  
         vid.size = (vid.width, vid.height)
         vid.pix_fmt = pix_fmt
         assert (not pix_fmt == "yuv420p") or (
             vid.height % 2 == 0 and vid.width % 2 == 0
         ), "yuv420p must be even"
         vid.out_numpy_shape = {
             "rgb24": (vid.height, vid.width, 3),
@@ -143,23 +144,31 @@
         if not ret:
             return False, None
         assert img.shape == (int(self.height * 1.5), self.width)
         img_gray = img[: self.height, :, None]
         return True, img_gray
 
     def read(self):
+        if self.waitInit:
+            self.process = run_async(self.ffmpeg_cmd)
+            self.waitInit = False
+            
         in_bytes = self.process.stdout.read(np.prod(self.out_numpy_shape))
         if not in_bytes:
             self.release()
             return False, None
         self.iframe += 1
         img = np.frombuffer(in_bytes, np.uint8).reshape(self.out_numpy_shape)
         return True, img
 
+    def isOpened(self):
+        return self._isopen
+
     def release(self):
+        self._isopen = False
         release_process(self.process)
 
     def close(self):
         return self.release()
 
 
 class FFmpegReaderNV(FFmpegReader):
@@ -263,15 +272,14 @@
 
         vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning -hwaccel cuda -hwaccel_device {gpu} "
             f' -vcodec {vid.codecNV} {cropopt} {scaleopt} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
         )
 
-        vid.process = run_async(vid.ffmpeg_cmd)
         vid.pix_fmt = pix_fmt
         assert (not pix_fmt == "yuv420p") or (
             vid.height % 2 == 0 and vid.width % 2 == 0
         ), "yuv420p must be even"
         vid.out_numpy_shape = {
             "rgb24": (vid.height, vid.width, 3),
             "bgr24": (vid.height, vid.width, 3),
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,28 +201,29 @@
     def __init__(self, vid, q):
         super(ProducerThread, self).__init__()
         self.vid = vid
         self.q = q
 
     def run(self):
         while True:
-            if not self.vid.isopened:
+            if not self.vid.isOpened():
                 break
             ret, img = self.vid.read_()
 
             try:
                 self.q.put_nowait((ret, img))  # drop frames
             except Exception:
                 pass
             continue
 
 
 class FFmpegReaderCAM:
     def __init__(self):
         self.iframe = -1
+        self._isopen = True
 
     def __repr__(self):
         props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
         return f"{self.__class__}\n" + props
 
     def __enter__(self):
         return self
@@ -390,16 +391,14 @@
             "rgb24": (vid.height, vid.width, 3),
             "bgr24": (vid.height, vid.width, 3),
             "yuv420p": (int(vid.height * 1.5), vid.width),
             "nv12": (int(vid.height * 1.5), vid.width),
         }[pix_fmt]
         vid.process = run_async(args)
 
-        vid.isopened = True
-
         # producer
         assert step >= 1 and isinstance(step, int)
         vid.step = step
         vid.q = Queue(maxsize=30)
         producer = ProducerThread(vid, vid.q)
         producer.start()
         return vid
@@ -428,13 +427,16 @@
         img_gray = img[: self.height, :, None]
         return True, img_gray
 
     def read(self):
         ret, img = self.q.get()
         return ret, img
 
+    def isOpened(self):
+        return self._isopen
+    
     def release(self):
-        self.isopened = False
+        self._isopen = False
         release_process(self.process)
 
     def close(self):
         return self.release()
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_noblock.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_noblock.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
                  vcap_fun,
                  *vcap_args, **vcap_kwargs):
         vid:FFmpegReader = vcap_fun(*vcap_args, **vcap_kwargs)
         vid.release()
 
         # work like normal FFmpegReaderObj
         props_name = ['width', 'height', 'fps', 'count', 'codec', 'ffmpeg_cmd',
-                      'size', 'pix_fmt', 'out_numpy_shape', 'iframe']
+                      'size', 'pix_fmt', 'out_numpy_shape', 'iframe', 
+                      'origin_width', 'origin_height']
         for name in props_name:
             setattr(self, name, getattr(vid, name, None))
         
         # 创建共享内存的NumPy数组
         shared_array = multiprocessing.Array('b', int(NFRAME*np.prod(self.out_numpy_shape)))
 
         # 将共享内存的NumPy数组转换为NumPy数组
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_stream.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_reader_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         stream_url,
         pix_fmt,
         crop_xywh,
         resize,
         resize_keepratio,
         resize_keepratioalign,
     ):
-        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12", "gray"]
         vid = FFmpegReaderStream()
         videoinfo = get_info(stream_url)
         vid.width, vid.height = videoinfo.width, videoinfo.height
         vid.fps = videoinfo.fps
         vid.codec = videoinfo.codec
         vid.count = videoinfo.count
         vid.duration = videoinfo.duration
@@ -66,37 +66,39 @@
                 }
                 assert (
                     resize_keepratioalign in paddings
                 ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
                 padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
 
-        if any([cropopt, scaleopt, padopt]):
-            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt] if x)
+        pix_fmtopt = 'extractplanes=y' if pix_fmt=='gray' else ''
+        if any([cropopt, scaleopt, padopt, pix_fmtopt]):
+            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt, pix_fmtopt] if x)
             filteropt = f"-vf {filterstr}"
         else:
             filteropt = ""
 
-        args = (
+        vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning "
             f' -vcodec {vid.codec} -i {stream_url} '
             f" {filteropt} -pix_fmt {pix_fmt}  -f rawvideo pipe:"
         )
         vid.size = (vid.width, vid.height)
         vid.pix_fmt = pix_fmt
         assert (not pix_fmt == "yuv420p") or (
             vid.height % 2 == 0 and vid.width % 2 == 0
         ), "yuv420p must be even"
         vid.out_numpy_shape = {
             "rgb24": (vid.height, vid.width, 3),
             "bgr24": (vid.height, vid.width, 3),
             "nv12": (int(vid.height * 1.5), vid.width),
             "yuv420p": (int(vid.height * 1.5), vid.width),
+            "gray": (vid.height, vid.width, 1)
         }[pix_fmt]
-        vid.process = run_async(args)
+        vid.process = run_async(vid.ffmpeg_cmd)
 
         vid.isopened = True
 
         # producer
         vid.step = 1
         vid.q = Queue(maxsize=30)
         producer = ProducerThread(vid, vid.q)
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 IN_COLAB = "google.colab" in sys.modules
 
 
 class FFmpegWriter:
     def __init__(self):
         self.iframe = -1
+        self.size = None
+        self.waitInit = True
+        self._isopen = True
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.release()
 
@@ -38,15 +41,14 @@
                 """
             )
 
         vid = FFmpegWriter()
         vid.fps, vid.size = fps, frameSize
         vid.width, vid.height = vid.size if vid.size else (None, None)
         vid.codec, vid.pix_fmt, vid.filename = codec, pix_fmt, filename
-        vid.waitInit = True
         vid.bitrate = bitrate
         return vid
 
     def _init_video_stream(self):
         bitrate_str = f'-b:v {self.bitrate} ' if self.bitrate else ''
         self.ffmpeg_cmd = (f'ffmpeg -y -loglevel warning ' 
                 f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
@@ -63,15 +65,19 @@
             self.waitInit = False
 
         self.iframe += 1
         assert self.size == (img.shape[1], img.shape[0])
         img = img.astype(np.uint8).tobytes()
         self.process.stdin.write(img)
 
+    def isOpened(self):
+        return self._isopen
+
     def release(self):
+        self._isopen = False
         if hasattr(self, "process"):
             release_process(self.process)
 
     def close(self):
         return self.release()
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer_noblock.py` & `ffmpegcv-0.3.6/ffmpegcv/ffmpeg_writer_noblock.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.5/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.6/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.5/ffmpegcv/video_info.py` & `ffmpegcv-0.3.6/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.5/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.6/ffmpegcv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
```

### Comparing `ffmpegcv-0.3.5/ffmpegcv.egg-info/SOURCES.txt` & `ffmpegcv-0.3.6/ffmpegcv.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 README.md
 setup.py
 ffmpegcv/__init__.py
-ffmpegcv/ffmpeg_framepick.py
 ffmpegcv/ffmpeg_noblock.py
 ffmpegcv/ffmpeg_reader.py
 ffmpegcv/ffmpeg_reader_camera.py
-ffmpegcv/ffmpeg_reader_laggy.py
 ffmpegcv/ffmpeg_reader_noblock.py
 ffmpegcv/ffmpeg_reader_stream.py
+ffmpegcv/ffmpeg_reader_stream_realtime.py
 ffmpegcv/ffmpeg_writer.py
 ffmpegcv/ffmpeg_writer_noblock.py
+ffmpegcv/ffmpeg_writer_stream_realtime.py
 ffmpegcv/stream_info.py
 ffmpegcv/video_info.py
 ffmpegcv.egg-info/PKG-INFO
 ffmpegcv.egg-info/SOURCES.txt
 ffmpegcv.egg-info/dependency_links.txt
 ffmpegcv.egg-info/requires.txt
 ffmpegcv.egg-info/top_level.txt
```

### Comparing `ffmpegcv-0.3.5/setup.py` & `ffmpegcv-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.5', # 版本号
+    version='0.3.6', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://github.com/chenxinfeng4/ffmpegcv',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

