# Comparing `tmp/py_phone_number_fmt-1.2b3-py3-none-any.whl.zip` & `tmp/py_phone_number_fmt-1.2b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8376 bytes, number of entries: 12
+Zip file size: 8377 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      179 b- defN 23-Feb-01 13:31 phonenumberfmt/__init__.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-Feb-01 13:31 phonenumberfmt/country.py
 -rw-r--r--  2.0 unx     1925 b- defN 23-Feb-01 13:31 phonenumberfmt/format_phone_number.py
--rw-r--r--  2.0 unx     5127 b- defN 23-Feb-01 13:31 phonenumberfmt/format_phone_number_list.py
+-rw-r--r--  2.0 unx     5127 b- defN 23-Aug-08 14:12 phonenumberfmt/format_phone_number_list.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 13:31 tests/__init__.py
 -rw-r--r--  2.0 unx     2061 b- defN 23-Feb-01 13:31 tests/test_format_phone_number.py
--rw-r--r--  2.0 unx     2411 b- defN 23-Feb-01 13:31 tests/test_format_phone_number_list.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Feb-01 13:33 py_phone_number_fmt-1.2b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2671 b- defN 23-Feb-01 13:33 py_phone_number_fmt-1.2b3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-01 13:33 py_phone_number_fmt-1.2b3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Feb-01 13:33 py_phone_number_fmt-1.2b3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1059 b- defN 23-Feb-01 13:33 py_phone_number_fmt-1.2b3.dist-info/RECORD
-12 files, 17707 bytes uncompressed, 6568 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     2411 b- defN 23-Aug-08 14:12 tests/test_format_phone_number_list.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Aug-08 14:14 py_phone_number_fmt-1.2b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2670 b- defN 23-Aug-08 14:14 py_phone_number_fmt-1.2b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 14:14 py_phone_number_fmt-1.2b4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Aug-08 14:14 py_phone_number_fmt-1.2b4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1059 b- defN 23-Aug-08 14:14 py_phone_number_fmt-1.2b4.dist-info/RECORD
+12 files, 17706 bytes uncompressed, 6569 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/test_format_phone_number.py
 Comment: 
 
 Filename: tests/test_format_phone_number_list.py
 Comment: 
 
-Filename: py_phone_number_fmt-1.2b3.dist-info/LICENSE
+Filename: py_phone_number_fmt-1.2b4.dist-info/LICENSE
 Comment: 
 
-Filename: py_phone_number_fmt-1.2b3.dist-info/METADATA
+Filename: py_phone_number_fmt-1.2b4.dist-info/METADATA
 Comment: 
 
-Filename: py_phone_number_fmt-1.2b3.dist-info/WHEEL
+Filename: py_phone_number_fmt-1.2b4.dist-info/WHEEL
 Comment: 
 
-Filename: py_phone_number_fmt-1.2b3.dist-info/top_level.txt
+Filename: py_phone_number_fmt-1.2b4.dist-info/top_level.txt
 Comment: 
 
-Filename: py_phone_number_fmt-1.2b3.dist-info/RECORD
+Filename: py_phone_number_fmt-1.2b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `py_phone_number_fmt-1.2b3.dist-info/LICENSE` & `py_phone_number_fmt-1.2b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_phone_number_fmt-1.2b3.dist-info/METADATA` & `py_phone_number_fmt-1.2b4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-phone-number-fmt
-Version: 1.2b3
+Version: 1.2b4
 Summary: Sanitize, validate and format phone numbers into E.164 valid phone numbers.
 Home-page: https://github.com/SectorLabs/py-phone-number-fmt
 Author: Sector Labs
 Author-email: open-source@sectorlabs.ro
 License: MIT License
 Keywords: phone number,phone,formatting,validation
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: phonenumbers (==8.13.5)
+Requires-Dist: phonenumbers ==8.13.18
 
 # py-phone-number-fmt
 
 [![License](https://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)
 [![PyPi](https://badge.fury.io/py/py-phone-number-fmt.svg)](https://pypi.python.org/pypi/py-phone-number-fmt)
 [![CircleCI](https://circleci.com/gh/SectorLabs/py-phone-number-fmt/tree/master.svg?style=svg&circle-token=134c614a21ff3a5ca674d34d67d3b65b429b86d8)](https://circleci.com/gh/SectorLabs/py-phone-number-fmt/tree/master)
```

## Comparing `py_phone_number_fmt-1.2b3.dist-info/RECORD` & `py_phone_number_fmt-1.2b4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 phonenumberfmt/__init__.py,sha256=CAVUfUqiVxQD1Ci2CmGSzKbQbpNANmPvLL8uD6VebhA,179
 phonenumberfmt/country.py,sha256=yHME2tzSZuXlUozFve0xMLv_EUqh_9wg_xshOkX5bvE,1093
 phonenumberfmt/format_phone_number.py,sha256=HKWCBG28RhToNYu_-SVzUqavrg0bPy8nBPsH8kBq-mQ,1925
 phonenumberfmt/format_phone_number_list.py,sha256=eBdvTqDuF6C5TIDSDMbZ0dyCPxWqsSECjGtvmEDc0Bg,5127
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_format_phone_number.py,sha256=MOCaVSQC2Zj483pxn2NWb1gb5wvEoA2xRzDp-HXxPHw,2061
 tests/test_format_phone_number_list.py,sha256=tEwcSPy1TnRKivkF55p9Op5nm9Ijr4f8qQU5ZlTCpXc,2411
-py_phone_number_fmt-1.2b3.dist-info/LICENSE,sha256=q1D-5xoESYW0qW1Owdutvhp9EOifNQVxGUNgknXii_U,1068
-py_phone_number_fmt-1.2b3.dist-info/METADATA,sha256=XDkA2wl_xRd0uqHR-F-cen2y53EuPejDRIzpqMil8jM,2671
-py_phone_number_fmt-1.2b3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-py_phone_number_fmt-1.2b3.dist-info/top_level.txt,sha256=E5WDgKZ-KEHSF4pS8zHGYxinyHjFWXgiE3neB3ouk9w,21
-py_phone_number_fmt-1.2b3.dist-info/RECORD,,
+py_phone_number_fmt-1.2b4.dist-info/LICENSE,sha256=q1D-5xoESYW0qW1Owdutvhp9EOifNQVxGUNgknXii_U,1068
+py_phone_number_fmt-1.2b4.dist-info/METADATA,sha256=NZmNWkyE6Ylnqxyve0KmrQKuAn6bwQwT0MQpbNTBi1E,2670
+py_phone_number_fmt-1.2b4.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+py_phone_number_fmt-1.2b4.dist-info/top_level.txt,sha256=E5WDgKZ-KEHSF4pS8zHGYxinyHjFWXgiE3neB3ouk9w,21
+py_phone_number_fmt-1.2b4.dist-info/RECORD,,
```

