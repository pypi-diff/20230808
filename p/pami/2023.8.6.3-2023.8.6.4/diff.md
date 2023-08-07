# Comparing `tmp/pami-2023.8.6.3.tar.gz` & `tmp/pami-2023.8.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.8.6.3.tar", last modified: Mon Aug  7 13:04:21 2023, max compression
+gzip compressed data, was "pami-2023.8.6.4.tar", last modified: Mon Aug  7 22:49:42 2023, max compression
```

## Comparing `pami-2023.8.6.3.tar` & `pami-2023.8.6.4.tar`

### file list

```diff
@@ -1,439 +1,439 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.910264 pami-2023.8.6.3/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.6.3/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.831052 pami-2023.8.6.3/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.831239 pami-2023.8.6.3/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.833095 pami-2023.8.6.3/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.833351 pami-2023.8.6.3/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.834959 pami-2023.8.6.3/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.835111 pami-2023.8.6.3/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.835912 pami-2023.8.6.3/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.836935 pami-2023.8.6.3/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.838320 pami-2023.8.6.3/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4194 2023-08-07 03:01:33.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.838695 pami-2023.8.6.3/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.840145 pami-2023.8.6.3/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15113 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/extras/dbStats/sequentialDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9475 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.840779 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.841309 pami-2023.8.6.3/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842264 pami-2023.8.6.3/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.6.3/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2428 2023-08-02 09:17:46.000000 pami-2023.8.6.3/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842488 pami-2023.8.6.3/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842749 pami-2023.8.6.3/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.843127 pami-2023.8.6.3/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.849851 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.850012 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.851095 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13539 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21425 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.851267 pami-2023.8.6.3/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.852505 pami-2023.8.6.3/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13211 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12603 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13581 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13664 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20368 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.853164 pami-2023.8.6.3/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.855073 pami-2023.8.6.3/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5835 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13146 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13904 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12502 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14048 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14219 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16723 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13776 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.855690 pami-2023.8.6.3/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25085 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.856696 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5611 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14955 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12298 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16532 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.857714 pami-2023.8.6.3/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.857884 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.858710 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25491 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.859182 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.860356 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20917 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26298 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.860529 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.861591 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27143 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.861789 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.862974 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.863146 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.864195 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23759 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.864422 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.865131 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.865311 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.866657 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.866965 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.867236 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868083 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868420 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868886 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.869053 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.870047 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.870293 pami-2023.8.6.3/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.871751 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.872297 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.873024 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.873469 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.874437 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.874921 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.875076 pami-2023.8.6.3/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.875923 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.876082 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877079 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877267 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877929 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.878083 pami-2023.8.6.3/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.880137 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50375 2023-08-07 12:47:16.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4176 2023-08-07 12:52:30.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24120 2023-08-07 12:44:11.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17698 2023-08-07 12:45:06.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-08-07 12:52:30.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.880643 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5613 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.881729 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28489 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4272 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.882362 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5775 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    30244 2023-08-07 03:36:58.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.883125 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7835 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884127 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884279 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884789 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884947 pami-2023.8.6.3/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.887479 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15647 2023-08-07 12:59:48.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25202 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24998 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16367 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33300 2023-08-07 12:59:56.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.888268 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.888848 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.889332 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.889901 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5380 2023-08-07 03:07:52.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24445 2023-08-07 03:35:37.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.890220 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.890683 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.891128 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.891299 pami-2023.8.6.3/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.893556 pami-2023.8.6.3/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.893874 pami-2023.8.6.3/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.894484 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.894624 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895032 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895185 pami-2023.8.6.3/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895281 pami-2023.8.6.3/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.896240 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18133 2023-08-02 09:17:46.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.896925 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.897034 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.898303 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.898752 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.899121 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.899257 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.901802 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.901992 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.903188 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.903529 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.904683 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.904978 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.905776 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.906005 pami-2023.8.6.3/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.906766 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.907081 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.907931 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.908093 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.908751 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 13:04:21.910051 pami-2023.8.6.3/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    60578 2023-08-02 07:28:07.000000 pami-2023.8.6.3/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.909680 pami-2023.8.6.3/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15566 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-07 13:04:21.910357 pami-2023.8.6.3/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1405 2023-08-07 13:04:00.000000 pami-2023.8.6.3/setup.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.475721 pami-2023.8.6.4/
+-rw-r--r--   0 likhitha   (505) staff       (20)    35149 2022-05-26 01:58:44.000000 pami-2023.8.6.4/LICENSE
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.368619 pami-2023.8.6.4/PAMI/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.368967 pami-2023.8.6.4/PAMI/AssociationRules/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.370677 pami-2023.8.6.4/PAMI/AssociationRules/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13175 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12870 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13078 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    12384 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6455 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/AssociationRules/basic/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      139 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.370868 pami-2023.8.6.4/PAMI/correlatedPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.372365 pami-2023.8.6.4/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    24834 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26312 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6065 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.372513 pami-2023.8.6.4/PAMI/coveragePattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.373197 pami-2023.8.6.4/PAMI/coveragePattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13863 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    15929 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7018 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.377199 pami-2023.8.6.4/PAMI/extras/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.379183 pami-2023.8.6.4/PAMI/extras/DF2DB/
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2178 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/DF2DB.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2243 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     1607 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4194 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4917 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     9942 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3607 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3359 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.382681 pami-2023.8.6.4/PAMI/extras/calculateMISValues/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/calculateMISValues/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3741 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3794 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.384373 pami-2023.8.6.4/PAMI/extras/dbStats/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/dbStats/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    13043 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    15113 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/dbStats/sequentialDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    14610 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     9475 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    13229 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    10040 2023-05-30 02:47:08.000000 pami-2023.8.6.4/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    11775 2023-05-30 02:42:12.000000 pami-2023.8.6.4/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.385303 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5195 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5925 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5919 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5803 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.386014 pami-2023.8.6.4/PAMI/extras/generateDatabase/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/generateDatabase/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2877 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7092 2023-05-31 04:57:18.000000 pami-2023.8.6.4/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3444 2023-05-31 04:55:28.000000 pami-2023.8.6.4/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3593 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.387402 pami-2023.8.6.4/PAMI/extras/graph/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1429 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2954 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1143 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     1753 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2428 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.387696 pami-2023.8.6.4/PAMI/extras/image2Database/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.387991 pami-2023.8.6.4/PAMI/extras/imageProcessing/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/imageProcessing/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4582 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.388523 pami-2023.8.6.4/PAMI/extras/neighbours/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/neighbours/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2834 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2651 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3031 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/plotPointOnMap.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     3214 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/plotPointOnMap_dump.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     2178 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.389997 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2332 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2297 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2555 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1887 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1860 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2126 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2079 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2265 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     1827 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/topKPatterns.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      473 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.390191 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.392580 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13539 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    21425 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6766 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.392748 pami-2023.8.6.4/PAMI/frequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.394517 pami-2023.8.6.4/PAMI/frequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13211 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12603 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13581 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13664 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    20368 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7733 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.395123 pami-2023.8.6.4/PAMI/frequentPattern/closed/
+-rw-r--r--   0 likhitha   (505) staff       (20)    19938 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/closed/CHARM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/closed/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6445 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.397099 pami-2023.8.6.4/PAMI/frequentPattern/cuda/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5835 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13146 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13904 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12502 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    14048 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    14219 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16723 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13776 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.397837 pami-2023.8.6.4/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25085 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/maximal/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6436 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.398940 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5611 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    14955 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12298 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16532 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.399702 pami-2023.8.6.4/PAMI/frequentPattern/topk/
+-rw-r--r--   0 likhitha   (505) staff       (20)    14742 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/frequentPattern/topk/FAE.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/topk/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4575 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.399928 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.400805 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25491 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6635 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.401117 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.404826 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    20917 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26298 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6450 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.405066 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.405912 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    24180 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    27143 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6580 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.406320 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.407391 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27023 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    32449 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6618 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.407802 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.409320 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    23759 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26218 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6668 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.409792 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.410795 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    20059 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    19117 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6680 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.411013 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.411995 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    19950 2023-06-11 10:45:26.000000 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6774 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.413197 pami-2023.8.6.4/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6676 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.413363 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.414147 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    19894 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6165 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.414334 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.414959 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    35398 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6081 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.415111 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.415572 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    39928 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6181 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.415714 pami-2023.8.6.4/PAMI/highUtilityPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.416658 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    32744 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24844 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26560 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5053 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16478 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.417138 pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5053 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16480 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.417823 pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 likhitha   (505) staff       (20)    29434 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    33678 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5195 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.418219 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6718 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.419242 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27644 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    34623 2023-06-11 10:53:12.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5955 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.419709 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    35216 2023-06-11 10:53:12.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6625 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.419880 pami-2023.8.6.4/PAMI/localPeriodicPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.421248 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    32664 2023-06-11 10:55:48.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    21999 2023-06-11 10:55:48.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    21120 2023-06-11 10:55:48.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     8378 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.421419 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.422464 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    22994 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    22318 2023-06-11 10:58:52.000000 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5913 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.422637 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.423335 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27316 2023-06-11 10:58:52.000000 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    21102 2023-06-11 10:58:52.000000 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     5392 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.423555 pami-2023.8.6.4/PAMI/partialPeriodicPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.425845 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    50375 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4176 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24120 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17698 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5550 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.426393 pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    21069 2023-06-11 11:03:52.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5613 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.426946 pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)    28489 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4272 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.427402 pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5775 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    30244 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.427901 pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7835 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17705 2023-06-16 10:18:07.000000 pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.429023 pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26067 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5550 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.429187 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.430055 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27518 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6652 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.430254 pami-2023.8.6.4/PAMI/periodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.431928 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    15648 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    25203 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24999 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16368 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    33301 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      726 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6525 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.432832 pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    21540 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6538 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.433624 pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6564 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    19356 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17474 2023-06-20 07:38:40.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.434868 pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    28740 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7873 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.435335 pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5380 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24445 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.435824 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.436771 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    18066 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6898 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.437534 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4583 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    17235 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.437767 pami-2023.8.6.4/PAMI/recurringPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.438651 pami-2023.8.6.4/PAMI/recurringPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    26300 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/recurringPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6632 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.438877 pami-2023.8.6.4/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.439496 pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26215 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4261 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.439690 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.440343 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    33570 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7391 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.440550 pami-2023.8.6.4/PAMI/sequence/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/sequence/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.440677 pami-2023.8.6.4/PAMI/sequentialPatternMining/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.442527 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    41062 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    18133 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6554 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    22592 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.443065 pami-2023.8.6.4/PAMI/sequentialPatternMining/closed/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6279 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.443171 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.459670 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    16326 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    25134 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17903 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7258 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.460728 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    26386 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7177 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.461360 pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)    14997 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6766 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.461593 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.466176 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    25974 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    26009 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    18710 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27060 2023-06-11 11:25:04.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27823 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    25507 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)    19046 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4962 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.466433 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.467410 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    28817 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5005 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.467580 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.468582 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    31092 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    31324 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6551 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.468914 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.469886 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27481 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6693 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.470127 pami-2023.8.6.4/PAMI/weightedFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.470885 pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    23859 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     6737 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.471238 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.471781 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/
+-rw-rw-r--   0 likhitha   (505) staff       (20)    27228 2023-06-11 11:25:06.000000 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     7555 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.472004 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/
+-rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.472693 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    29074 2023-08-07 22:47:35.000000 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-rw-r--   0 likhitha   (505) staff       (20)     4782 2023-05-05 14:19:32.000000 pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    61245 2023-08-07 22:49:42.475439 pami-2023.8.6.4/PKG-INFO
+-rw-r--r--   0 likhitha   (505) staff       (20)    60578 2023-08-07 22:47:35.000000 pami-2023.8.6.4/README.md
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-08-07 22:49:42.474991 pami-2023.8.6.4/pami.egg-info/
+-rw-r--r--   0 likhitha   (505) staff       (20)    61245 2023-08-07 22:49:42.000000 pami-2023.8.6.4/pami.egg-info/PKG-INFO
+-rw-r--r--   0 likhitha   (505) staff       (20)    15566 2023-08-07 22:49:42.000000 pami-2023.8.6.4/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-08-07 22:49:42.000000 pami-2023.8.6.4/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)      189 2023-08-07 22:49:42.000000 pami-2023.8.6.4/pami.egg-info/requires.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)        5 2023-08-07 22:49:42.000000 pami-2023.8.6.4/pami.egg-info/top_level.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)       38 2023-08-07 22:49:42.475787 pami-2023.8.6.4/setup.cfg
+-rw-r--r--   0 likhitha   (505) staff       (20)     1405 2023-08-07 22:49:08.000000 pami-2023.8.6.4/setup.py
```

### Comparing `pami-2023.8.6.3/LICENSE` & `pami-2023.8.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.8.6.4/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.8.6.4/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.8.6.4/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/correlatedPattern/__init__.py` & `pami-2023.8.6.4/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2023.8.6.4/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2023.8.6.4/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.8.6.4/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.8.6.4/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.8.6.4/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.8.6.4/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.8.6.4/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.8.6.4/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/sequentialDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/sequentialDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.8.6.4/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.8.6.4/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.8.6.4/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.8.6.4/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.8.6.4/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.8.6.4/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.8.6.4/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.8.6.4/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.8.6.4/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.8.6.4/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.8.6.4/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.8.6.4/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.8.6.4/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2023.8.6.4/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/plotPointOnMap.py` & `pami-2023.8.6.4/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.8.6.4/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.8.6.4/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.8.6.4/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/extras/topKPatterns.py` & `pami-2023.8.6.4/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.8.6.4/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.8.6.4/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.8.6.4/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.8.6.4/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.8.6.4/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.8.6.4/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.8.6.4/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/geoReferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.8.6.4/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.8.6.4/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.8.6.4/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2023.8.6.4/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                 item = candidates[j]
                 itemSet = item.split()
                 if prefixItemSet[:-1] == itemSet[:-1] and prefixItemSet[-1] != itemSet[-1]:
                     _value = self._finalPatterns[item][2].intersection(self._finalPatterns[prefixItem][2])
                     sup = len(_value)
                     per = self._getPeriodic(_value)
                     if sup >= self._minSup and per <= self._maxPer:
-                        newItem = prefixItem + " " + itemSet[-1]
+                        newItem = prefixItem + "\t" + itemSet[-1]
                         self._finalPatterns[newItem] = [sup, per, _value]
                         newCandidates.append(newItem)
 
         if len(newCandidates) > 0:
             self._generateEclat(newCandidates)
     
     def startMine(self):
```

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
         """ To convert the ranks of items in to their original item names
 
             :param itemSet: frequent pattern
             :return: frequent pattern with original item names
         """
         t1 = str()
         for i in itemSet:
-            t1 = t1 + self._rankedUp[i] + " "
+            t1 = t1 + self._rankedUp[i] + "\t"
         return t1
 
     def _convert(self, value):
         """
         To convert the given user specified value
 
         :param value: user specified value
```

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
         """
         To convert item ranks into original item names
         :param itemSet: periodic-frequent pattern
         :return: original itemSet
         """
         t1 = str()
         for i in itemSet:
-            t1 = t1 + self._rankedUp[i] + " "
+            t1 = t1 + self._rankedUp[i] + "\t"
         return t1
 
     def _convert(self, value):
         """
         To convert the given user specified value
 
         :param value: user specified value
```

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
                 i2_list = item2.split()
                 if i1_list[:-1] == i2_list[:-1]:
                     union_DiffSet = self._finalPatterns[item2][2].union(self._finalPatterns[item1][2])
                     sorted(union_DiffSet)
                     union_supp = self._dbSize - len(union_DiffSet)
                     period = self._getPeriodic(union_DiffSet)
                     if union_supp >= self._minSup and period <= self._maxPer:
-                        newKey = item1 + " " + i2_list[-1]
+                        newKey = item1 + "\t" + i2_list[-1]
                         self._finalPatterns[newKey] = [union_supp, period, union_DiffSet]
                         new_freqList.append(newKey)
                 else:
                     break
 
         if len(new_freqList) > 0:
             self._generateDiffsetEclat(new_freqList)
```

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,15 +822,15 @@
         info = {self._rank[k]: v for k, v in OneLengthPeriodicItems.items()}
         Tree = self._buildTree(info, OneLengthPeriodicItems)
         patterns = Tree.generatePatterns([])
         self._finalPatterns = {}
         for i in patterns:
             sample = str()
             for k in i[0]:
-                sample = sample + k + " "
+                sample = sample + k + "\t"
             self._finalPatterns[sample] = i[1]
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
```

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.8.6.4/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.8.6.4/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.8.6.4/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.8.6.4/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.8.6.4/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2023.8.6.4/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.4/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/PKG-INFO` & `pami-2023.8.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.6.3
+Version: 2023.8.6.4
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
@@ -386,9 +385,7 @@
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | PositionMining <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/contiguousFrequentPattern/basic/PositionMining.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 ## 4. Mining Graphs
 __coming soon__   
      
      
-
-
```

### Comparing `pami-2023.8.6.3/README.md` & `pami-2023.8.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.3/pami.egg-info/PKG-INFO` & `pami-2023.8.6.4/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.6.3
+Version: 2023.8.6.4
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
@@ -386,9 +385,7 @@
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | PositionMining <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/contiguousFrequentPattern/basic/PositionMining.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 ## 4. Mining Graphs
 __coming soon__   
      
      
-
-
```

### Comparing `pami-2023.8.6.3/pami.egg-info/SOURCES.txt` & `pami-2023.8.6.4/pami.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,23 +132,23 @@
 PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
 PAMI/fuzzyPeriodicFrequentPattern/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+PAMI/geoReferencedFrequentPattern/__init__.py
+PAMI/geoReferencedFrequentPattern/basic/FSPGrowth.py
+PAMI/geoReferencedFrequentPattern/basic/SpatialECLAT.py
+PAMI/geoReferencedFrequentPattern/basic/__init__.py
+PAMI/geoReferencedFrequentPattern/basic/abstract.py
 PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-PAMI/georeferencedFrequentPattern/__init__.py
-PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
-PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
-PAMI/georeferencedFrequentPattern/basic/__init__.py
-PAMI/georeferencedFrequentPattern/basic/abstract.py
 PAMI/georeferencedFrequentSequencePattern/__init__.py
 PAMI/georeferencedFrequentSequencePattern/abstract.py
 PAMI/georeferencedPartialPeriodicPattern/__init__.py
 PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
 PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
 PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
 PAMI/highUtilityFrequentPattern/__init__.py
```

### Comparing `pami-2023.8.6.3/setup.py` & `pami-2023.8.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2023.08.06.03',
+    version='2023.08.06.04',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

