# Comparing `tmp/gustav-0.8.1-py3-none-any.whl.zip` & `tmp/gustav-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 110741 bytes, number of entries: 25
--rw-r--r--  2.0 unx     1898 b- defN 23-Aug-08 17:17 gustav/__init__.py
+Zip file size: 110781 bytes, number of entries: 25
+-rw-r--r--  2.0 unx     1898 b- defN 23-Aug-08 19:01 gustav/__init__.py
 -rw-r--r--  2.0 unx     1068 b- defN 21-Mar-20 22:36 gustav/dataTemplate_adaptive.py
 -rw-r--r--  2.0 unx     8291 b- defN 22-Mar-12 18:39 gustav/gustav.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Feb-26 16:13 gustav/utils.py
 -rw-r--r--  2.0 unx      913 b- defN 21-Mar-20 22:36 gustav/forms/__init__.py
 -rw-r--r--  2.0 unx    56957 b- defN 22-Feb-01 00:32 gustav/forms/lateralization.py
 -rw-r--r--  2.0 unx    60675 b- defN 21-Dec-03 16:43 gustav/forms/localization.py
 -rw-r--r--  2.0 unx    53735 b- defN 22-Feb-07 18:00 gustav/forms/nafc.py
@@ -15,13 +15,13 @@
 -rw-r--r--  2.0 unx      833 b- defN 21-Mar-20 22:36 gustav/methods/__init__.py
 -rw-r--r--  2.0 unx    16104 b- defN 22-May-09 17:03 gustav/methods/adaptive.py
 -rw-r--r--  2.0 unx     3322 b- defN 21-Mar-20 22:36 gustav/methods/constant.py
 -rw-r--r--  2.0 unx    16146 b- defN 21-Mar-20 22:36 gustav/methods/pest.py
 -rw-r--r--  2.0 unx    10923 b- defN 23-Feb-26 16:16 gustav/user_scripts/gustav_exp__adaptive__frequency_discrim.py
 -rw-r--r--  2.0 unx    10965 b- defN 23-Feb-26 16:16 gustav/user_scripts/gustav_exp__adaptive_quietthresholds.py
 -rw-r--r--  2.0 unx     9890 b- defN 23-Feb-26 16:17 gustav/user_scripts/gustav_exp__lateralization.py
--rw-r--r--  2.0 unx    32423 b- defN 23-Aug-08 17:18 gustav-0.8.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1085 b- defN 23-Aug-08 17:18 gustav-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 17:18 gustav-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-08 17:18 gustav-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2098 b- defN 23-Aug-08 17:18 gustav-0.8.1.dist-info/RECORD
-25 files, 417670 bytes uncompressed, 107373 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    32423 b- defN 23-Aug-08 19:02 gustav-0.8.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1146 b- defN 23-Aug-08 19:02 gustav-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 19:02 gustav-0.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-08 19:02 gustav-0.8.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2098 b- defN 23-Aug-08 19:02 gustav-0.8.2.dist-info/RECORD
+25 files, 417731 bytes uncompressed, 107413 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: gustav/user_scripts/gustav_exp__adaptive_quietthresholds.py
 Comment: 
 
 Filename: gustav/user_scripts/gustav_exp__lateralization.py
 Comment: 
 
-Filename: gustav-0.8.1.dist-info/LICENSE.md
+Filename: gustav-0.8.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: gustav-0.8.1.dist-info/METADATA
+Filename: gustav-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: gustav-0.8.1.dist-info/WHEEL
+Filename: gustav-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: gustav-0.8.1.dist-info/top_level.txt
+Filename: gustav-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gustav-0.8.1.dist-info/RECORD
+Filename: gustav-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gustav/__init__.py

```diff
@@ -35,11 +35,11 @@
     set, such as the name of the experiment, where and how to save data, what 
     the experimental variables and their levels are, and so on. The best way 
     to understand how one works is to have a look at one. See the test_gustav 
     python scripts in the user_scripts directory for more information.
 
 """
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 from .gustav import run, info, main
 from . import frontends, methods, forms
```

## Comparing `gustav-0.8.1.dist-info/LICENSE.md` & `gustav-0.8.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `gustav-0.8.1.dist-info/METADATA` & `gustav-0.8.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gustav
-Version: 0.8.1
+Version: 0.8.2
 Summary: A simple but powerful python module to help with psychophysical experimentation
 Home-page: https://github.com/cbrown1/gustav
 Author: Christopher Brown
 Author-email: cbrown1@pitt.edu
 Maintainer: Christopher Brown
 Maintainer-email: cbrown1@pitt.edu
 Platform: linux
@@ -21,8 +21,9 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE.md
+Requires-Dist: windows-curses ; platform_system == "Windows"
```

## Comparing `gustav-0.8.1.dist-info/RECORD` & `gustav-0.8.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-gustav/__init__.py,sha256=r--zWYq-4lqLpQG4QeA36ZAQZUSkJ4CRjOVu1KOzk9E,1898
+gustav/__init__.py,sha256=l6lQgG_KTjM_oUbeTGffTKpz1Xr0H63VFMeFcNHGf6w,1898
 gustav/dataTemplate_adaptive.py,sha256=AhvsXWKrPc7TxwMpjYtcjUEWZrO5AND49F8N6Ph63yA,1068
 gustav/gustav.py,sha256=AjLJ9ii_CfhXHUIdmYzjeuoyHPpfS24e3KdCcO0BqPE,8291
 gustav/utils.py,sha256=cWxjMqFw59IlmP8wKRCIYEj0RV8YbYPCiF0UXkDGjio,32439
 gustav/forms/__init__.py,sha256=9G8DAJ-WLjW927pthWOzqZTr1j9HgHN1wFRaAYVW4qo,913
 gustav/forms/lateralization.py,sha256=17bLS4qq3cKSBDhjy_xRmPTsdJR13Zu5ZopTmJ2qdNs,56957
 gustav/forms/localization.py,sha256=V79mSWIVYXifJqjkGm1nJP8N0mo7dtqlOvgpGuZEYiI,60675
 gustav/forms/nafc.py,sha256=o7GbN5nrVudnt_7LlJ-XVI_4QD-R4deRv5BnaPTo4HU,53735
@@ -14,12 +14,12 @@
 gustav/methods/__init__.py,sha256=QdKlutb8aquhbSqNmgdf-IyEM4Eux5IvxFZfJsfhwA0,833
 gustav/methods/adaptive.py,sha256=ni3IlcnnzSmW4iQDfkdmQk3-1WDbHsCbHUIpo18glbA,16104
 gustav/methods/constant.py,sha256=JLJz2u5ce2H323HwKPjEh0a1UnZuF7JFoC1j_-E3RlU,3322
 gustav/methods/pest.py,sha256=DwqeYMafGwUf3CtymePBp79mIvugsmsaK1j1q32MK2M,16146
 gustav/user_scripts/gustav_exp__adaptive__frequency_discrim.py,sha256=3qveAMPTuleVn_Ew0-wScBog94aNH0M6QWVmaZM9Lxo,10923
 gustav/user_scripts/gustav_exp__adaptive_quietthresholds.py,sha256=rflaf9lAdp6un_AssuWqCcCIotH5dA9DX6yTo2NMows,10965
 gustav/user_scripts/gustav_exp__lateralization.py,sha256=YxTvgU_WTeD8PU1hbgcwd6TZSYNERAnl7dIgFmJ739c,9890
-gustav-0.8.1.dist-info/LICENSE.md,sha256=Z83GNTJq8cbx2oZmTTr6KH2yyUuaD292vabRCQ070yY,32423
-gustav-0.8.1.dist-info/METADATA,sha256=9lzgt8WudTl4oX3EuWU_8x5LnqY51hNQzml6Smt5-jQ,1085
-gustav-0.8.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gustav-0.8.1.dist-info/top_level.txt,sha256=IbqMtDPz6bMNDbHhyvA8gRfl38qr6j5EBOhQFeCut28,7
-gustav-0.8.1.dist-info/RECORD,,
+gustav-0.8.2.dist-info/LICENSE.md,sha256=Z83GNTJq8cbx2oZmTTr6KH2yyUuaD292vabRCQ070yY,32423
+gustav-0.8.2.dist-info/METADATA,sha256=PEar0AzRKoRtB-YjGlF_4RCNXQ5KIxDW2Gi5_CyH8Ss,1146
+gustav-0.8.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gustav-0.8.2.dist-info/top_level.txt,sha256=IbqMtDPz6bMNDbHhyvA8gRfl38qr6j5EBOhQFeCut28,7
+gustav-0.8.2.dist-info/RECORD,,
```

