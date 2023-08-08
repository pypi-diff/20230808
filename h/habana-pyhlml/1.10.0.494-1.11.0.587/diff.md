# Comparing `tmp/habana_pyhlml-1.10.0.494-py3-none-any.whl.zip` & `tmp/habana_pyhlml-1.11.0.587-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12904 bytes, number of entries: 10
--rw-r--r--  2.0 unx       25 b- defN 23-May-24 04:06 pyhlml/__init__.py
--rw-r--r--  2.0 unx     2113 b- defN 23-May-24 04:06 pyhlml/hlml_error.py
--rw-r--r--  2.0 unx     1430 b- defN 23-May-24 04:06 pyhlml/hlml_lib.py
--rw-r--r--  2.0 unx    10630 b- defN 23-May-24 04:06 pyhlml/hlml_types.py
--rw-r--r--  2.0 unx    36087 b- defN 23-May-24 04:06 pyhlml/main.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-May-24 04:07 habana_pyhlml-1.10.0.494.dist-info/LICENSE
--rw-r--r--  2.0 unx     1457 b- defN 23-May-24 04:07 habana_pyhlml-1.10.0.494.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 04:07 habana_pyhlml-1.10.0.494.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-24 04:07 habana_pyhlml-1.10.0.494.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      815 b- defN 23-May-24 04:07 habana_pyhlml-1.10.0.494.dist-info/RECORD
-10 files, 53721 bytes uncompressed, 11514 bytes compressed:  78.6%
+Zip file size: 12721 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-03 22:43 pyhlml/__init__.py
+-rw-r--r--  2.0 unx     2113 b- defN 23-Aug-03 22:43 pyhlml/hlml_error.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Aug-03 22:43 pyhlml/hlml_lib.py
+-rw-r--r--  2.0 unx    10442 b- defN 23-Aug-03 22:43 pyhlml/hlml_types.py
+-rw-r--r--  2.0 unx    35570 b- defN 23-Aug-03 22:43 pyhlml/main.py
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Aug-03 22:43 habana_pyhlml-1.11.0.587.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1457 b- defN 23-Aug-03 22:43 habana_pyhlml-1.11.0.587.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 22:43 habana_pyhlml-1.11.0.587.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-03 22:43 habana_pyhlml-1.11.0.587.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      815 b- defN 23-Aug-03 22:43 habana_pyhlml-1.11.0.587.dist-info/RECORD
+10 files, 53016 bytes uncompressed, 11331 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyhlml/hlml_types.py
 Comment: 
 
 Filename: pyhlml/main.py
 Comment: 
 
-Filename: habana_pyhlml-1.10.0.494.dist-info/LICENSE
+Filename: habana_pyhlml-1.11.0.587.dist-info/LICENSE
 Comment: 
 
-Filename: habana_pyhlml-1.10.0.494.dist-info/METADATA
+Filename: habana_pyhlml-1.11.0.587.dist-info/METADATA
 Comment: 
 
-Filename: habana_pyhlml-1.10.0.494.dist-info/WHEEL
+Filename: habana_pyhlml-1.11.0.587.dist-info/WHEEL
 Comment: 
 
-Filename: habana_pyhlml-1.10.0.494.dist-info/top_level.txt
+Filename: habana_pyhlml-1.11.0.587.dist-info/top_level.txt
 Comment: 
 
-Filename: habana_pyhlml-1.10.0.494.dist-info/RECORD
+Filename: habana_pyhlml-1.11.0.587.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyhlml/hlml_types.py

```diff
@@ -100,29 +100,20 @@
 
 class HLML_ECC_COUNTER:
     TYPE                                    = ctypes.c_uint()
     HLML_VOLATILE_ECC                       = 0
     HLML_AGGREGATE_ECC                      = 1
     HLML_ECC_COUNTER_TYPE_COUNT             = 2
 
-class HLML_ERR_INJECT:
-    TYPE                                    = ctypes.c_uint()
-    HLML_ERR_INJECT_ENDLESS_COMMAND         = 0
-    HLML_ERR_INJECT_NON_FATAL_EVENT         = 1
-    HLML_ERR_INJECT_FATAL_EVENT             = 2
-    HLML_ERR_INJECT_LOSS_OF_HEARTBEAT       = 3
-    HLML_ERR_INJECT_THERMAL_EVENT           = 4
-    HLML_ERR_INJECT_COUNT                   = 5
-
 class HLML_PCIE_UTIL_COUNTER:
     TYPE                                    = ctypes.c_uint()
     HLML_PCIE_UTIL_TX_BYTES                 = 0
     HLML_PCIE_UTIL_RX_BYTES                 = 1
     HLML_PCIE_UTIL_COUNT                    = 2
-    
+
 class HLML_EVENT_SET:
     TYPE                                    = ctypes.c_void_p()
 
 class HLML_ROW_REPLACEMENT_CAUSE:
     TYPE                                                      = ctypes.c_uint()
     HLML_ROW_REPLACEMENT_CAUSE_MULTIPLE_SINGLE_BIT_ECC_ERRORS = 0,
     HLML_ROW_REPLACEMENT_CAUSE_DOUBLE_BIT_ECC_ERROR           = 1,
@@ -139,26 +130,26 @@
 
 class HLML_UNIT:
     TYPE                                    = _struct_c_hlml_unit()
 
 class _PrintS(ctypes.Structure):
     """
     Produces nicer __str__ output than ctypes.Structure.
-    
+
     e.g. instead of:
-      
+
     > print str(obj)
     <class_name object at 0x7fdf82fef9e0>
-    
+
     this class will print...
 
     > print str(obj)
     class_name(field_name: formatted_value, field_name: formatted_value)
     _fmt_ dictionary of <str _field_ name> -> <str format>
-    
+
     Default formatting string for all fields can be set with key "<default>" like:
       _fmt_ = {"<default>" : "%d MHz"} # e.g all values are numbers in MHz.
 
     If not set it's assumed to be just "%s"
 
     e.g. class that has _field_ 'hex_value', c_uint could be formatted with
       _fmt_ = {"hex_value" : "%08X"}
@@ -176,15 +167,17 @@
             elif "<default>" in self._fmt_:
                 fmt = self._fmt_["<default>"]
             result.append(("%s: " + fmt) % (key, value))
         return self.__class__.__name__ + "(" +  ", ".join(result) + ")"
 
 class c_hlml_pci_cap(_PrintS):
     _fields_ = [("link_speed", ctypes.c_char * HLML_DEFINE.PCI_LINK_INFO_LEN),
-                ("link_width",ctypes.c_char * HLML_DEFINE.PCI_LINK_INFO_LEN)
+                ("link_width",ctypes.c_char * HLML_DEFINE.PCI_LINK_INFO_LEN),
+                ("link_max_speed", ctypes.c_char * HLML_DEFINE.PCI_LINK_INFO_LEN),
+                ("link_max_width",ctypes.c_char * HLML_DEFINE.PCI_LINK_INFO_LEN)
                ]
 
 class c_hlml_pci_info(_PrintS):
     """
     /*
         * bus - The bus on which the device resides, 0 to 0xf
         * bus_id - The tuple domain:bus:device.function
@@ -194,15 +187,16 @@
     */
     """
     _fields_ = [("bus", ctypes.c_uint),
                 ("bus_id", ctypes.c_char * HLML_DEFINE.PCI_ADDR_LEN),
                 ("device", ctypes.c_uint),
                 ("domain", ctypes.c_uint),
                 ("pci_device_id", ctypes.c_uint),
-                ("caps", c_hlml_pci_cap)
+                ("caps", c_hlml_pci_cap),
+                ("pci_rev", ctypes.c_uint)
                ]
 
 class c_hlml_utilization(_PrintS):
     _fields_ = [("aip", ctypes.c_uint)]
 
 class c_hlml_memory(_PrintS):
     _fields_ = [("free", ctypes.c_ulonglong),
@@ -254,15 +248,15 @@
                 ("pc", ctypes.c_uint8),
                 ("sid", ctypes.c_uint8),
                 ("bank_idx", ctypes.c_uint8),
                 ("row_addr", ctypes.c_uint16)
                ]
 
 class hlml_ecc_mode(_PrintS):
-    _fields_ = [("current", ctypes.c_uint), 
+    _fields_ = [("current", ctypes.c_uint),
                 ("pending", ctypes.c_uint)
                ]
 
 ## Alternative object
 # Allows the object to be printed
 # Allows mismatched types to be assigned
 #  - like None when the Structure variant requires c_uint
```

## pyhlml/main.py

```diff
@@ -418,15 +418,15 @@
     ret = fn(device, ctypes.byref(name), name_len)
 
     check_return(ret)
     return name.value
 
 def hlmlDeviceGetMinorNumber(device: hlml_t.HLML_DEVICE.TYPE) -> int:
     """ Retrieves the minor number of the device ( maps to the device node file )
-        at /sys/class/habanalabs/hl[minor]
+        at /sys/class/accel/accel[minor]
         Parameters:
             device (HLML_DEVICE.TYPE) - The handle for a habana device.
         Returns:
             number (int) - The minor number for the device.
     """
     global _hlmlOBJ
     number = ctypes.c_uint()
@@ -520,29 +520,14 @@
 
     fn = _hlmlOBJ.get_func_ptr("hlml_device_get_mac_info")
     ret = fn(device, ctypes.byref(mac), count, start, ctypes.byref(actual_info_count))
 
     check_return(ret)
     return mac
 
-def hlmlDeviceERRInject(device: hlml_t.HLML_DEVICE.TYPE, err_type: int) -> None:
-    """ Inject error to test response
-        Parameters:
-            device (HLML_DEVICE.TYPE) - The handle for a habana device.
-            err_type ( 0-endless_cmd / 1-non_fatal / 2-fatal / 3-lose_heartbeat / 4-thermal) - The type of error to inject.
-        Returns: None.
-    """
-    global _hlmlOBJ
-
-    fn = _hlmlOBJ.get_func_ptr("hlml_device_err_inject")
-    ret = fn(device, err_type)
-
-    check_return(ret)
-    return None
-
 def hlmlDeviceGetHLRevision(device: hlml_t.HLML_DEVICE.TYPE) -> int:
     """ Returns HL revision
         Parameters:
             device (HLML_DEVICE.TYPE) - The handle for a habana device.
         Returns:
             rev (int) - The HL revision
     """
```

## Comparing `habana_pyhlml-1.10.0.494.dist-info/LICENSE` & `habana_pyhlml-1.11.0.587.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `habana_pyhlml-1.10.0.494.dist-info/METADATA` & `habana_pyhlml-1.11.0.587.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habana-pyhlml
-Version: 1.10.0.494
+Version: 1.11.0.587
 Summary: Python3 wrapper for the HLML library.
 Home-page: UNKNOWN
 Author: HabanaAI
 Author-email: "support@habana.ai"
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `habana_pyhlml-1.10.0.494.dist-info/RECORD` & `habana_pyhlml-1.11.0.587.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyhlml/__init__.py,sha256=VjbHqSSypSMmVK7UTxuCyOs_AE8HhTXX9EGr6NbaQNk,25
 pyhlml/hlml_error.py,sha256=GQulGXf-jX38jEASXF22qJ0yL8eC57vUo8s9lVI7q_E,2113
 pyhlml/hlml_lib.py,sha256=JiHRLl3vpAozhCSs9eJC8xlhIMxR2wNVZdmahjlgDfc,1430
-pyhlml/hlml_types.py,sha256=RESPajQUNWCb0y8KmtyCtwRyKbTYflboOzjMJHY75mo,10630
-pyhlml/main.py,sha256=rCy1nkae5lPmC2nz5PGbp8lVE_1CcZboVqLw1CDrmug,36087
-habana_pyhlml-1.10.0.494.dist-info/LICENSE,sha256=_J8fTEtZF8y69onNU5_EAdOn0AC9RM2uHPh_q36-5bc,1065
-habana_pyhlml-1.10.0.494.dist-info/METADATA,sha256=JyxSH6kA33wOc9rSmhaLfRtrpOcEVJP9Gu_G1FCrePA,1457
-habana_pyhlml-1.10.0.494.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-habana_pyhlml-1.10.0.494.dist-info/top_level.txt,sha256=0jXJHTTotoeuyzpI1dcVr0mzCVB0NKY7LyCF4OwoMZU,7
-habana_pyhlml-1.10.0.494.dist-info/RECORD,,
+pyhlml/hlml_types.py,sha256=n1l2gaXj_tIy7DPJProizZ0zFc1cqwwINh-0rAgDw1o,10442
+pyhlml/main.py,sha256=XFpU940JNrTDsFwi4_Ih41W8od1uRdAZ5uoBLq4miZ4,35570
+habana_pyhlml-1.11.0.587.dist-info/LICENSE,sha256=_J8fTEtZF8y69onNU5_EAdOn0AC9RM2uHPh_q36-5bc,1065
+habana_pyhlml-1.11.0.587.dist-info/METADATA,sha256=bOLEvgcmkgKhS126qR1WgzkLtr_O6rMKqOJmJyX2zFg,1457
+habana_pyhlml-1.11.0.587.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+habana_pyhlml-1.11.0.587.dist-info/top_level.txt,sha256=0jXJHTTotoeuyzpI1dcVr0mzCVB0NKY7LyCF4OwoMZU,7
+habana_pyhlml-1.11.0.587.dist-info/RECORD,,
```

