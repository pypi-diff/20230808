# Comparing `tmp/rcsb.utils.struct-0.44.tar.gz` & `tmp/rcsb.utils.struct-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.struct-0.44.tar", last modified: Tue Apr 18 21:10:14 2023, max compression
+gzip compressed data, was "rcsb.utils.struct-0.45.tar", last modified: Mon Aug  7 22:26:08 2023, max compression
```

## Comparing `rcsb.utils.struct-0.44.tar` & `rcsb.utils.struct-0.45.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/
--rw-r--r--   0 vsts      (1001) docker     (122)     2496 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/rcsb/utils/struct/
--rw-r--r--   0 vsts      (1001) docker     (122)    12976 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/CathClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15694 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/EcodClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3191 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20575 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/Scop2ClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16717 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/ScopClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/rcsb/utils/struct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 21:10:14.005454 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 21:09:04.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-18 21:10:13.000000 rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-18 21:10:14.009454 rcsb.utils.struct-0.44/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2325 2023-04-18 21:08:26.000000 rcsb.utils.struct-0.44/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/rcsb/utils/struct/
+-rw-r--r--   0 vsts      (1001) docker     (122)    13214 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/CathClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15694 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/EcodClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3191 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21008 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/Scop2ClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16717 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/ScopClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-07 22:25:00.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2325 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/setup.py
```

### Comparing `rcsb.utils.struct-0.44/HISTORY.txt` & `rcsb.utils.struct-0.45/HISTORY.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,8 +30,9 @@
  10-Sep-2021    V0.37 Separate protein type and structural class in tree representation.
  22-Sep-2021    V0.38 Add module EntryInfoProvider and associated tests (accessor methods only)
  23-Sep-2021    V0.39 Update SCOP version and path details
  16-Nov-2021    V0.40 Append additional ECOD annotations for given entryId and chainId instead of overwriting
  24-Feb-2022    V0.41 Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
   9-Mar-2022    V0.42 Fix issue related to V0.41 update to Scop2 provider
   6-Jan-2023    V0.43 Configuration changes to support tox 4
- 18-Apr-2023    V0.44 Fix Ecod and Scop2 provider fall-back file import
+ 18-Apr-2023    V0.44 Fix Ecod and Scop2 provider fall-back file import
+ 18-Jul-2023    V0.45 Resolve duplication issues with Scop2 families and CATH residue range lists
```

### Comparing `rcsb.utils.struct-0.44/LICENSE` & `rcsb.utils.struct-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/PKG-INFO` & `rcsb.utils.struct-0.45/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.44
+Version: 0.45
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.struct-0.44/README.md` & `rcsb.utils.struct-0.45/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/rcsb/utils/struct/CathClassificationProvider.py` & `rcsb.utils.struct-0.45/rcsb/utils/struct/CathClassificationProvider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:  CathClassificationProvider.py
 #  Date:  3-Apr-2019 jdw
 #
 #  Updates:
-#  15-Jul-2021 jdw Update the constructor to common provider API conventions
+#   15-Jul-2021 jdw Update the constructor to common provider API conventions
+#   18-Jul-2023 dwp Resolve duplication issues with CATH residue range list
 ##
 """
   Extract CATH domain assignments, term descriptions and CATH classification hierarchy
   from CATH flat files.
 
 """
 
@@ -290,15 +291,20 @@
         =
            aD[(pdbId, authAsymId)] = [(cathId, domainId, (authAsymId, resBeg, resEnd), version)]
         """
         pdbD = {}
         for domId, dTup in dD.items():
             pdbId = domId[:4]
             for rTup in dTup[1]:
-                pdbD.setdefault((pdbId, rTup[0]), []).append((dTup[0], domId, rTup, dTup[2]))
+                cKey = (pdbId, rTup[0])
+                cTup = (dTup[0], domId, rTup, dTup[2])
+                if cKey not in pdbD:
+                    pdbD[cKey] = []
+                if cTup not in pdbD[cKey]:
+                    pdbD[cKey].append(cTup)
         return pdbD
 
     def __exportTreeNodeList(self, nD):
         """Create node list from name dictionary and lineage dictionaries."""
         # create parent dictionary
         #
         pL = []
```

### Comparing `rcsb.utils.struct-0.44/rcsb/utils/struct/EcodClassificationProvider.py` & `rcsb.utils.struct-0.45/rcsb/utils/struct/EcodClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/rcsb/utils/struct/EntryInfoProvider.py` & `rcsb.utils.struct-0.45/rcsb/utils/struct/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/rcsb/utils/struct/Scop2ClassificationProvider.py` & `rcsb.utils.struct-0.45/rcsb/utils/struct/Scop2ClassificationProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #  File:  Scop2ClassificationProvider.py
 #  Date:  29-Jun-2021 jdw
 #
 #  Updates:
 #   10-Sep-2021 jdw split tree with type and class roots
 #   24-Feb-2022 dwp Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
 #   18-Apr-2023 aae Use "pickle" as default file format
+#   18-Jul-2023 dwp Resolve duplication issues with Scop2 families list
 ##
 """
   Extract SCOP2 domain assignments, term descriptions and SCOP2 classification hierarchy
   from SCOP2 and SCOP2B flat files.
 
 """
 
@@ -383,19 +384,29 @@
                 ntD[tD["CF"]] = "CF"
                 ntD[tD["CL"]] = "CL"
                 ntD[tD["TP"]] = "TP"
                 #
                 pdbId = ff[1]
                 authAsymId, authSeqBeg, authSeqEnd = self.__parseAssignment(ff[2])
                 if authAsymId is not None:
-                    fD.setdefault((pdbId, authAsymId), []).append((domFamilyId, tD["FA"], authAsymId, authSeqBeg, authSeqEnd))
+                    fKey = (pdbId, authAsymId)
+                    fTup = (domFamilyId, tD["FA"], authAsymId, authSeqBeg, authSeqEnd)
+                    if fKey not in fD:
+                        fD[fKey] = []
+                    if fTup not in fD[fKey]:
+                        fD[fKey].append(fTup)
                 pdbId = ff[6]
                 authAsymId, authSeqBeg, authSeqEnd = self.__parseAssignment(ff[7])
                 if authAsymId is not None:
-                    sfD.setdefault((pdbId, authAsymId), []).append((domSuperFamilyId, tD["SF"], authAsymId, authSeqBeg, authSeqEnd))
+                    sfKey = (pdbId, authAsymId)
+                    sfTup = (domSuperFamilyId, tD["SF"], authAsymId, authSeqBeg, authSeqEnd)
+                    if sfKey not in sfD:
+                        sfD[sfKey] = []
+                    if sfTup not in sfD[sfKey]:
+                        sfD[sfKey].append(sfTup)
                 #
                 domToSfD[domSuperFamilyId] = tD["SF"]
             except Exception as e:
                 logger.exception("Failing for case %r: %s", dm, str(e))
         #
         logger.info("pAD (%d) pBD (%d) pBRootD (%d) ntD (%d)", len(pAD), len(pBD), len(pBRootD), len(ntD))
         logger.info("fD (%d) sfD (%d)", len(fD), len(sfD))
```

### Comparing `rcsb.utils.struct-0.44/rcsb/utils/struct/ScopClassificationProvider.py` & `rcsb.utils.struct-0.45/rcsb/utils/struct/ScopClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/PKG-INFO` & `rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.44
+Version: 0.45
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.struct-0.44/rcsb.utils.struct.egg-info/SOURCES.txt` & `rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.44/setup.py` & `rcsb.utils.struct-0.45/setup.py`

 * *Files identical despite different names*

