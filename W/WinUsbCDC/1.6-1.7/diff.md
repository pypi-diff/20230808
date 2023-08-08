# Comparing `tmp/WinUsbCDC-1.6-py3-none-any.whl.zip` & `tmp/WinUsbCDC-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18941 bytes, number of entries: 14
--rw-r--r--  2.0 unx      176 b- defN 23-Aug-02 12:13 winusbcdc/__init__.py
--rw-r--r--  2.0 unx     2909 b- defN 23-Aug-02 12:13 winusbcdc/__main__.py
--rw-r--r--  2.0 unx      148 b- defN 23-Aug-02 12:13 winusbcdc/__version__.py
--rw-r--r--  2.0 unx    13486 b- defN 23-Aug-02 12:13 winusbcdc/usb_cdc.py
--rw-r--r--  2.0 unx     2007 b- defN 23-Aug-02 12:13 winusbcdc/winusb.py
--rw-r--r--  2.0 unx     3485 b- defN 23-Aug-02 12:13 winusbcdc/winusbclasses.py
--rw-r--r--  2.0 unx      241 b- defN 23-Aug-02 12:13 winusbcdc/winusberror.py
--rw-r--r--  2.0 unx    14744 b- defN 23-Aug-02 12:13 winusbcdc/winusbpy.py
--rw-r--r--  2.0 unx    13569 b- defN 23-Aug-02 12:13 winusbcdc/winusbutils.py
--rw-rw-rw-  2.0 unx     1071 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     6699 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1099 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/RECORD
-14 files, 59736 bytes uncompressed, 17137 bytes compressed:  71.3%
+Zip file size: 19200 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      176 b- defN 23-Aug-08 00:32 winusbcdc/__init__.py
+-rw-r--r--  2.0 unx     2909 b- defN 23-Aug-08 00:32 winusbcdc/__main__.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Aug-08 00:32 winusbcdc/__version__.py
+-rw-r--r--  2.0 unx    13941 b- defN 23-Aug-08 00:32 winusbcdc/usb_cdc.py
+-rw-r--r--  2.0 unx     2007 b- defN 23-Aug-08 00:32 winusbcdc/winusb.py
+-rw-r--r--  2.0 unx     3485 b- defN 23-Aug-08 00:32 winusbcdc/winusbclasses.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Aug-08 00:32 winusbcdc/winusberror.py
+-rw-r--r--  2.0 unx    15148 b- defN 23-Aug-08 00:32 winusbcdc/winusbpy.py
+-rw-r--r--  2.0 unx    13569 b- defN 23-Aug-08 00:32 winusbcdc/winusbutils.py
+-rw-rw-rw-  2.0 unx     1071 b- defN 23-Aug-08 00:32 WinUsbCDC-1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6699 b- defN 23-Aug-08 00:32 WinUsbCDC-1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 00:32 WinUsbCDC-1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-08 00:32 WinUsbCDC-1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1099 b- defN 23-Aug-08 00:32 WinUsbCDC-1.7.dist-info/RECORD
+14 files, 60595 bytes uncompressed, 17396 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: winusbcdc/winusbpy.py
 Comment: 
 
 Filename: winusbcdc/winusbutils.py
 Comment: 
 
-Filename: WinUsbCDC-1.6.dist-info/LICENSE
+Filename: WinUsbCDC-1.7.dist-info/LICENSE
 Comment: 
 
-Filename: WinUsbCDC-1.6.dist-info/METADATA
+Filename: WinUsbCDC-1.7.dist-info/METADATA
 Comment: 
 
-Filename: WinUsbCDC-1.6.dist-info/WHEEL
+Filename: WinUsbCDC-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: WinUsbCDC-1.6.dist-info/top_level.txt
+Filename: WinUsbCDC-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: WinUsbCDC-1.6.dist-info/RECORD
+Filename: WinUsbCDC-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## winusbcdc/__version__.py

```diff
@@ -1,7 +1,7 @@
 # Version managed by git-versioner
-version = "v1.6"
-version_short = "v1.6"
-git_hash = "74b0dac"
-on_tag = 'v1.6'
+version = "v1.7"
+version_short = "v1.7"
+git_hash = "a4c8a9d"
+on_tag = 'v1.7'
 dirty = False
 SUPPORT_PATCH = False
```

## winusbcdc/usb_cdc.py

```diff
@@ -37,15 +37,15 @@
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import os
 import time
 import logging
 
-from .winusbpy import WinUsbPy
+from .winusbpy import WinUsbPy, WinUsbPyDevice
 from .winusb import UsbSetupPacket
 
 CDC_CMDS = {
     "SEND_ENCAPSULATED_COMMAND": 0x00,
     "GET_ENCAPSULATED_RESPONSE": 0x01,
     "SET_COMM_FEATURE": 0x02,
     "GET_COMM_FEATURE": 0x03,
@@ -69,80 +69,97 @@
         log.addHandler(fileHandler)
     return log
 
 
 log = config_log()
 
 
-class ComPort:
+def find_all_devices(name=None, vid=0, pid=0):
+    api = WinUsbPy()
+    devices = api.list_usb_devices(deviceinterface=True, present=True, vid=vid, pid=pid, name=name)
+    return [ComPort(device=d, start=False) for d in devices]
+
+
+class ComPort(WinUsbPy):
+
+    def __init__(self, name=None, vid=0, pid=0, start=True, device=None):
+        super().__init__()
 
-    def __init__(self, name=None, vid=0, pid=0, start=True):
         self.name = name
         self.vid = vid
         self.pid = pid
-        if not name and not (vid and pid):
-            raise AttributeError("Must provide friendly name _or_ vid & pid of device to connect to")
+        if not name and not (vid and pid) and not device:
+            raise AttributeError("Must provide friendly name, vid & pid, or device instance to connect to")
         if name and (vid or pid):
-            raise AttributeError("Must provide friendly name _or_ vid & pid of device to connect to")
+            raise AttributeError("Can't select on both friendly name and vid & pid of device to connect to")
 
         self.device = None
         self._rxremaining = b''
         self.baudrate = 9600
         self.parity = 0
         self.stopbits = 1
         self.databits = 8
         self.maximum_packet_size = 0
 
         self._timeout = 0
 
         self.is_open = False
-        self.device = self._select_device(self.name, self.vid, self.pid)
+        if device:
+            if not isinstance(device, WinUsbPyDevice):
+                raise ValueError("device must be a WinUsbPyDevice instance")
+
+            self.device = device
+        else:
+            self._select_device(self.name, self.vid, self.pid)
+
         if start:
             self.open()
 
     def open(self):
         # Control interface
         if not self.device:
             return False
 
+        if not self.is_open:
+            super().init_winusb_device_with_path(self.device.path)
+        
         # interface_descriptor = api.query_interface_settings(0)
         # pipe_info_list = map(api.query_pipe, range(interface_descriptor.b_num_endpoints))
 
         # Data Interface
-        self.device.change_interface(0)
-        interface2_descriptor = self.device.query_interface_settings(0)
+        super().change_interface(0)
+        interface2_descriptor = super().query_interface_settings(0)
 
-        pipe_info_list = map(self.device.query_pipe, range(interface2_descriptor.b_num_endpoints))
+        pipe_info_list = map(self.query_pipe, range(interface2_descriptor.b_num_endpoints))
         for item in pipe_info_list:
             if item.pipe_id & 0x80:
                 self._ep_in = item.pipe_id
             else:
                 self._ep_out = item.pipe_id
             self.maximum_packet_size = min(item.maximum_packet_size, self.maximum_packet_size) or item.maximum_packet_size
 
-        self.name = self.device.name
         self.is_open = True
 
         self.setControlLineState(True, True)
         self.setLineCoding()
-        self.device.set_timeout(self._ep_in, 2)
+        self.set_timeout(self._ep_in, 2)
         self.reset_input_buffer()
 
     @property
     def in_waiting(self):
         return False
 
     @property
     def timeout(self):
         return self._timeout
 
     def settimeout(self, timeout):
         self._timeout = timeout
         if self.is_open:
-            self.device.set_timeout(self._ep_in, timeout)
+            super().set_timeout(self._ep_in, timeout)
 
     @timeout.setter
     def timeout(self, timeout):
         self.settimeout(timeout)
 
     def readinto(self, buf):
         if not self.is_open:
@@ -151,18 +168,18 @@
         read = 0
         if self._rxremaining:
             l = len(self._rxremaining)
             read = min(l, orig_size)
             buf[0:read] = self._rxremaining[0:read]
             self._rxremaining = self._rxremaining[read:]
         end_timeout = time.time() + (self.timeout or 0.2)
-        self.device.set_timeout(self._ep_in, 2)
+        super().set_timeout(self._ep_in, 2)
         while read < orig_size:
             remaining = orig_size-read
-            c = self.device.read(self._ep_in, min(remaining, 1024*4))
+            c = super().read(self._ep_in, min(remaining, 1024*4))
             if c is not None and len(c):
                 if len(c) > remaining:
                     end_timeout += 0.2
                     buf[read:] = c[0:remaining]
                     self._rxremaining = c[remaining:]
                     return orig_size
                 else:
@@ -176,27 +193,27 @@
         if not self.is_open:
             return None
         rx = [self._rxremaining]
         length = len(self._rxremaining)
         self._rxremaining = b''
         end_timeout = time.time() + (self.timeout or 0.2)
         if size:
-            self.device.set_timeout(self._ep_in, 2)
+            super().set_timeout(self._ep_in, 2)
             while length < size:
-                c = self.device.read(self._ep_in, size-length)
+                c = super().read(self._ep_in, size-length)
                 if c is not None and len(c):
                     end_timeout += 0.2
                     rx.append(c)
                     length += len(c)
                 if time.time() > end_timeout:
                     break
         else:
-            self.device.set_timeout(self._ep_in, 0.2)
+            super().set_timeout(self._ep_in, 0.2)
             while True:
-                c = self.device.read(self._ep_in, self.maximum_packet_size)
+                c = super().read(self._ep_in, self.maximum_packet_size)
                 if c is not None and len(c):
                     end_timeout += 0.2
                     rx.append(c)
                     length += len(c)
                 else:
                     break
                 if time.time() > end_timeout:
@@ -213,17 +230,17 @@
     def readline(self, size=64*1024):
         if not self.is_open:
             return None
         rx = [self._rxremaining]
         length = len(self._rxremaining)
         self._rxremaining = b''
         end_timeout = time.time() + self.timeout
-        self.device.set_timeout(self._ep_in, 0.2)
+        super().set_timeout(self._ep_in, 0.2)
         while b'\n' not in rx[-1]:  # 10 == b'\n'
-            c = self.device.read(self._ep_in, size-length)
+            c = super().read(self._ep_in, size-length)
             if c is not None and len(c):
                 end_timeout += 0.2
                 length += len(c)
                 rx.append(c)
             if time.time() > end_timeout:
                 break
         line = b''.join(rx)
@@ -231,15 +248,15 @@
         self._rxremaining = line[i:]
         return line[0:i]
 
     def write(self, data):
         if not self.is_open:
             return None
         try:
-            ret = self.device.write(self._ep_out, data)
+            ret = super().write(self._ep_out, data)
         except Exception as e:
             log.warning("USB Error on write {}".format(e))
             return
 
         if len(data) != ret:
             log.error(
                 "Bytes written mismatch {0} vs {1}".format(
@@ -264,15 +281,15 @@
             value=ctrlstate,
             index=0x00,
             length=0x00
         )
         # buff = [0xc0, 0x12, 0x00, 0x00, 0x00, 0x00, 0x08]
         buff = None
 
-        wlen = self.device.control_transfer(pkt, buff)
+        wlen = super().control_transfer(pkt, buff)
         log.debug("Linecoding set, {}b sent".format(wlen))
 
     def setLineCoding(self, baudrate=None, parity=None,
                       databits=None, stopbits=None):
         if not self.is_open:
             return None
         sbits = {1: 0, 1.5: 1, 2: 2}
@@ -329,26 +346,26 @@
             index=0x00,
             length=len(linecode)
         )
         # buff = [0xc0, 0x12, 0x00, 0x00, 0x00, 0x00, 0x08]
         buff = linecode
 
 
-        wlen = self.device.control_transfer(pkt, buff)
+        wlen = super().control_transfer(pkt, buff)
             # req_type, CDC_CMDS["SET_LINE_CODING"],
             # data_or_wLength=linecode)
         log.debug("Linecoding set, {}b sent".format(wlen))
 
     # def getLineCoding(self):
     #     txdir = 1           # 0:OUT, 1:IN
     #     req_type = 1        # 0:std, 1:class, 2:vendor
     #     recipient = 1       # 0:device, 1:interface, 2:endpoint, 3:other
     #     req_type = (txdir << 7) + (req_type << 5) + recipient
     #
-    #     buf = self.device.ctrl_transfer(bmRequestType=req_type,
+    #     buf = super().ctrl_transfer(bmRequestType=req_type,
     #                                     bRequest=CDC_CMDS["GET_LINE_CODING"],
     #                                     wValue=0,
     #                                     wIndex=0,
     #                                     data_or_wLength=255,
     #                                     )
     #     self.baudrate = buf[0] + (buf[1] << 8) + \
     #         (buf[2] << 16) + (buf[3] << 24)
@@ -359,44 +376,42 @@
     #     print("  {0} baud, parity mode {1}".format(self.baudrate, self.parity))
     #     print(
     #         "  {0} data bits, {1} stop bits".format(
     #             self.databits,
     #             self.stopbits))
 
     def disconnect(self):
-        if self.device:
-            self.device.close_winusb_device()
+        super().close_winusb_device()
         self.is_open = False
 
     def __del__(self):
         self.disconnect()
 
     def reset_input_buffer(self):
         if self.is_open:
-            self.device.flush(self._ep_in)
+            super().flush(self._ep_in)
             while self.read():
                 pass
         self._rxremaining = b''
 
     def reset_output_buffer(self):
         pass
 
     def flush(self):
         if not self.is_open:
             return None
-        self.device.flush(self._ep_in)
+        super().flush(self._ep_in)
 
     def close(self):
         self.disconnect()
 
     def _select_device(self, name, vid, pid):
-        api = WinUsbPy()
-        devices = api.list_usb_devices(deviceinterface=True, present=True, vid=vid, pid=pid, name=name)
+        devices = self.list_usb_devices(deviceinterface=True, present=True, vid=vid, pid=pid, name=name)
 
         if not devices:
             log.warning("No devices detected")
             return None
 
-        if not api.init_winusb_device(name, vid, pid):
+        if not self.find_winusb_device(name, vid, pid):
             return None
 
-        return api
+        return self.device
```

## winusbcdc/winusbpy.py

```diff
@@ -21,29 +21,39 @@
     def __init__(self, path, name=None, parent=None):
         self.path = path
         self.name = name
         self.parent = parent
 
 
 class WinUsbPy(object):
+    api = WinUSBApi()
+    
+    byte_array = c_byte * 8
+    usb_device_guid = GUID(0xA5DCBF10, 0x6530, 0x11D2, byte_array(0x90, 0x1F, 0x00, 0xC0, 0x4F, 0xB9, 0x51, 0xED))
+    usb_winusb_guid = GUID(0xdee824ef, 0x729b, 0x4a0e, byte_array(0x9c, 0x14, 0xb7, 0x11, 0x7d, 0x33, 0xa8, 0x17))
+    usb_composite_guid = GUID(0x36FC9E60, 0xC465, 0x11CF, byte_array(0x80, 0x56, 0x44, 0x45, 0x53, 0x54, 0x00, 0x00))
+
 
     def __init__(self):
-        self.api = WinUSBApi()
-        byte_array = c_byte * 8
-        self.usb_device_guid = GUID(0xA5DCBF10, 0x6530, 0x11D2, byte_array(0x90, 0x1F, 0x00, 0xC0, 0x4F, 0xB9, 0x51, 0xED))
-        self.usb_winusb_guid = GUID(0xdee824ef, 0x729b, 0x4a0e, byte_array(0x9c, 0x14, 0xb7, 0x11, 0x7d, 0x33, 0xa8, 0x17))
-        self.usb_composite_guid = GUID(0x36FC9E60, 0xC465, 0x11CF, byte_array(0x80, 0x56, 0x44, 0x45, 0x53, 0x54, 0x00, 0x00))
         self.handle_file = INVALID_HANDLE_VALUE
         self.handle_winusb = [c_void_p()]
         self._index = -1
-        self.device_paths = []  # type: array
+        self.is_open = False
 
-    def list_usb_devices(self, default=False, present=False, allclasses=False, profile=False, deviceinterface=False,
-                         vid=None, pid=None, name=None, findparent=False):
-        self.device_paths = []
+        self.path = None
+        self.name = None
+        self.vid = None
+        self.pid = None
+        self.parent = None
+        self.device = None
+
+    @classmethod
+    def list_usb_devices(cls, default=False, present=False, allclasses=False, profile=False, deviceinterface=False,
+                         vid=None, pid=None, name=None, findparent=True):
+        device_paths = []
         vidpid = None
         value = 0x00000000
         try:
             if default:
                 value |= DIGCF_DEFAULT
             if present:
                 value |= DIGCF_PRESENT
@@ -56,95 +66,95 @@
 
         except KeyError:
             if value == 0x00000000:
                 value = 0x00000010
             pass
 
         flags = DWORD(value)
-        self.handle = self.api.exec_function_setupapi(SetupDiGetClassDevs, byref(self.usb_winusb_guid), None, None, flags)
+        handle = cls.api.exec_function_setupapi(SetupDiGetClassDevs, byref(cls.usb_winusb_guid), None, None, flags)
 
         sp_device_interface_data = SpDeviceInterfaceData()
         sp_device_interface_data.cb_size = sizeof(sp_device_interface_data)
         sp_device_interface_detail_data = SpDeviceInterfaceDetailData()
         sp_device_info_data = SpDevinfoData()
         sp_device_info_data.cb_size = sizeof(sp_device_info_data)
 
         i = 0
         required_size = DWORD(0)
         member_index = DWORD(i)
         cb_sizes = (8, 6, 5)  # different on 64 bit / 32 bit etc
 
-        while self.api.exec_function_setupapi(SetupDiEnumDeviceInterfaces, self.handle, None, byref(self.usb_winusb_guid),
+        while cls.api.exec_function_setupapi(SetupDiEnumDeviceInterfaces, handle, None, byref(cls.usb_winusb_guid),
                                               member_index, byref(sp_device_interface_data)):
-            self.api.exec_function_setupapi(SetupDiGetDeviceInterfaceDetail, self.handle,
+            cls.api.exec_function_setupapi(SetupDiGetDeviceInterfaceDetail, handle,
                                             byref(sp_device_interface_data), None, 0, byref(required_size), None)
             resize(sp_device_interface_detail_data, required_size.value)
 
             path = None
             for cb_size in cb_sizes:
                 sp_device_interface_detail_data.cb_size = cb_size
-                ret = self.api.exec_function_setupapi(SetupDiGetDeviceInterfaceDetail, self.handle,
+                ret = cls.api.exec_function_setupapi(SetupDiGetDeviceInterfaceDetail, handle,
                                                byref(sp_device_interface_data), byref(sp_device_interface_detail_data),
                                                required_size, byref(required_size), byref(sp_device_info_data))
                 if ret:
                     cb_sizes = (cb_size, )
                     path = wstring_at(byref(sp_device_interface_detail_data, sizeof(DWORD)))
                     break
             if path is None:
                 raise ctypes.WinError()
 
             parent = None
             if findparent:
                 dev_inst_parent = DWORD(0)
-                ret = self.api.exec_function_setupapi(CM_Get_Parent,
+                ret = cls.api.exec_function_setupapi(CM_Get_Parent,
                     byref(dev_inst_parent),
                     getattr(sp_device_info_data, "dev_inst"),
                     0,
                 )
                 if not ret:
                     buff_parent_path = ctypes.create_unicode_buffer(250)
-                    ret = self.api.exec_function_setupapi(CM_Get_Device_IDW,
+                    ret = cls.api.exec_function_setupapi(CM_Get_Device_IDW,
                         dev_inst_parent,
                         ctypes.byref(buff_parent_path),
                         ctypes.sizeof(buff_parent_path) - 1,
                         0,
                     )
                     if not ret:
                         parent = buff_parent_path.value
 
             # friendly name
             uname = path
             buff_friendly_name = ctypes.create_unicode_buffer(250)
-            if self.api.exec_function_setupapi(SetupDiGetDeviceRegistryProperty, self.handle,
+            if cls.api.exec_function_setupapi(SetupDiGetDeviceRegistryProperty, handle,
                                                 byref(sp_device_info_data),
                                                 SPDRP_FRIENDLYNAME,
                                                 None,
                                                 ctypes.byref(buff_friendly_name),
                                                 ctypes.sizeof(buff_friendly_name) - 1,
                                                 None):
 
                 uname = buff_friendly_name.value
             else:
-                err = self.get_last_error_code()
+                err = cls.get_last_error_code()
                 # print(ctypes.WinError())
 
-
             if vid is not None and pid is not None:
                 if is_device(name, vid, pid, path):
-                    self.device_paths.append(WinUsbPyDevice(path, uname, parent))
-                    return self.device_paths
+                    device_paths.append(WinUsbPyDevice(path, uname, parent))
             else:
                 if name is not None and uname == name:
-                    self.device_paths.append(WinUsbPyDevice(path, uname, parent))
-                    return self.device_paths
+                    device_paths.append(WinUsbPyDevice(path, uname, parent))
             i += 1
             member_index = DWORD(i)
             required_size = c_ulong(0)
             resize(sp_device_interface_detail_data, sizeof(SpDeviceInterfaceDetailData))
-        return self.device_paths
+        
+        if handle:
+            cls.api.exec_function_kernel32(Close_Handle, handle)
+        return device_paths
 
     def find_device(self, path):
         return is_device(self._name, self._vid, self._pid, path)
 
     def init_winusb_device_with_path(self, path):
         if path is None:
             return False
@@ -158,48 +168,56 @@
         result = self.api.exec_function_winusb(WinUsb_Initialize, self.handle_file, byref(self.handle_winusb[0]))
         if result == 0:
             err = self.get_last_error_code()
             raise ctypes.WinError()
             # return False
         else:
             self._index = 0
+            self.is_open = True
+            self.path = path
             return True
 
-    def init_winusb_device(self, name, vid, pid):
+    def find_winusb_device(self, name, vid, pid):
         self._vid = vid
         self._pid = pid
         self._name = name
-        path = None
-        try:
-            for d in self.device_paths:
-                if self.find_device(d.name) or self.find_device(d.path):
-                    path = d.path
-                    self._name = self._name or d.name
-                    break
+        self.path = None
+        devices = self.list_usb_devices(deviceinterface=True, present=True, vid=vid, pid=pid, name=name)
+        for d in devices:
+            if self.find_device(d.name) or self.find_device(d.path):
+                self.path = d.path
+                self.name = d.name
+                self.parent = d.parent
+                self.device = d
+                break
+        return self.path is not None
 
-        except IndexError:
-            return False
 
-        return self.init_winusb_device_with_path(path)
+    def init_winusb_device(self, name, vid, pid):
+
+        if self.find_winusb_device(name, vid, pid):
+            return self.init_winusb_device_with_path(self.path)
 
     def close_winusb_device(self):
         result_file = 1
         if self.handle_file:
             result_file = self.api.exec_function_kernel32(Close_Handle, self.handle_file)
             if result_file:
                 self.handle_file = None
 
         result_winusb = [self.api.exec_function_winusb(WinUsb_Free, h) for h in self.handle_winusb]
         if 0 in result_winusb:
             raise RuntimeError("Unable to close winusb handle")
-        self.handle_winusb = []
+        self.handle_winusb = [c_void_p()]
+        self.is_open = False
         return result_file != 0
 
-    def get_last_error_code(self):
-        return self.api.exec_function_kernel32(GetLastError)
+    @classmethod
+    def get_last_error_code(cls):
+        return cls.api.exec_function_kernel32(GetLastError)
 
     def query_device_info(self, query=1):
         info_type = c_ulong(query)
         buff = (c_void_p * 1)()
         buff_length = c_ulong(sizeof(c_void_p))
         result = self.api.exec_function_winusb(WinUsb_QueryDeviceInformation, self.handle_winusb[self._index], info_type,
                                                byref(buff_length), buff)
```

## Comparing `WinUsbCDC-1.6.dist-info/LICENSE` & `WinUsbCDC-1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `WinUsbCDC-1.6.dist-info/METADATA` & `WinUsbCDC-1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinUsbCDC
-Version: 1.6
+Version: 1.7
 Summary: Python package for communicating with USB / CDC devices on windows via the WinUsb driver
 Home-page: https://gitlab.com/alelec/winusbcdc
 Author: Andrew Leech
 Author-email: andrew@alelec.net
 License: MIT
 License-File: LICENSE
 
@@ -181,8 +181,8 @@
 Api <https://github.com/felHR85/WinUsbPy/blob/master/winusbpy/examples/winusbtest.py>`__
 
 `Using WinUsbPy High Level
 Api <https://github.com/felHR85/WinUsbPy/blob/master/winusbpy/examples/winusbtest2.py>`__
 
 
 
-version: 1.6
+version: 1.7
```

## Comparing `WinUsbCDC-1.6.dist-info/RECORD` & `WinUsbCDC-1.7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 winusbcdc/__init__.py,sha256=8_X10IAriFqxN-5QMW65TO0tKDR2hcKLhGdkuMGGHdY,176
 winusbcdc/__main__.py,sha256=iEOC_Ui2IqN1e_A_ubSDekH8Q0AhNlBZwAhl41M48tw,2909
-winusbcdc/__version__.py,sha256=UYR1wIBq9O4nmi-z0n3MTPSUnZ8LrUH_5ruyhhJfpy8,148
-winusbcdc/usb_cdc.py,sha256=FiHwU7KgWm-zirdE2stW7xy-dbn4yU_IhkErfgocq7o,13486
+winusbcdc/__version__.py,sha256=-wBasDGPl9LJpN4rq2PV61vnmg01nkh6sTTNPB7JQrQ,148
+winusbcdc/usb_cdc.py,sha256=mk3oZYip4D7hSv7DEM3Dapj0wdH0iUJoyOD3ZNaNwF4,13941
 winusbcdc/winusb.py,sha256=XkClRkkG75tLFDj7_8IeEUykvil1n6jgfvBuLsWAqlc,2007
 winusbcdc/winusbclasses.py,sha256=EYfaicEIEfYIHYk2PFEaBr6z2tZ2fHePl7pP1CO-mV4,3485
 winusbcdc/winusberror.py,sha256=5MoctDxNynDwkkTbzuCE-9TAZtclWzC5_5fVu7qWZ64,241
-winusbcdc/winusbpy.py,sha256=BiNwVk6MTnef06e1LUVMp1yGJDa1FZVNImybpX6wTcE,14744
+winusbcdc/winusbpy.py,sha256=0IhHEP-0UzgFcYf0EY62esQpq-fqkQdwXglz0vRhtrA,15148
 winusbcdc/winusbutils.py,sha256=bUenRf_vhzE56Mfw24ypIYWAKywDt8QZkzw-Q7u9XtM,13569
-WinUsbCDC-1.6.dist-info/LICENSE,sha256=SUJObmnFGU3-FgP1qUIUgv6tbBm2P4j6J3bUgykl6fU,1071
-WinUsbCDC-1.6.dist-info/METADATA,sha256=VMIOG1mZcJ6ptFZABuPk25kBlBRbGm7Aj1yVYwpgnqE,6699
-WinUsbCDC-1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-WinUsbCDC-1.6.dist-info/top_level.txt,sha256=tLDwJ0mo6iwg7-Sp2TpX2PfahyD_9VUj7o4ufxjqaus,10
-WinUsbCDC-1.6.dist-info/RECORD,,
+WinUsbCDC-1.7.dist-info/LICENSE,sha256=SUJObmnFGU3-FgP1qUIUgv6tbBm2P4j6J3bUgykl6fU,1071
+WinUsbCDC-1.7.dist-info/METADATA,sha256=vG0HYkDoXEY-5-9-fFmh76LlaBhYLSKF4xfkFspEcBA,6699
+WinUsbCDC-1.7.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+WinUsbCDC-1.7.dist-info/top_level.txt,sha256=tLDwJ0mo6iwg7-Sp2TpX2PfahyD_9VUj7o4ufxjqaus,10
+WinUsbCDC-1.7.dist-info/RECORD,,
```

