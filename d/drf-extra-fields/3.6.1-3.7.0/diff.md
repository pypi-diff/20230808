# Comparing `tmp/drf-extra-fields-3.6.1.tar.gz` & `tmp/drf-extra-fields-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-extra-fields-3.6.1.tar", last modified: Fri Jul 28 20:23:04 2023, max compression
+gzip compressed data, was "drf-extra-fields-3.7.0.tar", last modified: Tue Aug  8 18:15:31 2023, max compression
```

## Comparing `drf-extra-fields-3.6.1.tar` & `drf-extra-fields-3.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.114493 drf-extra-fields-3.6.1/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    11324 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/LICENSE
--rw-r--r--   0 furkan    (1000) furkan    (1000)       59 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/MANIFEST.in
--rw-r--r--   0 furkan    (1000) furkan    (1000)    14342 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/PKG-INFO
--rw-r--r--   0 furkan    (1000) furkan    (1000)    13329 2023-07-28 20:13:39.000000 drf-extra-fields-3.6.1/README.md
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields/
--rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/__init__.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)      115 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/compat.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)    10838 2023-07-27 11:55:22.000000 drf-extra-fields-3.6.1/drf_extra_fields/fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     2131 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/geo_fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     3814 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/relations.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields/runtests/
--rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/runtests/__init__.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     4308 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/runtests/settings.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    14342 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/PKG-INFO
--rw-r--r--   0 furkan    (1000) furkan    (1000)      550 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/SOURCES.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)        1 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/dependency_links.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       89 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/requires.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       17 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/top_level.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       61 2023-05-23 10:44:44.000000 drf-extra-fields-3.6.1/requirements.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       38 2023-07-28 20:23:04.114493 drf-extra-fields-3.6.1/setup.cfg
--rw-r--r--   0 furkan    (1000) furkan    (1000)     1714 2023-07-28 20:22:48.000000 drf-extra-fields-3.6.1/setup.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/tests/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    34084 2023-07-27 11:55:22.000000 drf-extra-fields-3.6.1/tests/test_fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     2241 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/tests/test_model_serializer.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     5169 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/tests/test_relations.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    11324 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/LICENSE
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       59 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/MANIFEST.in
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14462 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    13449 2023-08-08 18:14:46.000000 drf-extra-fields-3.7.0/README.md
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-08-08 18:15:31.382797 drf-extra-fields-3.7.0/drf_extra_fields/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/drf_extra_fields/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      596 2023-08-08 18:05:53.000000 drf-extra-fields-3.7.0/drf_extra_fields/compat.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    10782 2023-08-08 18:05:53.000000 drf-extra-fields-3.7.0/drf_extra_fields/fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2131 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/drf_extra_fields/geo_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     3814 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/drf_extra_fields/relations.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/drf_extra_fields/runtests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/drf_extra_fields/runtests/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     4308 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/drf_extra_fields/runtests/settings.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14462 2023-08-08 18:15:31.000000 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      550 2023-08-08 18:15:31.000000 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        1 2023-08-08 18:15:31.000000 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       89 2023-08-08 18:15:31.000000 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/requires.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       17 2023-08-08 18:15:31.000000 drf-extra-fields-3.7.0/drf_extra_fields.egg-info/top_level.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       61 2023-05-23 10:44:44.000000 drf-extra-fields-3.7.0/requirements.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       38 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/setup.cfg
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     1714 2023-08-08 18:14:46.000000 drf-extra-fields-3.7.0/setup.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-08-08 18:15:31.386130 drf-extra-fields-3.7.0/tests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    34199 2023-08-08 18:05:53.000000 drf-extra-fields-3.7.0/tests/test_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2281 2023-08-08 18:05:53.000000 drf-extra-fields-3.7.0/tests/test_model_serializer.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     5169 2023-05-22 10:26:49.000000 drf-extra-fields-3.7.0/tests/test_relations.py
```

### Comparing `drf-extra-fields-3.6.1/LICENSE` & `drf-extra-fields-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.6.1/PKG-INFO` & `drf-extra-fields-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-extra-fields
-Version: 3.6.1
+Version: 3.7.0
 Summary: Additional fields for Django Rest Framework.
 Home-page: https://github.com/Hipo/drf-extra-fields
 Author: hipo
 Author-email: pypi@hipolabs.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -33,14 +33,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.7.0**
+  - `psycopg` (psycopg 3) is now supported and it's used automatically instead of `psycopg2` if available.
 - **v3.6.0**
   - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
```

### Comparing `drf-extra-fields-3.6.1/README.md` & `drf-extra-fields-3.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.7.0**
+  - `psycopg` (psycopg 3) is now supported and it's used automatically instead of `psycopg2` if available.
 - **v3.6.0**
   - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
```

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields/fields.py` & `drf-extra-fields-3.7.0/drf_extra_fields/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 import base64
 import binascii
-import filetype
 import io
 import uuid
 
+import filetype
 from django.core.exceptions import ValidationError
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.utils.translation import gettext_lazy as _
 from rest_framework.fields import (
     DateField,
     DateTimeField,
+    DecimalField,
     DictField,
     EmailField,
     FileField,
     FloatField,
     ImageField,
     IntegerField,
-    DecimalField,
 )
 from rest_framework.serializers import ModelSerializer
 from rest_framework.utils import html
-from drf_extra_fields import compat
-
-try:
-    from django.contrib.postgres import fields as postgres_fields
-    from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange
-except ImportError:
-    postgres_fields = None
-    DateRange = None
-    DateTimeTZRange = None
-    NumericRange = None
 
+from drf_extra_fields import compat
+from drf_extra_fields.compat import DateRange, DateTimeTZRange, NumericRange
 
 DEFAULT_CONTENT_TYPE = "application/octet-stream"
 
 
 class Base64FieldMixin:
     EMPTY_VALUES = (None, "", [], (), {})
 
@@ -191,16 +183,16 @@
     default_error_messages = dict(DictField.default_error_messages)
     default_error_messages.update({
         'too_much_content': _('Extra content not allowed "{extra}".'),
         'bound_ordering': _('The start of the range must not exceed the end of the range.'),
     })
 
     def __init__(self, **kwargs):
-        if postgres_fields is None:
-            assert False, "'psgl2' is required to use {name}. Please install the  'psycopg2' library from 'pip'".format(
+        if compat.postgres_fields is None:
+            assert False, "'psycopg' is required to use {name}. Please install the 'psycopg2' (or 'psycopg' if you are using Django>=4.2) library from 'pip'".format(
                 name=self.__class__.__name__
             )
 
         self.child_attrs = kwargs.pop("child_attrs", {})
         self.child = self.child_class(**self.default_child_attrs, **self.child_attrs)
         super().__init__(**kwargs)
 
@@ -297,23 +289,23 @@
 
 class DateRangeField(RangeField):
     child_class = DateField
     default_child_attrs = {}
     range_type = DateRange
 
 
-if postgres_fields:
+if compat.postgres_fields:
     # monkey patch modelserializer to map Native django Range fields to
     # drf_extra_fiels's Range fields.
-    ModelSerializer.serializer_field_mapping[postgres_fields.DateTimeRangeField] = DateTimeRangeField
-    ModelSerializer.serializer_field_mapping[postgres_fields.DateRangeField] = DateRangeField
-    ModelSerializer.serializer_field_mapping[postgres_fields.IntegerRangeField] = IntegerRangeField
-    ModelSerializer.serializer_field_mapping[postgres_fields.DecimalRangeField] = DecimalRangeField
-    if compat.FloatRangeField:
-        ModelSerializer.serializer_field_mapping[compat.FloatRangeField] = FloatRangeField
+    ModelSerializer.serializer_field_mapping[compat.postgres_fields.DateTimeRangeField] = DateTimeRangeField
+    ModelSerializer.serializer_field_mapping[compat.postgres_fields.DateRangeField] = DateRangeField
+    ModelSerializer.serializer_field_mapping[compat.postgres_fields.IntegerRangeField] = IntegerRangeField
+    ModelSerializer.serializer_field_mapping[compat.postgres_fields.DecimalRangeField] = DecimalRangeField
+    if hasattr(compat.postgres_fields, "FloatRangeField"):
+        ModelSerializer.serializer_field_mapping[compat.postgres_fields.FloatRangeField] = FloatRangeField
 
 
 class LowercaseEmailField(EmailField):
     """
     An enhancement over django-rest-framework's EmailField to allow
     case-insensitive serialization and deserialization of e-mail addresses.
     """
```

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields/geo_fields.py` & `drf-extra-fields-3.7.0/drf_extra_fields/geo_fields.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields/relations.py` & `drf-extra-fields-3.7.0/drf_extra_fields/relations.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields/runtests/settings.py` & `drf-extra-fields-3.7.0/drf_extra_fields/runtests/settings.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields.egg-info/PKG-INFO` & `drf-extra-fields-3.7.0/drf_extra_fields.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-extra-fields
-Version: 3.6.1
+Version: 3.7.0
 Summary: Additional fields for Django Rest Framework.
 Home-page: https://github.com/Hipo/drf-extra-fields
 Author: hipo
 Author-email: pypi@hipolabs.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -33,14 +33,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.7.0**
+  - `psycopg` (psycopg 3) is now supported and it's used automatically instead of `psycopg2` if available.
 - **v3.6.0**
   - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
```

### Comparing `drf-extra-fields-3.6.1/drf_extra_fields.egg-info/SOURCES.txt` & `drf-extra-fields-3.7.0/drf_extra_fields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.6.1/setup.py` & `drf-extra-fields-3.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requirements = requirements_txt.read().strip().splitlines()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='drf-extra-fields',
-    version='3.6.1',
+    version='3.7.0',
     packages=['drf_extra_fields',
               'drf_extra_fields.runtests'],
     include_package_data=True,
     extras_require={
         "Base64ImageField": ["Pillow >= 6.2.1"],
     },
     license='Apache-2.0',
```

### Comparing `drf-extra-fields-3.6.1/tests/test_fields.py` & `drf-extra-fields-3.7.0/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import base64
 import copy
 import datetime
-import django
 import os
 from decimal import Decimal
+from unittest.mock import patch
 
+import django
 import pytest
 import pytz
 from django.core.exceptions import ValidationError
 from django.test import TestCase, override_settings
-from unittest.mock import patch
-from psycopg2._range import NumericRange, DateTimeTZRange, DateRange
 from rest_framework import serializers
 from rest_framework.fields import DecimalField
 
+from drf_extra_fields import compat
+from drf_extra_fields.compat import DateRange, DateTimeTZRange, NumericRange
 from drf_extra_fields.fields import (
-    Base64ImageField,
     Base64FileField,
+    Base64ImageField,
     DateRangeField,
     DateTimeRangeField,
+    DecimalRangeField,
     FloatRangeField,
     HybridImageField,
     IntegerRangeField,
     LowercaseEmailField,
-    DecimalRangeField,
 )
 from drf_extra_fields.geo_fields import PointField
-from drf_extra_fields import compat
 
 
 class UploadedBase64Image:
     def __init__(self, file=None, created=None):
         self.file = file
         self.created = created or datetime.datetime.now()
 
@@ -413,15 +413,15 @@
 class DateTimeRangeSerializer(serializers.Serializer):
 
     range = DateTimeRangeField()
 
 
 class DateRangeSerializer(serializers.Serializer):
 
-    range = DateRangeField(initial=DateRange(None, None))
+    range = DateRangeField(initial=DateRange(None, None, '()'))
 
 
 class DateRangeWithAllowEmptyFalseSerializer(serializers.Serializer):
 
     range = DateRangeField(allow_empty=False)
 
 
@@ -500,15 +500,15 @@
         ({'lower': 1, 'upper': None, 'bounds': '[)'}, ['This field may not be null.']),
         ({'lower': None, 'upper': 1, 'bounds': '[)'}, ['This field may not be null.']),
     ]
     outputs = [
         (NumericRange(**{'lower': '1', 'upper': '2'}),
          {'lower': 1, 'upper': 2, 'bounds': '[)'}),
         (NumericRange(**{'empty': True}), {'empty': True}),
-        (NumericRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (NumericRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': '1', 'upper': 2, 'bounds': '[)'},
          {'lower': 1, 'upper': 2, 'bounds': '[)'}),
         ({'lower': 1, 'upper': 2},
          {'lower': 1, 'upper': 2, 'bounds': None}),
         ({'lower': 1},
          {'lower': 1, 'upper': None, 'bounds': None}),
         ({'upper': 1},
@@ -553,15 +553,15 @@
         ({'foo': 'bar'}, ['Extra content not allowed "foo".']),
         ({'lower': 2, 'upper': 1}, ['The start of the range must not exceed the end of the range.']),
     ]
     outputs = [
         (NumericRange(**{'lower': '1', 'upper': '2'}),
          {'lower': 1, 'upper': 2, 'bounds': '[)'}),
         (NumericRange(**{'empty': True}), {'empty': True}),
-        (NumericRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (NumericRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': '1', 'upper': 2, 'bounds': '[)'},
          {'lower': 1, 'upper': 2, 'bounds': '[)'}),
         ({'lower': 1, 'upper': 2},
          {'lower': 1, 'upper': 2, 'bounds': None}),
         ({'lower': 1},
          {'lower': 1, 'upper': None, 'bounds': None}),
         ({'upper': 1},
@@ -592,15 +592,15 @@
         ('not a dict', ['Expected a dictionary of items but got type "str".']),
         ({'lower': 2., 'upper': 1.}, ['The start of the range must not exceed the end of the range.']),
     ]
     outputs = [
         (NumericRange(**{'lower': '1.1', 'upper': '2'}),
          {'lower': '1.1', 'upper': '2', 'bounds': '[)'}),
         (NumericRange(**{'empty': True}), {'empty': True}),
-        (NumericRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (NumericRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': Decimal('1.1'), 'upper': "2.3", 'bounds': '[)'},
          {'lower': "1.1", 'upper': "2.3", 'bounds': '[)'}),
         ({'lower': Decimal('1.1'), 'upper': "2.3"},
          {'lower': "1.1", 'upper': "2.3", 'bounds': None}),
         ({'lower': 1},
          {'lower': "1", 'upper': None, 'bounds': None}),
         ({'upper': 1},
@@ -643,28 +643,28 @@
         ('not a dict', ['Expected a dictionary of items but got type "str".']),
         ({'lower': 2., 'upper': 1.}, ['The start of the range must not exceed the end of the range.']),
     ]
     outputs = [
         (NumericRange(**{'lower': '1.1', 'upper': '2'}),
          {'lower': '1.10', 'upper': '2.00', 'bounds': '[)'}),
         (NumericRange(**{'empty': True}), {'empty': True}),
-        (NumericRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (NumericRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': Decimal('1.1'), 'upper': "2.3", 'bounds': '[)'},
          {'lower': "1.10", 'upper': "2.30", 'bounds': '[)'}),
         ({'lower': Decimal('1.1'), 'upper': "2.3"},
          {'lower': "1.10", 'upper': "2.30", 'bounds': None}),
         ({'lower': 1},
          {'lower': "1.00", 'upper': None, 'bounds': None}),
         ({'upper': 1},
          {'lower': None, 'upper': "1.00", 'bounds': None}),
         ({}, {}),
     ]
 
 
-@pytest.mark.skipif(django.VERSION >= (3, 1) or compat.FloatRangeField is None,
+@pytest.mark.skipif(django.VERSION >= (3, 1) or not hasattr(compat.postgres_fields, "FloatRangeField"),
                     reason='FloatRangeField deprecated on django 3.1 ')
 class TestFloatRangeField(FieldValues):
     """
     Values for `ListField` with CharField as child.
     """
     serializer_class = FloatRangeSerializer
 
@@ -686,15 +686,15 @@
         ('not a dict', ['Expected a dictionary of items but got type "str".']),
         ({'lower': 2., 'upper': 1.}, ['The start of the range must not exceed the end of the range.']),
     ]
     outputs = [
         (NumericRange(**{'lower': '1.1', 'upper': '2'}),
          {'lower': 1.1, 'upper': 2, 'bounds': '[)'}),
         (NumericRange(**{'empty': True}), {'empty': True}),
-        (NumericRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (NumericRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': '1', 'upper': 2., 'bounds': '[)'},
          {'lower': 1., 'upper': 2., 'bounds': '[)'}),
         ({'lower': 1., 'upper': 2.},
          {'lower': 1, 'upper': 2, 'bounds': None}),
         ({'lower': 1},
          {'lower': 1, 'upper': None, 'bounds': None}),
         ({'upper': 1},
@@ -756,16 +756,16 @@
             **{'lower': datetime.datetime(2001, 1, 1, 13, 00, tzinfo=pytz.utc),
                'upper': datetime.datetime(2001, 2, 2, 13, 00, tzinfo=pytz.utc)}),
             {'lower': '2001-01-01T13:00:00Z',
              'upper': '2001-02-02T13:00:00Z',
              'bounds': '[)'}),
         (DateTimeTZRange(**{'empty': True}),
          {'empty': True}),
-        (DateTimeTZRange(),
-         {'bounds': '[)', 'lower': None, 'upper': None}),
+        (DateTimeTZRange(bounds='()'),
+         {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': '2001-01-01T13:00:00Z',
           'upper': '2001-02-02T13:00:00Z',
           'bounds': '[)'},
          {'lower': '2001-01-01T13:00:00Z',
           'upper': '2001-02-02T13:00:00Z',
           'bounds': '[)'}),
         ({'lower': datetime.datetime(2001, 1, 1, 13, 00, tzinfo=pytz.utc),
@@ -834,15 +834,15 @@
             **{'lower': datetime.date(2001, 1, 1),
                'upper': datetime.date(2001, 2, 2)}),
             {'lower': '2001-01-01',
              'upper': '2001-02-02',
              'bounds': '[)'}),
         (DateRange(**{'empty': True}),
          {'empty': True}),
-        (DateRange(), {'bounds': '[)', 'lower': None, 'upper': None}),
+        (DateRange(bounds='()'), {'bounds': '()', 'lower': None, 'upper': None}),
         ({'lower': '2001-01-01',
           'upper': '2001-02-02',
           'bounds': '[)'},
          {'lower': '2001-01-01',
           'upper': '2001-02-02',
           'bounds': '[)'}),
         ({'lower': datetime.date(2001, 1, 1),
@@ -866,15 +866,15 @@
         assert str(exc_info.value) == (
             "The `source` argument is not meaningful when applied to a `child=` field. "
             "Remove `source=` from the field declaration."
         )
 
     def test_initial_value_of_field(self):
         serializer = DateRangeSerializer()
-        assert serializer.data['range'] == {'lower': None, 'upper': None, 'bounds': '[)'}
+        assert serializer.data['range'] == {'lower': None, 'upper': None, 'bounds': '()'}
 
     def test_allow_empty(self):
         serializer = DateRangeWithAllowEmptyFalseSerializer(data={"range": {}})
         with pytest.raises(serializers.ValidationError) as exc_info:
             serializer.is_valid(raise_exception=True)
             assert exc_info.value.detail == ["This dictionary may not be empty."]
```

### Comparing `drf-extra-fields-3.6.1/tests/test_model_serializer.py` & `drf-extra-fields-3.7.0/tests/test_model_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     integer_range_field = IntegerRangeField()
     decimal_range_field = DecimalRangeField()
 
     class Meta:
         app_label = 'tests'
 
 
-@pytest.mark.skipif(django.VERSION >= (3, 1) or compat.FloatRangeField is None,
+@pytest.mark.skipif(django.VERSION >= (3, 1) or not hasattr(compat.postgres_fields, "FloatRangeField"),
                     reason='FloatRangeField deprecated on django 3.1 ')
 class TestFloatRangeFieldMapping(TestCase):
 
     def test_float_range_field(self):
         class FloatRangeFieldModel(models.Model):
-            float_range_field = compat.FloatRangeField()
+            float_range_field = compat.postgres_fields.FloatRangeField()
 
             class Meta:
                 app_label = 'tests'
 
         class TestSerializer(serializers.ModelSerializer):
             class Meta:
                 model = FloatRangeFieldModel
```

### Comparing `drf-extra-fields-3.6.1/tests/test_relations.py` & `drf-extra-fields-3.7.0/tests/test_relations.py`

 * *Files identical despite different names*

