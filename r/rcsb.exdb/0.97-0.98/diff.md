# Comparing `tmp/rcsb.exdb-0.97.tar.gz` & `tmp/rcsb.exdb-0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.exdb-0.97.tar", last modified: Mon Jun  5 14:33:10 2023, max compression
+gzip compressed data, was "rcsb.exdb-0.98.tar", last modified: Tue Aug  8 17:36:13 2023, max compression
```

## Comparing `rcsb.exdb-0.97.tar` & `rcsb.exdb-0.98.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/
--rw-r--r--   0 vsts      (1001) docker     (122)     7326 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/exdb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/exdb/branch/
--rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/BranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/GlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/citation/
--rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/cli/ExDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/entry/
--rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/entry/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/entry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.567757 rcsb.exdb-0.97/rcsb/exdb/seq/
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/AnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/PolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/TaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/UniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/UniProtExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9677 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/fixturePdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testAnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testBranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5268 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testTaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3557 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testTreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtExtractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/tree/
--rw-r--r--   0 vsts      (1001) docker     (122)    11987 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tree/TreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tree/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectValidator.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)     2570 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10714 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/ExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2820 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/GlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10473 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/PubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb.exdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:05:52.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7490 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.116461 rcsb.exdb-0.98/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/branch/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/branch/BranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/branch/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/branch/GlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/branch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/citation/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/citation/CitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/citation/CitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/citation/CitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/cli/ExDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb/exdb/entry/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/entry/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/entry/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.124461 rcsb.exdb-0.98/rcsb/exdb/seq/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/AnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/LigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/PolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/TaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/UniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/UniProtExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/rcsb/exdb/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9679 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/fixturePdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testAnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testBranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testChemRefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testCitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testCitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testCitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testEntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5294 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testPolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testTaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testTreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tests/testUniProtExtractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/rcsb/exdb/tree/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12500 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tree/TreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/tree/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/rcsb/exdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/ObjectAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/ObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/ObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/ObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/ObjectValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/rcsb/exdb/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2570 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10838 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/wf/ExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2820 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/wf/GlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10473 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/wf/PubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/rcsb/exdb/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-08 17:36:13.120461 rcsb.exdb-0.98/rcsb.exdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-08 17:14:01.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-08-08 17:36:13.000000 rcsb.exdb-0.98/rcsb.exdb.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-08-08 17:36:13.128461 rcsb.exdb-0.98/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-08-08 17:09:07.000000 rcsb.exdb-0.98/setup.py
```

### Comparing `rcsb.exdb-0.97/HISTORY.txt` & `rcsb.exdb-0.98/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,8 +86,10 @@
                   Switch fixturePdbxLoader to use remote HTTP loading for Azure tests instead of local mock/sandbox paths
 25-May-2022 V0.92 Add error checking for SIFTS data loading in ReferenceSequenceAnnotationProvider and ReferenceSequenceAssignmentProvider
  9-Jan-2023 V0.93 Configuration changes to support tox 4
  9-Mar-2023 V0.94 Update ExDbWorkflow to make use of multiple processors for 'upd_ref_seq' operation;
                   Lower refChunkSize to 10 for requests to UniProt API
 13-Mar-2023 V0.95 Updates to PubChem workflow to use multiprocess count, disable git stash testing, remove obsolete entries from test data
 12-Apr-2023 V0.96 Add CARD ontology data to tree builder
- 1-Jun-2023 V0.97 Don't back up resources to GitHub during cache update workflows
+ 1-Jun-2023 V0.97 Don't back up resources to GitHub during cache update workflows
+ 8-Aug-2023 V0.98 Reduce memory and cpu footprint for Azure test cases;
+                  Load full (unfiltered) taxonomy tree node list, and stop loading GO tree
```

### Comparing `rcsb.exdb-0.97/LICENSE` & `rcsb.exdb-0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/PKG-INFO` & `rcsb.exdb-0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.97
+Version: 0.98
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.97/README.md` & `rcsb.exdb-0.98/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/branch/BranchedEntityExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/branch/BranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/branch/GlycanProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/branch/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/branch/GlycanUtils.py` & `rcsb.exdb-0.98/rcsb/exdb/branch/GlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefEtlWorker.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefMappingProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/ChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemDataCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemEtlWrapper.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemIndexCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/chemref/PubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/citation/CitationAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/citation/CitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/citation/CitationExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/citation/CitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/citation/CitationUtils.py` & `rcsb.exdb-0.98/rcsb/exdb/citation/CitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/cli/ExDbExec.py` & `rcsb.exdb-0.98/rcsb/exdb/cli/ExDbExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/entry/EntryInfoProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/entry/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/AnnotationExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/AnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/LigandNeighborMappingExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/LigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/PolymerEntityExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/PolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/TaxonomyExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/TaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/UniProtCoreEtlWorker.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/UniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/seq/UniProtExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/seq/UniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/fixturePdbxLoader.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/fixturePdbxLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
         configName = "site_info_configuration"
         self.__cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=self.__mockTopPath)
         #
         self.__resourceName = "MONGO_DB"
         self.__failedFilePath = os.path.join(HERE, "test-output", "failed-list.txt")
         self.__cachePath = os.path.join(TOPDIR, "CACHE")
         self.__readBackCheck = True
-        self.__numProc = 2
-        self.__chunkSize = 10
+        self.__numProc = 1
+        self.__chunkSize = 5
         self.__fileLimit = 38
         self.__documentStyle = "rowwise_by_name_with_cardinality"
         #
         self.__birdChemCompCoreIdList = [
             "PRD_000010",
             "PRD_000060",
             "PRD_000220",
@@ -168,15 +168,15 @@
                 "mergeContentTypes": None,
                 "validationLevel": "min",
                 "inputIdCodeList": self.__birdChemCompCoreIdList
             },
             {
                 "databaseName": "pdbx_core",
                 "collectionNameList": None,
-                "loadType": "full",
+                "loadType": "replace",
                 "mergeContentTypes": ["vrpt"],
                 "validationLevel": "min",
                 "inputIdCodeList": self.__pdbIdList
             },
             # {
             #     "databaseName": "pdbx_comp_model_core",
             #     "collectionNameList": None,
@@ -224,15 +224,15 @@
                 cachePath=self.__cachePath,
                 resourceName=self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
                 fileLimit=kwargs.get("fileLimit", self.__fileLimit),
                 verbose=self.__verbose,
                 readBackCheck=self.__readBackCheck,
-                maxStepLength=2000,
+                maxStepLength=1000,
                 useSchemaCache=True,
                 rebuildSchemaFlag=False,
             )
             ok = mw.load(
                 kwargs["databaseName"],
                 collectionLoadList=kwargs["collectionNameList"],
                 loadType=kwargs["loadType"],
```

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testAnnotationExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testAnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testBranchedEntityExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testBranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefLoader.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testChemRefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefMappingProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testCitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testCitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationUtils.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testCitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testEntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testExDbWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testExDbWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             "configName": configName,
             "cachePath": cachePath,
             "rebuildCache": False,
             "providerTypeExclude": self.__excludeType,
             "restoreUseGit": True,
             "restoreUseStash": False,
         }
-        self.__loadCommonD = {"readBackCheck": True, "numProc": 2, "chunkSize": 5, "refChunkSize": 5, "loadType": "full"}
+        self.__loadCommonD = {"readBackCheck": True, "numProc": 2, "chunkSize": 5, "refChunkSize": 5, "loadType": "full", "useFilteredLists": True}
         #
         # These are test source files for chemical component/BIRD indices
         ccUrlTarget = os.path.join(self.__dataPath, "components-abbrev.cif")
         birdUrlTarget = os.path.join(self.__dataPath, "prdcc-abbrev.cif")
         ccFileNamePrefix = "cc-abbrev"
         self.__chemEtlD = {
             "fetchLimit": 4,
```

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanUtils.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testGlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testLigandNeighborMappingProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testLigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectTransformer.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectUpdater.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testPolymerEntityExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testPolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemDataCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWrapper.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemIndexCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testPubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testTaxonomyExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testTaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testTreeNodeListWorker.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testTreeNodeListWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.__readBackCheck = True
         self.__numProc = 2
         self.__chunkSize = 10
         self.__documentLimit = None
         self.__debugFlag = False
         self.__loadType = "full"
         self.__useCache = True
+        self.__useFilteredLists = True
         #
         self.__startTime = time.time()
         logger.debug("Starting %s at %s", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
 
     def tearDown(self):
         unitS = "MB" if platform.system() == "Darwin" else "GB"
         rusageMax = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
@@ -84,14 +85,15 @@
                 self.__cachePath,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
                 documentLimit=self.__documentLimit,
                 verbose=self.__debugFlag,
                 readBackCheck=self.__readBackCheck,
                 useCache=self.__useCache,
+                useFilteredLists=self.__useFilteredLists,
             )
             #
             ok = rhw.load(updateId, loadType=self.__loadType, doLoad=self.__doLoad)
             self.assertTrue(ok)
             #
         except Exception as e:
             logger.exception("Failing with %s", str(e))
```

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtCoreEtlWorker.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testUniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/tests/testUniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/tree/TreeNodeListWorker.py` & `rcsb.exdb-0.98/rcsb/exdb/tree/TreeNodeListWorker.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,57 +3,59 @@
 # Date: 9-Apr-2019  jdw
 #
 # Loading worker for tree node list data.
 #
 # Updates:
 #  9-Sep-2019 jdw add AtcProvider() and ChemrefExtractor() for ATC tree.
 # 12-Apr-2023 dwp add CARD ontology tree
+#  8-Aug-2023 dwp Load full (unfiltered) taxonomy tree node list, and stop loading GO tree (will be loaded in DW instead)
 #
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
 import os.path
 
 from rcsb.db.mongo.DocumentLoader import DocumentLoader
 from rcsb.db.processors.DataExchangeStatus import DataExchangeStatus
 from rcsb.exdb.chemref.ChemRefExtractor import ChemRefExtractor
-from rcsb.exdb.seq.AnnotationExtractor import AnnotationExtractor
-from rcsb.exdb.seq.TaxonomyExtractor import TaxonomyExtractor
 from rcsb.utils.chemref.AtcProvider import AtcProvider
 from rcsb.utils.ec.EnzymeDatabaseProvider import EnzymeDatabaseProvider
 from rcsb.utils.targets.CARDTargetOntologyProvider import CARDTargetOntologyProvider
-from rcsb.utils.go.GeneOntologyProvider import GeneOntologyProvider
 from rcsb.utils.struct.CathClassificationProvider import CathClassificationProvider
 from rcsb.utils.struct.EcodClassificationProvider import EcodClassificationProvider
 from rcsb.utils.struct.ScopClassificationProvider import ScopClassificationProvider
 from rcsb.utils.struct.Scop2ClassificationProvider import Scop2ClassificationProvider
 from rcsb.utils.taxonomy.TaxonomyProvider import TaxonomyProvider
+from rcsb.exdb.seq.TaxonomyExtractor import TaxonomyExtractor
+# from rcsb.utils.go.GeneOntologyProvider import GeneOntologyProvider
+# from rcsb.exdb.seq.AnnotationExtractor import AnnotationExtractor
 
 logger = logging.getLogger(__name__)
 
 
 class TreeNodeListWorker(object):
     """Prepare and load repository holdings and repository update data."""
 
-    def __init__(self, cfgOb, cachePath, numProc=1, chunkSize=10, readBackCheck=False, documentLimit=None, verbose=False, useCache=False):
+    def __init__(self, cfgOb, cachePath, numProc=1, chunkSize=10, readBackCheck=False, documentLimit=None, verbose=False, useCache=False, useFilteredLists=False):
         self.__cfgOb = cfgOb
         self.__cachePath = os.path.abspath(cachePath)
         self.__readBackCheck = readBackCheck
         self.__numProc = numProc
         self.__chunkSize = chunkSize
         self.__documentLimit = documentLimit
         self.__resourceName = "MONGO_DB"
         self.__filterType = "assign-dates"
         self.__verbose = verbose
         self.__statusList = []
         self.__useCache = useCache
+        self.__useFilteredLists = useFilteredLists
 
     def __updateStatus(self, updateId, databaseName, collectionName, status, startTimestamp):
         try:
             sFlag = "Y" if status else "N"
             desp = DataExchangeStatus()
             desp.setStartTime(tS=startTimestamp)
             desp.setObject(databaseName, collectionName)
@@ -118,27 +120,29 @@
                 readBackCheck=self.__readBackCheck,
             )
             #
             databaseName = "tree_node_lists"
             # collectionVersion = self.__cfgOb.get("COLLECTION_VERSION_STRING", sectionName=sectionName)
             # addValues = {"_schema_version": collectionVersion}
             addValues = None
-            # --- GO
-            goP = GeneOntologyProvider(goDirPath=os.path.join(self.__cachePath, "go"), useCache=useCache)
-            ok = goP.testCache()
-            anEx = AnnotationExtractor(self.__cfgOb)
-            goIdL = anEx.getUniqueIdentifiers("GO")
-            logger.info("Unique GO assignments %d", len(goIdL))
-            nL = goP.exportTreeNodeList(goIdL)
-            logger.info("GO tree node list length %d", len(nL))
-            if doLoad:
-                collectionName = "tree_go_node_list"
-                ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
-                self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
-                # ---- CATH
+            #
+            # --- GO - TURNED OFF 08 Aug 2023 dwp (tree is now loaded in DW)
+            # goP = GeneOntologyProvider(goDirPath=os.path.join(self.__cachePath, "go"), useCache=useCache)
+            # ok = goP.testCache()
+            # anEx = AnnotationExtractor(self.__cfgOb)
+            # goIdL = anEx.getUniqueIdentifiers("GO")
+            # logger.info("Unique GO assignments %d", len(goIdL))
+            # nL = goP.exportTreeNodeList(goIdL)
+            # logger.info("GO tree node list length %d", len(nL))
+            # if doLoad:
+            #     collectionName = "tree_go_node_list"
+            #     ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
+            #     self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
+            #
+            # ---- CATH
             ccu = CathClassificationProvider(cachePath=self.__cachePath, useCache=useCache)
             nL = ccu.getTreeNodeList()
             logger.info("Starting load SCOP node tree length %d", len(nL))
             if doLoad:
                 collectionName = "tree_cath_node_list"
                 ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
                 self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
@@ -179,27 +183,31 @@
             nL = cou.getTreeNodeList()
             logger.info("Starting load of EC node tree length %d", len(nL))
             if doLoad:
                 collectionName = "tree_card_node_list"
                 ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
                 self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
             # ---- Taxonomy
-            # Get the taxon coverage in the current data set -
-            epe = TaxonomyExtractor(self.__cfgOb)
-            tL = epe.getUniqueTaxons()
-            logger.info("Taxon coverage length %d", len(tL))
-            #
             tU = TaxonomyProvider(cachePath=self.__cachePath, useCache=useCache)
-            fD = {1}
-            for taxId in tL:
-                fD.update({k: True for k in tU.getLineage(taxId)})
-            logger.info("Taxon filter dictionary length %d", len(fD))
-            # logger.info("fD %r" % sorted(fD))
-            #
-            nL = tU.exportNodeList(filterD=fD)
+            if self.__useFilteredLists:
+                # Get the taxon coverage in the current data set -
+                epe = TaxonomyExtractor(self.__cfgOb)
+                tL = epe.getUniqueTaxons()
+                logger.info("Taxon coverage length %d", len(tL))
+                #
+                fD = {1}
+                for taxId in tL:
+                    fD.update({k: True for k in tU.getLineage(taxId)})
+                logger.info("Taxon filter dictionary length %d", len(fD))
+                logger.debug("fD %r", sorted(fD))
+                #
+                nL = tU.exportNodeList(filterD=fD)
+            else:
+                # Get the full taxon node list without filtering
+                nL = tU.exportNodeList()
             self.__checkTaxonNodeList(nL)
             logger.info("Starting load of taxonomy node tree length %d", len(nL))
             if doLoad:
                 collectionName = "tree_taxonomy_node_list"
                 logger.debug("Taxonomy nodes (%d) %r", len(nL), nL[:5])
                 ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
                 self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
```

### Comparing `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectExtractor.py` & `rcsb.exdb-0.98/rcsb/exdb/utils/ObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectTransformer.py` & `rcsb.exdb-0.98/rcsb/exdb/utils/ObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectUpdater.py` & `rcsb.exdb-0.98/rcsb/exdb/utils/ObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectValidator.py` & `rcsb.exdb-0.98/rcsb/exdb/utils/ObjectValidator.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/wf/EntryInfoEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/wf/EntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/wf/ExDbWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/wf/ExDbWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
             dbType = kwargs.get("dbType", "mongo")
             tU = TimeUtil()
             dataSetId = kwargs.get("dataSetId") if "dataSetId" in kwargs else tU.getCurrentWeekSignature()
             #  Rebuild or reuse reference sequence cache
             rebuildSequenceCache = kwargs.get("rebuildSequenceCache", False)
             useSequenceCache = not rebuildSequenceCache
             #
+            useFilteredLists = kwargs.get("useFilteredLists", False)
         except Exception as e:
             logger.exception("Argument or configuration processing failing with %s", str(e))
             return False
         #
         okS = ok = False
         if dbType == "mongo":
             if op == "etl_tree_node_lists":
@@ -103,14 +104,15 @@
                     self.__cachePath,
                     numProc=numProc,
                     chunkSize=chunkSize,
                     documentLimit=documentLimit,
                     verbose=self.__debugFlag,
                     readBackCheck=readBackCheck,
                     useCache=self.__useCache,
+                    useFilteredLists=useFilteredLists,
                 )
                 ok = rhw.load(dataSetId, loadType=loadType)
                 okS = self.loadStatus(rhw.getLoadStatus(), readBackCheck=readBackCheck)
 
             elif op == "etl_chemref":
                 crw = ChemRefEtlWorker(
                     self.__cfgOb,
```

### Comparing `rcsb.exdb-0.97/rcsb/exdb/wf/GlycanEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/wf/GlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb/exdb/wf/PubChemEtlWorkflow.py` & `rcsb.exdb-0.98/rcsb/exdb/wf/PubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/rcsb.exdb.egg-info/PKG-INFO` & `rcsb.exdb-0.98/rcsb.exdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.97
+Version: 0.98
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.97/rcsb.exdb.egg-info/SOURCES.txt` & `rcsb.exdb-0.98/rcsb.exdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.97/setup.py` & `rcsb.exdb-0.98/setup.py`

 * *Files identical despite different names*

