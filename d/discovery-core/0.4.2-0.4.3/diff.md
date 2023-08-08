# Comparing `tmp/discovery-core-0.4.2.tar.gz` & `tmp/discovery-core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.4.2.tar", last modified: Fri Aug  4 20:25:59 2023, max compression
+gzip compressed data, was "discovery-core-0.4.3.tar", last modified: Tue Aug  8 20:59:18 2023, max compression
```

## Comparing `discovery-core-0.4.2.tar` & `discovery-core-0.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.025672 discovery-core-0.4.2/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.2/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.2/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-04 20:25:59.025864 discovery-core-0.4.2/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.2/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.015284 discovery-core-0.4.2/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.015644 discovery-core-0.4.2/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-02 16:54:47.000000 discovery-core-0.4.2/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.016866 discovery-core-0.4.2/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.2/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    26586 2023-08-04 18:24:32.000000 discovery-core-0.4.2/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.018172 discovery-core-0.4.2/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.2/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.2/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.018815 discovery-core-0.4.2/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.2/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.020616 discovery-core-0.4.2/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.2/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.2/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.2/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-04 20:25:59.026448 discovery-core-0.4.2/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.2/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.020976 discovery-core-0.4.2/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.2/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.022114 discovery-core-0.4.2/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.2/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21160 2023-08-04 18:29:25.000000 discovery-core-0.4.2/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.023163 discovery-core-0.4.2/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.2/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.2/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.024306 discovery-core-0.4.2/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.2/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.2/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.025372 discovery-core-0.4.2/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.2/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.2/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.354357 discovery-core-0.4.3/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.3/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.3/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-08 20:59:18.354566 discovery-core-0.4.3/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.3/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.330734 discovery-core-0.4.3/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-08 20:59:18.000000 discovery-core-0.4.3/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-08 20:59:18.000000 discovery-core-0.4.3/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-08 20:59:18.000000 discovery-core-0.4.3/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-08 20:59:18.000000 discovery-core-0.4.3/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.331092 discovery-core-0.4.3/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-04 20:27:04.000000 discovery-core-0.4.3/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.333191 discovery-core-0.4.3/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.3/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    26904 2023-08-08 18:30:00.000000 discovery-core-0.4.3/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.335232 discovery-core-0.4.3/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.3/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.3/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.336511 discovery-core-0.4.3/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.3/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.340541 discovery-core-0.4.3/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.3/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.3/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.3/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-08 20:59:18.355193 discovery-core-0.4.3/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.3/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.341493 discovery-core-0.4.3/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.3/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.344321 discovery-core-0.4.3/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.3/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21502 2023-08-08 20:07:25.000000 discovery-core-0.4.3/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.347469 discovery-core-0.4.3/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.3/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.3/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.350409 discovery-core-0.4.3/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.3/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.3/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-08 20:59:18.353540 discovery-core-0.4.3/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.3/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.3/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.3/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.4.2/LICENSE.txt` & `discovery-core-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/PKG-INFO` & `discovery-core-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.2/README.rst` & `discovery-core-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.4.3/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.2/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.4.3/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/components/abstract_component.py` & `discovery-core-0.4.3/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/components/core_commons.py` & `discovery-core-0.4.3/ds_core/components/core_commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,14 +409,21 @@
         """ attempt to cast a pyarrow array to the given type """
         try:
             return a.cast(ty)
         except (ArrowInvalid, ArrowTypeError, ArrowNotImplementedError):
             return a
 
     @staticmethod
+    def column_join(a: pa.Array, b: pa.Array, sep: str=None):
+        """ joins two columns to create a compound column. The separator is optional"""
+        sep = sep if isinstance(sep, str) else ''
+        return pc.binary_join_element_wise(pc.cast(a, pa.string()), pc.cast(b, pa.string()), sep)
+
+
+    @staticmethod
     def column_precision(a: pa.Array):
         """returns the max precision in a numeric pyarrow array"""
         if pa.types.is_floating(a.type) or pa.types.is_integer(a.type):
             return max([CoreCommons.precision_scale(x)[1] for x in a.drop_null().to_pylist()])
         raise ValueError(f"The array should be numeric, type '{a.type}' sent.")
 
     @staticmethod
```

### Comparing `discovery-core-0.4.2/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.4.3/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.4.3/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/intent/abstract_intent.py` & `discovery-core-0.4.3/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/properties/abstract_properties.py` & `discovery-core-0.4.3/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/properties/decorator_patterns.py` & `discovery-core-0.4.3/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/ds_core/properties/property_manager.py` & `discovery-core-0.4.3/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/setup.py` & `discovery-core-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/components/abstract_component_test.py` & `discovery-core-0.4.3/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/components/commons_test.py` & `discovery-core-0.4.3/test/components/commons_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,22 @@
         self.assertEqual(3, result)
         result = CoreCommons.column_precision(val)
         self.assertEqual(0, result)
         with self.assertRaises(ValueError) as context:
             result = CoreCommons.column_precision(text)
         self.assertTrue("The array should be numeric, type 'string' sent." in str(context.exception))
 
+    def test_column_join(self):
+        a = pa.array([1,2,3,4,5])
+        b = pa.array(list('abcde'))
+        c = CoreCommons.column_join(a,b)
+        self.assertEqual(['1a', '2b', '3c', '4d', '5e'], c.to_pylist())
+        c = CoreCommons.column_join(a,b,sep='_')
+        self.assertEqual(['1_a', '2_b', '3_c', '4_d', '5_e'], c.to_pylist())
+
     def test_array_cast(self):
         num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
         date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
         text = pa.array(["Blue", "Green", None, 'Blue'], pa.string())
         bool1 = pa.array([1, 0, 1, None], pa.int64())
         bool2 = pa.array(['true', 'true', None, 'false'], pa.string())
         bool3 = pa.array([None, 'no', 'yes', 'yes'], pa.string())
```

### Comparing `discovery-core-0.4.2/test/handlers/connector_contract_test.py` & `discovery-core-0.4.3/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/handlers/handler_factory_test.py` & `discovery-core-0.4.3/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/intent/abstract_intent_test.py` & `discovery-core-0.4.3/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/intent/pyarrow_intent_model.py` & `discovery-core-0.4.3/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.4.3/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.2/test/properties/property_manager_test.py` & `discovery-core-0.4.3/test/properties/property_manager_test.py`

 * *Files identical despite different names*

