# Comparing `tmp/sq-GUI-0.0.1.tar.gz` & `tmp/sq-GUI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sq-GUI-0.0.1.tar", last modified: Tue Aug  8 14:02:51 2023, max compression
+gzip compressed data, was "sq-GUI-0.0.2.tar", last modified: Tue Aug  8 14:21:25 2023, max compression
```

## Comparing `sq-GUI-0.0.1.tar` & `sq-GUI-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:02:51.807451 sq-GUI-0.0.1/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1074 2023-08-08 00:55:29.000000 sq-GUI-0.0.1/LICENSE
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1387 2023-08-08 14:02:51.803451 sq-GUI-0.0.1/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1047 2023-08-08 14:01:38.000000 sq-GUI-0.0.1/README.md
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      324 2023-08-08 14:02:30.000000 sq-GUI-0.0.1/pyproject.toml
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2023-08-08 14:02:51.807451 sq-GUI-0.0.1/setup.cfg
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:02:51.787452 sq-GUI-0.0.1/src/
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:02:51.791452 sq-GUI-0.0.1/src/GUI/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 00:41:33.000000 sq-GUI-0.0.1/src/GUI/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      890 2023-08-08 13:12:21.000000 sq-GUI-0.0.1/src/GUI/sq.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:02:51.803451 sq-GUI-0.0.1/src/sq_GUI.egg-info/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1387 2023-08-08 14:02:51.000000 sq-GUI-0.0.1/src/sq_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      202 2023-08-08 14:02:51.000000 sq-GUI-0.0.1/src/sq_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2023-08-08 14:02:51.000000 sq-GUI-0.0.1/src/sq_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2023-08-08 14:02:51.000000 sq-GUI-0.0.1/src/sq_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:21:25.530240 sq-GUI-0.0.2/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1074 2023-08-08 00:55:29.000000 sq-GUI-0.0.2/LICENSE
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1810 2023-08-08 14:21:25.530240 sq-GUI-0.0.2/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1470 2023-08-08 14:18:05.000000 sq-GUI-0.0.2/README.md
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      324 2023-08-08 14:07:49.000000 sq-GUI-0.0.2/pyproject.toml
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2023-08-08 14:21:25.530240 sq-GUI-0.0.2/setup.cfg
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:21:25.518240 sq-GUI-0.0.2/src/
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:21:25.522240 sq-GUI-0.0.2/src/GUI/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 00:41:33.000000 sq-GUI-0.0.2/src/GUI/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1314 2023-08-08 14:17:39.000000 sq-GUI-0.0.2/src/GUI/sq.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2023-08-08 14:21:25.526240 sq-GUI-0.0.2/src/sq_GUI.egg-info/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1810 2023-08-08 14:21:25.000000 sq-GUI-0.0.2/src/sq_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      202 2023-08-08 14:21:25.000000 sq-GUI-0.0.2/src/sq_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2023-08-08 14:21:25.000000 sq-GUI-0.0.2/src/sq_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2023-08-08 14:21:25.000000 sq-GUI-0.0.2/src/sq_GUI.egg-info/top_level.txt
```

### Comparing `sq-GUI-0.0.1/LICENSE` & `sq-GUI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sq-GUI-0.0.1/PKG-INFO` & `sq-GUI-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sq-GUI
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI para Square Cloud usando API!
 Author: Jetrom
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -17,46 +17,55 @@
 ```
 squarecloud
 ```
 
 O status da plataforma https://squarecloud.dev virá no formato *json* com uma interface gráfica.
 
 ```py
+import argparse
 import PySimpleGUI as sg
 import requests
 import json
 
 theme_name = "Tan"
 
-def get_api_data():
+def get_api_data(argument):
     url = "https://api.squarecloud.app/v2/service/statistics"
     response = requests.get(url)
     if response.status_code == 200:
         return response.json()
     else:
         return None
 
-layout = [
-    [sg.Text("Status da Square Cloud")],
-    [sg.Button("Get")],
-    [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
-]
-
-sg.theme(theme_name)
-
-window = sg.Window("Square Cloud", layout)
-
-while True:
-    event, values = window.read()
-    if event == sg.WINDOW_CLOSED:
-        break
-    elif event == "Get":
-        api_data = get_api_data()
-        if api_data:
-            formatted_data = json.dumps(api_data, indent=4) 
-            window["-OUTPUT-"].update(formatted_data)
-        else:
-            window["-OUTPUT-"].update("Erro ao obter dados da API.")
+parser = argparse.ArgumentParser(description="Obter status da Square Cloud")
+parser.add_argument("-s", "--service", dest="service", default="squarecloud", help="O serviço da API Square Cloud a ser usado")
 
-window.close()
+args = parser.parse_args()
 
+if args.service == "squarecloud":
+    layout = [
+        [sg.Text("Status da Square Cloud")],
+        [sg.Button("Get")],
+        [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
+    ]
+
+    sg.theme(theme_name)
+
+    window = sg.Window("Square Cloud", layout)
+
+    while True:
+        event, values = window.read()
+        if event == sg.WINDOW_CLOSED:
+            break
+        elif event == "Get":
+            api_data = get_api_data(args.service)
+            if api_data:
+                formatted_data = json.dumps(api_data, indent=4)
+                window["-OUTPUT-"].update(formatted_data)
+            else:
+                window["-OUTPUT-"].update("Erro ao obter dados da API.")
+
+    window.close()
+
+else:
+    print("Serviço não suportado")
 ```
```

### Comparing `sq-GUI-0.0.1/README.md` & `sq-GUI-0.0.2/src/GUI/sq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# O GUI
-
-Tente executar:
-
-```
-squarecloud
-```
-
-O status da plataforma https://squarecloud.dev virá no formato *json* com uma interface gráfica.
-
-```py
+import argparse
 import PySimpleGUI as sg
 import requests
 import json
 
 theme_name = "Tan"
 
-def get_api_data():
+def get_api_data(argument):
     url = "https://api.squarecloud.app/v2/service/statistics"
     response = requests.get(url)
     if response.status_code == 200:
         return response.json()
     else:
         return None
 
-layout = [
-    [sg.Text("Status da Square Cloud")],
-    [sg.Button("Get")],
-    [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
-]
-
-sg.theme(theme_name)
-
-window = sg.Window("Square Cloud", layout)
-
-while True:
-    event, values = window.read()
-    if event == sg.WINDOW_CLOSED:
-        break
-    elif event == "Get":
-        api_data = get_api_data()
-        if api_data:
-            formatted_data = json.dumps(api_data, indent=4) 
-            window["-OUTPUT-"].update(formatted_data)
-        else:
-            window["-OUTPUT-"].update("Erro ao obter dados da API.")
+parser = argparse.ArgumentParser(description="Obter status da Square Cloud")
+parser.add_argument("-s", "--service", dest="service", default="squarecloud", help="O serviço da API Square Cloud a ser usado")
+
+args = parser.parse_args()
+
+if args.service == "squarecloud":
+    layout = [
+        [sg.Text("Status da Square Cloud")],
+        [sg.Button("Get")],
+        [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
+    ]
+
+    sg.theme(theme_name)
+
+    window = sg.Window("Square Cloud", layout)
+
+    while True:
+        event, values = window.read()
+        if event == sg.WINDOW_CLOSED:
+            break
+        elif event == "Get":
+            api_data = get_api_data(args.service)
+            if api_data:
+                formatted_data = json.dumps(api_data, indent=4)
+                window["-OUTPUT-"].update(formatted_data)
+            else:
+                window["-OUTPUT-"].update("Erro ao obter dados da API.")
+
+    window.close()
 
-window.close()
+else:
+    print("Serviço não suportado")
 
-```
```

### Comparing `sq-GUI-0.0.1/src/sq_GUI.egg-info/PKG-INFO` & `sq-GUI-0.0.2/src/sq_GUI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sq-GUI
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI para Square Cloud usando API!
 Author: Jetrom
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -17,46 +17,55 @@
 ```
 squarecloud
 ```
 
 O status da plataforma https://squarecloud.dev virá no formato *json* com uma interface gráfica.
 
 ```py
+import argparse
 import PySimpleGUI as sg
 import requests
 import json
 
 theme_name = "Tan"
 
-def get_api_data():
+def get_api_data(argument):
     url = "https://api.squarecloud.app/v2/service/statistics"
     response = requests.get(url)
     if response.status_code == 200:
         return response.json()
     else:
         return None
 
-layout = [
-    [sg.Text("Status da Square Cloud")],
-    [sg.Button("Get")],
-    [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
-]
-
-sg.theme(theme_name)
-
-window = sg.Window("Square Cloud", layout)
-
-while True:
-    event, values = window.read()
-    if event == sg.WINDOW_CLOSED:
-        break
-    elif event == "Get":
-        api_data = get_api_data()
-        if api_data:
-            formatted_data = json.dumps(api_data, indent=4) 
-            window["-OUTPUT-"].update(formatted_data)
-        else:
-            window["-OUTPUT-"].update("Erro ao obter dados da API.")
+parser = argparse.ArgumentParser(description="Obter status da Square Cloud")
+parser.add_argument("-s", "--service", dest="service", default="squarecloud", help="O serviço da API Square Cloud a ser usado")
 
-window.close()
+args = parser.parse_args()
 
+if args.service == "squarecloud":
+    layout = [
+        [sg.Text("Status da Square Cloud")],
+        [sg.Button("Get")],
+        [sg.Multiline("", size=(30, 14), key="-OUTPUT-", disabled=True)]
+    ]
+
+    sg.theme(theme_name)
+
+    window = sg.Window("Square Cloud", layout)
+
+    while True:
+        event, values = window.read()
+        if event == sg.WINDOW_CLOSED:
+            break
+        elif event == "Get":
+            api_data = get_api_data(args.service)
+            if api_data:
+                formatted_data = json.dumps(api_data, indent=4)
+                window["-OUTPUT-"].update(formatted_data)
+            else:
+                window["-OUTPUT-"].update("Erro ao obter dados da API.")
+
+    window.close()
+
+else:
+    print("Serviço não suportado")
 ```
```

