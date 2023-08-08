# Comparing `tmp/dx_profiler-0.1.0.tar.gz` & `tmp/dx_profiler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dx_profiler-0.1.0.tar", max compression
+gzip compressed data, was "dx_profiler-0.1.1.tar", max compression
```

## Comparing `dx_profiler-0.1.0.tar` & `dx_profiler-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1473 2023-07-26 07:47:35.674613 dx_profiler-0.1.0/README.md
--rw-r--r--   0        0        0     3887 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/dx_profiler/cli.py
--rw-r--r--   0        0        0      556 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/file_writer.py
--rw-r--r--   0        0        0     1784 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/inference.py
--rw-r--r--   0        0        0     1024 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/nats_listener.py
--rw-r--r--   0        0        0     9352 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/player/player.py
--rw-r--r--   0        0        0     8818 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2.py
--rw-r--r--   0        0        0    10004 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2.pyi
--rw-r--r--   0        0        0    25768 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2_grpc.py
--rw-r--r--   0        0        0      692 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 dx_profiler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1473 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/README.md
+-rw-r--r--   0        0        0     4140 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/dx_profiler/cli.py
+-rw-r--r--   0        0        0      556 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/inference/file_writer.py
+-rw-r--r--   0        0        0     1784 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/inference/inference.py
+-rw-r--r--   0        0        0     1024 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/inference/nats_listener.py
+-rw-r--r--   0        0        0    11326 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/player/player.py
+-rw-r--r--   0        0        0     8818 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/proto_py/dx_pb2.py
+-rw-r--r--   0        0        0    10004 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/proto_py/dx_pb2.pyi
+-rw-r--r--   0        0        0    25768 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/proto_py/dx_pb2_grpc.py
+-rw-r--r--   0        0        0      665 2023-08-08 02:04:21.771027 dx_profiler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 dx_profiler-0.1.1/PKG-INFO
```

### Comparing `dx_profiler-0.1.0/README.md` & `dx_profiler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/dx_profiler/cli.py` & `dx_profiler-0.1.1/dx_profiler/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 async def cli_inference(file_path: Annotated[Path, typer.Option('-F', '--file', help='Input file path.')],
                   app_path: Annotated[Path, typer.Option('-A', '--app', help='Input app path.')],
                   output_path: Annotated[Path, typer.Option('-O', '--output', help='Store inference result.')]):
     """
     Inference video, save log.
     """
     # 파일 확인
+    if not os.geteuid() == 0:
+        print('Run with root privileged.')
+        raise typer.Exit(-1)
+
     if not file_path.exists():
         print(f'{file_path} is not exist.')
         raise typer.Exit(-1)
     
     if not app_path.exists():
         print(f'{app_path} is not exist.')
         raise typer.Exit(-1)
@@ -112,35 +116,33 @@
     await asyncio.sleep(0)
     await write_task
 
     print('Done.')
     
 
 @app.command('profile')
-def cli_profile(input_path: Annotated[Path, typer.Option('-F', '--file', help='Input file path.')]):
+def cli_profile(input_path: Annotated[Path, typer.Option('-F', '--file', help='Input file path.')],
+                draw_obj: Annotated[str, typer.Option('-O', '--obj', help='Input object_name "bbox" or "bboxd"')],
+                save_path: Annotated[str, typer.Option('-S', '--save', help='Input save video_path')] = None):
     """
     Play video with inference log info.
     """
     # 파일 확인
     if not input_path.exists():
         print(f'{input_path} is not exist.')
         raise typer.Exit(-1)
     
     print(f'input file: {input_path}')
 
     app = QApplication(sys.argv)
 
-    player = text_input_player(input_path)
+    if not save_path:
+        save_path = None
+
+    player = text_input_player(input_path, draw_obj, save_path)
     
     player.show()
     sys.exit(app.exec_())
 
 
-@app.callback()
-def check_privileged():
-    if not os.geteuid() == 0:
-        print('Run with root privileged.')
-        raise typer.Exit(-1)
-
-
 if __name__ == '__main__':
     app()
```

### Comparing `dx_profiler-0.1.0/inference/file_writer.py` & `dx_profiler-0.1.1/inference/file_writer.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/inference/inference.py` & `dx_profiler-0.1.1/inference/inference.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/inference/nats_listener.py` & `dx_profiler-0.1.1/inference/nats_listener.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/player/player.py` & `dx_profiler-0.1.1/player/player.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 import sys
+import numpy as np
 from collections import defaultdict
 
 import cv2
-from PyQt5.QtCore import Qt, QTimer
+from PyQt5.QtCore import Qt, QTimer, pyqtSignal
 from PyQt5.QtGui import QImage, QPixmap, QPainter, QPen
 from PyQt5.QtWidgets import QApplication, QMainWindow, QLabel, QDesktopWidget, \
 QProgressBar, QHBoxLayout, QVBoxLayout, QWidget, QPushButton
 
-
+RED = (255, 0, 0)
+GREEN = (0, 255, 0)
+font = cv2.FONT_HERSHEY_SIMPLEX
 VIDEO_EXTENSIONS = [".avi", ".mp4", ".mov"]
 
 
+class ClickProgressBar(QProgressBar):
+    clicked = pyqtSignal(int)
+
+    def mousePressEvent(self, event):
+        # Calculate the new value based on the click position
+        click_position = event.pos().x()
+        total_width = self.width()
+        new_value = int(self.minimum() + click_position / total_width * (self.maximum() - self.minimum()))
+
+        # Emit the clickedValue signal with the new value
+        self.clicked.emit(new_value)
+
 class VideoPlayer(QMainWindow):
     """Dx Video Player
 
     동영상 파일에 record.txt을 통해, 후처리를 한 Video를 관리하는 클래스.
     Space-bar로 동영상 재생 및 정지, Q/E 를 통해 Frame 이동 등의 기능을 제공한다.
 
     Attributes:
@@ -31,15 +46,15 @@
         playing (bool): 동영상이 재생이면 True, 정지면 False.
         scaled_width (int): resize 된  video label의 width.
         scaled_height (int): resize 된 video_label의 height.
         data (List[Dict]): dict 형태의 record 정보가 들어있는 data list.
                         bbox, id, label, classifier 등이 존재.
     """
 
-    def __init__(self, video_path: str, record: str, st_time_stamp: int) -> None:
+    def __init__(self, video_path: str, record: str, st_time_stamp: int, drawing:str = "bbox", save_path: str = None) -> None:
         """
         Args:
             video_path: 동영상 파일의 경로
             record: object message의 내용
             st_time_stamp: 동영상 시작 시간의 time-stamp ex) 1690210800
 
         Raises:
@@ -57,22 +72,25 @@
         self.cap = cv2.VideoCapture(video_path)
 
         if not self.cap.isOpened():
             raise Exception # OpenError : 동영상이 열리지 않음
         
         self.fps = int(self.cap.get(cv2.CAP_PROP_FPS))
         self.total_frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        self.drawing=drawing
+        self.save_path = save_path
 
         self.video_label = QLabel(self)
         self.video_label.setAlignment(Qt.AlignCenter)
 
-        self.progress_bar = QProgressBar(self)
+        self.progress_bar = ClickProgressBar(self)
         self.progress_bar.setTextVisible(False)
         self.progress_bar.setMaximum(self.total_frames)
         self.progress_bar.setValue(0)
+        self.progress_bar.clicked .connect(self.set_frame)
 
         self.start_stop_button = QPushButton("II", self)
         self.start_stop_button.clicked.connect(self.toggle_video)
         self.start_stop_button.setGeometry(10, 10, 100, 30)
 
         button_layout = QHBoxLayout()
         button_layout.addWidget(self.start_stop_button)
@@ -101,15 +119,23 @@
 
         # 나노 시간 처리 후에, 시작 time_stamp 값을 빼서 초(second)를 구합니다.
         # 초(second)에다가 fps 값을 곱해 frame_number를 구합니다.
         for line in record:
             line_data = eval(line)
             time_in_seconds = (line_data["metadata"]["timestamp"] / 1e9) - st_time_stamp
             frame_num = int(time_in_seconds * self.fps)
+            self.data[frame_num-1].append(line_data["objects"])
             self.data[frame_num].append(line_data["objects"])
+            self.data[frame_num+1].append(line_data["objects"])
+
+        if save_path is not None:
+            self.frame_width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+            self.frame_height = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+            fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+            self.out = cv2.VideoWriter(save_path,fourcc,self.fps,(self.frame_width,self.frame_height))
 
     def toggle_video(self):
         # video의 상태를 전환. 정지 -> 재생, 재생 -> 정지
         # 재생 -> 정지 시에는 timer는 정지.
         # 정지 -> 재생 시에는 timer를 다시 시작.
         if self.playing:
             self.timer.stop()
@@ -117,130 +143,145 @@
         
         else:
             self.timer.start(1000 // self.fps)
             self.start_stop_button.setText("II")
         
         self.playing = not self.playing
 
+    def set_frame(self, value):
+        self.current_frame = value - 1
+        self.cap.set(cv2.CAP_PROP_POS_FRAMES, self.current_frame)
+        self.update_frame()
+
     def update_frame(self):
         # frame을 하나 읽어들임
         # 현재 gui window의 size를 받아들여 frame을 resize.
                             # current_frame 값에 있는 data를 가져와서 id, label등을 draw.
         # frame 업데이트.
 
         ret, frame = self.cap.read()
         self.current_frame += 1
 
         if ret:
             frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-            h, w, ch = frame.shape
+            H, W, CH = frame.shape
 
             # GUI 창의 크기를 가져와서 비율에 맞게 영상 크기를 조절
             window_width = self.video_label.width()
             window_height = self.video_label.height()
-            aspect_ratio = w / h
+
+            aspect_ratio = W / H
 
             if window_width / window_height > aspect_ratio:
                 self.scaled_width = int(window_height * aspect_ratio)
                 self.scaled_height = window_height
             
             else:
                 self.scaled_width = window_width
                 self.scaled_height = int(window_width / aspect_ratio)
 
             frame = cv2.resize(frame, (self.scaled_width, self.scaled_height))
 
-            bytes_per_line = ch * self.scaled_width
-            q_image = QImage(frame.data, self.scaled_width, self.scaled_height, bytes_per_line, QImage.Format_RGB888)
-            
-            painter = QPainter(q_image)
-            red_pen = QPen(Qt.red, 3)
-            green_pen = QPen(Qt.green, 2)
-            
-            if self.current_frame in self.data: # 현재 frame에 해당하는 값의 정보들을 draw
+            if self.current_frame in self.data:
                 data = self.data[self.current_frame]
 
-                for datum in data:
-                    datum = datum[0]
-                    painter.setPen(red_pen)
-                    
-                    bbox = datum["bbox"]
-                    x, y, w, h = bbox["x"], bbox["y"], bbox["w"], bbox["h"]
-                    x, y, w, h = x * self.scaled_width, y * self.scaled_height, \
-                                    w * self.scaled_width, h * self.scaled_height
-
-                    if datum["id"] >= 10000:
-                        datum["id"] = -1
-
-                    x, y, w, h = map(int, [x, y, w, h])
-                    painter.drawRect(x, y, w, h)
-                    
-                    if datum["id"] != -1:
-                        painter.drawText(x, y-10, f"[{datum['id']}] {datum['label']}")
-                    else:
-                        painter.drawText(x, y-10, f"[None] {datum['label']}")
-
-                    painter.setPen(green_pen)
-
-                    drawing_texts = []
-
-                    if "classifiers" in datum:
-                        for idx, val in enumerate(datum["classifiers"]):
-                            drawing_texts.append(f"[{val['label']}] {val['type']}")
-                    
-                    if "score_d" in datum:
+                for datum_ in data:
+                    for datum in datum_:
+                        bbox = datum[self.drawing]
+                        x, y, w, h = bbox["x"], bbox["y"], bbox["w"], bbox["h"]
+                        x, y, w, h = x * self.scaled_width, y * self.scaled_height, w * self.scaled_width, h * self.scaled_height
+
+                        if datum["id"] >= 10000:
+                            datum["id"] = -1
+
+                        x, y, w, h = map(int, [x, y, w, h])
+                        cv2.rectangle(frame, (x, y), (x + w, y + h), RED, 3)
+
+                        if datum["id"] != -1:
+                            cv2.putText(frame, f"[{datum['id']}] {datum['label']}", (x, y-10), font, 1, GREEN, 2)
+                        else:
+                            cv2.putText(frame, f"[None] {datum['label']}", (x, y - 10), font, 1, GREEN, 2)
+
+                        drawing_texts = []
+
+                        if "classifiers" in datum:
+                            for idx, val in enumerate(datum["classifiers"]):
+                                drawing_texts.append(f"[{val['label']}] {val['type']}")
+
+                        if "score_d" in datum:
                             drawing_texts.append(f"Score: {datum['score_d']:.2f}")
-                    
-                    for idx, val in enumerate(drawing_texts):
-                        painter.drawText(x, y + (idx+1)*15, val)
 
-            painter.end()
+                        for idx, val in enumerate(drawing_texts):
+                            cv2.putText(frame, val, (x, y + (idx+1)*25), font, 1, GREEN, 2)
+
+            if self.save_path is not None:
+                resize_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                resize_frame = cv2.resize(resize_frame, (self.frame_width, self.frame_height))
+                self.out.write(resize_frame)
+
+            bytes_per_line = CH * self.scaled_width
+            q_image = QImage(frame.data, self.scaled_width, self.scaled_height, bytes_per_line, QImage.Format_RGB888)
             pixmap = QPixmap.fromImage(q_image)
+
             self.video_label.setPixmap(pixmap)
-            self.progress_bar.setValue(self.current_frame)
+            self.progress_bar.setValue(self.current_frame)  
 
         else:
             # exit
             self.timer.stop()
             self.cap.release()
             self.close()
+            if self.save_path is not None:
+                self.out.release()
 
     def keyPressEvent(self, event):
         if event.key() == Qt.Key_Space:
             self.toggle_video()
         
         elif event.key() == Qt.Key_Q:  # 이전 프레임으로 이동
             self.current_frame -= 2
             self.cap.set(cv2.CAP_PROP_POS_FRAMES, self.current_frame)
             self.update_frame()
 
         elif event.key() == Qt.Key_E:  # 다음 프레임으로 이동
             self.update_frame()
 
+        elif event.key() == Qt.Key_A:
+            self.current_frame -= 11
+            self.cap.set(cv2.CAP_PROP_POS_FRAMES, self.current_frame)
+            self.update_frame()
+
+        elif event.key() == Qt.Key_D:
+            self.current_frame += 9
+            self.cap.set(cv2.CAP_PROP_POS_FRAMES, self.current_frame)
+            self.update_frame()
+
     def closeEvent(self, event):
         self.cap.release()
         self.timer.stop()
+        if self.save_path is not None:
+            self.out.release()
 
 
-def text_input_player(text: str):
+def text_input_player(text: str, drawing: str = "bbox", save_path: str = None):
     """text 파일로 Videoplayer에 입력.
     
     첫 번째 줄, 영상 파일 경로
     두 번째 줄, timestamp (second)
     세번 째 줄 ~, 오브젝트 메시지
 
     Args:
         text: 위에 내용으로 구성된 text
     """
     with open(text, "r") as f:
         video_path = f.readline().strip()
         st_time_stamp = int(f.readline().strip())
         record = f.readlines()
     
-    return VideoPlayer(video_path, record, st_time_stamp)
+    return VideoPlayer(video_path, record, st_time_stamp, drawing, save_path)
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    player = text_input_player("sample.txt")
+    player = text_input_player("last.txt", drawing="bboxd", save_path="/home/daki/hello.mp4")
     player.show()
     sys.exit(app.exec_())
```

### Comparing `dx_profiler-0.1.0/proto_py/dx_pb2.py` & `dx_profiler-0.1.1/proto_py/dx_pb2.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/proto_py/dx_pb2.pyi` & `dx_profiler-0.1.1/proto_py/dx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/proto_py/dx_pb2_grpc.py` & `dx_profiler-0.1.1/proto_py/dx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.1.0/PKG-INFO` & `dx_profiler-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dx-profiler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Profile Dx App
 Author: SangHyeukYoon
 Author-email: shyoon@snuailab.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.56.2,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.56.2,<2.0.0)
 Requires-Dist: nats-py (>=2.3.1,<3.0.0)
-Requires-Dist: opencv-python (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: opencv-python-headless (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Waffle Profiler
 Dx 인퍼런스 분석 툴
```

