# Comparing `tmp/pyevspace-0.14.1.tar.gz` & `tmp/pyevspace-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevspace-0.14.1.tar", last modified: Fri Aug  4 02:36:04 2023, max compression
+gzip compressed data, was "pyevspace-0.14.2.tar", last modified: Tue Aug  8 02:07:23 2023, max compression
```

## Comparing `pyevspace-0.14.1.tar` & `pyevspace-0.14.2.tar`

### file list

```diff
@@ -1,26 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 02:35:56.000000 pyevspace-0.14.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 02:35:56.000000 pyevspace-0.14.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-04 02:36:04.067542 pyevspace-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-04 02:35:56.000000 pyevspace-0.14.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:36:04.071542 pyevspace-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-04 02:35:56.000000 pyevspace-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_angles.h
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_refframe.h
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_rotation.h
--rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspacemodule.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/src/evspacemodule.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.630334 pyevspace-0.14.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 02:07:14.000000 pyevspace-0.14.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 02:07:14.000000 pyevspace-0.14.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-08-08 02:07:23.630334 pyevspace-0.14.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-08 02:07:14.000000 pyevspace-0.14.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 02:07:14.000000 pyevspace-0.14.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:07:23.630334 pyevspace-0.14.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 02:07:14.000000 pyevspace-0.14.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.626335 pyevspace-0.14.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.626335 pyevspace-0.14.2/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/examples/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/examples/creating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/examples/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.626335 pyevspace-0.14.2/src/pyevspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.630334 pyevspace-0.14.2/src/pyevspace/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_angles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_refframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_rotation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspace_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/include/evspacemodule.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.630334 pyevspace-0.14.2/src/pyevspace/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/pyevspace/src/evspacemodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.626335 pyevspace-0.14.2/src/pyevspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-08-08 02:07:23.000000 pyevspace-0.14.2/src/pyevspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-08 02:07:23.000000 pyevspace-0.14.2/src/pyevspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:07:23.000000 pyevspace-0.14.2/src/pyevspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 02:07:23.000000 pyevspace-0.14.2/src/pyevspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:07:23.630334 pyevspace-0.14.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/angles_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/refframe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30859 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/rotation_answers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-08-08 02:07:14.000000 pyevspace-0.14.2/src/tests/vector_test.py
```

### Comparing `pyevspace-0.14.1/LICENSE.txt` & `pyevspace-0.14.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/PKG-INFO` & `pyevspace-0.14.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: pyevspace
-Version: 0.14.1
+Version: 0.14.2
 Summary: A Python 3-dimensional Euclidean vector space.
-Home-page: https://github.com/qbizzle68/pyevspace
-Author: Quinton Barnes
-Author-email: devqbizzle68@gmail.com
-License: MIT
+Author-email: Quinton Barnes <devqbizzle68@gmail.com>
+Project-URL: Homepage, https://github.com/qbizzle68/pyevspace
+Project-URL: Bug Tracker, https://github.com/qbizzle68/pyevspace/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyEVSpace 0.14.1
+# PyEVSpace 0.14.2
 
-This version of PyEVSpace is no functionally different than 0.14.0.
-This version was published to pypi using automated scripting workflows,
-and its existence means everything works!!
+[![Github test action](https://github.com/qbizzle68/pyevspace/actions/workflows/test-builds.yml/badge.svg)](https://github.com/qbizzle68/pyevspace/actions)
+[![PyPi](https://img.shields.io/pypi/v/pyevspace?style=plastic)](https://pypi.org/project/pyevspace/#history)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/pyevspace?style=plastic)
+[![License](https://img.shields.io/pypi/l/pyevspace?style-plastic)](https://opensource.org/licenses/MIT)
 
 PyEVSpace is a Python Euclidean vector space package containing types
 and methods for representing vector quantites and fasilitating rotating
 them between reference frames. PyEVSpace is designed for 3-dimensional
 space only, which allows for optimum speed since size checks do not
 occur.
```

### Comparing `pyevspace-0.14.1/README.md` & `pyevspace-0.14.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# PyEVSpace 0.14.1
+# PyEVSpace 0.14.2
 
-This version of PyEVSpace is no functionally different than 0.14.0.
-This version was published to pypi using automated scripting workflows,
-and its existence means everything works!!
+[![Github test action](https://github.com/qbizzle68/pyevspace/actions/workflows/test-builds.yml/badge.svg)](https://github.com/qbizzle68/pyevspace/actions)
+[![PyPi](https://img.shields.io/pypi/v/pyevspace?style=plastic)](https://pypi.org/project/pyevspace/#history)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/pyevspace?style=plastic)
+[![License](https://img.shields.io/pypi/l/pyevspace?style-plastic)](https://opensource.org/licenses/MIT)
 
 PyEVSpace is a Python Euclidean vector space package containing types
 and methods for representing vector quantites and fasilitating rotating
 them between reference frames. PyEVSpace is designed for 3-dimensional
 space only, which allows for optimum speed since size checks do not
 occur.
```

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_angles.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_angles.h`

 * *Files 8% similar despite different names*

```diff
@@ -167,30 +167,47 @@
 angles_set_item(EVSpace_Angles* self, Py_ssize_t index, PyObject* value)
 {
     double dbl_value = PyFloat_AsDouble(value);
     if (dbl_value == -1.0 && PyErr_Occurred()) {
         return -1;
     }
 
+    double* angle_addr = NULL;
     if (index == ROTATION_ANGLE_ALPHA) {
-        self->alpha = dbl_value;
+        //self->alpha = dbl_value;
+        angle_addr = &self->alpha;
     }
     else if (index == ROTATION_ANGLE_BETA) {
-        self->beta = dbl_value;
+        //self->beta = dbl_value;
+        angle_addr = &self->beta;
     }
     else if (index == ROTATION_ANGLE_GAMMA) {
-        self->gamma = dbl_value;
+        //self->gamma = dbl_value;
+        angle_addr = &self->gamma;
     }
     else {
         PyErr_Format(PyExc_IndexError,
                      "index (%i) must be in [0-2]",
                      index);
         return -1;
     }
 
+    // Track the original value to revert if computing matrix fails.
+    double old_value = *angle_addr;
+    *angle_addr = dbl_value;
+    EVSpace_ReferenceFrame* master = (EVSpace_ReferenceFrame*)self->master;
+
+    if (self->master) {
+        if (_refframe_update_matrix(master) < 0) {
+            *angle_addr = old_value;
+            return -1;
+        }
+    }
+    angle_addr = NULL;
+
     return 0;
 }
 
 static EVSpace_Order*
 _order_new(EVSpace_Axis first, EVSpace_Axis second, EVSpace_Axis third,
            PyTypeObject* type)
 {
```

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_api.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_api.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_common.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_common.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_matrix.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_matrix.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_refframe.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_refframe.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_rotation.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_rotation.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspace_vector.h` & `pyevspace-0.14.2/src/pyevspace/include/evspace_vector.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/include/evspacemodule.h` & `pyevspace-0.14.2/src/pyevspace/include/evspacemodule.h`

 * *Files identical despite different names*

### Comparing `pyevspace-0.14.1/src/pyevspace/src/evspacemodule.c` & `pyevspace-0.14.2/src/pyevspace/src/evspacemodule.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ﻿#define PY_SSIZE_T_CLEAN
 #include <Python.h>
-#include <structmember.h> // PyMemberDef
+#if PY_VERSION_HEX < 0x03120000
+    #include <structmember.h> // PyMemberDef
+#endif
 
 /* don't need the extra's for the C API */
 #define _EVSPACE_IMPL
 #include <evspacemodule.h>
 #include <evspace_vector.h>
 #include <evspace_matrix.h>
 #include <evspace_angles.h>
@@ -226,21 +228,33 @@
 static PySequenceMethods order_as_sequence = {
     .sq_length      = (lenfunc)vector_length,
     .sq_item        = (ssizeargfunc)order_get_item,
     .sq_ass_item    = (ssizeobjargproc)order_set_item
 };
 
 static PyMemberDef order_members[] = {
+#if PY_VERSION_HEX < 0x03120000
     {"first", T_INT, offsetof(EVSpace_Order, first), READONLY,
+#else
+    {"first", Py_T_INT, offsetof(EVSpace_Order, first), READONLY,
+#endif
      PyDoc_STR("first axis of a rotation")},
 
+#if PY_VERSION_HEX < 0x03120000
     {"second", T_INT, offsetof(EVSpace_Order, second), READONLY,
+#else
+    {"second", Py_T_INT, offsetof(EVSpace_Order, second), READONLY,
+#endif
      PyDoc_STR("second axis of a rotation")},
 
+#if PY_VERSION_HEX < 0x03120000
     {"third", T_INT, offsetof(EVSpace_Order, third), READONLY,
+#else
+    {"third", Py_T_INT, offsetof(EVSpace_Order, third), READONLY,
+#endif
      PyDoc_STR("third axis of a rotation")},
 
     {NULL}
 };
 
 PyDoc_STRVAR(order_reduce_doc, "__reduce__() -> (cls, state)\n\
 \n\
@@ -273,18 +287,26 @@
     .tp_doc         = order_doc,
     .tp_methods     = order_methods,
     .tp_members     = order_members,
     .tp_new         = (newfunc)order_new
 };
 
 static PyMemberDef reference_frame_members[] = {
+#if PY_VERSION_HEX < 0x03120000
     {"order", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, order), READONLY,
+#else
+    {"order", Py_T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, order), READONLY,
+#endif
      PyDoc_STR("order of axes in the rotation")},
 
+#if PY_VERSION_HEX < 0x03120000
     {"matrix", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, matrix), READONLY,
+#else
+    {"matrix", Py_T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, matrix), READONLY,
+#endif
      PyDoc_STR("internal matrix describing the rotation")},
 
     {NULL}
 };
 
 static PyGetSetDef reference_frame_getset[] = {
     {"angles", (getter)refframe_angles_getter,
```

### Comparing `pyevspace-0.14.1/src/pyevspace.egg-info/PKG-INFO` & `pyevspace-0.14.2/src/pyevspace.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: pyevspace
-Version: 0.14.1
+Version: 0.14.2
 Summary: A Python 3-dimensional Euclidean vector space.
-Home-page: https://github.com/qbizzle68/pyevspace
-Author: Quinton Barnes
-Author-email: devqbizzle68@gmail.com
-License: MIT
+Author-email: Quinton Barnes <devqbizzle68@gmail.com>
+Project-URL: Homepage, https://github.com/qbizzle68/pyevspace
+Project-URL: Bug Tracker, https://github.com/qbizzle68/pyevspace/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyEVSpace 0.14.1
+# PyEVSpace 0.14.2
 
-This version of PyEVSpace is no functionally different than 0.14.0.
-This version was published to pypi using automated scripting workflows,
-and its existence means everything works!!
+[![Github test action](https://github.com/qbizzle68/pyevspace/actions/workflows/test-builds.yml/badge.svg)](https://github.com/qbizzle68/pyevspace/actions)
+[![PyPi](https://img.shields.io/pypi/v/pyevspace?style=plastic)](https://pypi.org/project/pyevspace/#history)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/pyevspace?style=plastic)
+[![License](https://img.shields.io/pypi/l/pyevspace?style-plastic)](https://opensource.org/licenses/MIT)
 
 PyEVSpace is a Python Euclidean vector space package containing types
 and methods for representing vector quantites and fasilitating rotating
 them between reference frames. PyEVSpace is designed for 3-dimensional
 space only, which allows for optimum speed since size checks do not
 occur.
```

