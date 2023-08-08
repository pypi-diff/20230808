# Comparing `tmp/fyers_sdk-2.1.7.tar.gz` & `tmp/fyers_sdk-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.1.7.tar", last modified: Mon Aug  7 11:28:54 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.8.tar", last modified: Tue Aug  8 14:26:46 2023, max compression
```

## Comparing `fyers_sdk-2.1.7.tar` & `fyers_sdk-2.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 11:28:54.595658 fyers_sdk-2.1.7/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.7/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-07 11:28:54.595658 fyers_sdk-2.1.7/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.7/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 11:28:54.563658 fyers_sdk-2.1.7/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 11:28:54.591658 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    64370 2023-08-07 11:25:50.000000 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1203 2023-08-07 10:42:25.000000 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-02 11:15:05.000000 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15350 2023-08-04 05:44:36.000000 fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.7/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27374 2023-08-07 04:47:57.000000 fyers_sdk-2.1.7/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.7/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 11:28:54.587658 fyers_sdk-2.1.7/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-07 11:28:54.000000 fyers_sdk-2.1.7/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-07 11:28:54.000000 fyers_sdk-2.1.7/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-07 11:28:54.000000 fyers_sdk-2.1.7/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-08-07 11:28:54.000000 fyers_sdk-2.1.7/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-07 11:28:54.000000 fyers_sdk-2.1.7/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-07 11:28:54.595658 fyers_sdk-2.1.7/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1031 2023-08-07 09:56:51.000000 fyers_sdk-2.1.7/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-08 14:26:46.764031 fyers_sdk-2.1.8/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.8/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-08 14:26:46.764031 fyers_sdk-2.1.8/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.8/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-08 14:26:46.744031 fyers_sdk-2.1.8/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-08 14:26:46.764031 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    64145 2023-08-08 14:25:11.000000 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1203 2023-08-07 10:42:25.000000 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-02 11:15:05.000000 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15350 2023-08-04 05:44:36.000000 fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.8/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27346 2023-08-07 13:38:26.000000 fyers_sdk-2.1.8/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.8/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-08 14:26:46.764031 fyers_sdk-2.1.8/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-08 14:26:46.000000 fyers_sdk-2.1.8/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-08 14:26:46.000000 fyers_sdk-2.1.8/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-08 14:26:46.000000 fyers_sdk-2.1.8/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-08-08 14:26:46.000000 fyers_sdk-2.1.8/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-08 14:26:46.000000 fyers_sdk-2.1.8/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-08 14:26:46.764031 fyers_sdk-2.1.8/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1031 2023-08-08 14:26:38.000000 fyers_sdk-2.1.8/setup.py
```

### Comparing `fyers_sdk-2.1.7/LICENSE.txt` & `fyers_sdk-2.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/PKG-INFO` & `fyers_sdk-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.1.7
+Version: 2.1.8
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.7/README.md` & `fyers_sdk-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1039,15 +1039,15 @@
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
                                 0
                             ]
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
-                                "utf-8"
+                                "utf-8",errors='ignore'
                             )
                             self.resp[self.dp_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[self.dp_sym[topic_id]]["type"] = "dp"
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
                         self.__response_output(
                             self.resp[self.dp_sym[topic_id]], "depth"
@@ -1085,15 +1085,15 @@
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
                                 0
                             ]
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
-                                "utf-8"
+                                "utf-8",errors='ignore'
                             )
                             self.resp[self.index_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
                         self.resp[self.index_sym[topic_id]]["type"] = "if"
                         self.__response_output(
                             self.resp[self.index_sym[topic_id]], "index"
@@ -1126,16 +1126,16 @@
                         offset += 1
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
                                 0
                             ]
                             offset += 1
-                            string_data = data[offset : offset + string_len].decode(
-                                "utf-8"
+                            string_data = bytes(data[offset : offset + string_len]).decode(
+                                "utf-8" ,errors='ignore'
                             )
                             self.resp[self.scrips_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
                         self.resp[self.scrips_sym[topic_id]]["type"] = "sf"
                         self.__response_output(
                             self.resp[self.scrips_sym[topic_id]], "scrips"
@@ -1157,42 +1157,42 @@
                         if topic_id in self.scrips_sym:
                             if self.data_val[index] in self.resp[self.scrips_sym[topic_id]] and self.resp[self.scrips_sym[topic_id]][
                                 self.data_val[index]] != value and value != -2147483648:
                                 self.resp[self.scrips_sym[topic_id]][
                                     self.data_val[index]
                                 ] = value
                                 self.UpdateTick = True
-                            elif value != -2147483648:
+                            elif self.data_val[index] not in self.resp[self.scrips_sym[topic_id]] and value != -2147483648:
                                 self.resp[self.scrips_sym[topic_id]][
                                     self.data_val[index]
                                 ] = value
                                 self.UpdateTick = True
 
                             sf_flag = True
                         elif topic_id in self.index_sym:
                             if self.index_val[index] in self.resp[self.index_sym[topic_id]] and  self.resp[self.index_sym[topic_id]][self.index_val[index]] != value and value != "-2147483648":
 
                                 self.resp[self.index_sym[topic_id]][
                                     self.index_val[index]
                                 ] = value
                                 self.UpdateTick = True
-                            elif value != -2147483648:
+                            elif self.index_val[index] not in self.resp[self.index_sym[topic_id]] and value != -2147483648:
                                 self.resp[self.index_sym[topic_id]][
                                     self.index_val[index]
                                 ] = value
                                 self.UpdateTick = True
                             idx_flag = True
                         elif topic_id in self.dp_sym:
                             if self.depthvalue[index] in self.resp[self.dp_sym[topic_id]] and self.resp[self.dp_sym[topic_id]][
-                                self.depthvalue[index]] != value and value != "-2147483648":
+                                self.depthvalue[index]] != value and value != -2147483648:
                                 self.resp[self.dp_sym[topic_id]][
                                     self.depthvalue[index]
                                 ] = value
                                 self.UpdateTick = True
-                            elif value != -2147483648:
+                            elif self.depthvalue[index] not in self.resp[self.dp_sym[topic_id]] and  value != -2147483648:
                                 self.resp[self.dp_sym[topic_id]][
                                     self.depthvalue[index]
                                 ] = value
                                 self.UpdateTick = True                                
                             dp_flag = True
                     if self.UpdateTick:
                         if sf_flag:
@@ -1215,40 +1215,31 @@
                     offset += 2
                     sf_flag, idx_flag = False, False
                     if topic_id in self.scrips_sym:
 
                         # for index in range(3):
                         value = struct.unpack(">i", data[offset : offset + 4])[0]
                         offset += 4
-                        if value != self.resp[self.scrips_sym[topic_id]][self.data_val[0]] and value != 2147483648:
+                        if value != self.resp[self.scrips_sym[topic_id]][self.data_val[0]] and value != -2147483648:
                             self.resp[self.scrips_sym[topic_id]][self.data_val[0]] = value
                             sf_flag = True
 
                             self.__response_output(
                                 self.resp[self.scrips_sym[topic_id]], "scrips"
                             )
                     elif topic_id in self.index_sym:
-                        value = struct.unpack(">I", data[offset : offset + 4])[0]
+                        value = struct.unpack(">i", data[offset : offset + 4])[0]
                         offset += 4
-                        if value != self.resp[self.index_sym[topic_id]][self.index_val[0]] and value != 2147483648:
+                        if value != self.resp[self.index_sym[topic_id]][self.index_val[0]] and value != -2147483648:
                             self.resp[self.index_sym[topic_id]][self.index_val[0]] = value
                             idx_flag = True
                             self.__response_output(
                                 self.resp[self.index_sym[topic_id]], "index"
                             )
                         
-                    # if sf_flag:
-                    #     self.__response_output(
-                    #         self.resp[self.scrips_sym[topic_id]], "scrips"
-                    #     )
-                    # elif idx_flag:
-                    #     self.__response_output(
-                    #         self.resp[self.index_sym[topic_id]], "index"
-                    #     )
-
         except Exception as e:
             self.data_logger.exception(e)
 
 
     def __response_msg(self, data: bytearray):
         """
         Processes the response message based on the response type and calls the corresponding function.
@@ -1452,17 +1443,14 @@
             else:
                 print(f"Response: {message}")
 
     def on_open(self) -> None:
         """
         Handles the open action.
         """
-        # if self.__ws_object is None:
-        #     self.__init_connection()
-        #     time.sleep(2)
         if self.OnOpen:
             self.OnOpen()
 
 
     def connect(self) -> None:
         """
         Establishes a connection to the WebSocket.
@@ -1710,12 +1698,11 @@
             total_symbols = len(self.scrips_count[self.channel_num])
             symbol_chunks = [
                 self.scrips_count[self.channel_num][i : i + 100]
                 for i in range(0, total_symbols, 100)
             ]
             for symbols in symbol_chunks:
                 message = self.__subscription_msg(symbols)
-
                 self.message.append(message)
 
         except Exception as e:
             self.data_logger.exception(e)
```

### Comparing `fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.8/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.8/fyers_sdk/fyersModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         """
         try:
             response = requests.patch(
                 url=Config.API + api,
                 data=json.dumps(data),
                 headers={"Authorization": header, "Content-Type": self.content ,"version": "3"},
             )
-            print(response)
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
 
 class FyersServiceAsync:
     def __init__(self, logger):
```

### Comparing `fyers_sdk-2.1.7/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.8/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.7/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.8/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.1.7
+Version: 2.1.8
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.7/setup.py` & `fyers_sdk-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.1.7',
+     version='2.1.8',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

