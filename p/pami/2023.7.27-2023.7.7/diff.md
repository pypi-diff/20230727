# Comparing `tmp/pami-2023.7.27.tar.gz` & `tmp/pami-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.7.27.tar", last modified: Thu Jul 27 03:56:45 2023, max compression
+gzip compressed data, was "pami-2023.7.7.tar", last modified: Tue Jul 18 12:23:34 2023, max compression
```

## Comparing `pami-2023.7.27.tar` & `pami-2023.7.7.tar`

### file list

```diff
@@ -1,434 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.673537 pami-2023.7.27/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.7.27/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.611032 pami-2023.7.27/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.611207 pami-2023.7.27/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.612948 pami-2023.7.27/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.613183 pami-2023.7.27/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.614387 pami-2023.7.27/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.614529 pami-2023.7.27/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.615409 pami-2023.7.27/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.7.27/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.616565 pami-2023.7.27/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.617832 pami-2023.7.27/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4192 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.618219 pami-2023.7.27/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.619201 pami-2023.7.27/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.619876 pami-2023.7.27/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.620468 pami-2023.7.27/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.621327 pami-2023.7.27/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.621478 pami-2023.7.27/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.621707 pami-2023.7.27/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.622067 pami-2023.7.27/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.623318 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.623459 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.624723 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13292 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21358 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.624852 pami-2023.7.27/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.626109 pami-2023.7.27/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13321 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12584 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13190 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13538 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20301 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.626640 pami-2023.7.27/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19871 2023-07-26 05:11:46.000000 pami-2023.7.27/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.627884 pami-2023.7.27/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.628403 pami-2023.7.27/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25090 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.629152 pami-2023.7.27/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5605 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13201 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.629688 pami-2023.7.27/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.629826 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.630278 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.630535 pami-2023.7.27/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.631482 pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20733 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24620 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.631640 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.632300 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.632447 pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.632723 pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.632868 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.633562 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.633762 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.634540 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.634690 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.635161 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.635324 pami-2023.7.27/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.638756 pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.639008 pami-2023.7.27/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.639155 pami-2023.7.27/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.639570 pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.639716 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.640365 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.640567 pami-2023.7.27/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.641629 pami-2023.7.27/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.642101 pami-2023.7.27/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.642834 pami-2023.7.27/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.643180 pami-2023.7.27/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.643826 pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.644340 pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.644509 pami-2023.7.27/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.645322 pami-2023.7.27/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.645476 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.646269 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.646591 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.647205 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.647374 pami-2023.7.27/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.648604 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.649113 pami-2023.7.27/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.649599 pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.650097 pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.650550 pami-2023.7.27/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.650742 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.651235 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.651433 pami-2023.7.27/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.651944 pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.652128 pami-2023.7.27/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.656730 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.657286 pami-2023.7.27/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.657958 pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.658600 pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.658782 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.659356 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.659833 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.660046 pami-2023.7.27/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.660508 pami-2023.7.27/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.660670 pami-2023.7.27/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.661180 pami-2023.7.27/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26259 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.661330 pami-2023.7.27/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.661769 pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.661976 pami-2023.7.27/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.662069 pami-2023.7.27/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.662817 pami-2023.7.27/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.663541 pami-2023.7.27/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.663637 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.664584 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.665222 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.665652 pami-2023.7.27/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.665918 pami-2023.7.27/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.667727 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.667872 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.668851 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.669000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.669722 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.669858 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.670288 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.670454 pami-2023.7.27/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.670903 pami-2023.7.27/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.671161 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.671714 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.672047 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.672486 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39507 2023-07-27 03:56:45.673369 pami-2023.7.27/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    38841 2023-07-25 12:32:36.000000 pami-2023.7.27/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-27 03:56:45.673174 pami-2023.7.27/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39507 2023-07-27 03:56:45.000000 pami-2023.7.27/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15208 2023-07-27 03:56:45.000000 pami-2023.7.27/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-27 03:56:45.000000 pami-2023.7.27/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-07-27 03:56:45.000000 pami-2023.7.27/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-27 03:56:45.000000 pami-2023.7.27/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-27 03:56:45.673580 pami-2023.7.27/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1402 2023-07-27 03:50:52.000000 pami-2023.7.27/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.306139 pami-2023.7.7/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.7/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213420 pami-2023.7.7/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213780 pami-2023.7.7/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215229 pami-2023.7.7/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215381 pami-2023.7.7/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.216924 pami-2023.7.7/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.217089 pami-2023.7.7/PAMI/coveragePatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.218352 pami-2023.7.7/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.219319 pami-2023.7.7/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221044 pami-2023.7.7/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221516 pami-2023.7.7/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.223716 pami-2023.7.7/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.225281 pami-2023.7.7/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.227961 pami-2023.7.7/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231441 pami-2023.7.7/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231576 pami-2023.7.7/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231920 pami-2023.7.7/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.232234 pami-2023.7.7/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233791 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2280 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2257 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2509 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2124 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2075 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233937 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235273 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235589 pami-2023.7.7/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.237534 pami-2023.7.7/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.238433 pami-2023.7.7/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.240335 pami-2023.7.7/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.241160 pami-2023.7.7/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.242453 pami-2023.7.7/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243543 pami-2023.7.7/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243784 pami-2023.7.7/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.244809 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245067 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245890 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.246160 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247438 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247699 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.248928 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249301 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249802 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.250466 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251507 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251792 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.252874 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.254340 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255007 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255910 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256357 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256630 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257531 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257812 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261273 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261803 pami-2023.7.7/PAMI/highUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.264098 pami-2023.7.7/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265044 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16481 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265480 pami-2023.7.7/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.266895 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267687 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267930 pami-2023.7.7/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269128 pami-2023.7.7/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269369 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270382 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270633 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271619 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271849 pami-2023.7.7/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.273903 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.274936 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.275960 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.276849 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277438 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277755 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278324 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278541 pami-2023.7.7/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279293 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279512 pami-2023.7.7/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.281487 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.282417 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.283856 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19727 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.284826 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285069 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285761 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286394 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286673 pami-2023.7.7/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287396 pami-2023.7.7/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287636 pami-2023.7.7/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288407 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288643 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289267 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289510 pami-2023.7.7/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.290707 pami-2023.7.7/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291328 pami-2023.7.7/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291420 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.292688 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293628 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293913 pami-2023.7.7/PAMI/streams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294014 pami-2023.7.7/PAMI/streams/frequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294626 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31851 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7792 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295292 pami-2023.7.7/PAMI/streams/highUtility/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295424 pami-2023.7.7/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298349 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298597 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.299797 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300033 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300646 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300913 pami-2023.7.7/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.301700 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302005 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302627 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.303017 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.304367 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.305978 pami-2023.7.7/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34480 2023-07-07 08:24:43.000000 pami-2023.7.7/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.305715 pami-2023.7.7/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15099 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      102 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-18 12:23:34.306190 pami-2023.7.7/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1289 2023-07-18 12:22:32.000000 pami-2023.7.7/setup.py
```

### Comparing `pami-2023.7.27/LICENSE` & `pami-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-#  This code uses "confidence" metric to extract the association rules from given frequent patterns.
-#
+# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
+# ------------------------------------------------------------------
 #
-#     import PAMI.AssociationRules.basic import ARWithConfidence as alg
+#     import PAMI.frequentPattern.basic.ECLAT as alg
 #
-#     obj = alg.ARWithConfidence(iFile, minConf)
+#     obj = alg.ECLAT(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     associationRules = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Association Rules:", len(associationRules))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -26,15 +25,14 @@
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -44,339 +42,326 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-from PAMI.AssociationRules.basic import abstract as _ab
-
-
-class _Confidence:
-    """
-
-    :param  patterns: dict :
-                   Dictionary containing patterns and its support value.
-    :param  singleItems: list :
-                   List containing all the single frequent items.
-    :param  minConf: int :
-                   Minimum confidence to mine all the satisfying association rules.
+from PAMI.frequentPattern.basic import abstract as _ab
 
 
+class ECLAT(_ab._frequentPatterns):
     """
 
-    def __init__(self, patterns, singleItems, minConf):
-        """
-        :param patterns: given frequent patterns
-        :type patterns: dict
-        :param singleItems: one-length frequent patterns
-        :type singleItems: list
-        :param minConf: minimum confidence
-        :type minConf: float
-        """
-        self._frequentPatterns = patterns
-        self._singleItems = singleItems
-        self._minConf = minConf
-        self._finalPatterns = {}
-
-    def _generation(self, prefix, suffix):
-        """
-        To generate the combinations all association rules.
-
-        :param prefix: the prefix of association rule.
-        :type prefix: str
-        :param suffix: the suffix of association rule.
-        :type suffix: str
-        """
-        if len(suffix) == 1:
-            conf = self._generateWithConfidence(prefix, suffix[0])
-        for i in range(len(suffix)):
-            suffix1 = suffix[:i] + suffix[i + 1:]
-            prefix1 = prefix + ' ' + suffix[i]
-            for j in range(i + 1, len(suffix)):
-                self._generateWithConfidence(prefix + ' ' + suffix[i], suffix[j])
-                # self._generation(prefix+ ' ' +suffix[i], suffix[i+1:])
-            self._generation(prefix1, suffix1)
-
-    def _generateWithConfidence(self, lhs, rhs):
-        """
-        To find association rules satisfying user-specified minConf
-        :param lhs: the prefix of association rule.
-        :type lhs: str
-        :param rhs: the suffix of association rule.
-        :type rhs: str
-        """
-        s = lhs + '\t' + rhs
-        if self._frequentPatterns.get(s) == None:
-            return 0
-        minimum = self._frequentPatterns[s]
-        conf_lhs = minimum / self._frequentPatterns[lhs]
-        conf_rhs = minimum / self._frequentPatterns[rhs]
-        if conf_lhs >= self._minConf:
-            s1 = lhs + '->' + rhs
-            self._finalPatterns[s1] = conf_lhs
-        if conf_rhs >= self._minConf:
-            s1 = rhs + '->' + lhs
-            self._finalPatterns[s1] = conf_rhs
-
-    def run(self):
-        """
-        To generate the combinations all association rules.
-        """
-        for i in range(len(self._singleItems)):
-            suffix = self._singleItems[:i] + self._singleItems[i + 1:]
-            prefix = self._singleItems[i]
-            for j in range(i + 1, len(self._singleItems)):
-                self._generateWithConfidence(self._singleItems[i], self._singleItems[j])
-            self._generation(prefix, suffix)
+    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
+    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+            372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
-class ARWithConfidence:
-    """
-        :Description: Association Rules are derived from frequent patterns using "confidence" metric.
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of frequent patterns
+    :param  oFile: str :
+                   Name of the output file to store complete set of frequent patterns
+    :param  minSup: int or float or str :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-        :Reference:
 
-        :param iFile: str or df :
-                    Name of the Input file to mine the association rules
 
-        :param minConf: float
-                    The user can specify the minConf in float
-        :par sep: str :
-                    This variable is used to distinguish items from one another in given input file. The default seperator is tab space. However, the users can override their default seperator.
-        
-        
-        :Attributes:
+    :Attributes:
 
+        startTime : float
+          To record the start time of the mining process
 
-            startTime : float
-                To record the start time of the mining process
+        endTime : float
+          To record the completion time of the mining process
 
-            endTime : float
-                To record the completion time of the mining process
+        finalPatterns : dict
+          Storing the complete set of patterns in a dictionary variable
 
-            finalPatterns : dict
-              Storing the complete set of patterns in a dictionary variable
+        memoryUSS : float
+          To store the total amount of USS memory consumed by the program
 
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+          To store the total amount of RSS memory consumed by the program
 
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
+        Database : list
+          To store the transactions of a database in list
 
 
-     **Methods to execute code on terminal**
-     ----------------------------------------------------
+    **Methods to execute code on terminal**
+    ------------------------------------------
 
             Format:
-                      >>> python3 ARWithConfidence.py <inputFile> <outputFile> <minConf> <sep>
+                      >>> python3 ECLAT.py <inputFile> <outputFile> <minSup>
 
             Example:
-                     >>>  python3 ARWithConfidence.py sampleDB.txt patterns.txt 0.5 ' '
+                      >>>  python3 ECLAT.py sampleDB.txt patterns.txt 10.0
 
-            .. note:: minConf will be considered only in 0 to 1.
+            .. note:: minSup will be considered in percentage of database transactions
 
-    
-    
-    **Importing this algorithm into a python program**
-    ----------------------------------------------------
 
+    **Importing this algorithm into a python program**
+    ------------------------------------------------------------------
     .. code-block:: python
 
-             import PAMI.AssociationRules.basic import ARWithConfidence as alg
+            import PAMI.frequentPattern.basic.ECLAT as alg
 
-             obj = alg.ARWithConfidence(iFile, minConf)
+            obj = alg.ECLAT(iFile, minSup)
 
-             obj.startMine()
+            obj.startMine()
 
-             associationRules = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-             print("Total number of Association Rules:", len(associationRules))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.save(oFile)
+            obj.savePatterns(oFile)
 
-             Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-             memUSS = obj.getMemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
-             print("Total Memory in USS:", memUSS)
+            print("Total Memory in USS:", memUSS)
 
-             memRSS = obj.getMemoryRSS()
+            memRSS = obj.getMemoryRSS()
 
-             print("Total Memory in RSS", memRSS)
+            print("Total Memory in RSS", memRSS)
+
+            run = obj.getRuntime()
+
+            print("Total ExecutionTime in seconds:", run)
 
-             run = obj.getRuntime()
 
-             print("Total ExecutionTime in seconds:", run)
-            
     **Credits:**
-    -------------
+    ----------------------
+
+             The complete program was written by Kundai  under the supervision of Professor Rage Uday Kiran.
 
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
     """
 
-    _minConf = float()
+    _minSup = float()
     _startTime = float()
     _endTime = float()
+    _finalPatterns = {}
     _iFile = " "
     _oFile = " "
-    _Sep = " "
+    _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
-    _frequentPatterns = {}
+    _Database = []
 
-    def __init__(self, iFile, minConf, sep):
+    def _creatingItemSets(self):
         """
-        :param iFile: input file name or path
-        :type iFile: str
-        :param minConf: minimum confidence
-        :type minConf: float
-        :param sep: Delimiter of input file
-        :type sep: str
-        """
-        self._iFile = iFile
-        self._minConf = minConf
-        self._finalPatterns = {}
-        self._sep = sep
+            Storing the complete transactions of the database/input file in a database variable
 
-    def _readPatterns(self):
-        """
-            Reading the input file and storing all the frequent patterns and their support respectively in a frequentPatterns variable.
         """
-        self._frequentPatterns = {}
-        k = []
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            pattern, sup = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'pattern' in i:
-                pattern = self._iFile['pattern'].tolist()
-            if 'support' in i:
-                support = self._iFile['support'].tolist()
-            for i in range(len(pattern)):
-                s = '\t'.join(pattern[i])
-                self._frequentPattern[s] = support[i]
+            if 'Transactions' in i:
+                self._Database = self._iFile['Transactions'].tolist()
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line = line.strip()
-                    line = line.split(':')
-                    s = line[0].split(self._sep)
-                    s = '\t'.join(s)
-                    self._frequentPatterns[s.strip()] = int(line[1])
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            line = line.strip()
-                            line = line.split(':')
-                            s = line[0].split(self._sep)
-                            for j in s:
-                                if j not in k:
-                                    k.append(j)
-                            s = '\t'.join(s)
-                            self._frequentPatterns[s.strip()] = int(line[1])
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
-        return k
 
-    def startMine(self):
+    def _getUniqueItemList(self):
+        """
+        Generating one frequent patterns
         """
-        Association rule mining process will start from here
+        self._finalPatterns = {}
+        candidate = {}
+        uniqueItem = []
+        for i in range(len(self._Database)):
+            for j in range(len(self._Database[i])):
+                if self._Database[i][j] not in candidate:
+                    candidate[self._Database[i][j]] = {i}
+                else:
+                    candidate[self._Database[i][j]].add(i)
+        for key, value in candidate.items():
+            supp = len(value)
+            if supp >= self._minSup:
+                self._finalPatterns[key] = [value]
+                uniqueItem.append(key)
+        uniqueItem.sort()
+        return uniqueItem
+
+    def _generateFrequentPatterns(self, candidateFrequent):
+        """It will generate the combinations of frequent items
+
+        :param candidateFrequent :it represents the items with their respective transaction identifiers
+
+        :type candidateFrequent: list
+
+        :return: returning transaction dictionary
+
+        :rtype: dict
         """
+        new_freqList = []
+        for i in range(0, len(candidateFrequent)):
+            item1 = candidateFrequent[i]
+            i1_list = item1.split()
+            for j in range(i + 1, len(candidateFrequent)):
+                item2 = candidateFrequent[j]
+                i2_list = item2.split()
+                if i1_list[:-1] == i2_list[:-1]:
+                    interSet = self._finalPatterns[item1][0].intersection(self._finalPatterns[item2][0])
+                    if len(interSet) >= self._minSup:
+                        newKey = item1 + "\t" + i2_list[-1]
+                        self._finalPatterns[newKey] = [interSet]
+                        new_freqList.append(newKey)
+                else: break
+
+        if len(new_freqList) > 0:
+                self._generateFrequentPatterns(new_freqList)
+
+    def _convert(self, value):
+        """
+        To convert the user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    def startMine(self):
+        """Frequent pattern mining process will start from here"""
+
         self._startTime = _ab._time.time()
-        k = self._readPatterns()
-        a = _Confidence(self._frequentPatterns, k, self._minConf)
-        a.run()
-        self._finalPatterns = a._finalPatterns
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        uniqueItemList = self._getUniqueItemList()
+        self._generateFrequentPatterns(uniqueItemList)
+        for x, y in self._finalPatterns.items():
+            self._finalPatterns[x] = len(y[0])
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Association rules successfully  generated from frequent patterns ")
+        print("Frequent patterns were generated successfully using ECLAT algorithm")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
-        :param outFile: name of the outputfile
+        """Complete set of frequent patterns will be loaded in to a output file
+
+        :param outFile: name of the output file
+
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """ Function to send the result after completion of the mining process
-        """
-        print("Total number of Association Rules:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithConfidence(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
+            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ARWithConfidence(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Association Rules:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print(_ap.getPatternsAsDataFrame())
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  This code uses "leverage" metric to extract the association rules from given frequent patterns.
+# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
-#     import PAMI.AssociationRules.basic import ARWithLeverage as alg
+#     import PAMI.frequentPattern.cuda.cuEclat as alg
 #
-#     obj = alg.ARWithLeverage(iFile, minConf)
+#     obj = alg.cuEclat(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     associationRules = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Association Rules:", len(associationRules))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -45,331 +45,357 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-from PAMI.AssociationRules.basic import abstract as _ab
-
-
-class _Leverage:
-
-    """
-    :param  patterns: dict :
-                   Dictionary containing patterns and its support value.
-    :param  singleItems: list :
-                   List containing all the single frequent items.
-    :param  minConf: int :
-                   Minimum confidence to mine all the satisfying association rules.
-
+# from PAMI.frequentPattern.cuda import abstract as _ab
+import abstract as _ab
 
+class cuEclat(_ab._frequentPatterns):
     """
+    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
-    def __init__(self, patterns, singleItems, minConf):
-        """
-        :param patterns: given frequent patterns
-        :type inputFile: dict
-        :param singleItems: one-length frequent patterns
-        :type singleItems: list
-        :param minConf: minimum confidence
-        :type minConf: float
-        """
-        self._frequentPatterns = patterns
-        self._singleItems = singleItems
-        self._minConf = minConf
-        self._finalPatterns = {}
-
-    def _generation(self, prefix, suffix):
-        """
-
-        To generate the combinations all association rules.
-
-        :param prefix: the prefix of association rule.
-        :type prefix: str
-        :param suffix: the suffix of association rule.
-        :type suffix: str
-        """
-
-
-        if len(suffix) == 1:
-            conf = self._generateWithLeverage(prefix, suffix[0])
-        for i in range(len(suffix)):
-            suffix1 = suffix[:i] + suffix[i + 1:]
-            prefix1 = prefix + ' ' + suffix[i]
-            for j in range(i + 1, len(suffix)):
-                self._generateWithLeverage(prefix + ' ' + suffix[i], suffix[j])
-            self._generation(prefix1, suffix1)
-
-    def _generateWithLeverage(self, lhs, rhs):
-        """
-        To find association rules satisfying user-specified minConf
-        :param lhs: the prefix of association rule.
-        :type lhs: str
-        :param rhs: the suffix of association rule.
-        :type rhs: str
-        """
-        s = lhs + '\t' + rhs
-        if self._frequentPatterns.get(s) == None:
-            return 0
-        minimum = self._frequentPatterns[s]
-        conf_lhs = minimum / self._frequentPatterns[lhs]
-        conf_rhs = minimum / self._frequentPatterns[rhs]
-        lift_lhs = conf_lhs - self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
-        right_rhs = conf_rhs - self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
-        if lift_lhs >= self._minConf:
-            s1 = lhs + '->' + rhs
-            self._finalPatterns[s1] = conf_lhs
-        if right_rhs >= self._minConf:
-            s1 = rhs + '->' + lhs
-            self._finalPatterns[s1] = conf_rhs
-
-    def run(self):
-        """
-        To generate the combinations all association rules.
-        """
-        for i in range(len(self._singleItems)):
-            suffix = self._singleItems[:i] + self._singleItems[i + 1:]
-            prefix = self._singleItems[i]
-            for j in range(i + 1, len(self._singleItems)):
-                conf = self._generateWithLeverage(self._singleItems[i], self._singleItems[j])
-            self._generation(prefix, suffix)
+    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+            372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of frequent patterns
+    :param  oFile: str :
+                   Name of the output file to store complete set of frequent patterns
+    :param  minSup: int :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-class ARWithLeverage:
-    """
-       :Description: Association Rules are derived from frequent patterns using "leverage" metric.
 
-        :Reference:
 
-        :param iFile: str or df :
-                    Name of the Input file to mine the association rules
+    :Attributes:
 
-        :param minConf: float
-                    The user can specify the minConf in float
-        :par sep: str :
-                    This variable is used to distinguish items from one another in given input file. The default seperator is tab space. However, the users can override their default seperator.
-        
-        
-        :Attributes:
+        startTime : float
+          To record the start time of the mining process
 
+        endTime : float
+          To record the completion time of the mining process
 
-            startTime : float
-                To record the start time of the mining process
+        finalPatterns : dict
+          Storing the complete set of patterns in a dictionary variable
 
-            endTime : float
-                To record the completion time of the mining process
+        memoryUSS : float
+          To store the total amount of USS memory consumed by the program
 
-            finalPatterns : dict
-              Storing the complete set of patterns in a dictionary variable
+        memoryRSS : float
+          To store the total amount of RSS memory consumed by the program
 
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
+        Database : list
+          To store the transactions of a database in list
 
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
 
 
-     **Methods to execute code on terminal**
-     ----------------------------------------------------
+    **Methods to execute code on terminal**
+    ----------------------------------------------------
 
             Format:
-                      >>> python3 ARWithLeverage.py <inputFile> <outputFile> <minConf> <sep>
+                      >>> python3 cuEclat.py <inputFile> <outputFile> <minSup>
 
             Example:
-                      >>>  python3 ARWithLeverage.py sampleDB.txt patterns.txt 10.0 ' '
+                      >>>  python3 cuEclat.py sampleDB.txt patterns.txt 10.0
+
+            .. note:: minSup will be considered in percentage of database transactions
 
-            .. note:: minConf will be considered only in 0 to 1.
 
-    
-    
     **Importing this algorithm into a python program**
     ----------------------------------------------------
 
     .. code-block:: python
 
-             import PAMI.AssociationRules.basic import ARWithLeverage as alg
+             import PAMI.frequentPattern.cuda.cuEclat as alg
 
-             obj = alg.ARWithLeverage(iFile, minConf)
+             obj = alg.cuEclat(iFile, minSup)
 
              obj.startMine()
 
-             associationRules = obj.getPatterns()
+             frequentPatterns = obj.getPatterns()
 
-             print("Total number of Association Rules:", len(associationRules))
+             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.save(oFile)
+             obj.savePatterns(oFile)
 
              Df = obj.getPatternInDataFrame()
 
              memUSS = obj.getMemoryUSS()
 
              print("Total Memory in USS:", memUSS)
 
              memRSS = obj.getMemoryRSS()
 
              print("Total Memory in RSS", memRSS)
 
              run = obj.getRuntime()
 
              print("Total ExecutionTime in seconds:", run)
-            
+
+
     **Credits:**
     -------------
 
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+
     """
 
-    def __init__(self, iFile, minConf, sep):
-        """
-        :param inputFile: input file name or path
-        :type inputFile: str
-        :param sep:
-        """
-        self._iFile = iFile
-        self._minConf = minConf
-        self._finalPatterns = {}
-        self._sep = sep
+    _ab._cp.cuda.Device(0).use()
+
+
+
+    _minSup = float()
+    _startTime = float()
+    _endTime = float()
+    _finalPatterns = {}
+    _iFile = " "
+    _oFile = " "
+    _sep = " "
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+
+    _sumKernel = _ab._cp.RawKernel(r'''
+
+    #define uint32_t unsigned int
 
-    def _readPatterns(self):
+    extern "C" __global__
+
+    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
+    {
+        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
+        if (i < numElements)
+        {  
+            atomicAdd(&sum[0], __popc(d_a[i]));
+        }
+        return;    
+    }
+
+    ''', 'sumKernel')
+
+
+    def _creatingItemSets(self):
         """
-                To read patterns  of leverage.
+            Storing the complete transactions of the database/input file in a database variable
+
+
         """
-        self._frequentPatterns = {}
-        k = []
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            pattern, sup = [], []
+            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'pattern' in i:
-                pattern = self._iFile['pattern'].tolist()
-            if 'support' in i:
-                support = self._iFile['support'].tolist()
-            for i in range(len(pattern)):
-                s = '\t'.join(pattern[i])
-                self._frequentPattern[s] = support[i]
+            if 'Transactions' in i:
+                temp = self._iFile['Transactions'].tolist()
+
+            for k in temp:
+                self._Database.append(set(k))
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line = line.strip()
-                    line = line.split(':')
-                    s = line[0].split(self._sep)
-                    s = '\t'.join(s)
-                    self._frequentPatterns[s.strip()] = int(line[1])
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(set(temp))
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            line = line.strip()
-                            line = line.split(':')
-                            s = line[0].split(self._sep)
-                            for j in s:
-                                if j not in k:
-                                    k.append(j)
-                            s = '\t'.join(s)
-                            self._frequentPatterns[s.strip()] = int(line[1])
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
-        return k
 
+    def _convert(self, value):
+        """
+        To convert the user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+    
+    def arraysAndItems(self):
+        ArraysAndItems = {}
+
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                j = tuple([j])
+                if j not in ArraysAndItems:
+                    ArraysAndItems[j] = [i]
+                else:
+                    ArraysAndItems[j].append(i)
+
+        newArraysAndItems = {}
+
+        for k,v in ArraysAndItems.items():
+            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
+            if len(v) >= self._minSup:
+                self._finalPatterns[k] = len(v)
+                newArraysAndItems[k] = ArraysAndItems[k]
+
+        return newArraysAndItems
+
+    
     def startMine(self):
         """
-                Association rule mining process will start from here
+            Frequent pattern mining process will start from here
         """
+        self._Database = []
         self._startTime = _ab._time.time()
-        k = self._readPatterns()
-        a = _Leverage(self._frequentPatterns, k, self._minConf)
-        a.run()
-        self._finalPatterns = a._finalPatterns
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+
+        ArraysAndItems = self.arraysAndItems()
+
+        while len(ArraysAndItems) > 0:
+            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
+            newArraysAndItems = {}
+            keys = list(ArraysAndItems.keys())
+            for i in range(len(ArraysAndItems)):
+                iList = list(keys[i])
+                for j in range(i+1, len(ArraysAndItems)):
+                    # print(i, "/", len(ArraysAndItems), end="\r")
+                    jList = list(keys[j])
+                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
+                        union = iList + [jList[-1]]
+                        union = tuple(union)
+                        intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]], assume_unique=True)
+                        if len(intersect) >= self._minSup:
+                            newArraysAndItems[union] = intersect
+                            self._finalPatterns[union] = len(intersect)
+                    else: 
+                        break
+
+            ArraysAndItems = newArraysAndItems
+            # print()
+
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Association rules successfully  generated from frequent patterns ")
+        print("Frequent patterns were generated successfully using cuEclat algorithm ")
+            
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
-        :param outFile: name of the outputfile
+        """Complete set of frequent patterns will be loaded in to a output file
+
+        :param outFile: name of the output file
+
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """ Function to send the result after completion of the mining process
-        """
-        print("Total number of Association Rules:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in s:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithLeverage(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
+            _ap = cuEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ARWithLeverage(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuEclat(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Association Rules:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        print("Total ExecutionTime in s:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
 
+    _ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
+    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+    _ap.startMine()
+    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+    print("Total Memory in USS:", _ap.getMemoryUSS())
+    print("Total Memory in RSS", _ap.getMemoryRSS())
+    print("Total ExecutionTime in s:", _ap.getRuntime())
+
```

### Comparing `pami-2023.7.27/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-#  This code uses "lift" metric to extract the association rules from given frequent patterns.
+#  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
+#  **Importing this algorithm into a python program**
+#  ---------------------------------------------------------
 #
-# **Importing this algorithm into a python program**
-# ----------------------------------------------------
+#     import PAMI.frequentPattern.basic.ECLATbitset as alg
 #
-#     import PAMI.AssociationRules.basic import ARWithLift as alg
-#
-#     obj = alg.ARWithLift(iFile, minConf)
+#     obj = alg.ECLATbitset(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     associationRules = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Association Rules:", len(associationRules))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
+#
+#
+#
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -45,256 +47,264 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+from PAMI.frequentPattern.basic import abstract as _ab
 
-from PAMI.AssociationRules.basic import abstract as _ab
-
-class Lift:
-
+class ECLATbitset(_ab._frequentPatterns):
     """
-    :param  patterns: dict :
-                   Dictionary containing patterns and its support value.
-    :param  singleItems: list :
-                   List containing all the single frequent items.
-    :param  minConf: int :
-                   Minimum confidence to mine all the satisfying association rules.
-
-    """
-    
-    def __init__(self, patterns, singleItems, minConf):
-        """
-        :param patterns: given frequent patterns
-        :type inputFile: dict
-        :param singleItems: one-length frequent patterns
-        :type singleItems: list
-        :param minConf: minimum confidence
-        :type minConf: float
-        """
-        self._frequentPatterns = patterns
-        self._singleItems = singleItems
-        self._minConf = minConf
-        self._finalPatterns = {}
-
-    def _generation(self, prefix, suffix):
-        """
-        To generate the combinations all association rules.
-
-        :param prefix: the prefix of association rule.
-        :type prefix: str
-        :param suffix: the suffix of association rule.
-        :type suffix: str
-        """
-        if len(suffix) == 1:
-            self._generateWithLift(prefix, suffix[0])
-        for i in range(len(suffix)):
-            suffix1 = suffix[:i] + suffix[i + 1:]
-            prefix1 = prefix + ' ' + suffix[i]
-            for j in range(i + 1, len(suffix)):
-                self._generateWithLift(prefix + ' ' + suffix[i], suffix[j])
-                # self._generation(prefix+ ' ' +suffix[i], suffix[i+1:])
-            self._generation(prefix1, suffix1)
-
-    def _generateWithLift(self, lhs, rhs):
-        """
-        To find association rules satisfying user-specified minConf
-        :param lhs: the prefix of association rule.
-        :type lhs: str
-        :param rhs: the suffix of association rule.
-        :type rhs: str
-        """
-        s = lhs + '\t' + rhs
-        if self._frequentPatterns.get(s) == None:
-            return 0
-        minimum = self._frequentPatterns[s]
-        conf_lhs = minimum / self._frequentPatterns[lhs]
-        conf_rhs = minimum / self._frequentPatterns[rhs]
-        lift_lhs = conf_lhs / self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
-        right_rhs = conf_rhs / self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
-        if lift_lhs >= self._minConf:
-            s1 = lhs + '->' + rhs
-            self._finalPatterns[s1] = conf_lhs
-        if right_rhs >= self._minConf:
-            s1 = rhs + '->' + lhs
-            self._finalPatterns[s1] = conf_rhs
-
-    def run(self):
-        """
-        To generate the combinations all association rules.
-        """
-        for i in range(len(self._singleItems)):
-            suffix = self._singleItems[:i] + self._singleItems[i + 1:]
-            prefix = self._singleItems[i]
-            for j in range(i + 1, len(self._singleItems)):
-                self._generateWithLift(self._singleItems[i], self._singleItems[j])
-            self._generation(prefix, suffix)
+    :Description:  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
+    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+            372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
-class ARWithLift:
-    """
-        :Description: Association Rules are derived from frequent patterns using "lift" metric.
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of frequent patterns
+    :param  oFile: str :
+                   Name of the output file to store complete set of frequent patterns
+    :param  minSup: int or float or str :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-        :Reference:
 
-        :param iFile: str or df :
-                    Name of the Input file to mine the association rules
 
-        :param minConf: float
-                    The user can specify the minConf in float
-        :par sep: str :
-                    This variable is used to distinguish items from one another in given input file. The default seperator is tab space. However, the users can override their default seperator.
-        
-        
-        :Attributes:
-        ------------
+    :Attributes:
 
+        startTime : float
+          To record the start time of the mining process
 
-            startTime : float
-                To record the start time of the mining process
+        endTime : float
+          To record the completion time of the mining process
 
-            endTime : float
-                To record the completion time of the mining process
+        finalPatterns : dict
+          Storing the complete set of patterns in a dictionary variable
 
-            finalPatterns : dict
-              Storing the complete set of patterns in a dictionary variable
+        memoryUSS : float
+          To store the total amount of USS memory consumed by the program
 
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+          To store the total amount of RSS memory consumed by the program
 
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
+        Database : list
+          To store the transactions of a database in list
 
 
-     **Methods to execute code on terminal**
-     ----------------------------------------------------
+    **Methods to execute code on terminal**
+    ----------------------------------------
 
             Format:
-                      >>> python3 ARWithLift.py <inputFile> <outputFile> <minConf> <sep>
+                      >>> python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
 
             Example:
-                      >>>  python3 ARWithLift.py sampleDB.txt patterns.txt 0.5 ' '
+                      >>> python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
 
-            .. note:: minConf will be considered only in 0 to 1.
+            .. note:: minSup will be considered in percentage of database transactions
 
-    
-    
-    **Importing this algorithm into a python program**
-    ----------------------------------------------------
 
+    **Importing this algorithm into a python program**
+    ---------------------------------------------------------
     .. code-block:: python
 
-             import PAMI.AssociationRules.basic import ARWithLift as alg
+                import PAMI.frequentPattern.basic.ECLATbitset as alg
 
-             obj = alg.ARWithLift(iFile, minConf)
+                obj = alg.ECLATbitset(iFile, minSup)
 
-             obj.startMine()
+                obj.startMine()
 
-             associationRules = obj.getPatterns()
+                frequentPatterns = obj.getPatterns()
 
-             print("Total number of Association Rules:", len(associationRules))
+                print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.save(oFile)
+                obj.savePatterns(oFile)
 
-             Df = obj.getPatternInDataFrame()
+                Df = obj.getPatternInDataFrame()
 
-             memUSS = obj.getMemoryUSS()
+                memUSS = obj.getMemoryUSS()
 
-             print("Total Memory in USS:", memUSS)
+                print("Total Memory in USS:", memUSS)
 
-             memRSS = obj.getMemoryRSS()
+                memRSS = obj.getMemoryRSS()
 
-             print("Total Memory in RSS", memRSS)
+                print("Total Memory in RSS", memRSS)
 
-             run = obj.getRuntime()
+                run = obj.getRuntime()
+
+                print("Total ExecutionTime in seconds:", run)
 
-             print("Total ExecutionTime in seconds:", run)
-            
     **Credits:**
-    -------------
+    -------------------
+
+               The complete program was written by Yudai Masu under the supervision of Professor Rage Uday Kiran.
 
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
     """
 
-    def __init__(self, iFile, minConf, sep):
-        """
-        :param inputFile: input file name or path
-        :type inputFile: str
-        :param minConf: minimum confidence
-        :type minConf: float
-        :param sep: Delimiter of input file
-        :type sep: str
-        """
-        self._iFile = iFile
-        self._minConf = minConf
-        self._finalPatterns = {}
-        self._sep = sep
+    _startTime = float()
+    _endTime = float()
+    _finalPatterns = {}
+    _iFile = " "
+    _oFile = " "
+    _sep = " "
+    _minSup = str()
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _mapSupport = {}
+    _lno = 0
+
+
+    def _convert(self, value):
+        """
+        To convert the user specified minSup value
+        :param value: user specified minSup value
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-    def _readPatterns(self):
+    def _creatingItemSets(self):
         """
-            Reading the input file and storing all the frequent patterns and their support respectively in a frequentPatterns variable.
+            Storing the complete transactions of the database/input file in a database variable
         """
-        self._frequentPatterns = {}
-        k = []
+        self._Database = []
+        self._mapSupport = {}
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            pattern, sup = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'pattern' in i:
-                pattern = self._iFile['pattern'].tolist()
-            if 'support' in i:
-                support = self._iFile['support'].tolist()
-            for i in range(len(pattern)):
-                s = '\t'.join(pattern[i])
-                self._frequentPattern[s] = support[i]
+            if 'Transactions' in i:
+                self._Database = self._iFile['Transactions'].tolist()
+
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line = line.strip()
-                    line = line.split(':')
-                    s = line[0].split(self._sep)
-                    s = '\t'.join(s)
-                    self._frequentPatterns[s.strip()] = int(line[1])
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line = line.strip()
-                            line = line.split(':')
-                            s = line[0].split(self._sep)
-                            for j in s:
-                                if j not in k:
-                                    k.append(j)
-                            s = '\t'.join(s)
-                            self._frequentPatterns[s.strip()] = int(line[1])
+                            self._lno += 1
+                            splitter = [i.rstrip() for i in line.split(self._sep)]
+                            splitter = [x for x in splitter if x]
+                            self._Database.append(splitter)
                 except IOError:
                     print("File Not Found")
-                    quit()
-        return k
+        self._minSup = self._convert(self._minSup)
 
-    def startMine(self):
+    def creatingFrequentItems(self):
         """
-        Association rule mining process will start from here
+        This function creates frequent items from _database.
+        :return: frequentTidData that stores frequent items and their tid list.
         """
+        tidData = {}
+        self._lno = 0
+        for transaction in self._Database:
+            self._lno = self._lno + 1
+            for item in transaction:
+                if item not in tidData:
+                    tidData[item] = [self._lno]
+                else:
+                    tidData[item].append(self._lno)
+        frequentTidData = {k: v for k, v in tidData.items() if len(v) >= self._minSup}
+        frequentTidData = dict(sorted(frequentTidData.items(), reverse=True, key=lambda x: len(x[1])))
+        return frequentTidData
+
+    def tidToBitset(self,itemset):
+        """
+        This function converts tid list to bitset.
+        :param itemset:
+        :return:
+        """
+        bitset = {}
+
+        for k,v in itemset.items():
+            bitset[k] = 0b1
+            bitset[k] = (bitset[k] << int(v[0])) | 0b1
+            for i in range(1,len(v)):
+                diff = int(v[i]) - int(v[i-1])
+                bitset[k] = (bitset[k] << diff) | 0b1
+            bitset[k] = (bitset[k] << (self._lno - int(v[i])))
+        return bitset
+
+    def genPatterns(self,prefix,tidData):
+        """
+        This function generate frequent pattern about prefix.
+        :param prefix: String
+        :param tidData: list
+        :return:
+        """
+        # variables to store frequent item set and
+        itemset = prefix[0]
+
+        # Get the length of tidData
+        length = len(tidData)
+
+        for i in range(length):
+            #tid = prefix[1].intersection(tidData[i][1])
+            tid = prefix[1] & tidData[i][1]
+            count = bin(tid).count("1") - 1
+            #tidLength = len(tid)
+            if count >= self._minSup:
+                frequentItemset = itemset + '\t' + tidData[i][0]
+                self._finalPatterns[frequentItemset] = count
+                self.genPatterns((frequentItemset,tid),tidData[i+1:length])
+
+    def genAllFrequentPatterns(self,frequentItems):
+        """
+        This function generates all frequent patterns.
+        :param frequentItems: frequent items
+        :return:
+        """
+        tidData = list(frequentItems.items())
+        length = len(tidData)
+        for i in range(length):
+            #print(i,tidData[i][0])
+            self.genPatterns(tidData[i],tidData[i+1:length])
+
+    def startMine(self):
+        """Frequent pattern mining process will start from here
+                We start with the scanning the itemSets and store the bitsets respectively.
+                We form the combinations of single items and  check with minSup condition to check the frequency of patterns
+                """
+
         self._startTime = _ab._time.time()
-        k = self._readPatterns()
-        a = Lift(self._frequentPatterns, k, self._minConf)
-        a.run()
-        self._finalPatterns = a._finalPatterns
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+
+        self._creatingItemSets()
+        frequentItems = self.creatingFrequentItems()
+        self._finalPatterns = {k: len(v) for k, v in frequentItems.items()}
+        frequentItemsBitset = self.tidToBitset(frequentItems)
+        self.genAllFrequentPatterns(frequentItemsBitset)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Association rules successfully  generated from frequent patterns ")
+        print("Frequent patterns were generated successfully using Eclat_bitset algorithm")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
@@ -323,52 +333,48 @@
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
-        :param outFile: name of the outputfile
+        """Complete set of frequent patterns will be loaded in to a output file
+        :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """ Function to send the result after completion of the mining process
-        """
-        print("Total number of Association Rules:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
-
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
-if __name__ == "__main__":
+if __name__=="__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithLift(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
+            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ARWithLift(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Association Rules:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-__copyright__ = """
-
- Copyright (C)  2021 Rage Uday Kiran
-
-     This program is free software: you can redistribute it and/or modify
-     it under the terms of the GNU General Public License as published by
-     the Free Software Foundation, either version 3 of the License, or
-     (at your option) any later version.
-
-     This program is distributed in the hope that it will be useful,
-     but WITHOUT ANY WARRANTY; without even the implied warranty of
-     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-     GNU General Public License for more details.
-
-     You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-     This program is free software: you can redistribute it and/or modify
-     it under the terms of the GNU General Public License as published by
-     the Free Software Foundation, either version 3 of the License, or
-     (at your option) any later version.
-
-     This program is distributed in the hope that it will be useful,
-     but WITHOUT ANY WARRANTY; without even the implied warranty of
-     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-     GNU General Public License for more details.
-
-     You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-"""
+#  Copyright (C)  2021 Rage Uday Kiran
+#
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
+#
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
+#
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
@@ -41,21 +37,21 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _AssociationRules(_ABC):
+class _fuzzyFrequentPattenrs(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-       Attributes:
-       ----------
+    Attributes :
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -71,16 +67,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+    Methods :
+    -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -90,36 +86,36 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minConf, sep="\t"):
+    def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
-        self._minConf = minConf
-        self._finalPatterns = {}
-        self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._minSup = minSup
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._oFile = str()
+        self._finalPatterns = {}
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -153,18 +149,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-        pass
+
 
     @_abstractmethod
     def printResults(self):
-        """ To print result of the execution"""
+        """ To print all the results of execution"""
 
         pass
```

### Comparing `pami-2023.7.27/PAMI/correlatedPattern/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# CoMine is one of the fundamental algorithm to discover correlated patterns in a transactional database.
+# CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.correlatedPattern.basic import CoMine as alg
+#             from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
 #
-#             obj = alg.CoMine(iFile, minSup, minAllConf, sep)
+#             obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
 #
 #             obj.startMine()
 #
 #             Rules = obj.getPatterns()
 #
 #             print("Total number of  Patterns:", len(Patterns))
 #
-#             obj.save(oFile)
+#             obj.savePatterns(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -53,15 +53,15 @@
 
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 
 class _Node:
     """
-    A class used to represent the node of correlatedPatternTree
+    A class used to represent the node of frequentPatternTree
 
 
     Attributes :
     ----------
         itemId : int
             storing item of a node
         counter : int
@@ -73,40 +73,34 @@
         nodeLink : node
             Points to the node with same itemId
 
     Methods :
     -------
 
         getChild(itemName)
-            returns the node with same itemName from correlatedPatternTree
+            returns the node with same itemName from frequentPatternTree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
         self.nodeLink = None
 
     def getChild(self, id1):
-        """
-
-        Param id1: give item id as input
-        type id1:
-
-        """
         for i in self.child:
             if i.itemId == id1:
                 return i
         return None
 
 
 class _Tree:
     """
-        A class used to represent the correlatedPatternGrowth tree structure
+        A class used to represent the frequentPatternGrowth tree structure
 
     Attributes :
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
@@ -117,34 +111,34 @@
 
 
     Methods :
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in correlatedPatternTree
+            creating transaction as a branch in frequentPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
         printTree(Node)
-            gives the details of node in correlatedPatternGrowth tree
+            gives the details of node in frequentPatternGrowth tree
         addPrefixPath(prefix,port,minSup)
            It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
         """
         adding transaction into tree
 
-        :param transaction : it represents a single transaction in a database
+        :param transaction : it represents the one transactions in database
         :type transaction : list
         """
 
         current = self.root
         for i in transaction:
             child = current.getChild(i)
             if child is None:
@@ -156,36 +150,37 @@
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
         """
-        Fixing node link for the newNode that inserted into correlatedPatternTree
+        Fixing node link for the newNode that inserted into frequentPatternTree
 
         :param item: it represents the item of newNode
         :type item : int
-        :param newNode : it represents the newNode that inserted in correlatedPatternTree
+        :param newNode : it represents the newNode that inserted in frequentPatternTree
         :type newNode : Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
         """
-        This method is to find the details of parent, children, and support of a Node
+        This method is to find the details of parent,children,support of Node
 
-        :param root: it represents the Node in correlatedPatternTree
+        :param root: it represents the Node in frequentPatternTree
         :type root: Node
 
+        
         """
 
         if root.child is None:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
@@ -206,15 +201,15 @@
             if y >= minSup:
                 t1.append(x)
         itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
     def addPrefixPath(self, prefix, mapSupportBeta, minSup):
         """
-        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
+        To construct the conditional tree with prefix paths of a node in frequentPatternTree
 
         :param prefix : it represents the prefix items of a Node
         :type prefix : list
         :param mapSupportBeta : it represents the items with their supports
         :param mapSupportBeta : dictionary
         :param minSup : to check the item meets with minSup
         :param minSup : float
@@ -235,32 +230,33 @@
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CoMine(_ab._correlatedPatterns):
+class CPGrowth(_ab._correlatedPatterns):
     """
-    :Description: CoMine is one of the fundamental algorithm to discover correlated  patterns in a transactional database. It is based on the traditional FP-Growth algorithm. This algorithm uses depth-first search technique to find all correlated patterns in a transactional database.
+    :Description: CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database. It is based on the traditional Fpgrowth Algorithm, this algorithm uses breadth-first search technique to find the correlated Frequent patterns in transactional database.
 
     :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
-
     :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-    :param minAllConf: float :
-                    The user can specify minAllConf values within the range (0, 1).
+    :param minAllConf: str : Name of Neighbourhood file name
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
+
+
+
     :Attributes:
 
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
         startTime:float
@@ -289,37 +285,37 @@
            it represents the constraint for pattern length
 
 
     **Methods to execute code on terminal**
     ----------------------------------------
 
             Format:
-                      >>> python3 CoMine.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+                      >>> python3 CSPGrowth.py <inputFile> <outputFile> <neighbourFile> <minSup> <minAllConf> <sep>
             Example:
-                      >>>  python3 CoMine.py sampleTDB.txt output.txt 0.25 0.2
+                      >>>  python3 CSPGrowth.py sampleTDB.txt output.txt sampleN.txt 0.25 0.2
 
                      .. note:: minSup will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
     --------------------------------------------------------------------------------
     .. code-block:: python
 
-            from PAMI.correlatedPattern.basic import CoMine as alg
+            from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
 
-            obj = alg.CoMine(iFile, minSup, minAllConf,sep)
+            obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
 
             obj.startMine()
 
-            patterns = obj.getPatterns()
+            Rules = obj.getPatterns()
 
-            print("Total number of  Patterns:", len(patterns))
+            print("Total number of  Patterns:", len(Patterns))
 
             obj.savePatterns(oFile)
 
-            df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
@@ -351,22 +347,14 @@
     _itemSetBuffer = None
     _fpNodeTempBuffer = []
     _itemSetCount = 0
     _maxPatternLength = 1000
     _sep = "\t"
 
     def __init__(self, iFile, minSup, minAllConf, sep="\t"):
-        """param iFile: give the input file
-           type iFile: str or DataFrame or url
-           param minSup: minimum support
-           type minSup:   int or float
-           param sep: Delimiter of input file
-           type sep: str
-        """
-
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
             """
@@ -413,46 +401,45 @@
         maximums = 0
         for ele in range(prefixLength):
             i = prefix[ele]
             if maximums < self._mapSupport.get(i):
                 maximums = self._mapSupport.get(i)
         return s / maximums
 
-    def _correlatedOneItem(self):
-        """
-            Generating One correlated item
+    def _frequentOneItem(self):
+        """Generating One frequent items sets
+
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
     def _saveItemSet(self, prefix, prefixLength, support):
-        """
-        To save the correlated patterns mined form correlatedPatternTree
+        """To save the frequent patterns mined form frequentPatternTree
 
-        :param prefix: the correlated pattern
+        :param prefix: the frequent pattern
         :type prefix: list
-        :param prefixLength : the length of a correlated pattern
+        :param prefixLength : the length of a frequent pattern
         :type prefixLength : int
         :param support: the support of a pattern
         :type support :  int
-        :The correlated patterns were stored in a global variable finalPatterns
+        :The frequent patterns are update into global variable finalPatterns
         """
-        all_conf = self._getRatio(prefix, prefixLength, support)
-        if all_conf < self._minAllConf:
+        allconf = self._getRatio(prefix, prefixLength, support)
+        if allconf < self._minAllConf:
             return
         l = []
         for i in range(prefixLength):
             l.append(prefix[i])
         self._itemSetCount += 1
-        self._finalPatterns[tuple(l)] = [support, all_conf]
+        self._finalPatterns[tuple(l)] = [support, allconf]
     
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
@@ -465,17 +452,17 @@
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
     def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
-        """Generating all the combinations for items in single branch in correlatedPatternTree
+        """Generating all the combinations for items in single branch in frequentPatternTree
 
-        :param tempBuffer: items in a single branch
+        :param tempBuffer: items in a list
         :type tempBuffer: list
         :param s : support at leaf node of a branch
         :param position : the length of a tempBuffer
         :type position : int
         :param prefix : it represents the list of leaf node
         :type prefix : list
         :param prefixLength : the length of prefix
@@ -488,59 +475,59 @@
             for j in range(position):
                 isSet = i & (1 << j)
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
             self._saveItemSet(prefix, newPrefixLength, s)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport):
+    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport):
         """
 
         Mining the fp tree
 
-        :param correlatedPatternTree: it represents the correlatedPatternTree
-        :type correlatedPatternTree: class Tree
-        :param prefix : it represents an empty list and store the patterns that are mined
+        :param frequentPatternTree: it represents the frequentPatternTree
+        :type frequentPatternTree: class Tree
+        :param prefix : it represents a empty list and store the patterns that are mined
         :type prefix : list
-        :param prefixLength : the length of prefix
+        :param param prefixLength : the length of prefix
         :type prefixLength :int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
 
         """
 
         singlePath = True
         position = 0
         s = 0
-        if len(correlatedPatternTree.root.child) > 1:
+        if len(frequentPatternTree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = correlatedPatternTree.root.child[0]
+            currentNode = frequentPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
                 self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(correlatedPatternTree.headerList):
+            for i in reversed(frequentPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
                 betaSupport = support
                 prefix.insert(prefixLength, item)
                 self._saveItemSet(prefix, prefixLength + 1, betaSupport)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = correlatedPatternTree.mapItemNodes.get(item)
+                    path = frequentPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
                             prefixPath = []
                             prefixPath.append(path)
                             pathCount = path.counter
                             parent1 = path.parent
@@ -554,43 +541,43 @@
                             prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
+                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
     
     def startMine(self):
         """
         main method to start
 
         """
         self._startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         self._tree = _Tree()
         self._finalPatterns = {}
-        self._correlatedOneItem()
+        self._frequentOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
-        print("Correlated patterns were generated successfully using CoMine algorithm")
+            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
+        print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
@@ -624,17 +611,17 @@
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
 
-        Storing final correlated patterns in a dataframe
+        Storing final frequent patterns in a dataframe
 
-        :return: returning correlated patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             pat = " "
@@ -642,55 +629,50 @@
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
         """
-        Complete set of correlated patterns will be saved into an output file
+        Complete set of frequent patterns will be loaded in to a output file
 
-        :param outFile: name of the outputfile
+        :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             pat = ""
             for i in x:
                 pat += str(i) + "\t"
             patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """
-        Function to send the set of correlated patterns after completion of the mining process
+        Function to send the set of frequent patterns after completion of the mining process
 
-        :return: returning correlated patterns
+        :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """
-
-        function to print the result after completing the process
-
-        """
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = CPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = CPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
```

### Comparing `pami-2023.7.27/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# CPGrowthPlus is one of the efficient algorithm to discover Correlated patterns in a transactional database.
+# CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
 #
 #  **Importing this algorithm into a python program**
 #   -----------------------------------------------
 #
-#                 from PAMI.correlatedPattern.basic import CPGrowthPlus as alg
+#                 from PAMI.coveragePattern.basic import CPPG as alg
 #
-#                 obj = alg.CPGrowthPlus(iFile, minSup, minAllConf, sep)
+#                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 #
 #                 obj.startMine()
 #
-#                 correlatedPattern = obj.getPatterns()
+#                 coveragePatterns = obj.getPatterns()
 #
-#                 print("Total number of correlated Patterns:", len(correlatedPattern))
+#                 print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -25,14 +25,17 @@
 #
 #                 print("Total Memory in RSS", memRSS)
 #
 #                 run = obj.getRuntime()
 #
 #                 print("Total ExecutionTime in seconds:", run)
 
+
+
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -46,17 +49,18 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 
 
+
 class _Node:
     """
-        A class used to represent the node of correlatedPatternTree
+        A class used to represent the node of frequentPatternTree
 
     Attributes :
     ----------
         itemId: int
             storing item of a node
         counter: int
             To maintain the support of node
@@ -67,15 +71,15 @@
         nodeLink : node
             Points to the node with same itemId
 
     Methods :
     -------
 
         getChild(itemName)
-            returns the node with same itemName from correlatedPatternTree
+            returns the node with same itemName from frequentPatternTree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
@@ -83,27 +87,27 @@
 
     def getChild(self, itemName):
         """
         Retrieving the child from the tree
 
             :param itemName: name of the child
             :type itemName: list
-            :return: returns the node with same itemName from correlatedPatternTree
+            :return: returns the node with same itemName from frequentPatternTree
             :rtype: list
 
         """
         for i in self.child:
             if i.itemId == itemName:
                 return i
         return None
 
 
 class _Tree:
     """
-        A class used to represent the correlatedPatternGrowth tree structure
+        A class used to represent the frequentPatternGrowth tree structure
 
     Attributes :
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
@@ -113,34 +117,34 @@
             representing the root Node in a tree
 
     Methods :
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in correlatedPatternTree
+            creating transaction as a branch in frequentPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
         printTree(Node)
-            gives the details of node in correlatedPatternGrowth tree
+            gives the details of node in frequentPatternGrowth tree
         addPrefixPath(prefix,port,minSup)
            It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
         """
         Adding a transaction into a tree
 
-        :param transaction: it represents a transaction in a database
+        :param transaction: it represents the one transactions in database
         :type transaction: list
         """
 
         # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
@@ -153,78 +157,80 @@
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
         """
-        Fixing node link for the newNode that inserted into correlatedPatternTree
+        Fixing node link for the newNode that inserted into frequentPatternTree
 
         :param item: it represents the item of newNode
         :type item: int
-        :param newNode: it represents the newNode that inserted in correlatedPatternTree
+        :param newNode: it represents the newNode that inserted in frequentPatternTree
         :type newNode: Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
         """
 
-        Print the details of Node in correlatedPatternTree
+        Print the details of Node in frequentPatternTree
 
-        :param root: it represents the Node in correlatedPatternTree
+        :param root: it represents the Node in frequentPatternTree
         :type root: Node
 
         """
+
         # this method is used print the details of tree
         if not root.child:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
     def createHeaderList(self, mapSupport, minSup):
         """
+
         To create the headerList
 
         :param mapSupport: it represents the items with their supports
         :type mapSupport: dictionary
         :param minSup: it represents the minSup
         :param minSup: float
 
         """
-        # the correlatedPatternTree always maintains the header table to start the mining from leaf nodes
+        # the frequentPatternTree always maintains the header table to start the mining from leaf nodes
         t1 = []
         for x, y in mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda val: val[1], reverse=True)]
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
     def addPrefixPath(self, prefix, mapSupportBeta, minSup):
         """
 
-        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
+        To construct the conditional tree with prefix paths of a node in frequentPatternTree
 
         :param prefix: it represents the prefix items of a Node
         :type prefix: list
         :param mapSupportBeta: it represents the items with their supports
         :param mapSupportBeta: dictionary
         :param minSup: to check the item meets with minSup
         :param minSup: float
 
         """
-        # this method is used to add prefix paths in conditional trees of correlatedPatternTree
+        # this method is used to add prefix paths in conditional trees of frequentPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
             if mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
@@ -237,27 +243,29 @@
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CoMinePlus(_ab._correlatedPatterns):
+class CPGrowthPlus(_ab._correlatedPatterns):
     """ 
-    :Description:    CoMinePlus is one of the efficient algorithm to discover correlated patterns in a transactional database. Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that have support within specified interval.
+    :Description:    CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
+                     Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that
+                     have support within specified interval.
 
     :Reference:
         Uday Kiran R., Kitsuregawa M. (2012) Efficient Discovery of Correlated Patterns in Transactional Databases Using Items’ Support Intervals.
         In: Liddle S.W., Schewe KD., Tjoa A.M., Zhou X. (eds) Database and Expert Systems Applications. DEXA 2012. Lecture Notes in Computer Science, vol 7446. Springer, Berlin, Heidelberg.
         https://doi.org/10.1007/978-3-642-32600-4_18
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  minAllConf: str :
                    Name of Neighbourhood file name
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
@@ -293,39 +301,39 @@
         maxPatternLength : int
            it represents the constraint for pattern length
 
     **Methods to execute code on terminal**
     ---------------------------------------
 
             Format:
-                      >>>  python3 CoMinePlus.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+                      >>>  python3 CPPG.py <inputFile> <outputFile> <minRF> <minCS> <maxOR> <'\t'>
 
             Example:
-                      >>>   python3 CoMinePlus.py sampleTDB.txt patterns.txt 0.4 0.5 ','
+                      >>>   python3 CPPG.py sampleTDB.txt patterns.txt 0.4 0.7 0.5 ','
 
 
 
     **Importing this algorithm into a python program**
     -----------------------------------------------------------------
 
     .. code-block:: python
 
-                from PAMI.correlatedPattern.basic import CoMinePlus as alg
+                from PAMI.coveragePattern.basic import CPPG as alg
 
-                obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
+                obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 
                 obj.startMine()
 
-                correlatedPatterns = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of correlated patterns:", len(correlatedPatterns))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
-                df = obj.getPatternsAsDataFrame()
+                Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
                 print("Total Memory in USS:", memUSS)
 
                 memRSS = obj.getMemoryRSS()
 
@@ -359,30 +367,22 @@
     _itemSetBuffer = None
     _fpNodeTempBuffer = []
     _itemSetCount = 0
     _maxPatternLength = 1000
     _sep = "\t"
 
     def __init__(self, iFile, minSup, minAllConf, sep="\t"):
-        """
-        param iFile: input file name
-        type iFile: str or DataFrame or url
-        param minSup: user-specified minimum support
-        type minSup: int or float
-        param minAllConf: user-specified minimum all confidence
-        type minAllConf: float
-        param sep: delimiter of input file
-        type sep : str
-        """
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
-        """
+
+
+            """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
@@ -403,50 +403,50 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _correlatedOneItem(self):
+    def _frequentOneItem(self):
         """
-        Generating One correlated items sets
+        Generating One frequent items sets
 
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
     def _saveItemSet(self, prefix, prefixLength, support, ratio):
         """
-        To save the correlated patterns mined form correlatedPatternTree
+        To save the frequent patterns mined form frequentPatternTree
 
-        :param prefix: the correlated pattern
+        :param prefix: the frequent pattern
         :type prefix: list
-        :param prefixLength: the length of a correlated pattern
+        :param prefixLength: the length of a frequent pattern
         :type prefixLength: int
         :param support: the support of a pattern
         :type support:  int
         """
 
         sample = []
         for i in range(prefixLength):
             sample.append(prefix[i])
         self._itemSetCount += 1
         self._finalPatterns[tuple(sample)] = [support, ratio]
 
     def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
         """
-        Generating all the combinations for items in single branch in correlatedPatternTree
+        Generating all the combinations for items in single branch in frequentPatternTree
 
-        :param tempBuffer: items in a single branch
+        :param tempBuffer: items in a list
         :type tempBuffer: list
         :param s: support at leaf node of a branch
         :param position: the length of a tempBuffer
         :type position: int
         :param prefix: it represents the list of leaf node
         :type prefix: list
         :param prefixLength: the length of prefix
@@ -461,73 +461,73 @@
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
             ratio = s/self._mapSupport[self._getMaxItem(prefix, newPrefixLength)]
             if ratio >= self._minAllConf:
                 self._saveItemSet(prefix, newPrefixLength, s, ratio)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport, minConf):
+    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport, minConf):
         """
         Mining the fp tree
 
-        :param correlatedPatternTree: it represents the correlatedPatternTree
-        :type correlatedPatternTree: class Tree
-        :param prefix: it represents an empty list and store the patterns that are mined
+        :param frequentPatternTree: it represents the frequentPatternTree
+        :type frequentPatternTree: class Tree
+        :param prefix: it represents a empty list and store the patterns that are mined
         :type prefix: list
         :param param prefixLength: the length of prefix
         :type prefixLength: int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
         """
         singlePath = True
         position = 0
         s = 0
-        if len(correlatedPatternTree.root.child) > 1:
+        if len(frequentPatternTree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = correlatedPatternTree.root.child[0]
+            currentNode = frequentPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
                 self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(correlatedPatternTree.headerList):
+            for i in reversed(frequentPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
                 low = max(int(_ab._math.floor(mapSupport[i]*self._minAllConf)), self._minSup)
                 high = max(int(_ab._math.floor(mapSupport[i]/minConf)), self._minSup)
-                betaSupport = support
+                betaSupport = support              
                 prefix.insert(prefixLength, item)
                 max1 = self._getMaxItem(prefix, prefixLength)
                 if self._mapSupport[max1] < self._mapSupport[item]:
                     max1 = item
                 ratio = support / self._mapSupport[max1]
                 if ratio >= self._minAllConf:
                     self._saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = correlatedPatternTree.mapItemNodes.get(item)
+                    path = frequentPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
                             prefixPath = [path]
                             pathCount = path.counter
                             parent1 = path.parent
                             if mapSupport.get(parent1.itemId) >= low and mapSupport.get(parent1.itemId) <= high:
                                 while parent1.itemId != -1:
-                                    all_conf = int(support/max(mapSupport.get(parent1.itemId), support))
-                                    if mapSupport.get(parent1.itemId) >= all_conf:
+                                    allconf = int(support/max(mapSupport.get(parent1.itemId), support))
+                                    if mapSupport.get(parent1.itemId) >= allconf:
                                         prefixPath.append(parent1)
                                         if mapSupportBeta.get(parent1.itemId) is None:
                                             mapSupportBeta[parent1.itemId] = pathCount
                                         else:
                                             mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
                                         parent1 = parent1.parent
                                     else:
@@ -535,15 +535,15 @@
                                 prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
+                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
 
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
@@ -569,28 +569,28 @@
             raise Exception("Please enter the file path or file name:")
         if self._minSup is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         self._finalPatterns = {}
         self._tree = _Tree()
         self._minSup = self._convert(self._minSup)
-        self._correlatedOneItem()
+        self._frequentOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
+            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
         print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
         self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
@@ -617,31 +617,31 @@
 
     def _getMaxItem(self, prefix, prefixLength):
         maxItem = prefix[0]
         for i in range(prefixLength):
             if self._mapSupport[maxItem] < self._mapSupport[prefix[i]]:
                 maxItem = prefix[i]
         return maxItem
-
+    
     def getRuntime(self):
         """
         Calculating the total amount of runtime taken by the mining process
 
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
-        Storing final correlated patterns in a dataframe
+        Storing final frequent patterns in a dataframe
 
-        :return: returning correlated patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             pat = " "
@@ -649,56 +649,53 @@
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
         """
-        Complete set of correlated patterns will be loaded in to an output file
+        Complete set of frequent patterns will be loaded in to a output file
 
-        :param outFile: name of the outputfile
+        :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             pattern = str()
             for i in x:
                 pattern = pattern + i + "\t"
             s1 = str(pattern.strip()) + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """
-        Function to send the set of correlated patterns after completion of the mining process
+        Function to send the set of frequent patterns after completion of the mining process
 
-        :return: returning correlated patterns
+        :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """
-        function to print the result after completing the process
-        """
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = CPGrowthPlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = CPGrowthPlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
         _correlatedPatterns = _ap.getPatterns()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,57 +8,70 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
+#
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
+import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-import sys as _sys
-import math as _math
+from collections import OrderedDict as _OrderedDict
 
 
-class _correlatedPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every correlated pattern mining algorithm must
+class _spatialFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
     Attributes :
     ----------
         iFile : str
             Input file name or path of the input file
+        nFile: str
+            Neighbourhoof file name
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        minAllConf: float
-            The user given minimum all confidence Ratio(should be in range of 0 to 1)
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of correlated patterns
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
     Methods :
     -------
@@ -75,66 +88,67 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
+    def __init__(self, iFile, nFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
+        :param nFile: Neighbourhood name of the input
+        :type nFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
-        :param minAllConf: The user given minimum all confidence Ratio(should be in range of 0 to 1)
-        :type minAllConf :float
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
+        self._nFile = nFile
+        self._oFile = str()
         self._sep = sep
         self._minSup = minSup
-        self._minAllConf = minAllConf
-        self._finalPatterns = {}
-        self._oFile = str()
-        self._memoryRSS = float()
-        self._memoryUSS = float()
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._finalPatterns = {}
+        self._oFile = str()
 
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of correlated patterns generated will be retrieved from this function"""
+        """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of correlated patterns will be saved in to an output file from this function
+        """Complete set of frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of correlated patterns will be loaded in to data frame from this function"""
+        """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
@@ -151,10 +165,11 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print the results of execution."""
+
+        """ To print the results of execution"""
 
         pass
```

### Comparing `pami-2023.7.27/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 #                 from PAMI.coveragePattern.basic import CMine as alg
 #
 #                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 #
 #                 obj.startMine()
 #
-#                 coveragePattern = obj.getPatterns()
+#                 coveragePatterns = obj.getPatterns()
 #
-#                 print("Total number of coverage Patterns:", len(coveragePattern))
+#                 print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -46,26 +46,26 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 
-from PAMI.coveragePattern.basic import abstract as _ab
+from PAMI.coveragePatterns.basic import abstract as _ab
 
 class CMine(_ab._coveragePatterns):
     """
 
     :Description:  CMine algorithms aims to discover the coverage patterns in transactional databases.
 
     :Reference:    Bhargav Sripada, Polepalli Krishna Reddy, Rage Uday Kiran:
                    Coverage patterns for efficient banner advertisement placement. WWW (Companion Volume) 2011: 131-132
                    https://dl.acm.org/doi/10.1145/1963192.1963259
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent pattern's
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minRF: float:
                    Controls the minimum number of transactions in which every item must appear in a database.
     :param  minCS: float:
                    Controls the minimum number of transactions in which at least one time within a pattern must appear in a database.
     :param  maxOR: float:
@@ -111,17 +111,17 @@
 
                 from PAMI.coveragePattern.basic import CMine as alg
 
                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 
                 obj.startMine()
 
-                coveragePattern = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePattern))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
@@ -222,23 +222,23 @@
                     tidData[item] = [self._lno]
                 else:
                     tidData[item].append(self._lno)
         coverageTidData = {k: v for k, v in tidData.items() if len(v) / len(self._Database) >= self._minRF}
         coverageTidData = dict(sorted(coverageTidData.items(), reverse=True, key=lambda x: len(x[1])))
         return coverageTidData
 
-    def tidToBitset(self,item_set):
+    def tidToBitset(self,itemset):
         """
         This function converts tid list to bitset.
-        :param item_set:
+        :param itemset:
         :return:
         """
         bitset = {}
 
-        for k,v in item_set.items():
+        for k,v in itemset.items():
             bitset[k] = 0b1
             bitset[k] = (bitset[k] << int(v[0])) | 0b1
             for i in range(1,len(v)):
                 diff = int(v[i]) - int(v[i-1])
                 bitset[k] = (bitset[k] << diff) | 0b1
             bitset[k] = (bitset[k] << (self._lno - int(v[i])))
         return bitset
@@ -247,28 +247,28 @@
         """
         This function generate coverage pattern about prefix.
         :param prefix: String
         :param tidData: list
         :return:
         """
         # variables to store coverage item set and
-        item_set = prefix[0]
+        itemset = prefix[0]
 
         # Get the length of tidData
         length = len(tidData)
         for i in range(length):
             tid = prefix[1] & tidData[i][1]
             tid1 = prefix[1] | tidData[i][1]
             andCount = bin(tid).count("1") - 1
             orCount = bin(tid1).count("1") - 1
             if orCount/len(self._Database) >= self._minCS and andCount / len(str(prefix[1])) <= self._maxOR:
-                coverageItem_set = item_set + '\t' + tidData[i][0]
+                coverageItemset = itemset + '\t' + tidData[i][0]
                 if orCount / len(self._Database) >= self._minRF:
-                    self._finalPatterns[coverageItem_set] = andCount
-                self.genPatterns((coverageItem_set,tid),tidData[i+1:length])
+                    self._finalPatterns[coverageItemset] = andCount
+                self.genPatterns((coverageItemset,tid),tidData[i+1:length])
 
     def generateAllPatterns(self,coverageItems):
         """
         This function generates all coverage patterns.
         :param coverageItems: coverage items
         :return:
         """
@@ -335,16 +335,16 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of coverage patterns will be loaded in to an output file
-        :param outFile: name of the outputfile
+        """Complete set of coverage patterns will be loaded in to a output file
+        :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
@@ -353,17 +353,14 @@
         """ Function to send the set of coverage patterns after completion of the mining process
         :return: returning coverage patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """
-         This function is used to print the result
-        """
         print("Total number of Coverage Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__=="__main__":
@@ -376,8 +373,13 @@
         _ap.startMine()
         print("Total number of coverage Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = CPPG('sample.txt', 0.4, 0.7, 0.5, ' ')
+        _ap.startMine()
+        print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
+        _ap.save('output.txt')
+        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# CPPG algorithm discovers coverage patterns in a transactional database.
+# CPPG  algorithm discovers coverage patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------
 #
 #             from PAMI.coveragePattern.basic import CPPG as alg
 #
 #             obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 #
 #             obj.startMine()
 #
-#             coveragePattern = obj.getPatterns()
+#             coveragePatterns = obj.getPatterns()
 #
-#             print("Total number of coverage Patterns:", len(coveragePattern))
+#             print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -45,15 +45,15 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.coveragePattern.basic import abstract as _ab
+from PAMI.coveragePatterns.basic import abstract as _ab
 
 
 _maxPer = float()
 _minSup = float()
 _lno = int()
 
 
@@ -63,15 +63,15 @@
     :Description:  CPPG  algorithm discovers coverage patterns in a transactional database.
 
     :Reference:     Gowtham Srinivas, P.; Krishna Reddy, P.; Trinath, A. V.; Bhargav, S.; Uday Kiran, R. (2015).
                     Mining coverage patterns from transactional databases. Journal of Intelligent Information Systems, 45(3), 423–439.
                     https://link.springer.com/article/10.1007/s10844-014-0318-3
 
     :param  iFile: str :
-           Name of the Input file to mine complete set of frequent pattern's
+           Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minRF: float:
                    Controls the minimum number of transactions in which every item must appear in a database.
     :param  minCS: float:
                    Controls the minimum number of transactions in which at least one time within a pattern must appear in a database.
     :param  maxOR: float:
@@ -120,17 +120,17 @@
 
                 from PAMI.coveragePattern.basic import CPPG as alg
 
                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 
                 obj.startMine()
 
-                coveragePattern = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePattern))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
@@ -294,15 +294,15 @@
 
         if len(new_freqList) > 0:
             self._generateFrequentPatterns(new_freqList)
 
     def _savePeriodic(self, itemSet):
         """ To convert the ranks of items in to their original item names
 
-            :param itemSet: frequent patterns
+            :param itemSet: frequent pattern
             :return: frequent pattern with original item names
         """
         t1 = str()
         for i in itemSet:
             t1 = t1 + self._rankedUp[i] + "\t"
         return t1
 
@@ -403,17 +403,17 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b[0], b[1]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of periodic-frequent patterns will be loaded in to an output file
+        """Complete set of periodic-frequent patterns will be loaded in to a output file
 
-        :param outFile: name of the outputfile
+        :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(len(y))
             writer.write("%s \n" % s1)
@@ -423,17 +423,14 @@
 
         :return: returning periodic-frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """
-           Function used to print the result
-        """
         print("Total number of Coverage Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
@@ -446,8 +443,13 @@
         _ap.startMine()
         print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = CPPG('sample.txt', 0.4, 0.7, 0.5, ' ')
+        _ap.startMine()
+        print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
+        _ap.save('output.txt')
+        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
 class _coveragePatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every coverage pattern mining algorithm must
+    """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
         employ in PAMI
 
        Attributes
         ----------
         iFile : str
             Input file name or path of the input file
         minCS: int or float or str
@@ -50,60 +50,59 @@
             The user can specify minRF either in count or proportion of database size.
             If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
             Otherwise, it will be treated as float.
             Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
-        startTime: float
+        startTime:float
             To record the start time of the algorithm
-        endTime: float
+        endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of coverage patterns
+            Name of the output file to store complete set of periodic-frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
         Methods
         -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of coverage patterns will be loaded in to a output file
+            Complete set of periodic-frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
-            Complete set of coverage patterns will be loaded in to data frame
+            Complete set of periodic-frequent patterns will be loaded in to data frame
         getMemoryUSS()
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minRF, minCS, maxOR, sep='\t'):
+    def __init__(self, iFile, minRF, minCS, maxOR, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minRF: The user can specify minimum relative frequency either in count or proportion of database size.
-            If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
+        :param minSup: The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
-        :type minRF: int or float or str
-        :param minCS: The user can specify minimum coverage support either in count or proportion of database size.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        :type minSup: int or float or str
+        :param maxPer: The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        :param maxOR: The user can specify maximum overlap ratio either in count or proportion of database size.
-        :type maxOR: int or float or str
+        :type maxPer: int or float or str
         :param sep: separator used in user specified input file
         :type sep: str
         """
 
         self._iFile = iFile
         self._minCS = minCS
         self._minRF = minRF
@@ -120,31 +119,31 @@
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of coverage patterns generated will be retrieved from this function"""
+        """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of coverage patterns will be saved in to an output file from this function
+        """Complete set of periodic-frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of coverage patterns will be loaded in to data frame from this function"""
+        """Complete set of periodic-frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
```

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
         """
 
         self.outputFile = outputFile
         with open(outputFile, 'w') as f:
              if self.condition not in condition_operator:
                 print('Condition error')
-             else:
+            else:
                 for tid in self.tids:
                     transaction = [item for item in self.items if condition_operator[self.condition](self.inputDF.at[tid, item], self.thresholdValue)]
                     if len(transaction) > 1:
                         f.write(f'{transaction[0]}')
                         for item in transaction[1:]:
                             f.write(f'\t{item}')
                     elif len(transaction) == 1:
-                        f.write(f'{transaction[0]}')
+                        f.write(f'{transaction}')
                     else:
                         continue
                     f.write('\n')
 
 
 
 
@@ -86,15 +86,15 @@
                     transaction = [item for item in self.items if condition_operator[self.condition](self.inputDF.at[tid, item], self.thresholdValue)]
                     if len(transaction) > 1:
                         f.write(f'{tid}')
                         for item in transaction:
                             f.write(f',{item}')
                     elif len(transaction) == 1:
                         f.write(f'{tid}')
-                        f.write(f',{transaction[0]}')
+                        f.write(f',{transaction}')
                     else:
                         continue
                     f.write('\n')
 
             
 
     def createUtility(self, outputFile):
```

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/plotPointOnMap.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,65 +4,65 @@
 
 class createSyntheticGeoreferentialTemporal:
     """
         This class create synthetic geo-referential temporal database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        noOfItems : int or float
+        items : int or float
             No of items
-        avgTransactionLength : str
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialTemporalDatabase(outputFile)
-            Create geo-referential temporal database and store into outputFile
+        getGeoreferentialTemporalDatabase(outputFile)
+            Create geo-referential temporal database store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
         count = 1
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str(count)
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             count += 1
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTemporal(100000, 870, 10)
     _ap.createGeoreferentialTemporalDatabase("T10_geo_temp.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 
 class createSyntheticGeoreferentialTransaction:
     """
         This class create synthetic geo-referential transaction database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        items : int 
+        items : int or float
             No of items
-        avgTransactionLength : str
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialTransactionDatabase(outputFile)
-            Create geo-referential transactional database and store into outputFile
+        getGeoreferentialTransactionDatabase(outputFile)
+            Create geo-referential transactional database store into outputFile
 
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTransaction(100000, 870, 10)
     _ap.createGeoreferentialTransactionalDatabase("T10_geo.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import random as _rd
 import sys as _sys
 
 
 class createSyntheticGeoreferentialUncertainTransaction:
     """
-        This class is to create synthetic geo-referential uncertain transaction database. 
+        This class create synthetic geo-referential uncertain transaction database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        noOfItems : int 
+        items : int or float
             No of items
-        avgTransactionLength : int
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialuncertainTransactionDatabase(outputFile)
+        getGeoreferentialuncertainTransactionDatabase(outputFile)
             Create geo-referential transactional database store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
 
 
 
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialUncertainTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str()
             st1 = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
@@ -68,8 +68,8 @@
             writer.write("%s \n" % st1)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialUncertainTransaction(100000, 870, 10)
     _ap.createGeoreferentialUncertainTransactionalDatabase("T10_geo_un.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic temporal database. 
 
         Attribute:
         ----------
         totalTransactions : int
             Total no of transactions
-        noOfItems : int 
+        items : int 
             No of items
         avgTransactionLength : int
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
@@ -29,15 +29,15 @@
 
 
     """
     
     def __init__(self, totalTransactions, items, avgTransaction):
         self._totalTransactions = totalTransactions
         self._items = items
-        self._avgTransactionLength = avgTransaction
+        self._avgTransactionLength = avgTransactionLength
     
     def createUncertainTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
@@ -45,15 +45,15 @@
         writer = open(outputFile, 'w+')
         count = 1
         for i in range(self._totalTransactions):
             length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str(count) + '\t'
             st1 = str()
             for i in range(length):
-                item = _rd.randint(1, self._noOfItems)
+                item = _rd.randint(1, self._items)
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
                 st1 = st1 + str(probability) + '\t'
             writer.write("%s:" % st)
             writer.write("%s \n" % st1)
             count += 1
```

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic transaction database. 
 
         Attribute:
         ----------
         totalTransactions : int
             No of transactions
-        noOfItems : int 
+        items : int 
             No of items
         avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
```

### Comparing `pami-2023.7.27/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         ----------
         totalTransactions : int
             No of transactions
         noOfItems : int 
             No of items
         maxUtilRange: int
             Maximum utility range
-        avgTransactionLength : int
+        avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
         --------
         createUtilitylDatabase(outputFile)
```

### Comparing `pami-2023.7.27/PAMI/extras/topKPatterns.py` & `pami-2023.7.7/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# FTApriori is one of the fundamental algorithm to discover fault-tolerant frequent patterns in a transactional database.
+# FT-Apriori is one of the fundamental algorithm to discover fault tolerant frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------------------
 #
-#     from PAMI.faultTolerantFrequentPattern.basic import FTApriori as alg
+#     from PAMI.uncertainCorrelatedPattern.basic import CFFI as alg
 #
-#     obj = alg.FTApriori(inputFile,minSup,itemSup,minLength,faultTolerance)
+#     obj = alg.CFFI("input.txt", 2, 0.4)
 #
 #     obj.startMine()
 #
-#     patterns = obj.getPatterns()
+#     Patterns = obj.getPatterns()
 #
-#     print("Total number of fault-tolerant frequent patterns:", len(patterns))
+#     print("Total number of Correlated Fuzzy Frequent Patterns:", len(Patterns))
 #
-#     obj.save("outputFile")
+#     obj.savePatterns("outputFile")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
@@ -44,41 +44,35 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from PAMI.faultTolerantFrequentPattern.basic import abstract as _ab
 
-
 class FTApriori(_ab._faultTolerantFrequentPatterns):
     """
     
-    :Description:   FT-Apriori is one of the fundamental algorithm to discover fault-tolerant frequent patterns in a transactional database.
+    :Description:   FT-Apriori is one of the fundamental algorithm to discover fault tolerant frequent patterns in a transactional database.
                     This program employs apriori property (or downward closure property) to  reduce the search space effectively.
 
     :Reference:       Pei, Jian & Tung, Anthony & Han, Jiawei. (2001). Fault-Tolerant Frequent Pattern Mining: Problems and Challenges.
 
     :param  iFile: str :
            Name of the Input file to mine complete set of frequent patterns
-
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-
     :param  minSup: float or int or str :
                     The user can specify minSup either in count or proportion of database size.
                     If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
                     Otherwise, it will be treated as float.
                     Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-
     :param  itemSup: int or float :
                     Frequency of an item
-
     :param minLength: int :
                     minimum length of a pattern
-
     :param faultTolerance: int
 
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
     :Attributes:
@@ -112,23 +106,23 @@
     
             .. note:: minSup will be considered in times of minSup and count of database transactions
     
     **Importing this algorithm into a python program**
     ----------------------------------------------------------------
     .. code-block:: python
     
-            from PAMI.faultTolerantFrequentPattern.basic import FTApriori as alg
+            from PAMI.uncertainCorrelatedPattern.basic import CFFI as alg
     
-            obj = alg.FTApriori(inputFile,minSup,itemSup,minLength,faultTolerance)
+            obj = alg.CFFI("input.txt", 2, 0.4)
     
             obj.startMine()
     
-            patterns = obj.getPatterns()
+            Patterns = obj.getPatterns()
     
-            print("Total number of fault-tolerant frequent patterns:",  len(patterns))
+            print("Total number of Correlated Fuzzy Frequent Patterns:",  len(Patterns))
     
             obj.savePatterns("outputFile")
     
             memUSS = obj.getMemoryUSS()
     
             print("Total Memory in USS:",  memUSS)
     
@@ -160,14 +154,16 @@
     _memoryRSS = float()
     _Database = []
     _mapSupport = {}
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
+
+
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
@@ -214,18 +210,14 @@
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
     def _Count(self, k):
-        """
-        param k: list of items
-        type k: list
-        """
         count = 0
         items = []
         k = list(k)
         n = len(k) - self._faultTolerance
         c = _ab._itertools.combinations(k, n)
         count = 0
         for j in c:
@@ -241,47 +233,81 @@
         self._mapSupport = {}
         for li in self._Database:
             for i in li:
                 if i not in self._mapSupport:
                     self._mapSupport[i] = 1
                 else:
                     self._mapSupport[i] += 1
-        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._itemSup}
+        self._mapSupport = {k:v for k, v in self._mapSupport.items() if v >= self._itemSup}
 
     def _countItemSupport(self, itemset):
         tids = {}
         res = True
+        # for i in itemset:
+        #     for k in transactions:
+        #         if i in k:
+        #             if i not in tids:
+        #                 tids[i] = 1
+        #             else:
+        #                 tids[i] += 1
         count = 0
         for x in self._Database:
+            print(x, itemset, set(x) & set(itemset), abs(len(itemset) - len(set(x) & set(itemset))))
             if abs(len(itemset) - len(set(x) & set(itemset))) <= self._faultTolerance:
                 count += 1
+        # for x, y in tids.items():
+        #     if y < self._itemSup:
+        #         res = False
         return count
 
     def _getFaultPatterns(self):
         l = [k for k, v in self._mapSupport.items()]
-        for i in range(0, len(l) + 1):
+        for i in range(0, len(l)+1):
             c = _ab._itertools.combinations(l, i)
             for j in c:
+                #support, items = self._Count(j)
+                #print(support, items)
                 res = self._countItemSupport(j)
+                print(j, res)
                 if len(j) >= self._minLength and res >= self._minSup:
                     self._finalPatterns[tuple(j)] = res
 
     def startMine(self):
         """
-            Fault-tolerant frequent pattern mining process will start from here
+            Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         self._itemSup = self._convert(self._itemSup)
         self._minLength = int(self._minLength)
         self._faultTolerance = int(self._faultTolerance)
         self._oneLengthFrequentItems()
-
+        #l = [k for k, v in self._mapSupport.items()]
+        # for i in range(len(l)):
+        #     for j in range(i + 1, len(l)):
+        #         x, y = l[i], l[j]
+        #         li = [x, y]
+        #         count = 0
+        #         tids = {x: 0, y: 0}
+        #         for k in self._Database:
+        #             if x in k and y in k:
+        #                 count += 1
+        #             if x in k and y not in k:
+        #                 count += 1
+        #             if x not in k and y in k:
+        #                 count += 1
+        #         # re = True
+        #         # for x, y in tids.items():
+        #         #     if y < self._itemSup:
+        #         #         re = False
+        #         print(li, count)
+        #     if len(li) > self._faultTolerance:
+        #         self._finalPatterns[tuple(li)] = count
         self._getFaultPatterns()
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
@@ -332,15 +358,15 @@
             for i in a:
                 s = s + i + ' '
             data.append([s, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -357,31 +383,33 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """ this is function is used to print the result
-        """
         print("Total number of Fault-Tolerant Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 7 or len(_ab._sys.argv) == 8:
         if len(_ab._sys.argv) == 8:
-            _ap = FTApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4],
-                            _ab._sys.argv[5], _ab._sys.argv[6], _ab._sys.argv[7], )
+            _ap = FTApriori(_ab._sys.argv[1], _ab._sys.argv[3],  _ab._sys.argv[4],
+                            _ab._sys.argv[5], _ab._sys.argv[6], _ab._sys.argv[7],)
         if len(_ab._sys.argv) == 7:
             _ap = FTApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = FTApriori('/Users/Likhitha/Downloads/fault/sample4.txt', 5, 3, 2, 1, ' ')
+        _ap.startMine()
+        _ap.printResults()
+        print(_ap.getPatternsAsDataFrame())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# FTFPGrowth algorithm aims to discover all fault-tolerant frequent patterns that may exist in a transactional database.
-#
 # **Importing this algorithm into a python program**
 # --------------------------------------------------
 #
-#     from PAMI.faultTolerantFrequentPattern.basic import FTFPGrowth as alg
+#     from PAMI.frequentPattern.basic import FPGrowth as alg
 #
-#     obj = alg.FTFPGrowth(inputFile,minSup,itemSup,minLength,faultTolerance)
+#     obj = alg.FPGrowth(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     faultTolerantFrequentPatterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of fault-tolerant frequent patterns:", len(faultTolerantFrequentPatterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
 #     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
@@ -87,15 +85,15 @@
         self.parent = None
         self.children = children
 
     def addChild(self, node):
         """
             Retrieving the child from the tree
 
-            :param node: Child Node
+            :param node: Children node
             :type node: Node
             :return: Updates the children nodes and parent nodes
 
         """
         self.children[node.itemId] = node
         node.parent = self
 
@@ -130,15 +128,15 @@
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
     def addTransaction(self, transaction, count):
         """adding transaction into tree
 
-        :param transaction: it represents the one transaction in database
+        :param transaction: it represents the one transactions in database
 
         :type transaction: list
 
         :param count: frequency of item
 
         :type count: int
         """
@@ -249,15 +247,15 @@
 
 class FTFPGrowth(_fp._faultTolerantFrequentPatterns):
     """
     Description:
     ------------
        FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database.
        It stores the database in compressed fp-tree decreasing the memory usage and extracts the
-       patterns from tree.It employs downward closure property to  reduce the search space effectively.
+       patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
 
     Reference :
     ---------
        Han, J., Pei, J., Yin, Y. et al. Mining Frequent Patterns without Candidate Generation: A Frequent-Pattern
        Tree Approach. Data  Mining and Knowledge Discovery 8, 53–87 (2004). https://doi.org/10.1023
 
     Attributes :
@@ -296,15 +294,15 @@
     Methods :
     -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to an output file
+            Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
@@ -326,23 +324,23 @@
 
 
 
     Sample run of the importing code:
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.faultTolerantFrequentPattern.basic import FTFPGrowth as alg
+        from PAMI.frequentPattern.basic import FPGrowth as alg
 
-        obj = alg.FTFPGrowth(inputFile,minSup,itemSup,minLength,faultTolerance)
+        obj = alg.FPGrowth(iFile, minSup)
 
         obj.startMine()
 
-        patterns = obj.getPatterns()
+        frequentPatterns = obj.getPatterns()
 
-        print("Total number of Frequent Patterns:", len(patterns))
+        print("Total number of Frequent Patterns:", len(frequentPatterns))
 
         obj.save(oFile)
 
         Df = obj.getPatternInDataFrame()
 
         memUSS = obj.getMemoryUSS()
 
@@ -592,15 +590,15 @@
         data = []
         for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.27/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 import itertools as _itertools
 
 
 class _faultTolerantFrequentPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every fault-tolerant frequent pattern mining algorithm must
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
@@ -63,15 +63,15 @@
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of fault-tolerant frequent patterns
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
        Methods:
        -------
@@ -126,31 +126,31 @@
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of fault-tolerant frequent patterns generated will be retrieved from this function"""
+        """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of fault-tolerant frequent patterns will be saved in to an output file from this function
+        """Complete set of frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of fault-tolerant frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -149,15 +149,15 @@
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
 
-    def _creatingItemSets(self) -> List[set]:
+    def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
@@ -187,15 +187,15 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _convert(self, value) -> Union[int, float]:
+    def _convert(self, value):
         """
         To convert the user specified minSup value
 
         :param value: user specified minSup value
 
         :return: converted type
         """
@@ -207,15 +207,15 @@
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _candidateToFrequent(self, candidateList) -> Dict[frozenset, int]:
+    def _candidateToFrequent(self, candidateList):
         """Generates frequent patterns from the candidate patterns
 
         :param candidateList: Candidate patterns will be given as input
 
         :type candidateList: list
 
         :return: returning set of all frequent patterns
@@ -230,15 +230,15 @@
             candidateToFrequentList.update(dictionary)
         candidateToFrequentList = {key: value for key, value in candidateToFrequentList.items() if
                                    value >= self._minSup}
 
         return candidateToFrequentList
 
     @staticmethod
-    def _frequentToCandidate(frequentList, length) -> List[set]:
+    def _frequentToCandidate(frequentList, length):
         """Generates candidate patterns from the frequent patterns
 
         :param frequentList: set of all frequent patterns to generate candidate patterns of each of size is length
 
         :type frequentList: dict
 
         :param length: size of each candidate patterns to be generated
@@ -282,45 +282,45 @@
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using Apriori algorithm ")
 
-    def getMemoryUSS(self) -> float:
+    def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self) -> float:
+    def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self) -> float:
+    def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> DataFrame:
+    def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
 
         :rtype: pd.DataFrame
         """
 
@@ -329,40 +329,36 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, int]:
+    def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """
-        this function is used to print the result
-
-        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-#
+# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
+
 # **Importing this algorithm into a python program**
-# ------------------------------------------------------------------
+# ---------------------------------------------------------
 #
-#     import PAMI.frequentPattern.basic.ECLAT as alg
+#                 import PAMI.frequentPattern.basic.ECLATDiffset as alg
 #
-#     obj = alg.ECLAT(iFile, minSup)
+#                 obj = alg.ECLATDiffset(iFile, minSup)
 #
-#     obj.startMine()
+#                 obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#                 frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#                 print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#                 obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternInDataFrame()
+#                 Df = obj.getPatternInDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#                 memUSS = obj.getMemoryUSS()
 #
-#     print("Total Memory in USS:", memUSS)
+#                 print("Total Memory in USS:", memUSS)
 #
-#     memRSS = obj.getMemoryRSS()
+#                 memRSS = obj.getMemoryRSS()
 #
-#     print("Total Memory in RSS", memRSS)
+#                 print("Total Memory in RSS", memRSS)
 #
-#     run = obj.getRuntime()
+#                 run = obj.getRuntime()
 #
-#     print("Total ExecutionTime in seconds:", run)
+#                 print("Total ExecutionTime in seconds:", run)
+
+
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
@@ -42,117 +44,121 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.frequentPattern.basic import abstract as _ab
 
+# from abstract import *
 
-class ECLAT(_ab._frequentPatterns):
-    """
+from PAMI.frequentPattern.basic import abstract as _ab
 
-    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
-    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+class ECLATDiffset(_ab._frequentPatterns):
+    """
+    :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
 
+    :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
+            August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
+            
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent pattern's
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-
+     
+ 
+    
     :Attributes:
-
+    
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
 
         finalPatterns : dict
           Storing the complete set of patterns in a dictionary variable
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
-
+        
         Database : list
           To store the transactions of a database in list
-
-
+          
+        
     **Methods to execute code on terminal**
-    ------------------------------------------
-
+    ----------------------------------------
+    
             Format:
-                      >>> python3 ECLAT.py <inputFile> <outputFile> <minSup>
-
+                      >>> python3 ECLATbitset.py <inputFile> <outputFile> <minSup>
+    
             Example:
-                      >>>  python3 ECLAT.py sampleDB.txt patterns.txt 10.0
-
+                      >>> python3 ECLATbitset.py sampleDB.txt patterns.txt 10.0
+    
             .. note:: minSup will be considered in percentage of database transactions
-
-
+    
+    
     **Importing this algorithm into a python program**
-    ------------------------------------------------------------------
+    ---------------------------------------------------------
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.ECLAT as alg
+                import PAMI.frequentPattern.basic.ECLATDiffset as alg
 
-            obj = alg.ECLAT(iFile, minSup)
+                obj = alg.ECLATDiffset(iFile, minSup)
 
-            obj.startMine()
+                obj.startMine()
 
-            frequentPatterns = obj.getPatterns()
+                frequentPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+                print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.savePatterns(oFile)
+                obj.savePatterns(oFile)
 
-            Df = obj.getPatternInDataFrame()
+                Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+                memUSS = obj.getMemoryUSS()
 
-            print("Total Memory in USS:", memUSS)
+                print("Total Memory in USS:", memUSS)
 
-            memRSS = obj.getMemoryRSS()
+                memRSS = obj.getMemoryRSS()
 
-            print("Total Memory in RSS", memRSS)
+                print("Total Memory in RSS", memRSS)
 
-            run = obj.getRuntime()
+                run = obj.getRuntime()
 
-            print("Total ExecutionTime in seconds:", run)
+                print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
-    ----------------------
+    -------------------
 
-             The complete program was written by Kundai  under the supervision of Professor Rage Uday Kiran.
+               The complete program was written by Kundai under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
+    _diffSets = {}
+    _trans_set = set()
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
         """
         self._Database = []
@@ -179,64 +185,14 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _getUniqueItemList(self):
-        """
-        Generating one frequent patterns
-        """
-        self._finalPatterns = {}
-        candidate = {}
-        uniqueItem = []
-        for i in range(len(self._Database)):
-            for j in range(len(self._Database[i])):
-                if self._Database[i][j] not in candidate:
-                    candidate[self._Database[i][j]] = {i}
-                else:
-                    candidate[self._Database[i][j]].add(i)
-        for key, value in candidate.items():
-            supp = len(value)
-            if supp >= self._minSup:
-                self._finalPatterns[key] = [value]
-                uniqueItem.append(key)
-        uniqueItem.sort()
-        return uniqueItem
-
-    def _generateFrequentPatterns(self, candidateFrequent):
-        """It will generate the combinations of frequent items
-
-        :param candidateFrequent :it represents the items with their respective transaction identifiers
-
-        :type candidateFrequent: list
-
-        :return: returning transaction dictionary
-
-        :rtype: dict
-        """
-        new_freqList = []
-        for i in range(0, len(candidateFrequent)):
-            item1 = candidateFrequent[i]
-            i1_list = item1.split()
-            for j in range(i + 1, len(candidateFrequent)):
-                item2 = candidateFrequent[j]
-                i2_list = item2.split()
-                if i1_list[:-1] == i2_list[:-1]:
-                    interSet = self._finalPatterns[item1][0].intersection(self._finalPatterns[item2][0])
-                    if len(interSet) >= self._minSup:
-                        newKey = item1 + "\t" + i2_list[-1]
-                        self._finalPatterns[newKey] = [interSet]
-                        new_freqList.append(newKey)
-                else: break
-
-        if len(new_freqList) > 0:
-                self._generateFrequentPatterns(new_freqList)
-
     def _convert(self, value):
         """
         To convert the user specified minSup value
 
         :param value: user specified minSup value
 
         :return: converted type
@@ -249,35 +205,91 @@
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
+    def _getUniqueItemList(self):
+
+        # tidSets will store all the initial tids
+        tidSets = {}
+        # uniqueItem will store all frequent 1 items
+        uniqueItem = []
+        for line in self._Database:
+                transNum = 0
+                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
+                for transaction in self._Database:
+                    transNum += 1
+                    self._trans_set.add(transNum)
+                    for item in transaction:
+                        if item in tidSets:
+                            tidSets[item].add(transNum)
+                        else:
+                            tidSets[item] = {transNum}
+        for key, value in tidSets.items():
+            supp = len(value)
+            if supp >= self._minSup:
+                self._diffSets[key] = [supp, self._trans_set.difference(value)]
+                uniqueItem.append(key)
+        # for x, y in self._diffSets.items():
+        #     print(x, y)
+        uniqueItem.sort()
+        # print()
+        return uniqueItem
+
+    def _runDeclat(self, candidateList):
+
+        newList = []
+        for i in range(0, len(candidateList)):
+            item1 = candidateList[i]
+            iList = item1.split()
+            for j in range(i + 1, len(candidateList)):
+                item2 = candidateList[j]
+                jList = item2.split()
+                if iList[:-1] == jList[:-1]:
+                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
+                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
+                    if unionSup >= self._minSup:
+                        newKey = item1 + "\t" + jList[-1]
+                        self._diffSets[newKey] = [unionSup, unionDiffSet]
+                        newList.append(newKey)
+                    else: 
+                        break
+
+        if len(newList) > 0:
+            self._runDeclat(newList)
+
     def startMine(self):
         """Frequent pattern mining process will start from here"""
 
         self._startTime = _ab._time.time()
+        self._Database = []
+        self._finalPatterns = {}
+        self._diffSets = {}
+        self._trans_set = set()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         if self._minSup is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
+        #print(len(self._Database))
         self._minSup = self._convert(self._minSup)
+        uniqueItemList = []
         uniqueItemList = self._getUniqueItemList()
-        self._generateFrequentPatterns(uniqueItemList)
-        for x, y in self._finalPatterns.items():
-            self._finalPatterns[x] = len(y[0])
+        self._runDeclat(uniqueItemList)
+        self._finalPatterns = self._diffSets
+        #print(len(self._finalPatterns), len(uniqueItemList))
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT algorithm")
+        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -312,59 +324,57 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
+            data.append([a.replace('\t', ' '), b[0]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
+            patternsAndSupport = x.strip() + ":" + str(y[0])
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """Function used to print the results
-
-        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print(_ap.getPatternsAsDataFrame())
-        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
-
+# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+#
+#
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# ----------------------------------------------------
 #
-#                 import PAMI.frequentPattern.basic.ECLATDiffset as alg
+#     import PAMI.frequentPattern.cuda.cuEclatBit as alg
 #
-#                 obj = alg.ECLATDiffset(iFile, minSup)
+#     obj = alg.cuEclatBit(iFile, minSup)
 #
-#                 obj.startMine()
+#     obj.startMine()
 #
-#                 frequentPatterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#                 print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#                 obj.savePatterns(oFile)
+#     obj.savePatterns(oFile)
 #
-#                 Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternInDataFrame()
 #
-#                 memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#                 print("Total Memory in USS:", memUSS)
+#     print("Total Memory in USS:", memUSS)
 #
-#                 memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#                 print("Total Memory in RSS", memRSS)
+#     print("Total Memory in RSS", memRSS)
 #
-#                 run = obj.getRuntime()
+#     run = obj.getRuntime()
 #
-#                 print("Total ExecutionTime in seconds:", run)
-
+#     print("Total ExecutionTime in seconds:", run)
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -45,150 +45,176 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-# from abstract import *
+# from PAMI.frequentPattern.cuda import abstract as _ab
+import abstract as _ab
 
-from PAMI.frequentPattern.basic import abstract as _ab
-
-
-class ECLATDiffset(_ab._frequentPatterns):
+class cuEclatBit(_ab._frequentPatterns):
     """
-    :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
+    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+
+    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+            372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
-    :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
-            August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
-            
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent pattern's
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  minSup: int :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-     
- 
-    
+
+
+
     :Attributes:
-    
+
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
 
         finalPatterns : dict
           Storing the complete set of patterns in a dictionary variable
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
-        
+
         Database : list
           To store the transactions of a database in list
-          
-        
+
+
+
     **Methods to execute code on terminal**
-    ----------------------------------------
-    
+    ----------------------------------------------------
+
             Format:
-                      >>> python3 ECLATbitset.py <inputFile> <outputFile> <minSup>
-    
+                      >>> python3 cuEclatBit.py <inputFile> <outputFile> <minSup>
+
             Example:
-                      >>> python3 ECLATbitset.py sampleDB.txt patterns.txt 10.0
-    
+                      >>>  python3 cuEclatBit.py sampleDB.txt patterns.txt 10.0
+
             .. note:: minSup will be considered in percentage of database transactions
-    
-    
+
+
     **Importing this algorithm into a python program**
-    ---------------------------------------------------------
+    ----------------------------------------------------
+
     .. code-block:: python
 
-                import PAMI.frequentPattern.basic.ECLATDiffset as alg
+             import PAMI.frequentPattern.cuda.cuEclatBit as alg
 
-                obj = alg.ECLATDiffset(iFile, minSup)
+             obj = alg.cuEclatBit(iFile, minSup)
 
-                obj.startMine()
+             obj.startMine()
 
-                frequentPatterns = obj.getPatterns()
+             frequentPatterns = obj.getPatterns()
 
-                print("Total number of Frequent Patterns:", len(frequentPatterns))
+             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                obj.savePatterns(oFile)
+             obj.savePatterns(oFile)
 
-                Df = obj.getPatternInDataFrame()
+             Df = obj.getPatternInDataFrame()
 
-                memUSS = obj.getMemoryUSS()
+             memUSS = obj.getMemoryUSS()
 
-                print("Total Memory in USS:", memUSS)
+             print("Total Memory in USS:", memUSS)
 
-                memRSS = obj.getMemoryRSS()
+             memRSS = obj.getMemoryRSS()
 
-                print("Total Memory in RSS", memRSS)
+             print("Total Memory in RSS", memRSS)
 
-                run = obj.getRuntime()
+             run = obj.getRuntime()
 
-                print("Total ExecutionTime in seconds:", run)
+             print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
-    -------------------
+    -------------
 
-               The complete program was written by Kundai under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
+
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _diffSets = {}
-    _trans_set = set()
+
+    _sumKernel = _ab._cp.RawKernel(r'''
+
+    #define uint32_t unsigned int
+
+    extern "C" __global__
+
+    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
+    {
+        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
+        if (i < numElements)
+        {  
+            atomicAdd(&sum[0], __popc(d_a[i]));
+        }
+        return;    
+    }
+
+    ''', 'sumKernel')
+
+
+
+
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
+
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
+                temp = self._iFile['Transactions'].tolist()
+
+            for k in temp:
+                self._Database.append(set(k))
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    self._Database.append(set(temp))
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _convert(self, value):
         """
         To convert the user specified minSup value
@@ -204,92 +230,98 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
+    
+    def arraysAndItems(self):
+        ArraysAndItems = {}
+
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                j = tuple([j])
+                if j not in ArraysAndItems:
+                    ArraysAndItems[j] = [i]
+                else:
+                    ArraysAndItems[j].append(i)
+
+        newArraysAndItems = {}
+
+        for k,v in ArraysAndItems.items():
+            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
+            if len(v) >= self._minSup:
+                self._finalPatterns[k] = len(v)
+                newArraysAndItems[k] = ArraysAndItems[k]
 
-    def _getUniqueItemList(self):
+        return newArraysAndItems
+    
+    def createBitRepresentation(self, ArraysAndItems):
+        bitRep = {}
+        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
 
-        # tidSets will store all the initial tids
-        tidSets = {}
-        # uniqueItem will store all frequent 1 items
-        uniqueItem = []
-        for line in self._Database:
-                transNum = 0
-                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
-                for transaction in self._Database:
-                    transNum += 1
-                    self._trans_set.add(transNum)
-                    for item in transaction:
-                        if item in tidSets:
-                            tidSets[item].add(transNum)
-                        else:
-                            tidSets[item] = {transNum}
-        for key, value in tidSets.items():
-            supp = len(value)
-            if supp >= self._minSup:
-                self._diffSets[key] = [supp, self._trans_set.difference(value)]
-                uniqueItem.append(key)
-        # for x, y in self._diffSets.items():
-        #     print(x, y)
-        uniqueItem.sort()
-        # print()
-        return uniqueItem
-
-    def _runDeclat(self, candidateList):
-
-        newList = []
-        for i in range(0, len(candidateList)):
-            item1 = candidateList[i]
-            iList = item1.split()
-            for j in range(i + 1, len(candidateList)):
-                item2 = candidateList[j]
-                jList = item2.split()
-                if iList[:-1] == jList[:-1]:
-                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
-                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
-                    if unionSup >= self._minSup:
-                        newKey = item1 + "\t" + jList[-1]
-                        self._diffSets[newKey] = [unionSup, unionDiffSet]
-                        newList.append(newKey)
-                    else: 
-                        break
 
-        if len(newList) > 0:
-            self._runDeclat(newList)
+        for k, v in ArraysAndItems.items():
+            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
+            for i in v:
+                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
 
-    def startMine(self):
-        """Frequent pattern mining process will start from here"""
+        for k, v in bitRep.items():
+            bitRep[k] = _ab._cp.array(v)
 
-        self._startTime = _ab._time.time()
+        return bitRep
+
+    
+    def startMine(self):
+        """
+            Frequent pattern mining process will start from here
+        """
         self._Database = []
-        self._finalPatterns = {}
-        self._diffSets = {}
-        self._trans_set = set()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
+        self._startTime = _ab._time.time()
         self._creatingItemSets()
-        #print(len(self._Database))
+        itemsList = sorted(list(set.union(*self._Database)))  # because Database is list
         self._minSup = self._convert(self._minSup)
-        uniqueItemList = []
-        uniqueItemList = self._getUniqueItemList()
-        self._runDeclat(uniqueItemList)
-        self._finalPatterns = self._diffSets
-        #print(len(self._finalPatterns), len(uniqueItemList))
+
+        ArraysAndItems = self.arraysAndItems()
+
+        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
+
+        while len(ArraysAndItems) > 0:
+            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
+            newArraysAndItems = {}
+            keys = list(ArraysAndItems.keys())
+            for i in range(len(ArraysAndItems)):
+                iList = list(keys[i])
+                # print(i, "/", len(ArraysAndItems), end="\r")
+                for j in range(i+1, len(ArraysAndItems)):  
+                    jList = list(keys[j])
+                    union = []
+                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
+                        union = iList + [jList[-1]]
+                        union = tuple(union)
+                        unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
+                        sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
+                        self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
+                        sum = sum[0]
+                        if sum >= self._minSup and union not in self._finalPatterns:
+                            newArraysAndItems[union] = unionData
+                            string = "\t".join(union)
+                            self._finalPatterns[string] = sum
+            ArraysAndItems = newArraysAndItems
+            # print()
+
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
+        print("Frequent patterns were generated successfully using cuEclatBit algorithm ")
+            
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -324,57 +356,64 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b[0]])
+            data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y[0])
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
+    _ap = cuEclatBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+    _ap.startMine()
+    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+    _ap.save(_ab._sys.argv[2])
+    print("Total Memory in USS:", _ap.getMemoryUSS())
+    print("Total Memory in RSS", _ap.getMemoryRSS())
+    print("Total ExecutionTime in s:", _ap.getRuntime())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-#  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
-#  **Importing this algorithm into a python program**
-#  ---------------------------------------------------------
 #
-#     import PAMI.frequentPattern.basic.ECLATbitset as alg
+# **Importing this algorithm into a python program**
+# ----------------------------------------------------
 #
-#     obj = alg.ECLATbitset(iFile, minSup)
+#     import PAMI.frequentPattern.cuda.cuApriori as alg
+#
+#     obj = alg.cuApriori(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
-#
-#
-#
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -47,29 +45,30 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-from PAMI.frequentPattern.basic import abstract as _ab
+# from PAMI.frequentPattern.cuda import abstract as _ab
+import abstract as _ab
 
-class ECLATbitset(_ab._frequentPatterns):
+class cuApriori(_ab._frequentPatterns):
     """
-    :Description:  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+    :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
-    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+    :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
+            In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  minSup: int :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
 
     :Attributes:
 
@@ -88,295 +87,310 @@
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
         Database : list
           To store the transactions of a database in list
 
 
+
     **Methods to execute code on terminal**
-    ----------------------------------------
+    ----------------------------------------------------
 
             Format:
-                      >>> python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
+                      >>> python3 cuApriori.py <inputFile> <outputFile> <minSup>
 
             Example:
-                      >>> python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
+                      >>>  python3 cuApriori.py sampleDB.txt patterns.txt 10.0
 
             .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
-    ---------------------------------------------------------
+    ----------------------------------------------------
+
     .. code-block:: python
 
-                import PAMI.frequentPattern.basic.ECLATbitset as alg
+             import PAMI.frequentPattern.cuda.cuApriori as alg
+
+             obj = alg.cuApriori(iFile, minSup)
 
-                obj = alg.ECLATbitset(iFile, minSup)
+             obj.startMine()
 
-                obj.startMine()
+             frequentPatterns = obj.getPatterns()
 
-                frequentPatterns = obj.getPatterns()
+             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                print("Total number of Frequent Patterns:", len(frequentPatterns))
+             obj.savePatterns(oFile)
 
-                obj.savePatterns(oFile)
+             Df = obj.getPatternInDataFrame()
 
-                Df = obj.getPatternInDataFrame()
+             memUSS = obj.getMemoryUSS()
 
-                memUSS = obj.getMemoryUSS()
+             print("Total Memory in USS:", memUSS)
 
-                print("Total Memory in USS:", memUSS)
+             memRSS = obj.getMemoryRSS()
 
-                memRSS = obj.getMemoryRSS()
+             print("Total Memory in RSS", memRSS)
 
-                print("Total Memory in RSS", memRSS)
+             run = obj.getRuntime()
 
-                run = obj.getRuntime()
+             print("Total ExecutionTime in seconds:", run)
 
-                print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    -------------------
+    -------------
 
-               The complete program was written by Yudai Masu under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
+    _ab._cp.cuda.Device(0).use()
+
+
+
+    _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _minSup = str()
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
-    _lno = 0
 
+    _sumKernel = _ab._cp.RawKernel(r'''
+
+    #define uint32_t unsigned int
+
+    extern "C" __global__
+
+    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
+    {
+        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
+        if (i < numElements)
+        {  
+            atomicAdd(&sum[0], __popc(d_a[i]));
+        }
+        return;    
+    }
+
+    ''', 'sumKernel')
 
-    def _convert(self, value):
-        """
-        To convert the user specified minSup value
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
+
+
         """
         self._Database = []
-        self._mapSupport = {}
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
+                temp = self._iFile['Transactions'].tolist()
 
+            for k in temp:
+                self._Database.append(set(k))
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    self._Database.append(set(temp))
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            self._lno += 1
-                            splitter = [i.rstrip() for i in line.split(self._sep)]
-                            splitter = [x for x in splitter if x]
-                            self._Database.append(splitter)
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
-        self._minSup = self._convert(self._minSup)
+                    quit()
 
-    def creatingFrequentItems(self):
+    def _convert(self, value):
         """
-        This function creates frequent items from _database.
-        :return: frequentTidData that stores frequent items and their tid list.
+        To convert the user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
         """
-        tidData = {}
-        self._lno = 0
-        for transaction in self._Database:
-            self._lno = self._lno + 1
-            for item in transaction:
-                if item not in tidData:
-                    tidData[item] = [self._lno]
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+    
+    def arraysAndItems(self):
+        ArraysAndItems = {}
+
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                j = tuple([j])
+                if j not in ArraysAndItems:
+                    ArraysAndItems[j] = [i]
                 else:
-                    tidData[item].append(self._lno)
-        frequentTidData = {k: v for k, v in tidData.items() if len(v) >= self._minSup}
-        frequentTidData = dict(sorted(frequentTidData.items(), reverse=True, key=lambda x: len(x[1])))
-        return frequentTidData
-
-    def tidToBitset(self,itemset):
-        """
-        This function converts tid list to bitset.
-        :param itemset:
-        :return:
-        """
-        bitset = {}
-
-        for k,v in itemset.items():
-            bitset[k] = 0b1
-            bitset[k] = (bitset[k] << int(v[0])) | 0b1
-            for i in range(1,len(v)):
-                diff = int(v[i]) - int(v[i-1])
-                bitset[k] = (bitset[k] << diff) | 0b1
-            bitset[k] = (bitset[k] << (self._lno - int(v[i])))
-        return bitset
-
-    def genPatterns(self,prefix,tidData):
-        """
-        This function generate frequent pattern about prefix.
-        :param prefix: String
-        :param tidData: list
-        :return:
-        """
-        # variables to store frequent item set and
-        itemset = prefix[0]
-
-        # Get the length of tidData
-        length = len(tidData)
-
-        for i in range(length):
-            #tid = prefix[1].intersection(tidData[i][1])
-            tid = prefix[1] & tidData[i][1]
-            count = bin(tid).count("1") - 1
-            #tidLength = len(tid)
-            if count >= self._minSup:
-                frequentItemset = itemset + '\t' + tidData[i][0]
-                self._finalPatterns[frequentItemset] = count
-                self.genPatterns((frequentItemset,tid),tidData[i+1:length])
-
-    def genAllFrequentPatterns(self,frequentItems):
-        """
-        This function generates all frequent patterns.
-        :param frequentItems: frequent items
-        :return:
-        """
-        tidData = list(frequentItems.items())
-        length = len(tidData)
-        for i in range(length):
-            #print(i,tidData[i][0])
-            self.genPatterns(tidData[i],tidData[i+1:length])
+                    ArraysAndItems[j].append(i)
 
-    def startMine(self):
-        """Frequent pattern mining process will start from here
-                We start with the scanning the itemSets and store the bitsets respectively.
-                We form the combinations of single items and  check with minSup condition to check the frequency of patterns
-                """
+        newArraysAndItems = {}
 
-        self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
+        for k,v in ArraysAndItems.items():
+            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
+            if len(v) >= self._minSup:
+                self._finalPatterns[k] = len(v)
+                newArraysAndItems[k] = ArraysAndItems[k]
 
+        return newArraysAndItems
+
+    
+    def startMine(self):
+        """
+            Frequent pattern mining process will start from here
+        """
+        self._Database = []
+        self._startTime = _ab._time.time()
         self._creatingItemSets()
-        frequentItems = self.creatingFrequentItems()
-        self._finalPatterns = {k: len(v) for k, v in frequentItems.items()}
-        frequentItemsBitset = self.tidToBitset(frequentItems)
-        self.genAllFrequentPatterns(frequentItemsBitset)
+        self._minSup = self._convert(self._minSup)
+
+        ArraysAndItems = self.arraysAndItems()
+
+        while len(ArraysAndItems) > 0:
+            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
+            newArraysAndItems = {}
+            keys = list(ArraysAndItems.keys())
+            for i in range(len(ArraysAndItems)):
+                # print(i, "/", len(ArraysAndItems), end="\r")
+                iList = list(keys[i])
+                for j in range(i+1, len(ArraysAndItems)):
+                    jList = list(keys[j])
+                    union = tuple(sorted(set(iList + jList)))
+                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]], assume_unique=True)
+                    if len(intersect) >= self._minSup and union not in self._finalPatterns:
+                        newArraysAndItems[union] = intersect
+                        self._finalPatterns[union] = len(intersect)
+            ArraysAndItems = newArraysAndItems
+            # print()
+
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using Eclat_bitset algorithm")
+        print("Frequent patterns were generated successfully using cuApriori algorithm ")
+            
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
-        :param outFile: name of the outputfile
+        """Complete set of frequent patterns will be loaded in to a output file
+
+        :param outFile: name of the output file
+
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        """ this function is used to print the result
-        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in s:", self.getRuntime())
+
 
-if __name__=="__main__":
+if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        print("Total ExecutionTime in s:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
+
+    _ap = cuApriori("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
+    _ap = cuApriori("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+    _ap.startMine()
+    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+    print("Total Memory in USS:", _ap.getMemoryUSS())
+    print("Total Memory in RSS", _ap.getMemoryRSS())
+    print("Total ExecutionTime in s:", _ap.getRuntime())
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It  employs downward closure property to  reduce the search space effectively.
+# FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #     from PAMI.frequentPattern.basic import FPGrowth as alg
 #
 #     obj = alg.FPGrowth(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -131,15 +131,15 @@
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
     def addTransaction(self, transaction, count):
         """adding transaction into tree
 
-        :param transaction: it represents the one transaction in database
+        :param transaction: it represents the one transactions in database
 
         :type transaction: list
 
         :param count: frequency of item
 
         :type count: int
         """
@@ -247,15 +247,15 @@
                 for q in conditionalTree.generatePatterns(pattern):
                     yield q
 
 
 class FPGrowth(_fp._frequentPatterns):
     """
 
-    :Description:   FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+    :Description:   FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
 
     :Reference:  Han, J., Pei, J., Yin, Y. et al. Mining Frequent Patterns without Candidate Generation: A Frequent-Pattern
            Tree Approach. Data  Mining and Knowledge Discovery 8, 53–87 (2004). https://doi.org/10.1023
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
@@ -575,15 +575,15 @@
         data = []
         for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# CHARM is an algorithm to discover closed frequent patterns in a transactional database. Closed frequent patterns are patterns if there exists no superset that has the same support count as this original itemset . This algorithm employs depth-first search technique to find the complete set of closed frequent patterns in a
+# CHARM is an algorithm to discover closed frequent patterns in a transactional database. Closed frequent patterns are patterns if there exists no superset that has the same support count as this original itemset. This algorithm employs depth-first search technique to find the complete set of closed frequent patterns in a
 #
 #  **Importing this algorithm into a python program**
 #  --------------------------------------------------------------
 #
 #
-#             from PAMI.frequentPattern.closed import CHARM as alg
+#             from PAMI.frequentPattern.closed import closed as alg
 #
-#             obj = alg.CHARM(iFile, minSup)
+#             obj = alg.Closed(iFile, minSup)
 #
 #             obj.startMine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Closed Frequent Patterns:", len(frequentPatterns))
 #
@@ -120,17 +120,17 @@
             .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
     --------------------------------------------------------------
     .. code-block:: python
 
-            from PAMI.frequentPattern.closed import CHARM as alg
+            from PAMI.frequentPattern.closed import closed as alg
 
-            obj = alg.CHARM(iFile, minSup)
+            obj = alg.Closed(iFile, minSup)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Closed Frequent Patterns:", len(frequentPatterns))
 
@@ -349,14 +349,15 @@
 
             :type itemSets: list
 
             :param tidSets: timestamps of the items in the argument itemSets
 
             :type tidSets: list
 
+
         """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
         if len(itemSets) == 2:
@@ -500,15 +501,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
-#     import PAMI.frequentPattern.cuda.cuApriori as alg
+#     import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 #
-#     obj = alg.cuApriori(iFile, minSup)
+#     obj = alg.cuAprioriBit(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -48,15 +48,15 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 # from PAMI.frequentPattern.cuda import abstract as _ab
 import abstract as _ab
 
-class cuApriori(_ab._frequentPatterns):
+class cuAprioriBit(_ab._frequentPatterns):
     """
     :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
     :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
             In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
     :param  iFile: str :
@@ -92,30 +92,30 @@
 
 
 
     **Methods to execute code on terminal**
     ----------------------------------------------------
 
             Format:
-                      >>> python3 cuApriori.py <inputFile> <outputFile> <minSup>
+                      >>> python3 cuAprioriBit.py <inputFile> <outputFile> <minSup>
 
             Example:
-                      >>>  python3 cuApriori.py sampleDB.txt patterns.txt 10.0
+                      >>>  python3 cuAprioriBit.py sampleDB.txt patterns.txt 10.0
 
             .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
     ----------------------------------------------------
 
     .. code-block:: python
 
-             import PAMI.frequentPattern.cuda.cuApriori as alg
+             import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 
-             obj = alg.cuApriori(iFile, minSup)
+             obj = alg.cuAprioriBit(iFile, minSup)
 
              obj.startMine()
 
              frequentPatterns = obj.getPatterns()
 
              print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -139,17 +139,14 @@
     **Credits:**
     -------------
 
              The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _ab._cp.cuda.Device(0).use()
-
-
 
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
@@ -173,14 +170,17 @@
         }
         return;    
     }
 
     ''', 'sumKernel')
 
 
+
+
+
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
         self._Database = []
@@ -245,57 +245,77 @@
                     ArraysAndItems[j] = [i]
                 else:
                     ArraysAndItems[j].append(i)
 
         newArraysAndItems = {}
 
         for k,v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
+            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
             if len(v) >= self._minSup:
                 self._finalPatterns[k] = len(v)
                 newArraysAndItems[k] = ArraysAndItems[k]
 
         return newArraysAndItems
+    
+    def createBitRepresentation(self, ArraysAndItems):
+        bitRep = {}
+        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
+
+
+        for k, v in ArraysAndItems.items():
+            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
+            for i in v:
+                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
+
+        for k, v in bitRep.items():
+            bitRep[k] = _ab._cp.array(v)
+
+        return bitRep
 
     
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
 
         ArraysAndItems = self.arraysAndItems()
+        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 # print(i, "/", len(ArraysAndItems), end="\r")
                 iList = list(keys[i])
-                for j in range(i+1, len(ArraysAndItems)):
+                for j in range(i+1, len(ArraysAndItems)):   
+                    unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
+                    sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
+                    self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
+                    sum = sum[0]
                     jList = list(keys[j])
                     union = tuple(sorted(set(iList + jList)))
-                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]], assume_unique=True)
-                    if len(intersect) >= self._minSup and union not in self._finalPatterns:
-                        newArraysAndItems[union] = intersect
-                        self._finalPatterns[union] = len(intersect)
+                    if sum >= self._minSup and union not in self._finalPatterns:
+                        newArraysAndItems[union] = unionData
+                        string = "\t".join(union)
+                        self._finalPatterns[string] = sum
             ArraysAndItems = newArraysAndItems
             # print()
 
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuApriori algorithm ")
+        print("Frequent patterns were generated successfully using cuAprioriBit algorithm ")
             
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
@@ -362,35 +382,33 @@
         """
         return self._finalPatterns
 
     def printResults(self):
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in s:", self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in s:", _ap.getRuntime())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-
-    _ap = cuApriori("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
-    _ap = cuApriori("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+    _ap = cuAprioriBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
     _ap.startMine()
     print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+    _ap.save(_ab._sys.argv[2])
     print("Total Memory in USS:", _ap.getMemoryUSS())
     print("Total Memory in RSS", _ap.getMemoryRSS())
     print("Total ExecutionTime in s:", _ap.getRuntime())
-
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
-#
+# VBFTMine is one of the fundamental algorithm to discover fault tolerant frequent patterns in a uncertain transactional database based on bitset representation.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
-#
-#     import PAMI.frequentPattern.cuda.cuAprioriBit as alg
-#
-#     obj = alg.cuAprioriBit(iFile, minSup)
-#
-#     obj.startMine()
+# ---------------------------------------------------
 #
-#     frequentPatterns = obj.getPatterns()
+# import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+# obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
 #
-#     obj.savePatterns(oFile)
+# obj.startMine()
 #
-#     Df = obj.getPatternInDataFrame()
+# faultTolerantFrequentPatterns = obj.getPatterns()
 #
-#     memUSS = obj.getMemoryUSS()
+# print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
 #
-#     print("Total Memory in USS:", memUSS)
+# obj.save(oFile)
 #
-#     memRSS = obj.getMemoryRSS()
+# Df = obj.getPatternInDataFrame()
 #
-#     print("Total Memory in RSS", memRSS)
+# print("Total Memory in USS:", obj.getMemoryUSS())
 #
-#     run = obj.getRuntime()
+# print("Total Memory in RSS", obj.getMemoryRSS())
 #
-#     print("Total ExecutionTime in seconds:", run)
-
+# print("Total ExecutionTime in seconds:", obj.getRuntime())
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
@@ -44,36 +36,47 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+import numpy as _np
+from PAMI.faultTolerantFrequentPattern.basic import abstract as _ab
 
-# from PAMI.frequentPattern.cuda import abstract as _ab
-import abstract as _ab
-
-class cuAprioriBit(_ab._frequentPatterns):
+class VBFTMine(_ab._faultTolerantFrequentPatterns):
     """
-    :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
-
-    :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
-            In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
-
+    
+    :Description:  VBFTMine is one of the fundamental algorithm to discover fault tolerant frequent patterns in a uncertain transactional database based on
+                   bitset representation.
+                   This program employs apriori property (or downward closure property) to  reduce the search space effectively.
+
+    :Reference:         Koh, JL., Yo, PW. (2005). An Efficient Approach for Mining Fault-Tolerant Frequent Patterns Based on Bit Vector Representations.
+                        In: Zhou, L., Ooi, B.C., Meng, X. (eds) Database Systems for Advanced Applications. DASFAA 2005. Lecture Notes in Computer Science,
+                        vol 3453. Springer, Berlin, Heidelberg. https://doi.org/10.1007/11408079_51
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+           Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
+    :param  minSup: float or int or str :
+                    The user can specify minSup either in count or proportion of database size.
+                    If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+                    Otherwise, it will be treated as float.
+                    Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+    :param  itemSup: int or float :
+                    Frequency of an item
+    :param minLength: int
+                    minimum length of a pattern
+    :param faultTolerance: int
+
+
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
-
     :Attributes:
 
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
@@ -87,99 +90,71 @@
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
         Database : list
           To store the transactions of a database in list
 
 
+    Executing the code on terminal:
+    -------------------------------
 
-    **Methods to execute code on terminal**
-    ----------------------------------------------------
-
-            Format:
-                      >>> python3 cuAprioriBit.py <inputFile> <outputFile> <minSup>
+        Format:
+        --------
+            >>> python3 VBFTMine.py <inputFile> <outputFile> <minSup> <itemSup> <minLength> <faultTolerance>
 
-            Example:
-                      >>>  python3 cuAprioriBit.py sampleDB.txt patterns.txt 10.0
+        Examples:
+        ---------
+            >>> python3 VBFTMine.py sampleDB.txt patterns.txt 10.0 3.0 3 1  (minSup will be considered in times of minSup and count of database transactions)
 
-            .. note:: minSup will be considered in percentage of database transactions
-
-
-    **Importing this algorithm into a python program**
-    ----------------------------------------------------
 
+    Sample run of the importing code:
+    ---------------------------------
     .. code-block:: python
+    
+        import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
 
-             import PAMI.frequentPattern.cuda.cuAprioriBit as alg
-
-             obj = alg.cuAprioriBit(iFile, minSup)
-
-             obj.startMine()
-
-             frequentPatterns = obj.getPatterns()
-
-             print("Total number of Frequent Patterns:", len(frequentPatterns))
-
-             obj.savePatterns(oFile)
-
-             Df = obj.getPatternInDataFrame()
-
-             memUSS = obj.getMemoryUSS()
+        obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
 
-             print("Total Memory in USS:", memUSS)
+        obj.startMine()
 
-             memRSS = obj.getMemoryRSS()
+        faultTolerantFrequentPatterns = obj.getPatterns()
 
-             print("Total Memory in RSS", memRSS)
+        print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
 
-             run = obj.getRuntime()
+        obj.save(oFile)
 
-             print("Total ExecutionTime in seconds:", run)
+        Df = obj.getPatternInDataFrame()
 
+        print("Total Memory in USS:", obj.getMemoryUSS())
 
-    **Credits:**
-    -------------
+        print("Total Memory in RSS", obj.getMemoryRSS())
 
-             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+        print("Total ExecutionTime in seconds:", obj.getRuntime())
 
-    """
+    Credits:
+    --------
+        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
+        """
 
     _minSup = float()
+    _itemSup = float()
+    _minLength = int()
+    _faultTolerance = int()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
+    _plist = []
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-
-    _sumKernel = _ab._cp.RawKernel(r'''
-
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
-
-    ''', 'sumKernel')
-
-
-
-
+    _mapSupport = {}
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
@@ -206,14 +181,17 @@
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
+                            for i in temp:
+                                if i not in self._plist:
+                                    self._plist.append(i)
                             self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _convert(self, value):
         """
@@ -230,93 +208,115 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
-    
-    def arraysAndItems(self):
-        ArraysAndItems = {}
 
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                j = tuple([j])
-                if j not in ArraysAndItems:
-                    ArraysAndItems[j] = [i]
+    def _Count(self, tids):
+        count = 0
+        for i in tids:
+            if i == 1:
+                count += 1
+        return count
+
+    def _save(self, prefix, suffix, tidsetx):
+        if (prefix == None):
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        prefix = list(set(prefix))
+        prefix.sort()
+        val = self._Count(tidsetx)
+        if len(prefix) > self._faultTolerance:
+            self._finalPatterns[tuple(prefix)] = val
+
+    def _processEquivalenceClass(self, prefix, itemsets, tidsets):
+        if (len(itemsets) == 1):
+            i = itemsets[0]
+            tidi = tidsets[0]
+            self._save(prefix, [i], tidi)
+            return
+        for i in range(len(itemsets)):
+            itemx = itemsets[i]
+            if (itemx == None):
+                continue
+            tidsetx = tidsets[i]
+            classItemsets = []
+            classtidsets = []
+            itemsetx = [itemx]
+            for j in range(i + 1, len(itemsets)):
+                itemj = itemsets[j]
+                tidsetj = tidsets[j]
+                y = list(_np.array(tidsetx) & _np.array(tidsetj))
+                total = self._Count(y)
+                if total >= self._minSup:
+                    classItemsets.append(itemj)
+                    classtidsets.append(y)
+            if (len(classItemsets) > 0):
+                newprefix = list(set(itemsetx)) + prefix
+                self._processEquivalenceClass(newprefix, classItemsets, classtidsets)
+            self._save(prefix, list(set(itemsetx)), tidsetx)
+
+    def _oneLengthFrequentItems(self):
+        """ To calculate the one Length items"""
+        Vector = {}
+        items = []
+        for i in self._Database:
+            for j in self._plist:
+                count = 0
+                if j in i:
+                    count = 1
+                if j in Vector:
+                    Vector[j].append(count)
                 else:
-                    ArraysAndItems[j].append(i)
-
-        newArraysAndItems = {}
-
-        for k,v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
-            if len(v) >= self._minSup:
-                self._finalPatterns[k] = len(v)
-                newArraysAndItems[k] = ArraysAndItems[k]
+                    Vector[j] = [count]
+        for x, y in Vector.items():
+            v = self._Count(y)
+            if v >= self._itemSup:
+                items.append(x)
+        return Vector, items
 
-        return newArraysAndItems
-    
-    def createBitRepresentation(self, ArraysAndItems):
-        bitRep = {}
-        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
-
-
-        for k, v in ArraysAndItems.items():
-            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
-            for i in v:
-                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
-
-        for k, v in bitRep.items():
-            bitRep[k] = _ab._cp.array(v)
-
-        return bitRep
-
-    
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
-
-        ArraysAndItems = self.arraysAndItems()
-        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
-
-        while len(ArraysAndItems) > 0:
-            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
-            newArraysAndItems = {}
-            keys = list(ArraysAndItems.keys())
-            for i in range(len(ArraysAndItems)):
-                # print(i, "/", len(ArraysAndItems), end="\r")
-                iList = list(keys[i])
-                for j in range(i+1, len(ArraysAndItems)):   
-                    unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
-                    sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
-                    self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
-                    sum = sum[0]
-                    jList = list(keys[j])
-                    union = tuple(sorted(set(iList + jList)))
-                    if sum >= self._minSup and union not in self._finalPatterns:
-                        newArraysAndItems[union] = unionData
-                        string = "\t".join(union)
-                        self._finalPatterns[string] = sum
-            ArraysAndItems = newArraysAndItems
-            # print()
-
+        self._itemSup = self._convert(self._itemSup)
+        self._minLength = int(self._minLength)
+        self._faultTolerance = int(self._faultTolerance)
+        Vector, plist = self._oneLengthFrequentItems()
+        for i in range(len(plist)):
+            itemx = plist[i]
+            tidsetx = Vector[itemx]
+            itemsetx = [itemx]
+            itemsets = []
+            tidsets = []
+            for j in range(i + 1, len(plist)):
+                itemj = plist[j]
+                tidsetj = Vector[itemj]
+                y1 = list(_np.array(tidsetx) | _np.array(tidsetj))
+                total = self._Count(y1)
+                if total >= self._minSup:
+                    itemsets.append(itemj)
+                    tidsets.append(y1)
+            if (len(itemsets) > 0):
+                self._processEquivalenceClass(itemsetx, itemsets, tidsets)
+            self._save(None, itemsetx, tidsetx)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuAprioriBit algorithm ")
-            
+        print("Fault-Tolerant Frequent patterns were generated successfully using VBFTMine algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -351,30 +351,36 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
+            s = str()
+            for i in a:
+                s = s + i + ' '
+            data.append([s, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s = str()
+            for i in x:
+                s = s + i + '\t'
+            s1 = s.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
@@ -387,28 +393,25 @@
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_ab._sys.argv) == 7 or len(_ab._sys.argv) == 8:
+        if len(_ab._sys.argv) == 8:
+            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3],  _ab._sys.argv[4],
+                            _ab._sys.argv[5], _ab._sys.argv[6], _ab._sys.argv[7],)
+        if len(_ab._sys.argv) == 7:
+            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = VBFTMine('/Users/Likhitha/Downloads/fault/sample4.txt', 5, 3, 2, 1, ' ')
+        _ap.startMine()
+        _ap.printResults()
+        print(_ap.getPatternsAsDataFrame())
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-    _ap = cuAprioriBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    _ap.save(_ab._sys.argv[2])
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-#
+# Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
+#  ----------------------------------------------------
+#
 #
-#     import PAMI.frequentPattern.cuda.cuEclat as alg
+#     import PAMI.frequentPattern.pyspark.parallelECLAT as alg
 #
-#     obj = alg.cuEclat(iFile, minSup)
+#     obj = alg.parallelECLAT(iFile, minSup, numWorkers)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -25,16 +25,16 @@
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
-
-
+#
+#
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -45,33 +45,39 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-# from PAMI.frequentPattern.cuda import abstract as _ab
-import abstract as _ab
 
-class cuEclat(_ab._frequentPatterns):
+
+
+# from pyspark import SparkConf, SparkContext
+# import abstract as _ab
+from PAMI.frequentPattern.pyspark import abstract as _ab
+
+
+class parallelECLAT(_ab._frequentPatterns):
     """
-    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
-    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+    :Description: Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
+
+    :Reference:
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
+    :param  numPartitions: int :
+                   The number of partitions. On each worker node, an executor process is started and this process performs processing.The processing unit of worker node is partition
 
 
     :Attributes:
 
         startTime : float
           To record the start time of the mining process
 
@@ -83,319 +89,236 @@
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
-        Database : list
-          To store the transactions of a database in list
-
-
+        lno : int
+                the number of transactions
 
+    
     **Methods to execute code on terminal**
     ----------------------------------------------------
-
+    
             Format:
-                      >>> python3 cuEclat.py <inputFile> <outputFile> <minSup>
-
+                      >>> python3 parallelECLAT.py <inputFile> <outputFile> <minSup> <numWorkers>
+    
             Example:
-                      >>>  python3 cuEclat.py sampleDB.txt patterns.txt 10.0
-
+                      >>> python3 parallelECLAT.py sampleDB.txt patterns.txt 10.0 3
+    
             .. note:: minSup will be considered in percentage of database transactions
-
-
+    
+    
     **Importing this algorithm into a python program**
     ----------------------------------------------------
-
     .. code-block:: python
-
-             import PAMI.frequentPattern.cuda.cuEclat as alg
-
-             obj = alg.cuEclat(iFile, minSup)
-
-             obj.startMine()
-
-             frequentPatterns = obj.getPatterns()
-
-             print("Total number of Frequent Patterns:", len(frequentPatterns))
-
-             obj.savePatterns(oFile)
-
-             Df = obj.getPatternInDataFrame()
-
-             memUSS = obj.getMemoryUSS()
-
-             print("Total Memory in USS:", memUSS)
-
-             memRSS = obj.getMemoryRSS()
-
-             print("Total Memory in RSS", memRSS)
-
-             run = obj.getRuntime()
-
-             print("Total ExecutionTime in seconds:", run)
-
-
+    
+                import PAMI.frequentPattern.pyspark.parallelECLAT as alg
+    
+                obj = alg.parallelECLAT(iFile, minSup, numWorkers)
+    
+                obj.startMine()
+    
+                frequentPatterns = obj.getPatterns()
+    
+                print("Total number of Frequent Patterns:", len(frequentPatterns))
+    
+                obj.savePatterns(oFile)
+    
+                Df = obj.getPatternInDataFrame()
+    
+                memUSS = obj.getMemoryUSS()
+    
+                print("Total Memory in USS:", memUSS)
+    
+                memRSS = obj.getMemoryRSS()
+    
+                print("Total Memory in RSS", memRSS)
+    
+                run = obj.getRuntime()
+    
+                print("Total ExecutionTime in seconds:", run)
+    
+    
     **Credits:**
-    -------------
-
-             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+    ----------------------------------------------------
+             The complete program was written by Yudai Masu under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _ab._cp.cuda.Device(0).use()
-
-
-
     _minSup = float()
+    _numPartitions = int()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
-    _Database = []
-
-    _sumKernel = _ab._cp.RawKernel(r'''
-
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
-
-    ''', 'sumKernel')
-
-
-    def _creatingItemSets(self):
-        """
-            Storing the complete transactions of the database/input file in a database variable
-
-
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            temp = []
-            if self._iFile.empty:
-                print("its empty..")
-            i = self._iFile.columns.values.tolist()
-            if 'Transactions' in i:
-                temp = self._iFile['Transactions'].tolist()
-
-            for k in temp:
-                self._Database.append(set(k))
-        if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
-                for line in data:
-                    line.strip()
-                    line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    self._Database.append(set(temp))
-            else:
-                try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
-                        for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self._Database.append(set(temp))
-                except IOError:
-                    print("File Not Found")
-                    quit()
-
-    def _convert(self, value):
-        """
-        To convert the user specified minSup value
-
-        :param value: user specified minSup value
-
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
-    
-    def arraysAndItems(self):
-        ArraysAndItems = {}
-
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                j = tuple([j])
-                if j not in ArraysAndItems:
-                    ArraysAndItems[j] = [i]
-                else:
-                    ArraysAndItems[j].append(i)
-
-        newArraysAndItems = {}
-
-        for k,v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
-            if len(v) >= self._minSup:
-                self._finalPatterns[k] = len(v)
-                newArraysAndItems[k] = ArraysAndItems[k]
-
-        return newArraysAndItems
-
-    
-    def startMine(self):
-        """
-            Frequent pattern mining process will start from here
-        """
-        self._Database = []
-        self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
+    _lno = int()
 
-        ArraysAndItems = self.arraysAndItems()
-
-        while len(ArraysAndItems) > 0:
-            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
-            newArraysAndItems = {}
-            keys = list(ArraysAndItems.keys())
-            for i in range(len(ArraysAndItems)):
-                iList = list(keys[i])
-                for j in range(i+1, len(ArraysAndItems)):
-                    # print(i, "/", len(ArraysAndItems), end="\r")
-                    jList = list(keys[j])
-                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
-                        union = iList + [jList[-1]]
-                        union = tuple(union)
-                        intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]], assume_unique=True)
-                        if len(intersect) >= self._minSup:
-                            newArraysAndItems[union] = intersect
-                            self._finalPatterns[union] = len(intersect)
-                    else: 
-                        break
-
-            ArraysAndItems = newArraysAndItems
-            # print()
-
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuEclat algorithm ")
-            
+    def __init__(self, iFile, minSup, numWorkers, sep='\t'):
+        super().__init__(iFile, minSup, int(numWorkers), sep)
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
+            data.append([a, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
-    def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
-
+    def savePatterns(self, outFile):
+        """
+        Complete set of frequent patterns will be loaded in to a output file
         :param outFile: name of the output file
-
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s1 = x + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
-
+        """
+        Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
-
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
-        print("Total Memory in USS:", self.getMemoryUSS())
-        print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in s:", self.getRuntime())
+    def _genPatterns(self, suffix, pattern, data):
+        freqPatterns = {}
+        index = data.index(suffix)
+        for i in range(index + 1, len(data)):
+            tid = pattern[1].intersection(data[i][1])
+            if len(tid) >= self._minSup:
+                freqPattern = pattern[0] + ' ' + data[i][0]
+                freqPatterns[freqPattern] = len(tid)
+                freqPatterns.update(self._genPatterns(data[i], (freqPattern, tid), data))
+        return freqPatterns
+
+    def _convert(self, value):
+        """
+        To convert the user specified minSup value
+        :param value: user specified minSup value
+        :return: converted type
+        """
+        print(value, type(value))
+        if type(value) is int:
+            value = int(value)
+        elif type(value) is float:
+            value = (self._lno * value)
+        elif type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (self._lno * value)
+            else:
+                value = int(value)
+        else:
+            print("None")
+        print(type(value), value)
+        return value
+
+    def startMine(self):
+        """
+        Frequent pattern mining process will start from here
+        """
+
+        self._startTime = _ab._time.time()
+        conf = SparkConf().setAppName("Parallel ECLAT").setMaster("local[*]")
+        sc = SparkContext(conf=conf)
+
+        data = sc.textFile(self._iFile, self._numPartitions) \
+            .map(lambda line: [int(y) for y in line.rstrip().split(self._sep)]).persist()
+        self._lno = data.count()
+        self._minSup = self._convert(self._minSup)
+
+        frequentItems = None
+        if 'transactional' in self._iFile:
+            frequentItems = data.zipWithIndex() \
+                .flatMap(lambda x: [(str(item), x[1]) for item in x[0]]) \
+                .groupByKey() \
+                .filter(lambda x: len(x[1]) >= self._minSup) \
+                .sortBy(lambda x: len(x[1])) \
+                .mapValues(set) \
+                .persist()
+            data.unpersist()
+        elif 'temporal' in self._iFile:
+            frequentItems = data.flatMap(lambda trans: [(str(item), trans[0]) for item in trans[1:]]) \
+                .groupByKey() \
+                .filter(lambda x: len(x[1]) >= self._minSup) \
+                .mapValues(set) \
+                .persist()
+            data.unpersist()
+        else:
+            pass
+            # print("may be not able to process the input file")
+
+        freqItems = dict(frequentItems.collect())
+        # print(len(freqItems))
+        self._finalPatterns = {k: len(v) for k, v in freqItems.items()}
+
+        freqPatterns = list(frequentItems.map(lambda x: self._genPatterns(x, x, list(freqItems.items())))
+                            .filter(lambda x: len(x) != 0).collect())
+        for value in freqPatterns:
+            self._finalPatterns.update(value)
+
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
+        print("Frequent patterns were generated successfully using Parallel ECLAT algorithm")
+        sc.stop()
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
+        if len(_ab._sys.argv) == 6:
+            _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = cuEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = cuEclat(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in s:", _ap.getRuntime())
+        _finalPatterns = _ap.getPatterns()
+        print("Total number of Frequent Patterns:", len(_finalPatterns))
+        # _ap.savePatterns(_ab._sys.argv[2])
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
-    _ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
-    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
-
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-#
-#
+
+
+
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
+# --------------------------------------------------------
 #
-#     import PAMI.frequentPattern.cuda.cuEclatBit as alg
+#     from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 #
-#     obj = alg.cuEclatBit(iFile, minSup)
+#     obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 #
 #     obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#     periodicFrequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.savePatterns("patterns")
 #
-#     Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
+#
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -42,378 +43,374 @@
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
+
 """
 
+from PAMI.periodicFrequentPattern.basic import abstract as _ab
 
-# from PAMI.frequentPattern.cuda import abstract as _ab
-import abstract as _ab
 
-class cuEclatBit(_ab._frequentPatterns):
+class PFECLAT(_ab._periodicFrequentPatterns):
     """
-    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-
-    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
-
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  minSup: int :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-
-    :Attributes:
-
-        startTime : float
-          To record the start time of the mining process
-
-        endTime : float
-          To record the completion time of the mining process
-
-        finalPatterns : dict
-          Storing the complete set of patterns in a dictionary variable
+    Description:
+    -------------
+        EclatPFP is the fundamental approach to mine the periodic-frequent patterns.
 
+    Reference:
+    -----------
+        P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
+        periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
+
+    Attributes:
+    -----------
+        iFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup: int or float or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        maxPer: int or float or str
+            The user can specify maxPer either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
         memoryUSS : float
-          To store the total amount of USS memory consumed by the program
-
+            To store the total amount of USS memory consumed by the program
         memoryRSS : float
-          To store the total amount of RSS memory consumed by the program
-
+            To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
         Database : list
-          To store the transactions of a database in list
-
-
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            it represents the total no of transactions
+        tree : class
+            it represents the Tree class
+        itemSetCount : int
+            it represents the total no of patterns
+        finalPatterns : dict
+            it represents to store the patterns
+        tidList : dict
+            stores the timestamps of an item
+        hashing : dict
+            stores the patterns with their support to check for the closed property
+
+    Methods:
+    ---------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        save(oFile)
+            Complete set of periodic-frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of periodic-frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingOneItemSets()
+            Scan the database and store the items with their timestamps which are periodic frequent 
+        getPeriodAndSupport()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
+            
 
     **Methods to execute code on terminal**
-    ----------------------------------------------------
 
             Format:
-                      >>> python3 cuEclatBit.py <inputFile> <outputFile> <minSup>
-
+                      >>>  python3 PFECLAT.py <inputFile> <outputFile> <minSup>
             Example:
-                      >>>  python3 cuEclatBit.py sampleDB.txt patterns.txt 10.0
+                      >>>   python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
 
             .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
-    ----------------------------------------------------
 
     .. code-block:: python
 
-             import PAMI.frequentPattern.cuda.cuEclatBit as alg
+             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 
-             obj = alg.cuEclatBit(iFile, minSup)
+                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 
-             obj.startMine()
+                obj.startMine()
 
-             frequentPatterns = obj.getPatterns()
+                periodicFrequentPatterns = obj.getPatterns()
 
-             print("Total number of Frequent Patterns:", len(frequentPatterns))
+                print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
-             obj.savePatterns(oFile)
+                obj.savePatterns("patterns")
 
-             Df = obj.getPatternInDataFrame()
+                Df = obj.getPatternsAsDataFrame()
 
-             memUSS = obj.getMemoryUSS()
+                memUSS = obj.getMemoryUSS()
 
-             print("Total Memory in USS:", memUSS)
+                print("Total Memory in USS:", memUSS)
 
-             memRSS = obj.getMemoryRSS()
+                memRSS = obj.getMemoryRSS()
 
-             print("Total Memory in RSS", memRSS)
+                print("Total Memory in RSS", memRSS)
 
-             run = obj.getRuntime()
-
-             print("Total ExecutionTime in seconds:", run)
+                run = obj.getRuntime()
 
+                print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    -------------
-
-             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
-    """
+             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
 
-    _minSup = float()
-    _startTime = float()
-    _endTime = float()
-    _finalPatterns = {}
+        """
+    
     _iFile = " "
     _oFile = " "
     _sep = " "
+    _dbSize = None
+    _Database = None
+    _minSup = str()
+    _maxPer = str()
+    _tidSet = set()
+    _finalPatterns = {}
+    _startTime = None
+    _endTime = None
     _memoryUSS = float()
     _memoryRSS = float()
-    _Database = []
-
-    _sumKernel = _ab._cp.RawKernel(r'''
-
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
 
-    ''', 'sumKernel')
+    def _getPeriodic(self, tids: set):
+        tidList = list(tids)
+        tidList.sort()
+        tidList.append(self._dbSize)
+        cur = 0
+        per = 0
+        for tid in tidList:
+            per = max(per, tid - cur)
+            if per > self._maxPer:  # early stopping
+                break
+            cur = tid
+        return per
 
-
-
-
-
-    def _creatingItemSets(self):
+    def _convert(self, value):
         """
-            Storing the complete transactions of the database/input file in a database variable
+        To convert the given user specified value
 
+        :param value: user specified value
+        :return: converted value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (self._dbSize * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (self._dbSize * value)
+            else:
+                value = int(value)
+        return value
 
+    def _creatingOneItemSets(self):
+        """Storing the complete transactions of the database/input file in a database variable
         """
-        self._Database = []
+        plist = []
+        Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            temp = []
+            ts, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
+            if 'TS' in i:
+                ts = self._iFile['TS'].tolist()
             if 'Transactions' in i:
-                temp = self._iFile['Transactions'].tolist()
-
-            for k in temp:
-                self._Database.append(set(k))
+                data = self._iFile['Transactions'].tolist()
+            for i in range(len(data)):
+                tr = [ts[i][0]]
+                tr = tr + data[i]
+                Database.append(tr)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(set(temp))
+                    Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(set(temp))
+                            Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
-
-    def _convert(self, value):
-        """
-        To convert the user specified minSup value
-
-        :param value: user specified minSup value
-
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
-    
-    def arraysAndItems(self):
-        ArraysAndItems = {}
-
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                j = tuple([j])
-                if j not in ArraysAndItems:
-                    ArraysAndItems[j] = [i]
+        tid = 0
+        itemsets = {}  # {key: item, value: list of tids}
+        periodicHelper = {}  # {key: item, value: [period, last_tid]}
+        for line in Database:
+            tid = int(line[0])
+            self._tidSet.add(tid)
+            for item in line[1:]:
+                if item in itemsets:
+                    itemsets[item].add(tid)
+                    periodicHelper[item][0] = max(periodicHelper[item][0],
+                                                  abs(tid - periodicHelper[item][1]))  # update current max period
+                    periodicHelper[item][1] = tid  # update the last tid
                 else:
-                    ArraysAndItems[j].append(i)
+                    itemsets[item] = {tid}
+                    periodicHelper[item] = [abs(0 - tid), tid]  # initialize helper
 
-        newArraysAndItems = {}
-
-        for k,v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
-            if len(v) >= self._minSup:
-                self._finalPatterns[k] = len(v)
-                newArraysAndItems[k] = ArraysAndItems[k]
-
-        return newArraysAndItems
+        # finish all items' period
+        self._dbSize = len(Database)
+        self._minSup = self._convert(self._minSup)
+        self._maxPer = self._convert(self._maxPer)
+        del Database
+        for item, _ in periodicHelper.items():
+            periodicHelper[item][0] = max(periodicHelper[item][0],
+                                          abs(self._dbSize - periodicHelper[item][1]))  # tid of the last transaction
+        candidates = []
+        for item, tids in itemsets.items():
+            per = periodicHelper[item][0]
+            sup = len(tids)
+            if sup >= self._minSup and per <= self._maxPer:
+                candidates.append(item)
+                self._finalPatterns[item] = [sup, per, tids]
+        return candidates
     
-    def createBitRepresentation(self, ArraysAndItems):
-        bitRep = {}
-        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
-
-
-        for k, v in ArraysAndItems.items():
-            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
-            for i in v:
-                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
-
-        for k, v in bitRep.items():
-            bitRep[k] = _ab._cp.array(v)
-
-        return bitRep
+    def _generateEclat(self, candidates):
+        newCandidates = []
+        for i in range(0, len(candidates)):
+            prefixItem = candidates[i]
+            prefixItemSet = prefixItem.split()
+            for j in range(i + 1, len(candidates)):
+                item = candidates[j]
+                itemSet = item.split()
+                if prefixItemSet[:-1] == itemSet[:-1] and prefixItemSet[-1] != itemSet[-1]:
+                    _value = self._finalPatterns[item][2].intersection(self._finalPatterns[prefixItem][2])
+                    sup = len(_value)
+                    per = self._getPeriodic(_value)
+                    if sup >= self._minSup and per <= self._maxPer:
+                        newItem = prefixItem + " " + itemSet[-1]
+                        self._finalPatterns[newItem] = [sup, per, _value]
+                        newCandidates.append(newItem)
 
+        if len(newCandidates) > 0:
+            self._generateEclat(newCandidates)
     
     def startMine(self):
-        """
-            Frequent pattern mining process will start from here
-        """
-        self._Database = []
         self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        itemsList = sorted(list(set.union(*self._Database)))  # because Database is list
-        self._minSup = self._convert(self._minSup)
-
-        ArraysAndItems = self.arraysAndItems()
-
-        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
-
-        while len(ArraysAndItems) > 0:
-            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
-            newArraysAndItems = {}
-            keys = list(ArraysAndItems.keys())
-            for i in range(len(ArraysAndItems)):
-                iList = list(keys[i])
-                # print(i, "/", len(ArraysAndItems), end="\r")
-                for j in range(i+1, len(ArraysAndItems)):  
-                    jList = list(keys[j])
-                    union = []
-                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
-                        union = iList + [jList[-1]]
-                        union = tuple(union)
-                        unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
-                        sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
-                        self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
-                        sum = sum[0]
-                        if sum >= self._minSup and union not in self._finalPatterns:
-                            newArraysAndItems[union] = unionData
-                            string = "\t".join(union)
-                            self._finalPatterns[string] = sum
-            ArraysAndItems = newArraysAndItems
-            # print()
-
+        self._finalPatterns = {}
+        frequentSets = self._creatingOneItemSets()
+        self._generateEclat(frequentSets)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
         self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuEclatBit algorithm ")
-            
+        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
 
-        :return: returning total amount of runtime taken by the mining process
 
+        :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
-        """Storing final frequent patterns in a dataframe
-
-        :return: returning frequent patterns in a dataframe
+        """Storing final periodic-frequent patterns in a dataframe
 
+        :return: returning periodic-frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
-        return dataFrame
+            data.append([a, b[0], b[1]])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
+        return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of periodic-frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
-
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
-
-        :return: returning frequent patterns
+        """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
+        :return: returning periodic-frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
-
+        print("Total ExecutionTime in ms:",  self.getRuntime())
+                    
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
+        if len(_ab._sys.argv) == 6:
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-    _ap = cuEclatBit("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    _ap.save(_ab._sys.argv[2])
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 #
 #
 
+
+#
+#
+#
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
 
 class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
             employ in PAMI
-
            Attributes:
            ----------
             iFile : str
                 Input file name or path of the input file
             minSup: integer or float or str
                 The user can specify minSup either in count or proportion of database size.
                 If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
@@ -39,15 +38,14 @@
                 Storing the complete set of patterns in a dictionary variable
             oFile : str
                 Name of the output file to store complete set of frequent patterns
             memoryUSS : float
                 To store the total amount of USS memory consumed by the program
             memoryRSS : float
                 To store the total amount of RSS memory consumed by the program
-
            Methods:
            -------
             startMine()
                 Calling this function will start the actual mining process
             getPatterns()
                 This function will output all interesting patterns discovered by an algorithm
             save(oFile)
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Parallel Apriori is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
+
 #
 #
 #  **Importing this algorithm into a python program**
 #  ---------------------------------------------------
 #
 #         import PAMI.frequentPattern.pyspark.parallelApriori as alg
 #
@@ -25,14 +26,15 @@
 #         memRSS = obj.getMemoryRSS()
 #
 #         print("Total Memory in RSS", memRSS)
 #
 #         run = obj.getRuntime()
 #
 #         print("Total ExecutionTime in seconds:", run)
+
 #
 #
 #
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
@@ -137,15 +139,16 @@
                 run = obj.getRuntime()
     
                 print("Total ExecutionTime in seconds:", run)
     
     
     **Credits:**
     -----------------------------------------
-            The complete program was written by Yudai Masu  under the supervision of Professor Rage Uday Kiran.
+    
+             The complete program was written by Yudai Masu  under the supervision of Professor Rage Uday Kiran.
 
 
     """
 
     _minSup = float()
     _startTime = float()
     _endTime = float()
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
+
+
+# Top - K is and algorithm to discover top frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-#  ----------------------------------------------------
+# ---------------------------------------------------------
 #
+#         import PAMI.frequentPattern.topK.FAE as alg
 #
-#     import PAMI.frequentPattern.pyspark.parallelECLAT as alg
+#         obj = alg.FAE(iFile, K)
 #
-#     obj = alg.parallelECLAT(iFile, minSup, numWorkers)
+#         obj.startMine()
 #
-#     obj.startMine()
+#         topKFrequentPatterns = obj.getPatterns()
 #
-#     frequentPatterns = obj.getPatterns()
+#         print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#         obj.save(oFile)
 #
-#     obj.savePatterns(oFile)
+#         Df = obj.getPatternInDataFrame()
 #
-#     Df = obj.getPatternInDataFrame()
+#         memUSS = obj.getMemoryUSS()
 #
-#     memUSS = obj.getMemoryUSS()
+#         print("Total Memory in USS:", memUSS)
 #
-#     print("Total Memory in USS:", memUSS)
+#         memRSS = obj.getMemoryRSS()
 #
-#     memRSS = obj.getMemoryRSS()
+#         print("Total Memory in RSS", memRSS)
 #
-#     print("Total Memory in RSS", memRSS)
+#         run = obj.getRuntime()
 #
-#     run = obj.getRuntime()
+#         print("Total ExecutionTime in seconds:", run)
+
 #
-#     print("Total ExecutionTime in seconds:", run)
 #
 #
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -44,40 +47,33 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+from PAMI.frequentPattern.topk import abstract as _ab
 
 
-
-
-# from pyspark import SparkConf, SparkContext
-# import abstract as _ab
-from PAMI.frequentPattern.pyspark import abstract as _ab
-
-
-class parallelECLAT(_ab._frequentPatterns):
+class FAE(_ab._frequentPatterns):
     """
+    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
 
-    :Description: Parallel Eclat is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
-
-    :Reference:
 
+    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
+                  https://ieeexplore.ieee.org/document/4370261
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
+    :param  k: int :
+                    User specified count of top frequent patterns
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-    :param  numPartitions: int :
-                   The number of partitions. On each worker node, an executor process is started and this process performs processing.The processing unit of worker node is partition
+
 
 
     :Attributes:
 
         startTime : float
           To record the start time of the mining process
 
@@ -89,236 +85,349 @@
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
-        lno : int
-                the number of transactions
+        finalPatterns : dict
+            it represents to store the patterns
+
 
-    
     **Methods to execute code on terminal**
-    ----------------------------------------------------
-    
-            Format:
-                      >>> python3 parallelECLAT.py <inputFile> <outputFile> <minSup> <numWorkers>
-    
-            Example:
-                      >>> python3 parallelECLAT.py sampleDB.txt patterns.txt 10.0 3
-    
-            .. note:: minSup will be considered in percentage of database transactions
-    
-    
+    ----------------------------------------
+
+        Format:
+
+           >>> python3 FAE.py <inputFile> <outputFile> <K>
+
+        Examples:
+
+           >>> python3 FAE.py sampleDB.txt patterns.txt 10
+
+
     **Importing this algorithm into a python program**
-    ----------------------------------------------------
+    ---------------------------------------------------------
     .. code-block:: python
-    
-                import PAMI.frequentPattern.pyspark.parallelECLAT as alg
-    
-                obj = alg.parallelECLAT(iFile, minSup, numWorkers)
-    
-                obj.startMine()
-    
-                frequentPatterns = obj.getPatterns()
-    
-                print("Total number of Frequent Patterns:", len(frequentPatterns))
-    
-                obj.savePatterns(oFile)
-    
-                Df = obj.getPatternInDataFrame()
-    
-                memUSS = obj.getMemoryUSS()
-    
-                print("Total Memory in USS:", memUSS)
-    
-                memRSS = obj.getMemoryRSS()
-    
-                print("Total Memory in RSS", memRSS)
-    
-                run = obj.getRuntime()
-    
-                print("Total ExecutionTime in seconds:", run)
-    
-    
-    **Credits:**
-    ----------------------------------------------------
-             The complete program was written by Yudai Masu under the supervision of Professor Rage Uday Kiran.
+
+        import PAMI.frequentPattern.topK.FAE as alg
+
+        obj = alg.FAE(iFile, K)
+
+        obj.startMine()
+
+        topKFrequentPatterns = obj.getPatterns()
+
+        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+
+        obj.save(oFile)
+
+        Df = obj.getPatternInDataFrame()
+
+        memUSS = obj.getMemoryUSS()
+
+        print("Total Memory in USS:", memUSS)
+
+        memRSS = obj.getMemoryRSS()
+
+        print("Total Memory in RSS", memRSS)
+
+        run = obj.getRuntime()
+
+        print("Total ExecutionTime in seconds:", run)
+
+    Credits:
+    --------
+        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _minSup = float()
-    _numPartitions = int()
     _startTime = float()
     _endTime = float()
+    _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
-    _lno = int()
+    _Database = []
+    _tidList = {}
+    _minimum = int()
+
+    def _creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+
+        """
+
+        self._Database = []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            if self._iFile.empty:
+                print("its empty..")
+            i = self._iFile.columns.values.tolist()
+            if 'Transactions' in i:
+                self._Database = self._iFile['Transactions'].tolist()
+
+            # print(self.Database)
+        if isinstance(self._iFile, str):
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(temp)
+            else:
+                try:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(temp)
+                except IOError:
+                    print("File Not Found")
+                    quit()
+
+    def _frequentOneItem(self):
+        """
+        Generating one frequent patterns
+        """
+        candidate = {}
+        self._tidList = {}
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                if j not in candidate:
+                    candidate[j] = 1
+                    self._tidList[j] = [i]
+                else:
+                    candidate[j] += 1
+                    self._tidList[j].append(i)
+        self._finalPatterns = {}
+        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+        for i in plist:
+            if len(self._finalPatterns) >= self._k:
+                break
+            else:
+                self._finalPatterns[i] = candidate[i]
+        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        plist = list(self._finalPatterns.keys())
+        return plist
+
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
+
+            :param prefix: the prefix of a pattern
+            :type prefix: list
+            :param suffix: the suffix of a patterns
+            :type suffix: list
+            :param tidSetI: the timestamp of a patterns
+            :type tidSetI: list
+        """
 
-    def __init__(self, iFile, minSup, numWorkers, sep='\t'):
-        super().__init__(iFile, minSup, int(numWorkers), sep)
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = len(tidSetI)
+        sample = str()
+        for i in prefix:
+            sample = sample + i + "\t"
+        if len(self._finalPatterns) < self._k:
+            if val > self._minimum:
+                self._finalPatterns[sample] = val
+                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                self._minimum = min([i for i in self._finalPatterns.values()])
+        else:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
+                if val > y:
+                    del self._finalPatterns[x]
+                    self._finalPatterns[sample] = val
+                    self._finalPatterns = {k: v for k, v in
+                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
+                                                     reverse=True)}
+                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    return
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+            :param prefix:  main equivalence prefix
+            :type prefix: periodic-frequent item or pattern
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
+            :type itemSets: list
+            :param tidSets: timestamps of the items in the argument itemSets
+            :type tidSets: list
+
+
+                    """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = list(set(tidSetI).intersection(tidSetJ))
+                if len(y) >= self._minimum:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
+
+    def _convert(self, value):
+        """
+        to convert the type of user specified minSup value
+        :param value: user specified minSup value
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = ((len(self._Database)) * value)
+            else:
+                value = int(value)
+        return value
+
+    def startMine(self):
+        """
+            Main function of the program
+
+        """
+        self._startTime = _ab._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._k is None:
+            raise Exception("Please enter the Minimum Support")
+        self._creatingItemSets()
+        self._k = self._convert(self._k)
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i + 1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                if len(y1) >= self._minimum:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
+        self._endTime = _ab._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-        :return: returning USS memory consumed by the mining process
-        :rtype: float
+
+                    :return: returning USS memory consumed by the mining process
+
+                    :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b])
+            data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def savePatterns(self, outFile):
-        """
-        Complete set of frequent patterns will be loaded in to a output file
+    def save(self, outFile):
+        """Complete set of frequent patterns will be loaded in to a output file
+
         :param outFile: name of the output file
+
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
-        """
-        Function to send the set of frequent patterns after completion of the mining process
+        """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
-    def _genPatterns(self, suffix, pattern, data):
-        freqPatterns = {}
-        index = data.index(suffix)
-        for i in range(index + 1, len(data)):
-            tid = pattern[1].intersection(data[i][1])
-            if len(tid) >= self._minSup:
-                freqPattern = pattern[0] + ' ' + data[i][0]
-                freqPatterns[freqPattern] = len(tid)
-                freqPatterns.update(self._genPatterns(data[i], (freqPattern, tid), data))
-        return freqPatterns
-
-    def _convert(self, value):
-        """
-        To convert the user specified minSup value
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        print(value, type(value))
-        if type(value) is int:
-            value = int(value)
-        elif type(value) is float:
-            value = (self._lno * value)
-        elif type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (self._lno * value)
-            else:
-                value = int(value)
-        else:
-            print("None")
-        print(type(value), value)
-        return value
-
-    def startMine(self):
-        """
-        Frequent pattern mining process will start from here
-        """
-
-        self._startTime = _ab._time.time()
-        conf = SparkConf().setAppName("Parallel ECLAT").setMaster("local[*]")
-        sc = SparkContext(conf=conf)
-
-        data = sc.textFile(self._iFile, self._numPartitions) \
-            .map(lambda line: [int(y) for y in line.rstrip().split(self._sep)]).persist()
-        self._lno = data.count()
-        self._minSup = self._convert(self._minSup)
-
-        frequentItems = None
-        if 'transactional' in self._iFile:
-            frequentItems = data.zipWithIndex() \
-                .flatMap(lambda x: [(str(item), x[1]) for item in x[0]]) \
-                .groupByKey() \
-                .filter(lambda x: len(x[1]) >= self._minSup) \
-                .sortBy(lambda x: len(x[1])) \
-                .mapValues(set) \
-                .persist()
-            data.unpersist()
-        elif 'temporal' in self._iFile:
-            frequentItems = data.flatMap(lambda trans: [(str(item), trans[0]) for item in trans[1:]]) \
-                .groupByKey() \
-                .filter(lambda x: len(x[1]) >= self._minSup) \
-                .mapValues(set) \
-                .persist()
-            data.unpersist()
-        else:
-            pass
-            # print("may be not able to process the input file")
-
-        freqItems = dict(frequentItems.collect())
-        # print(len(freqItems))
-        self._finalPatterns = {k: len(v) for k, v in freqItems.items()}
-
-        freqPatterns = list(frequentItems.map(lambda x: self._genPatterns(x, x, list(freqItems.items())))
-                            .filter(lambda x: len(x) != 0).collect())
-        for value in freqPatterns:
-            self._finalPatterns.update(value)
-
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using Parallel ECLAT algorithm")
-        sc.stop()
+    def printTOPK(self):
+        print("Top K Frequent  Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
-        if len(_ab._sys.argv) == 6:
-            _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = parallelECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        _finalPatterns = _ap.getPatterns()
-        print("Total number of Frequent Patterns:", len(_finalPatterns))
-        # _ap.savePatterns(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -52,15 +52,14 @@
 
 
 
 # from pyspark import SparkConf, SparkContext
 from collections import defaultdict
 from PAMI.frequentPattern.pyspark import abstract as _ab
 from operator import add
-from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
 
 
 class Node:
     """
         Attribute
         ---------
             item : int
@@ -207,15 +206,15 @@
     
                     obj.startMine()
     
                     frequentPatterns = obj.getPatterns()
     
                     print("Total number of Frequent Patterns:", len(frequentPatterns))
     
-                    obj.save(oFile)
+                    obj.savePatterns(oFile)
     
                     Df = obj.getPatternInDataFrame()
     
                     memUSS = obj.getMemoryUSS()
     
                     print("Total Memory in USS:", memUSS)
     
@@ -255,16 +254,16 @@
 
 
     def startMine(self):
         """Frequent pattern mining process will start from here"""
 
         self._startTime = _ab._time.time()
 
-        conf = _SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
-        sc = _SparkContext(conf=conf)
+        conf = SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
+        sc = SparkContext(conf=conf)
 
         rdd = sc.textFile(self._iFile, self._numPartitions)\
             .map(lambda x: x.rstrip().split('\t'))\
             .persist()
 
         self._lno = rdd.count()
         self._minSup = self._convert(self._minSup)
@@ -402,15 +401,15 @@
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def save(self, outFile):
+    def savePatterns(self, outFile):
         """
         Complete set of frequent patterns will be loaded in to a output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -428,21 +427,14 @@
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
-        print("Total Memory in USS:", self.getMemoryUSS())
-        print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
-
-
     def _convert(self, value):
         """
         To convert the user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
         if type(value) is int:
@@ -465,15 +457,15 @@
         if len(_ab._sys.argv) == 6:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         _finalPatterns = _ap.getPatterns()
         print("Total number of Frequent Patterns:", len(_finalPatterns))
-        # _ap.save(_ab._sys.argv[2])
+        # _ap.savePatterns(_ab._sys.argv[2])
         _memUSS = _ap.getMemoryUSS()
         print("Total Memory in USS:", _memUSS)
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-
-
-# Top - K is and algorithm to discover top frequent patterns in a transactional database.
-#
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# --------------------------------------------------------
 #
-#         import PAMI.frequentPattern.topK.FAE as alg
 #
-#         obj = alg.FAE(iFile, K)
+#     import PAMI.periodicFrequentPattern.kPFPMiner as alg
 #
-#         obj.startMine()
+#     obj = alg.kPFPMiner(iFile, k)
 #
-#         topKFrequentPatterns = obj.getPatterns()
+#     obj.startMine()
 #
-#         print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+#     periodicFrequentPatterns = obj.getPatterns()
 #
-#         obj.save(oFile)
+#     print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
-#         Df = obj.getPatternInDataFrame()
+#     obj.save(oFile)
 #
-#         memUSS = obj.getMemoryUSS()
+#     Df = obj.getPatternInDataFrame()
 #
-#         print("Total Memory in USS:", memUSS)
+#     memUSS = obj.getMemoryUSS()
 #
-#         memRSS = obj.getMemoryRSS()
+#     print("Total Memory in USS:", memUSS)
 #
-#         print("Total Memory in RSS", memRSS)
-#
-#         run = obj.getRuntime()
-#
-#         print("Total ExecutionTime in seconds:", run)
-
+#     memRSS = obj.getMemoryRSS()
 #
+#     print("Total Memory in RSS", memRSS)
 #
+#     run = obj.getRuntime()
 #
+#     print("Total ExecutionTime in seconds:", run)
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -45,118 +39,143 @@
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from PAMI.frequentPattern.topk import abstract as _ab
-
-
-class FAE(_ab._frequentPatterns):
-    """
-    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
-
-
-    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
-                  https://ieeexplore.ieee.org/document/4370261
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  k: int :
-                    User specified count of top frequent patterns
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-
-    :Attributes:
-
-        startTime : float
-          To record the start time of the mining process
-
-        endTime : float
-          To record the completion time of the mining process
-
-        finalPatterns : dict
-          Storing the complete set of patterns in a dictionary variable
-
-        memoryUSS : float
-          To store the total amount of USS memory consumed by the program
+     Copyright (C)  2021 Rage Uday Kiran
 
-        memoryRSS : float
-          To store the total amount of RSS memory consumed by the program
-
-        finalPatterns : dict
-            it represents to store the patterns
-
-
-    **Methods to execute code on terminal**
-    ----------------------------------------
-
-        Format:
-
-           >>> python3 FAE.py <inputFile> <outputFile> <K>
-
-        Examples:
-
-           >>> python3 FAE.py sampleDB.txt patterns.txt 10
-
-
-    **Importing this algorithm into a python program**
-    ---------------------------------------------------------
-    .. code-block:: python
-
-        import PAMI.frequentPattern.topK.FAE as alg
-
-        obj = alg.FAE(iFile, K)
-
-        obj.startMine()
-
-        topKFrequentPatterns = obj.getPatterns()
-
-        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
-
-        obj.save(oFile)
-
-        Df = obj.getPatternInDataFrame()
-
-        memUSS = obj.getMemoryUSS()
+"""
 
-        print("Total Memory in USS:", memUSS)
 
-        memRSS = obj.getMemoryRSS()
+from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
 
-        print("Total Memory in RSS", memRSS)
 
-        run = obj.getRuntime()
+class kPFPMiner(_ab._periodicFrequentPatterns):
+    """
+        Description:
+        ------------
 
-        print("Total ExecutionTime in seconds:", run)
+            Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
 
-    Credits:
-    --------
-        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+        Reference:
+        -----------
+            Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
+            Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
+            BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
+
+        Attributes:
+        -----------
+            iFile : str
+                Input file name or path of the input file
+            k: int
+                User specified counte of top-k periodic frequent patterns
+            sep : str
+                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+                However, the users can override their default separator.
+            oFile : str
+                Name of the output file or the path of the output file
+            startTime:float
+                To record the start time of the mining process
+            endTime:float
+                To record the completion time of the mining process
+            finalPatterns: dict
+                Storing the complete set of patterns in a dictionary variable
+            memoryUSS : float
+                To store the total amount of USS memory consumed by the program
+            memoryRSS : float
+                To store the total amount of RSS memory consumed by the program
+
+        Methods:
+        ---------
+            startMine()
+                Mining process will start from here
+            getPatterns()
+                Complete set of patterns will be retrieved with this function
+            savePatterns(oFile)
+                Complete set of frequent patterns will be loaded in to a output file
+            getPatternsAsDataFrame()
+                Complete set of frequent patterns will be loaded in to a dataframe
+            getMemoryUSS()
+                Total amount of USS memory consumed by the mining process will be retrieved from this function
+            getMemoryRSS()
+                Total amount of RSS memory consumed by the mining process will be retrieved from this function
+            getRuntime()
+                Total amount of runtime taken by the mining process will be retrieved from this function
+            creatingItemSets()
+                Scans the dataset or dataframes and stores in list format
+            frequentOneItem()
+                Generates one frequent patterns
+            eclatGeneration(candidateList)
+                It will generate the combinations of frequent items
+            generateFrequentPatterns(tidList)
+                It will generate the combinations of frequent items from a list of items
+
+        Executing the code on terminal:
+        -------------------------------
+
+            Format:
+            ------
+            >>> python3 kPFPMiner.py <inputFile> <outputFile> <k>
+
+            Examples:
+            ---------
+            >>> python3 kPFPMiner.py sampleDB.txt patterns.txt 10
+
+
+        Sample run of the importing code:
+        ---------------------------------
+        .. code-block:: python
+
+            import PAMI.periodicFrequentPattern.kPFPMiner as alg
+
+            obj = alg.kPFPMiner(iFile, k)
+
+            obj.startMine()
+
+            periodicFrequentPatterns = obj.getPatterns()
+
+            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+
+            obj.save(oFile)
+
+            Df = obj.getPatternInDataFrame()
+
+            memUSS = obj.getMemoryUSS()
+
+            print("Total Memory in USS:", memUSS)
+
+            memRSS = obj.getMemoryRSS()
+
+            print("Total Memory in RSS", memRSS)
+
+            run = obj.getRuntime()
+
+            print("Total ExecutionTime in seconds:", run)
+
+        Credits:
+        --------
+            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _startTime = float()
     _endTime = float()
     _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _tidList = {}
-    _minimum = int()
+    lno = int()
+    _maximum = int()
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
         """
 
@@ -185,40 +204,63 @@
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
+                    
+    def getPer_Sup(self, tids):
+        tids.sort()
+        cur=0
+        per=list()
+        sup=0
+        #print(tids)
+        for i in range(len(tids)-1):
+            j = i + 1
+            #if tids[j] - cur <= periodicity:
+                #return [0,0]
+            per.append(tids[j] - cur)
+            cur = tids[j]
+        per.append(self.lno - cur)
+        return max(per)
 
     def _frequentOneItem(self):
         """
         Generating one frequent patterns
         """
-        candidate = {}
+        self._mapSupport = {}
         self._tidList = {}
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                if j not in candidate:
-                    candidate[j] = 1
-                    self._tidList[j] = [i]
+        n = 0
+        for line in self._Database:
+            self.lno += 1
+            n = int(line[0])
+            for i in range(1, len(line)):
+                si = line[i]
+                if self._mapSupport.get(si) is None:
+                    self._mapSupport[si] = [1, abs(0 - n), n]
+                    self._tidList[si] = [n]
                 else:
-                    candidate[j] += 1
-                    self._tidList[j].append(i)
-        self._finalPatterns = {}
-        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+                    self._mapSupport[si][0] += 1
+                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
+                    self._mapSupport[si][2] = n
+                    self._tidList[si].append(n)
+        for x, y in self._mapSupport.items():
+            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
+        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in plist:
             if len(self._finalPatterns) >= self._k:
                 break
             else:
-                self._finalPatterns[i] = candidate[i]
-        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+                self._finalPatterns[i] = self._mapSupport[i][1]
+        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
         plist = list(self._finalPatterns.keys())
         return plist
 
+
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
 
             :param prefix: the prefix of a pattern
             :type prefix: list
             :param suffix: the suffix of a patterns
             :type suffix: list
@@ -226,32 +268,32 @@
             :type tidSetI: list
         """
 
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = len(tidSetI)
+        val = self.getPer_Sup(tidSetI)
         sample = str()
         for i in prefix:
-            sample = sample + i + "\t"
+            sample = sample + i + " "
         if len(self._finalPatterns) < self._k:
-            if val > self._minimum:
+            if val < self._maximum:
                 self._finalPatterns[sample] = val
                 self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._minimum = min([i for i in self._finalPatterns.values()])
+                self._maximum = max([i for i in self._finalPatterns.values()])
         else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
-                if val > y:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
+                if val < y:
                     del self._finalPatterns[x]
                     self._finalPatterns[sample] = val
                     self._finalPatterns = {k: v for k, v in
                                               sorted(self._finalPatterns.items(), key=lambda item: item[1],
                                                      reverse=True)}
-                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    self._maximum = max([i for i in self._finalPatterns.values()])
                     return
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
             :param prefix:  main equivalence prefix
             :type prefix: periodic-frequent item or pattern
@@ -276,15 +318,15 @@
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
                 y = list(set(tidSetI).intersection(tidSetJ))
-                if len(y) >= self._minimum:
+                if self.getPer_Sup(y) <= self._maximum:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
             self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def _convert(self, value):
@@ -324,19 +366,19 @@
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i + 1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
                 y1 = list(set(tidSetI).intersection(tidSetJ))
-                if len(y1) >= self._minimum:
+                if self.getPer_Sup(y1) <= self._maximum:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
+        print("kPFPMiner has successfully generated top-k frequent patterns")
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
@@ -377,57 +419,61 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            data.append([a, b])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
         return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
+            patternsAndSupport = x + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printTOPK(self):
-        print("Top K Frequent  Patterns:", len(self.getPatterns()))
+    def printResults(self):
+        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
+        _Patterns = _ap.getPatterns()
+        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.27/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+#     from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 #
 #     obj = alg.FFIMiner("input.txt", 2)
 #
 #     obj.startMine()
 #
-#     fuzzyFrequentPattern = obj.getPatterns()
+#     fuzzyFrequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 #
 #     obj.save("outputFile")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
+from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
@@ -217,23 +217,23 @@
             >>> python3  FFIMiner.py sampleTDB.txt output.txt 6  (minSup will be considered in support count or frequency)
 
 
     Sample run of importing the code:
     ----------------------------------
     .. code-block:: python
 
-        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", 2)
 
         obj.startMine()
 
-        fuzzyFrequentPattern = obj.getPatterns()
+        fuzzyFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
+from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
@@ -203,23 +203,23 @@
                                                       (it will consider '\t' as a separator)
 
             python3  FFIMinerMiner.py sampleTDB.txt output.txt 6 , (it consider ',' as a separator)
 
     Sample run of importing the code:
     -------------------------------
 
-        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", "fuzzyMembership.txt" 2)
 
         obj.startMine()
 
-        fuzzyFrequentPattern = obj.getPatterns()
+        fuzzyFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyFrequentPattenrs(_ABC):
+class _fuzzyPartialPattenrs(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
     Attributes :
     ----------
         iFile : str
```

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
@@ -37,20 +38,20 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyPartialPattenrs(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+class _sequentialPatterns(_ABC):
+    """
+    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
         employ in PAMI
 
-
-    Attributes :
+    Attributes:
     ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
@@ -67,15 +68,15 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods :
+    Methods:
     -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
@@ -83,39 +84,38 @@
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
-
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
+        self._finalPatterns = {}
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
-        self._oFile = str()
-        self._finalPatterns = {}
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -124,15 +124,14 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -149,19 +148,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-
+        pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#         from PAMI.georeferencedFrequentPattern.basic import FSPGrowth as alg
+#         from PAMI.frequentSpatialPattern.basic import FSPGrowth as alg
 #
 #         obj = alg.FSPGrowth("sampleTDB.txt", "sampleN.txt", 5)
 #
 #         obj.startMine()
 #
 #         spatialFrequentPatterns = obj.getPatterns()
 #
@@ -42,15 +42,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.georeferencedFrequentPattern.basic import abstract as _ab
+from PAMI.frequentSpatialPattern.basic import abstract as _ab
 
 
 class _Node:
     """
     A class used to represent the node of frequentPatternTree
     Attributes
     ----------
@@ -291,15 +291,15 @@
 
             >>> python3 FSPGrowth.py sampleTDB.txt output.txt sampleN.txt 0.5 (minSup will be considered in percentage of database transactions)
 
     Sample run of importing the code :
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.georeferencedFrequentPattern.basic import FSPGrowth as alg
+        from PAMI.frequentSpatialPattern.basic import FSPGrowth as alg
 
         obj = alg.FSPGrowth("sampleTDB.txt", "sampleN.txt", 5)
 
         obj.startMine()
 
         spatialFrequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  **Importing this algorithm into a python program**
 #  ---------------------------------------------------
 #
-#     from PAMI.georeferencedFrequentPattern.basic import SpatialECLAT as alg
+#     from PAMI.frequentSpatialPattern.basic import SpatialECLAT as alg
 #
 #     obj = alg.SpatialECLAT("sampleTDB.txt", "sampleN.txt", 5)
 #
 #     obj.startMine()
 #
 #     spatialFrequentPatterns = obj.getPatterns()
 #
@@ -41,15 +41,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.georeferencedFrequentPattern.basic import abstract as _ab
+from PAMI.frequentSpatialPattern.basic import abstract as _ab
 
 
 class SpatialECLAT(_ab._spatialFrequentPatterns):
     """
     Description:
     --------------
         Spatial Eclat is a Extension of ECLAT algorithm,which  stands for Equivalence Class Clustering and bottom-up
@@ -130,15 +130,15 @@
 
             >>> python3 SpatialECLAT.py sampleTDB.txt output.txt sampleN.txt 0.5 (minSup will be considered in percentage of database transactions)
             
     Sample run of importing the code :
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.georeferencedFrequentPattern.basic import SpatialECLAT as alg
+        from PAMI.frequentSpatialPattern.basic import SpatialECLAT as alg
         
         obj = alg.SpatialECLAT("sampleTDB.txt", "sampleN.txt", 5)
 
         obj.startMine()
 
         spatialFrequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,17 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 from collections import OrderedDict as _OrderedDict
 
 
-class _spatialFrequentPatterns(_ABC):
+class _sequentialSpatialPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-
-
     Attributes :
     ----------
         iFile : str
             Input file name or path of the input file
         nFile: str
             Neighbourhoof file name
         minSup: integer or float or str
@@ -68,15 +66,14 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-
     Methods :
     -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
@@ -85,15 +82,14 @@
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
-
     """
 
     def __init__(self, iFile, nFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param nFile: Neighbourhood name of the input
@@ -131,15 +127,14 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -168,8 +163,8 @@
         pass
 
     @_abstractmethod
     def printResults(self):
 
         """ To print the results of execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.27/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,38 +22,39 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-from collections import OrderedDict as _OrderedDict
+import functools as _functools
 
 
-class _sequentialSpatialPatterns(_ABC):
+class _AssociationRules(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-    Attributes :
-    ----------
+
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
-        nFile: str
-            Neighbourhoof file name
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -66,59 +67,56 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-    Methods :
-    -------
+
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
+
     """
 
-    def __init__(self, iFile, nFile, minSup, sep="\t"):
+    def __init__(self, iFile, threshold, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
-        :param nFile: Neighbourhood name of the input
-        :type nFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
-        self._nFile = nFile
-        self._oFile = str()
         self._sep = sep
-        self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._threshold = threshold
         self._finalPatterns = {}
         self._oFile = str()
-
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -127,14 +125,15 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -151,20 +150,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-
-        """ To print the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
+#     from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
 #
 #     ob j =alg.HUFIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -45,15 +45,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.highUtilityFrequentPattern.basic import abstract as _ab
+from PAMI.highUtilityFrequentPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -396,15 +396,15 @@
 
             >>>  python3 HUFIM.py sampleTDB.txt output.txt 35 20 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
+        from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
 
         obj=alg.HUFIM("input.txt", 35, 20)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#         from PAMI.highUtilityPattern.basic import EFIM as alg
+#         from PAMI.highUtilityPatterns.basic import EFIM as alg
 #
 #         obj=alg.EFIM("input.txt",35)
 #
 #         obj.startMine()
 #
 #         Patterns = obj.getPatterns()
 #
@@ -44,15 +44,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -373,15 +373,15 @@
            >>> python3 EFIM sampleTDB.txt output.txt 35  (it will consider "\t" as separator)
            >>> python3 EFIM sampleTDB.txt output.txt 35 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
         
-        from PAMI.highUtilityPattern.basic import EFIM as alg
+        from PAMI.highUtilityPatterns.basic import EFIM as alg
 
         obj=alg.EFIM("input.txt",35)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPattern.basic import HMiner as alg
+#     from PAMI.highUtilityPatterns.basic import HMiner as alg
 #
 #     obj = alg.HMiner("input.txt", 35)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _Element:
     """
     A class represents an Element of a utility list .
     Attributes :
     ----------
@@ -199,15 +199,15 @@
 
             >>> python3 HMiner.py sampleTDB.txt output.txt 35 (separator will be "\t")
 
     Sample run of importing the code:
     --------------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityPattern.basic import HMiner as alg
+        from PAMI.highUtilityPatterns.basic import HMiner as alg
         
         obj = alg.HMiner("input.txt",35)
         
         obj.startMine()
         
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPattern.basic import UPGrowth as alg
+#     from PAMI.highUtilityPatterns.basic import UPGrowth as alg
 #
 #     obj=alg.UPGrowth("input.txt",35)
 #
 #     obj.startMine()
 #
-#     highUtilityPattern = obj.getPatterns()
+#     highUtilityPatterns = obj.getPatterns()
 #
-#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
+#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
 #
 #     obj.save("output")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _UPItem:
     """
     A class to represent the UPItem
 
     Attribute :
@@ -379,23 +379,23 @@
         ------------
           >>> python3 UPGrowth sampleTDB.txt output.txt sampleN.txt 35  (it will consider "\t" as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
     
-        from PAMI.highUtilityPattern.basic import UPGrowth as alg
+        from PAMI.highUtilityPatterns.basic import UPGrowth as alg
 
         obj=alg.UPGrowth("input.txt",35)
 
         obj.startMine()
 
-        highUtilityPattern = obj.getPatterns()
+        highUtilityPatterns = obj.getPatterns()
 
-        print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
+        print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
 
         obj.save("output")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.parallel import abstract as _ab
+from PAMI.highUtilityPatterns.parallel import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.27/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.7.7/PAMI/streams/highUtility/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-
-
-
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 #
-#     obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+#     from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+#
+#     obj = alg.TUFP(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     periodicFrequentPatterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns("patterns")
+#     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getmemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
-#
-
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
@@ -47,44 +43,63 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.periodicFrequentPattern.basic import abstract as _ab
 
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+
+_minSup = float()
+_finalPatterns = {}
+
+
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+
+    ...
+
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
 
-class PFECLAT(_ab._periodicFrequentPatterns):
+
+class TUFP(_ab._frequentPatterns):
     """
     Description:
     -------------
-        EclatPFP is the fundamental approach to mine the periodic-frequent patterns.
+        It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database
+        using CUP-Lists.
 
     Reference:
-    -----------
-        P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
-        periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
+    ----------
+        Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
+        Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
 
     Attributes:
-    -----------
+    ------------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
-        minSup: int or float or str
+        minSup: float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        maxPer: int or float or str
-            The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
@@ -93,324 +108,418 @@
         endTime:float
             To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
         tree : class
-            it represents the Tree class
+            To represents the Tree class
         itemSetCount : int
-            it represents the total no of patterns
+            To represents the total no of patterns
         finalPatterns : dict
-            it represents to store the patterns
-        tidList : dict
-            stores the timestamps of an item
-        hashing : dict
-            stores the patterns with their support to check for the closed property
-
+            To store the complete patterns
     Methods:
     ---------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to a output file
-        getPatternsAsDataFrame()
-            Complete set of periodic-frequent patterns will be loaded in to a dataframe
+        storePatternsInFile(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsInDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingOneItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent 
-        getPeriodAndSupport()
-            Calculates the support and period for a list of timestamps.
-        Generation()
-            Used to implement prefix class equivalence method to generate the periodic patterns recursively
-            
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
+
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>>  python3 PFECLAT.py <inputFile> <outputFile> <minSup>
+                      >>> python3 TUFP.py <inputFile> <outputFile> <minSup>
             Example:
-                      >>>   python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
-
-            .. note:: minSup will be considered in percentage of database transactions
+                      >>>  python3 TUFP.py sampleTDB.txt patterns.txt 0.6
 
+            .. note:: minSup  will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
+            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 
-                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+            obj = alg.TUFP(iFile, minSup)
 
-                obj.startMine()
+            obj.startMine()
 
-                periodicFrequentPatterns = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-                print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                obj.savePatterns("patterns")
+            obj.savePatterns(oFile)
 
-                Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
-                memUSS = obj.getMemoryUSS()
+            memUSS = obj.getmemoryUSS()
 
-                print("Total Memory in USS:", memUSS)
+            print("Total Memory in USS:", memUSS)
 
-                memRSS = obj.getMemoryRSS()
+            memRSS = obj.getMemoryRSS()
 
-                print("Total Memory in RSS", memRSS)
+            print("Total Memory in RSS", memRSS)
 
-                run = obj.getRuntime()
+            run = obj.getRuntime()
 
-                print("Total ExecutionTime in seconds:", run)
+            print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
-             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
+    """
 
-        """
-    
+    _startTime = float()
+    _endTime = float()
+    _minSup = str()
+    _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _dbSize = None
-    _Database = None
-    _minSup = str()
-    _maxPer = str()
-    _tidSet = set()
-    _finalPatterns = {}
-    _startTime = None
-    _endTime = None
     _memoryUSS = float()
     _memoryRSS = float()
+    _Database = []
+    _cupList = {}
+    _topk = {}
+    _minimum = 9999
 
-    def _getPeriodic(self, tids: set):
-        tidList = list(tids)
-        tidList.sort()
-        tidList.append(self._dbSize)
-        cur = 0
-        per = 0
-        for tid in tidList:
-            per = max(per, tid - cur)
-            if per > self._maxPer:  # early stopping
-                break
-            cur = tid
-        return per
-
-    def _convert(self, value):
+    def _creatingItemSets(self):
         """
-        To convert the given user specified value
-
-        :param value: user specified value
-        :return: converted value
+            Scans the dataset
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (self._dbSize * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (self._dbSize * value)
-            else:
-                value = int(value)
-        return value
-
-    def _creatingOneItemSets(self):
-        """Storing the complete transactions of the database/input file in a database variable
-        """
-        plist = []
-        Database = []
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            ts, data = [], []
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'TS' in i:
-                ts = self._iFile['TS'].tolist()
             if 'Transactions' in i:
-                data = self._iFile['Transactions'].tolist()
-            for i in range(len(data)):
-                tr = [ts[i][0]]
-                tr = tr + data[i]
-                Database.append(tr)
+                self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    Database.append(temp)
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-        tid = 0
-        itemsets = {}  # {key: item, value: list of tids}
-        periodicHelper = {}  # {key: item, value: [period, last_tid]}
-        for line in Database:
-            tid = int(line[0])
-            self._tidSet.add(tid)
-            for item in line[1:]:
-                if item in itemsets:
-                    itemsets[item].add(tid)
-                    periodicHelper[item][0] = max(periodicHelper[item][0],
-                                                  abs(tid - periodicHelper[item][1]))  # update current max period
-                    periodicHelper[item][1] = tid  # update the last tid
+
+    def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
+
+                :param self.Database : it represents the one self.Database in database
+
+                :type self.Database : list
+        """
+
+        mapSupport = {}
+        k = 0
+        for i in self._Database:
+            k += 1
+            for j in i:
+                if j.item not in mapSupport:
+                    mapSupport[j.item] = j.probability
+                    self._cupList[j.item] = {k:j.probability}
                 else:
-                    itemsets[item] = {tid}
-                    periodicHelper[item] = [abs(0 - tid), tid]  # initialize helper
+                    mapSupport[j.item] += j.probability
+                    self._cupList[j.item].update({k: j.probability})
+        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        k = 0
+        for x, in plist:
+            k +=1
+            if k >= self._minSup:
+                break
+            self._finalPatterns[x] = mapSupport[x]
+        self._minimum = min(list(self._finalPatterns.values()))
+        return plist
+
+    @staticmethod
+    def _convert(value):
+        """
+        To convert the type of user specified minSup value
+
+            :param value: user specified minSup value
+
+            :return: converted type minSup value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = float(value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+            else:
+                value = int(value)
+        return value
+
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
+
+            :param prefix: the prefix of a pattern
+            :type prefix: list
+            :param suffix: the suffix of a patterns
+            :type suffix: list
+            :param tidSetI: the timestamp of a patterns
+            :type tidSetI: dict
+        """
+
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = sum(tidSetI.values())
+        #print(prefix, val)
+        if len(self._finalPatterns) <= self._minSup:
+            sample = str()
+            for i in prefix:
+                sample = sample + i + " "
+            self._finalPatterns[sample] = val
+        if len(self._finalPatterns) == self._minSup:
+            if val > self._minimum:
+                sample = str()
+                for i in prefix:
+                    sample = sample + i + " "
+                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
+                del self._finalPatterns[index]
+                self._finalPatterns[sample] = val
+                self._minimum = min(list(self._finalPatterns.values()))
+        #print(self.finalPatterns, self.minimum, self.minSup)
+
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+            :param prefix:  main equivalence prefix
+            :type prefix: periodic-frequent item or pattern
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
+            :type itemSets: list
+            :param tidSets: timestamps of the items in the argument itemSets
+            :type tidSets: list
+
+
+                    """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(0, len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i+1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
+                sum2 = sum(list(y.values()))
+                #print(prefix, itemJ, y, sum2)
+                #if sum2 >= self.minimum:
+                self._save(prefix, [itemJ], y)
+                classItemSets.append(itemJ)
+                classTidSets.append(y)
+            #print(itemI, tidSetI, classItemSets)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            #self.save(prefix, list(set(itemSetX)), tidSetI)
 
-        # finish all items' period
-        self._dbSize = len(Database)
-        self._minSup = self._convert(self._minSup)
-        self._maxPer = self._convert(self._maxPer)
-        del Database
-        for item, _ in periodicHelper.items():
-            periodicHelper[item][0] = max(periodicHelper[item][0],
-                                          abs(self._dbSize - periodicHelper[item][1]))  # tid of the last transaction
-        candidates = []
-        for item, tids in itemsets.items():
-            per = periodicHelper[item][0]
-            sup = len(tids)
-            if sup >= self._minSup and per <= self._maxPer:
-                candidates.append(item)
-                self._finalPatterns[item] = [sup, per, tids]
-        return candidates
-    
-    def _generateEclat(self, candidates):
-        newCandidates = []
-        for i in range(0, len(candidates)):
-            prefixItem = candidates[i]
-            prefixItemSet = prefixItem.split()
-            for j in range(i + 1, len(candidates)):
-                item = candidates[j]
-                itemSet = item.split()
-                if prefixItemSet[:-1] == itemSet[:-1] and prefixItemSet[-1] != itemSet[-1]:
-                    _value = self._finalPatterns[item][2].intersection(self._finalPatterns[prefixItem][2])
-                    sup = len(_value)
-                    per = self._getPeriodic(_value)
-                    if sup >= self._minSup and per <= self._maxPer:
-                        newItem = prefixItem + " " + itemSet[-1]
-                        self._finalPatterns[newItem] = [sup, per, _value]
-                        newCandidates.append(newItem)
-
-        if len(newCandidates) > 0:
-            self._generateEclat(newCandidates)
-    
     def startMine(self):
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
+
+
+        """
+        global _minSup
         self._startTime = _ab._time.time()
-        self._finalPatterns = {}
-        frequentSets = self._creatingOneItemSets()
-        self._generateEclat(frequentSets)
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        _minSup = self._minSup
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._cupList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i+1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._cupList[itemJ]
+                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
+                self._save(itemSetX, [itemJ], y1)
+                itemSets.append(itemJ)
+                tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
         self._memoryUSS = float()
+        self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
 
 
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
-        """Storing final periodic-frequent patterns in a dataframe
+        """Storing final frequent patterns in a dataframe
+
+        :return: returning frequent patterns in a dataframe
 
-        :return: returning periodic-frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b[0], b[1]])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
+            data.append([a, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of periodic-frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
+
         :type outFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
-        """ Function to send the set of periodic-frequent patterns after completion of the mining process
+        """ Function to send the set of frequent patterns after completion of the mining process
+
+        :return: returning frequent patterns
 
-        :return: returning periodic-frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
-        print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
-        print("Total Memory in USS:", self.getMemoryUSS())
-        print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
-                    
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
-        if len(_ab._sys.argv) == 6:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
+        _Patterns = _ap.getPatterns()
+        print("Total number of Patterns:", len(_Patterns))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
     else:
+        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
+        ap.startMine()
+        Patterns = ap.getPatterns()
+        print("Total number of Patterns:", len(Patterns))
+        ap.save("patterns.txt")
+        memUSS = ap.getMemoryUSS()
+        print("Total Memory in USS:", memUSS)
+        memRSS = ap.getMemoryRSS()
+        print("Total Memory in RSS", memRSS)
+        run = ap.getRuntime()
+        print("Total ExecutionTime in ms:", run)'''
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,20 @@
             Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-
+        creatingOneItemSets()
+            Scan the database and store the items with their timestamps which are periodic frequent 
+        getPeriodAndSupport()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
             
 
     **Methods to execute code on terminal**
 
             Format:
                         >>>  python3 PFECLAT.py <inputFile> <outputFile> <minSup>
             Example:
@@ -258,14 +263,16 @@
                     return;
                 }
             }
         }
 
     }
     
+    
+    
     ''', 'supportAndPeriod')
 
     def _convert(self, value):
         """
         To convert the given user specified value
 
         :param value: user specified value
```

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     import PAMI.periodicFrequentPattern.kPFPMiner as alg
+#     from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
 #
-#     obj = alg.kPFPMiner(iFile, k)
+#     obj = alg.UVEclat(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     periodicFrequentPatterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getmemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -43,271 +44,351 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
+import operator as _operator
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+
 
-from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
+_minSup = float()
+_finalPatterns = {}
 
 
-class kPFPMiner(_ab._periodicFrequentPatterns):
+class _Item:
     """
-        Description:
-        ------------
+    A class used to represent the item with probability in transaction of dataset
+    ...
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
 
-            Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
 
-        Reference:
-        -----------
-            Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
-            Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
-            BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
-
-        Attributes:
-        -----------
-            iFile : str
-                Input file name or path of the input file
-            k: int
-                User specified counte of top-k periodic frequent patterns
-            sep : str
-                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-                However, the users can override their default separator.
-            oFile : str
-                Name of the output file or the path of the output file
-            startTime:float
-                To record the start time of the mining process
-            endTime:float
-                To record the completion time of the mining process
-            finalPatterns: dict
-                Storing the complete set of patterns in a dictionary variable
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
-
-        Methods:
-        ---------
-            startMine()
-                Mining process will start from here
-            getPatterns()
-                Complete set of patterns will be retrieved with this function
-            savePatterns(oFile)
-                Complete set of frequent patterns will be loaded in to a output file
-            getPatternsAsDataFrame()
-                Complete set of frequent patterns will be loaded in to a dataframe
-            getMemoryUSS()
-                Total amount of USS memory consumed by the mining process will be retrieved from this function
-            getMemoryRSS()
-                Total amount of RSS memory consumed by the mining process will be retrieved from this function
-            getRuntime()
-                Total amount of runtime taken by the mining process will be retrieved from this function
-            creatingItemSets()
-                Scans the dataset or dataframes and stores in list format
-            frequentOneItem()
-                Generates one frequent patterns
-            eclatGeneration(candidateList)
-                It will generate the combinations of frequent items
-            generateFrequentPatterns(tidList)
-                It will generate the combinations of frequent items from a list of items
+class UVEclat(_ab._frequentPatterns):
+    """
+    Description:
+    -------------
+        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
+        using PUF-Tree.
+    Reference:
+    ----------
+    Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
+    SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
+    https://doi.org/10.1145/1982185.1982399
+
+    Attributes:
+    ------------
+        iFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup: float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            To represent the total no of transaction
+        tree : class
+            To represents the Tree class
+        itemSetCount : int
+            To represents the total no of patterns
+        finalPatterns : dict
+            To store the complete patterns
+    Methods:
+    ---------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        storePatternsInFile(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsInDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
+
 
-        Executing the code on terminal:
-        -------------------------------
+    **Methods to execute code on terminal**
 
             Format:
-            ------
-            >>> python3 kPFPMiner.py <inputFile> <outputFile> <k>
+                      >>> python3 uveclat.py <inputFile> <outputFile> <minSup>
+            Example:
+                      >>>  python3 uveclat.py sampleTDB.txt patterns.txt 3
 
-            Examples:
-            ---------
-            >>> python3 kPFPMiner.py sampleDB.txt patterns.txt 10
+            .. note:: minSup  will be considered in support count or frequency
 
+    **Importing this algorithm into a python program**
 
-        Sample run of the importing code:
-        ---------------------------------
-        .. code-block:: python
+    .. code-block:: python
 
-            import PAMI.periodicFrequentPattern.kPFPMiner as alg
+            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+
+            obj = alg.UVEclat(iFile, minSup)
 
-            obj = alg.kPFPMiner(iFile, k)
 
             obj.startMine()
 
-            periodicFrequentPatterns = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
-            Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+            memUSS = obj.getmemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
-        Credits:
-        --------
-            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    **Credits:**
 
-    """
+         The complete program was written by   P.Likhitha    under the supervision of Professor Rage Uday Kiran.
 
+    """
     _startTime = float()
     _endTime = float()
-    _k = int()
+    _minSup = str()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _tidList = {}
-    lno = int()
-    _maximum = int()
+    _rank = {}
 
     def _creatingItemSets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
-
+            Scans the dataset
         """
-
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
 
             # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-                    
-    def getPer_Sup(self, tids):
-        tids.sort()
-        cur=0
-        per=list()
-        sup=0
-        #print(tids)
-        for i in range(len(tids)-1):
-            j = i + 1
-            #if tids[j] - cur <= periodicity:
-                #return [0,0]
-            per.append(tids[j] - cur)
-            cur = tids[j]
-        per.append(self.lno - cur)
-        return max(per)
 
     def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
         """
-        Generating one frequent patterns
-        """
-        self._mapSupport = {}
-        self._tidList = {}
-        n = 0
-        for line in self._Database:
-            self.lno += 1
-            n = int(line[0])
-            for i in range(1, len(line)):
-                si = line[i]
-                if self._mapSupport.get(si) is None:
-                    self._mapSupport[si] = [1, abs(0 - n), n]
-                    self._tidList[si] = [n]
+
+        mapSupport = {}
+        k = 0
+        for i in self._Database:
+            k += 1
+            for j in i:
+                if j.item not in mapSupport:
+                    mapSupport[str(j.item)] = j.probability
+                    self._tidList[str(j.item)] = {k: j.probability}
                 else:
-                    self._mapSupport[si][0] += 1
-                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
-                    self._mapSupport[si][2] = n
-                    self._tidList[si].append(n)
-        for x, y in self._mapSupport.items():
-            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
-        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        for i in plist:
-            if len(self._finalPatterns) >= self._k:
-                break
+                    mapSupport[str(j.item)] += j.probability
+                    self._tidList[str(j.item)].update({k: j.probability})
+        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
+        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
+        return list(plist.keys())
+
+    @staticmethod
+    def _check(i, x):
+        """To check the presence of item or pattern in transaction
+                :param x: it represents the pattern
+                :type x : list
+                :param i : represents the uncertain self.Database
+                :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
+
+    @staticmethod
+    def _convert(value):
+        """
+        To convert the type of user specified minSup value
+            :param value: user specified minSup value
+            :return: converted type minSup value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = float(value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
             else:
-                self._finalPatterns[i] = self._mapSupport[i][1]
-        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        plist = list(self._finalPatterns.keys())
-        return plist
+                value = int(value)
+        return value
+
+    def _removeFalsePositives(self):
+        """
+            To remove the false positive patterns generated in frequent patterns
+            :return: patterns with accurate probability
+        """
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            if y >= self._minSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
+
+    @staticmethod
+    def _Intersection(tidSetx, tidSetY):
+        tids = []
+        support = []
+        tidDict = {}
+        for x, y in tidSetx.items():
+            for x1, y1 in tidSetY.items():
+                if x == x1:
+                    tids.append(x)
+                    support.append(y * y1)
+                    tidDict.update({x: y * y1})
+        return tidDict
 
+    def _calculateExpSup(self, tidList):
+        return sum(tidList.values())
 
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
-
             :param prefix: the prefix of a pattern
             :type prefix: list
             :param suffix: the suffix of a patterns
             :type suffix: list
             :param tidSetI: the timestamp of a patterns
-            :type tidSetI: list
+            :type tidSetI: dict
         """
 
+        global _finalPatterns
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = self.getPer_Sup(tidSetI)
-        sample = str()
-        for i in prefix:
-            sample = sample + i + " "
-        if len(self._finalPatterns) < self._k:
-            if val < self._maximum:
-                self._finalPatterns[sample] = val
-                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._maximum = max([i for i in self._finalPatterns.values()])
-        else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
-                if val < y:
-                    del self._finalPatterns[x]
-                    self._finalPatterns[sample] = val
-                    self._finalPatterns = {k: v for k, v in
-                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
-                                                     reverse=True)}
-                    self._maximum = max([i for i in self._finalPatterns.values()])
-                    return
+        val = self._calculateExpSup(tidSetI)
+        _finalPatterns[tuple(prefix)] = val
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
             :param prefix:  main equivalence prefix
             :type prefix: periodic-frequent item or pattern
             :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
                             and frequent with their timestamps
             :type itemSets: list
             :param tidSets: timestamps of the items in the argument itemSets
             :type tidSets: list
-
-
                     """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
         for i in range(len(itemSets)):
@@ -317,163 +398,126 @@
             tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y) <= self._maximum:
+                y = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y) >= self._minSup:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
             self._save(prefix, list(set(itemSetX)), tidSetI)
 
-    def _convert(self, value):
-        """
-        to convert the type of user specified minSup value
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = ((len(self._Database)) * value)
-            else:
-                value = int(value)
-        return value
-
     def startMine(self):
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
         """
-            Main function of the program
-
-        """
+        global _minSup
         self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._k = self._convert(self._k)
+        self._minSup = self._convert(self._minSup)
+        _minSup = self._minSup
         plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
             tidSetI = self._tidList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
-            for j in range(i + 1, len(plist)):
+            for j in range(i+1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y1) <= self._maximum:
+                y1 = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y1) >= self._minSup:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print("kPFPMiner has successfully generated top-k frequent patterns")
+            self._save(None, itemSetX, tidSetI)
+        self._removeFalsePositives()
+        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
         self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
-                    :return: returning USS memory consumed by the mining process
-
-                    :rtype: float
+        :return: returning USS memory consumed by the mining process
+        :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
-        return dataFrame
+            data.append([a.replace('\t', ' '), b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        return dataframe
 
-    def save(self, outFile):
+    def save(self, oFile):
         """Complete set of frequent patterns will be loaded in to a output file
-
-        :param outFile: name of the output file
-
-        :type outFile: file
+        :param oFile: name of the output file
+        :type oFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = oFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
-
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        _Patterns = _ap.getPatterns()
-        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
+        print("Total number of Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.27/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.relativeFrequentPattern.basic import abstract as _ab
+from PAMI.relativeFrequentPatterns.basic import abstract as _ab
 
 
 class _Node:
     """
         A class used to represent the node of frequentPatterntree
 
     Attributes:
```

### Comparing `pami-2023.7.27/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
+#     from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
 #
 #     obj = alg.RHUIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
@@ -46,15 +46,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.relativeHighUtilityPattern.basic import abstract as _ab
+from PAMI.relativeHighUtilityPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -379,15 +379,15 @@
                       >>>  python3 RHUIM.py sampleTDB.txt output.txt 35 20
 
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
+            from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
 
             obj=alg.RHUIM("input.txt", 35, 20)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _defaultdict
+from collections import defaultdict as _dd
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
+import resource as _resource
+import math as _math
 import sys as _sys
-import validators as _validators
-from urllib.request import urlopen as _urlopen
-import functools as _functools
 
 
-class _sequentialPatterns(_ABC):
-    """
-    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
+class _frequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
-    Attributes:
-    ----------
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -68,54 +66,55 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods:
-    -------
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
+
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._finalPatterns = {}
         self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._finalPatterns = {}
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -124,14 +123,15 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -153,13 +153,7 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
-
-    @_abstractmethod
-    def printResults(self):
-        """ To print result of the execution"""
-
-        pass
```

### Comparing `pami-2023.7.27/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,56 +8,46 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _dd
+from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
-import resource as _resource
-import math as _math
+import validators as _validators
+from urllib.request import urlopen as _urlopen
 import sys as _sys
+import math as _math
 
 
-class _frequentPatterns(_ABC):
+class _correlatedPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-       Attributes:
-       ----------
+    Attributes :
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        minAllConf: float
+            The user given minimum all confidence Ratio(should be in range of 0 to 1)
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -66,16 +56,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+    Methods :
+    -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -85,36 +75,40 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, sep="\t"):
+    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
+        :param minAllConf: The user given minimum all confidence Ratio(should be in range of 0 to 1)
+        :type minAllConf :float
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._oFile = str()
+        self._minAllConf = minAllConf
         self._finalPatterns = {}
+        self._oFile = str()
+        self._memoryRSS = float()
+        self._memoryUSS = float()
         self._startTime = float()
         self._endTime = float()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -148,12 +142,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
+
+    @_abstractmethod
+    def printResults(self):
+        """ To print the results of execution."""
+
+        pass
```

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,18 @@
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
-import itertools as _itertools
 
 
-class _faultTolerantFrequentPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every fault-tolerant frequent pattern mining algorithm must
+class _weightedFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
@@ -63,15 +62,15 @@
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of fault-tolerant frequent patterns
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
        Methods:
        -------
@@ -88,69 +87,66 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, itemSup, minLength, faultTolerance, sep="\t"):
+    def __init__(self, iFile, wFile, minSup, minWeight, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
+        :param wFile: Input file name or path of the input file
+        :type wFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
+        self._wFile = wFile
         self._sep = sep
         self._minSup = minSup
-        self._itemSup = itemSup
-        self._minLength = minLength
-        self._faultTolerance = faultTolerance
+        self._minWeight = minWeight
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
-        """Variable to store USS memory consumed by the program"""
-
-
-
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of fault-tolerant frequent patterns generated will be retrieved from this function"""
+        """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of fault-tolerant frequent patterns will be saved in to an output file from this function
+        """Complete set of frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of fault-tolerant frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
@@ -163,7 +159,14 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
+
+    @_abstractmethod
+    def printResults(self):
+        """ To print all the results of execution"""
+
+
+        pass
```

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+#     from PAMI.weightFrequentPattern.basic import WFIM as alg
 #
-#     obj = alg.TUFP(iFile, minSup)
+#     obj = alg.WFIM(iFile, wFile, minSup, minWeight)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -43,132 +43,280 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
+from PAMI.weightedFrequentPattern.basic import abstract as _fp
 
-from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+_minSup = str()
+_minWeight = int()
+_miniWeight = int()
+_maxWeight = int()
+_weights = {}
+_fp._sys.setrecursionlimit(20000)
 
-_minSup = float()
-_finalPatterns = {}
 
-
-class _Item:
+class _Node:
+    """
+        A class used to represent the node of frequentPatternTree
+    Attributes:
+    ----------
+        itemId: int
+            storing item of a node
+        counter: int
+            To maintain the support of node
+        parent: node
+            To maintain the parent of node
+        children: list
+            To maintain the children of node
+    Methods:
+    -------
+        addChild(node)
+            Updates the nodes children list and parent for the given node
     """
-    A class used to represent the item with probability in transaction of dataset
 
-    ...
+    def __init__(self, item, children):
+        self.itemId = item
+        self.counter = 1
+        self.parent = None
+        self.children = children
 
+    def addChild(self, node):
+        """
+            Retrieving the child from the tree
+            :param node: Children node
+            :type node: Node
+            :return: Updates the children nodes and parent nodes
+        """
+        self.children[node.itemId] = node
+        node.parent = self
+
+
+class _Tree:
+    """
+    A class used to represent the frequentPatternGrowth tree structure
     Attributes:
-    __________
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
+    ----------
+        root : Node
+            The first node of the tree set to Null.
+        summaries : dictionary
+            Stores the nodes itemId which shares same itemId
+        info : dictionary
+            frequency of items in the transactions
+    Methods:
+    -------
+        addTransaction(transaction, freq)
+            adding items of  transactions into the tree as nodes and freq is the count of nodes
+        getFinalConditionalPatterns(node)
+            getting the conditional patterns from fp-tree for a node
+        getConditionalPatterns(patterns, frequencies)
+            sort the patterns by removing the items with lower minSup
+        generatePatterns(prefix)
+            generating the patterns from fp-tree
     """
 
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
+    def __init__(self):
+        self.root = _Node(None, {})
+        self.summaries = {}
+        self.info = {}
+
+    def addTransaction(self, transaction, count):
+        """adding transaction into tree
+        :param transaction: it represents the one transactions in database
+        :type transaction: list
+        :param count: frequency of item
+        :type count: int
+        """
+
+        # This method takes transaction as input and returns the tree
+        currentNode = self.root
+        for i in range(len(transaction)):
+            if transaction[i] not in currentNode.children:
+                newNode = _Node(transaction[i], {})
+                newNode.freq = count
+                currentNode.addChild(newNode)
+                if transaction[i] in self.summaries:
+                    self.summaries[transaction[i]].append(newNode)
+                else:
+                    self.summaries[transaction[i]] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i]]
+                currentNode.freq += count
 
+    def getFinalConditionalPatterns(self, alpha):
+        """
+        generates the conditional patterns for a node
+        Parameters:
+        ----------
+            alpha: node to generate conditional patterns
+        Returns
+        -------
+            returns conditional patterns, frequency of each item in conditional patterns
+        """
+        finalPatterns = []
+        finalFreq = []
+        for i in self.summaries[alpha]:
+            set1 = i.freq
+            set2 = []
+            while i.parent.itemId is not None:
+                set2.append(i.parent.itemId)
+                i = i.parent
+            if len(set2) > 0:
+                set2.reverse()
+                finalPatterns.append(set2)
+                finalFreq.append(set1)
+        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
+        return finalPatterns, finalFreq, info
 
-class TUFP(_ab._frequentPatterns):
+    @staticmethod
+    def getConditionalTransactions(ConditionalPatterns, conditionalFreq):
+        """
+        To calculate the frequency of items in conditional patterns and sorting the patterns
+        Parameters
+        ----------
+        ConditionalPatterns: paths of a node
+        conditionalFreq: frequency of each item in the path
+        Returns
+        -------
+            conditional patterns and frequency of each item in transactions
+        """
+        global _minSup, _miniWeight
+        pat = []
+        freq = []
+        data1 = {}
+        for i in range(len(ConditionalPatterns)):
+            for j in ConditionalPatterns[i]:
+                if j in data1:
+                    data1[j] += conditionalFreq[i]
+                else:
+                    data1[j] = conditionalFreq[i]
+        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+        count = 0
+        for p in ConditionalPatterns:
+            p1 = [v for v in p if v in up_dict]
+            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+            if len(trans) > 0:
+                pat.append(trans)
+                freq.append(conditionalFreq[count])
+            count += 1
+        return pat, freq, up_dict
+
+    def generatePatterns(self, prefix):
+        """
+        To generate the frequent patterns
+        Parameters
+        ----------
+        prefix: an empty list
+        Returns
+        -------
+        Frequent patterns that are extracted from fp-tree
+        """
+        global _miniWeight, _maxWeight, _minWeight, _minSup
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+            pattern = prefix[:]
+            pattern.append(i)
+            yield pattern, self.info[i]
+            patterns, freq, info = self.getFinalConditionalPatterns(i)
+            conditionalTree = _Tree()
+            conditionalTree.info = info.copy()
+            for pat in range(len(patterns)):
+                conditionalTree.addTransaction(patterns[pat], freq[pat])
+            if len(patterns) > 0:
+                for q in conditionalTree.generatePatterns(pattern):
+                    yield q
+
+
+class WFIM(_fp._weightedFrequentPatterns):
     """
     Description:
     -------------
-        It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database
-        using CUP-Lists.
-
-    Reference:
-    ----------
-        Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
-        Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
-
-    Attributes:
+       WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
+       It stores the database in compressed fp-tree decreasing the memory usage and extracts the
+       patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+    Reference :
+    -----------
+           U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
+           in Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
+           https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+    Attributes :
     ------------
         iFile : file
-            Name of the Input file or path of the input file
-        oFile : file
-            Name of the output file or path of the output file
+            Input file name or path of the input file
         minSup: float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        minWeight: float or int or str
+            The user can specify minWeight either in count or proportion of database size.
+            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
+        oFile : file
+            Name of the output file or the path of the output file
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            To represent the total no of transaction
+            it represents the total no of transactions
         tree : class
-            To represents the Tree class
-        itemSetCount : int
-            To represents the total no of patterns
+            it represents the Tree class
         finalPatterns : dict
-            To store the complete patterns
-    Methods:
+            it represents to store the patterns
+    Methods :
     ---------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        storePatternsInFile(oFile)
+        save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
-        getPatternsInDataFrame()
+        getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
+        creatingItemSets()
+            Scans the dataset or dataframes and stores in list format
         frequentOneItem()
-            Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
-
-
-    **Methods to execute code on terminal**
+            Extracts the one-frequent patterns from transactions
+    Methods to execute code on terminal
+    ------------------------------------
+        Format:
+                  >>>  python3 WFIM.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
+        Example:
+                  >>>  python3 WFIM.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
 
-            Format:
-                      >>> python3 TUFP.py <inputFile> <outputFile> <minSup>
-            Example:
-                      >>>  python3 TUFP.py sampleTDB.txt patterns.txt 0.6
-
-            .. note:: minSup  will be considered in support count or frequency
+                 .. note:: minSup and maxPer will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
-
+    --------------------------------------------------
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+            from PAMI.weightFrequentPattern.basic import WFIM as alg
 
-            obj = alg.TUFP(iFile, minSup)
+            obj = alg.WFIM(iFile, wFile, minSup, minWeight)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -186,340 +334,310 @@
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
-             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
-    """
+  """
 
-    _startTime = float()
-    _endTime = float()
+    __startTime = float()
+    __endTime = float()
     _minSup = str()
-    _finalPatterns = {}
+    __finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _Database = []
-    _cupList = {}
-    _topk = {}
-    _minimum = 9999
-
-    def _creatingItemSets(self):
-        """
-            Scans the dataset
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __mapSupport = {}
+    __lno = 0
+    __tree = _Tree()
+    __rank = {}
+    __rankDup = {}
+
+    def __init__(self, iFile, wFile, minSup, minWeight, sep='\t'):
+        super().__init__(iFile, wFile, minSup, minWeight, sep)
+
+    def __creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+        """
+        self.__Database = []
+        if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
+                self.__Database = self._iFile['Transactions'].tolist()
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
+            if _fp._validators.url(self._iFile):
+                data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    tr = []
-                    for i in temp:
-                        i1 = i.index('(')
-                        i2 = i.index(')')
-                        item = i[0:i1]
-                        probability = float(i[i1 + 1:i2])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(temp)
+                    self.__Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            tr = []
-                            for i in temp:
-                                i1 = i.index('(')
-                                i2 = i.index(')')
-                                item = i[0:i1]
-                                probability = float(i[i1 + 1:i2])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
+                            # print(len(temp))
+                            self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
-        """takes the self.Database and calculates the support of each item in the dataset and assign the
-            ranks to the items by decreasing support and returns the frequent items list
-
-                :param self.Database : it represents the one self.Database in database
-
-                :type self.Database : list
-        """
-
-        mapSupport = {}
-        k = 0
-        for i in self._Database:
-            k += 1
-            for j in i:
-                if j.item not in mapSupport:
-                    mapSupport[j.item] = j.probability
-                    self._cupList[j.item] = {k:j.probability}
-                else:
-                    mapSupport[j.item] += j.probability
-                    self._cupList[j.item].update({k: j.probability})
-        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        k = 0
-        for x, in plist:
-            k +=1
-            if k >= self._minSup:
-                break
-            self._finalPatterns[x] = mapSupport[x]
-        self._minimum = min(list(self._finalPatterns.values()))
-        return plist
-
-    @staticmethod
-    def _convert(value):
+    def _scanningWeights(self):
+        """
+            Storing the weights of the variables in input file in a weights variable
         """
-        To convert the type of user specified minSup value
+        global _weights
+        _weights = {}
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            items, weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                items = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for i in range(len(weights)):
+                _weights[items[i]] = weights[i]
 
-            :param value: user specified minSup value
+            # print(self.Database)
+        if isinstance(self._wFile, str):
+            if _fp._validators.url(self._wFile):
+                data = _fp._urlopen(self._wFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    _weights[temp[0]] = temp[1]
+            else:
+                try:
+                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            s = int(float(temp[1]))
+                            _weights[temp[0]] = s
+                except IOError:
+                    print("File Not Found")
+                    quit()
 
-            :return: converted type minSup value
+    def __convert(self, value):
+        """
+        to convert the type of user specified minSup value
+        :param value: user specified minSup value
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = float(value)
+            value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
+                value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _save(self, prefix, suffix, tidSetI):
-        """Saves the patterns that satisfy the periodic frequent property.
+    def __frequentOneItem(self):
+        """
+        Generating One frequent items sets
+        """
+        global _maxWeight
+        self.__mapSupport = {}
+        for tr in self.__Database:
+            for i in range(0, len(tr)):
+                if tr[i] not in self.__mapSupport:
+                    self.__mapSupport[tr[i]] = 1
+                else:
+                    self.__mapSupport[tr[i]] += 1
+        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
+        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        return genList
+
+    def __updateTransactions(self, itemSet):
+        """
+        Updates the items in transactions with rank of items according to their support
+        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
+                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+        Parameters
+        ----------
+        itemSet: list of one-frequent items
+        -------
+        """
+        list1 = []
+        for tr in self.__Database:
+            list2 = []
+            for i in range(len(tr)):
+                if tr[i] in itemSet:
+                    list2.append(self.__rank[tr[i]])
+            if len(list2) >= 1:
+                list2.sort()
+                list1.append(list2)
+        return list1
 
-            :param prefix: the prefix of a pattern
-            :type prefix: list
-            :param suffix: the suffix of a patterns
-            :type suffix: list
-            :param tidSetI: the timestamp of a patterns
-            :type tidSetI: dict
-        """
-
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = sum(tidSetI.values())
-        #print(prefix, val)
-        if len(self._finalPatterns) <= self._minSup:
-            sample = str()
-            for i in prefix:
-                sample = sample + i + " "
-            self._finalPatterns[sample] = val
-        if len(self._finalPatterns) == self._minSup:
-            if val > self._minimum:
-                sample = str()
-                for i in prefix:
-                    sample = sample + i + " "
-                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
-                del self._finalPatterns[index]
-                self._finalPatterns[sample] = val
-                self._minimum = min(list(self._finalPatterns.values()))
-        #print(self.finalPatterns, self.minimum, self.minSup)
-
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
-            :param prefix:  main equivalence prefix
-            :type prefix: periodic-frequent item or pattern
-            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
-                            and frequent with their timestamps
-            :type itemSets: list
-            :param tidSets: timestamps of the items in the argument itemSets
-            :type tidSets: list
-
-
-                    """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(0, len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i+1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
-                sum2 = sum(list(y.values()))
-                #print(prefix, itemJ, y, sum2)
-                #if sum2 >= self.minimum:
-                self._save(prefix, [itemJ], y)
-                classItemSets.append(itemJ)
-                classTidSets.append(y)
-            #print(itemI, tidSetI, classItemSets)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            #self.save(prefix, list(set(itemSetX)), tidSetI)
+    @staticmethod
+    def __buildTree(transactions, info):
+        """
+        Builds the tree with updated transactions
+        Parameters:
+        ----------
+            transactions: updated transactions
+            info: support details of each item in transactions
+        Returns:
+        -------
+            transactions compressed in fp-tree
+        """
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(transactions)):
+            rootNode.addTransaction(transactions[i], 1)
+        return rootNode
+
+    def __savePeriodic(self, itemSet):
+        """
+        The duplication items and their ranks
+        Parameters:
+        ----------
+            itemSet: frequent itemSet that generated
+        Returns:
+        -------
+            patterns with original item names.
+        """
+        temp = str()
+        for i in itemSet:
+            temp = temp + self.__rankDup[i] + "\t"
+        return temp
 
     def startMine(self):
-        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
-            by counting the original support of a patterns
-
-
         """
-        global _minSup
-        self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
+            main program to start the operation
+        """
+        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
+        self.__startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self.__creatingItemSets()
+        self._scanningWeights()
+        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
+        _maxWeight = max([s for s in _weights.values()])
+        _miniWeight = min([s for s in _weights.values()])
+        self._minSup = self.__convert(self._minSup)
         _minSup = self._minSup
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._cupList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i+1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._cupList[itemJ]
-                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
-                self._save(itemSetX, [itemJ], y1)
-                itemSets.append(itemJ)
-                tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        itemSet = self.__frequentOneItem()
+        updatedTransactions = self.__updateTransactions(itemSet)
+        for x, y in self.__rank.items():
+            self.__rankDup[y] = x
+        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
+        __Tree = self.__buildTree(updatedTransactions, info)
+        patterns = __Tree.generatePatterns([])
+        self.__finalPatterns = {}
+        for k in patterns:
+            s = self.__savePeriodic(k[0])
+            self.__finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent patterns were generated successfully using WFIM algorithm")
+        self.__endTime = _fp._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
-        return self._memoryUSS
+        return self.__memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.__memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
-        return self._endTime - self._startTime
+        return self.__endTime - self.__startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
-            data.append([a, b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        for a, b in self.__finalPatterns.items():
+            data.append([a.replace('\t', ' '), b])
+            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
-
         :param outFile: name of the output file
-
         :type outFile: file
         """
-        self.oFile = outFile
-        writer = open(self.oFile, 'w+')
-        for x, y in self._finalPatterns.items():
-            s1 = x + ":" + str(y)
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self.__finalPatterns.items():
+            s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
-
         :rtype: dict
         """
-        return self._finalPatterns
+        return self.__finalPatterns
+
+    def printResults(self):
+        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
+
+        
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
+        if len(_fp._sys.argv) == 7:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 6:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        _Patterns = _ap.getPatterns()
-        print("Total number of Patterns:", len(_Patterns))
-        _ap.save(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_fp._sys.argv[2])
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
-        ap.startMine()
-        Patterns = ap.getPatterns()
-        print("Total number of Patterns:", len(Patterns))
-        ap.save("patterns.txt")
-        memUSS = ap.getMemoryUSS()
-        print("Total Memory in USS:", memUSS)
-        memRSS = ap.getMemoryRSS()
-        print("Total Memory in RSS", memRSS)
-        run = ap.getRuntime()
-        print("Total ExecutionTime in ms:", run)'''
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.uncertainGeoreferenceFrequentPattern.basic import GFPGrowth as alg
+#     from PAMI.geoReferenceFrequentPattern.basic import GFPGrowth as alg
 #
 #     obj = alg.GFPGrowth(iFile, nFile, minSup)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -45,15 +45,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 # from geoReferencedFrequentPatterns import abstract as _ab
-from PAMI.uncertainGeoreferencedFrequentPattern.basic import abstract as _ab
+from PAMI.geoReferencedFrequentPaterns import abstract as _ab
 # import abstract as _ab
 
 _minSup = str()
 _neighbourList = {}
 _ab._sys.setrecursionlimit(20000)
 _finalPatterns = {}
 
@@ -296,22 +296,18 @@
             self.removeNode(i)
 
 
 class GFPGrowth(_ab._frequentPatterns):
     """
     Description:
     ------------
-        GFPGrowth algorithm is used to discover geo-referenced frequent patterns in a uncertain transactional database
+        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
         using GFP-Tree.
     Reference:
     -----------
-         Palla Likhitha,Pamalla Veena, Rage, Uday Kiran, Koji Zettsu (2023).
-         "Discovering Geo-referenced Frequent Patterns in Uncertain Geo-referenced
-         Transactional Databases".  PAKDD 2023.
-         https://doi.org/10.1007/978-3-031-33380-4_3
         
     Attributes:
     ----------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
@@ -380,15 +376,15 @@
         ------------
           >>> python3 GFPGrowth.py sampleTDB.txt sampleNeighbor.txt patterns.txt 3    (minSup  will be considered in support count or frequency)
     
     Sample run of importing the code:
     -----------------------------------
      .. code-block:: python
 
-        from PAMI.uncertainGeoreferencedFrequentPattern.basic import GFPGrowth as alg
+        from PAMI.geoReferenceFrequentPattern.basic import GFPGrowth as alg
 
         obj = alg.GFPGrowth(iFile, nFile, minSup)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.27/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,7 +132,9 @@
         pass
       
     @_abstractmethod
     def printResults(self):
         """To print all the statistics"""
 
         pass
+
+
```

### Comparing `pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.weightFrequentPattern.basic import WFIM as alg
+#     from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 #
-#     obj = alg.WFIM(iFile, wFile, minSup, minWeight)
+#     obj = alg.WFRIMiner(iFile, WS, regularity)
 #
 #     obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#     weightedFrequentRegularPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 #
 #     obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternInDataFrame()
 #
-#     memUSS = obj.getmemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -43,71 +44,84 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.weightedFrequentPattern.basic import abstract as _fp
+from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
 
-_minSup = str()
-_minWeight = int()
-_miniWeight = int()
-_maxWeight = int()
+_WS = str()
+_regularity = str()
+_lno = int()
 _weights = {}
+_wf = {}
 _fp._sys.setrecursionlimit(20000)
 
 
 class _Node:
     """
         A class used to represent the node of frequentPatternTree
+
     Attributes:
     ----------
         itemId: int
             storing item of a node
         counter: int
             To maintain the support of node
         parent: node
             To maintain the parent of node
         children: list
             To maintain the children of node
+
     Methods:
     -------
+
         addChild(node)
             Updates the nodes children list and parent for the given node
+
     """
 
     def __init__(self, item, children):
-        self.itemId = item
-        self.counter = 1
-        self.parent = None
+        """ Initializing the Node class
+
+        :param item: Storing the item of a node
+        :type item: int or None
+        :param children: To maintain the children of a node
+        :type children: dict
+        """
+
+        self.item = item
         self.children = children
+        self.parent = None
+        self.timeStamps = []
 
     def addChild(self, node):
+        """ To add the children to a node
+
+            :param node: parent node in the tree
         """
-            Retrieving the child from the tree
-            :param node: Children node
-            :type node: Node
-            :return: Updates the children nodes and parent nodes
-        """
-        self.children[node.itemId] = node
+
+        self.children[node.item] = node
         node.parent = self
 
 
 class _Tree:
     """
     A class used to represent the frequentPatternGrowth tree structure
+
     Attributes:
     ----------
         root : Node
             The first node of the tree set to Null.
         summaries : dictionary
             Stores the nodes itemId which shares same itemId
         info : dictionary
             frequency of items in the transactions
+
     Methods:
     -------
         addTransaction(transaction, freq)
             adding items of  transactions into the tree as nodes and freq is the count of nodes
         getFinalConditionalPatterns(node)
             getting the conditional patterns from fp-tree for a node
         getConditionalPatterns(patterns, frequencies)
@@ -117,147 +131,211 @@
     """
 
     def __init__(self):
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction, count):
-        """adding transaction into tree
-        :param transaction: it represents the one transactions in database
-        :type transaction: list
-        :param count: frequency of item
-        :type count: int
+    def addTransaction(self, transaction, tid):
+        """     Adding a transaction into tree
+
+                :param transaction: To represent the complete database
+                :type transaction: list
+                :param tid: To represent the timestamp of a database
+                :type tid: list
+                :return: pfp-growth tree
         """
 
-        # This method takes transaction as input and returns the tree
         currentNode = self.root
         for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
-                newNode.freq = count
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-                currentNode.freq += count
+        currentNode.timeStamps = currentNode.timeStamps + tid
 
-    def getFinalConditionalPatterns(self, alpha):
-        """
-        generates the conditional patterns for a node
-        Parameters:
-        ----------
-            alpha: node to generate conditional patterns
-        Returns
-        -------
-            returns conditional patterns, frequency of each item in conditional patterns
+    def getConditionalPatterns(self, alpha, pattern):
+        """Generates all the conditional patterns of a respective node
+
+            :param alpha: To represent a Node in the tree
+            :type alpha: Node
+            :param pattern: prefix of the pattern
+            :type alpha: list
+            :return: A tuple consisting of finalPatterns, conditional pattern base and information
         """
         finalPatterns = []
-        finalFreq = []
+        finalSets = []
         for i in self.summaries[alpha]:
-            set1 = i.freq
+            set1 = i.timeStamps
             set2 = []
-            while i.parent.itemId is not None:
-                set2.append(i.parent.itemId)
+            while i.parent.item is not None:
+                set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalFreq.append(set1)
-        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
-        return finalPatterns, finalFreq, info
+                finalSets.append(set1)
+        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
+        return finalPatterns, finalSets, info
 
     @staticmethod
-    def getConditionalTransactions(ConditionalPatterns, conditionalFreq):
+    def generateTimeStamps(node):
+        """To get the timestamps of a node
+
+        :param node: A node in the tree
+        :return: Timestamps of a node
         """
-        To calculate the frequency of items in conditional patterns and sorting the patterns
-        Parameters
-        ----------
-        ConditionalPatterns: paths of a node
-        conditionalFreq: frequency of each item in the path
-        Returns
-        -------
-            conditional patterns and frequency of each item in transactions
+
+        finalTimeStamps = node.timeStamps
+        return finalTimeStamps
+
+    def removeNode(self, nodeValue):
+        """ Removing the node from tree
+
+            :param nodeValue: To represent a node in the tree
+            :type nodeValue: node
+            :return: Tree with their nodes updated with timestamps
+        """
+
+        for i in self.summaries[nodeValue]:
+            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
+            del i.parent.children[nodeValue]
+
+    def getTimeStamps(self, alpha):
+        """ To get all the timestamps of the nodes which share same item name
+
+            :param alpha: Node in a tree
+            :return: Timestamps of a  node
+        """
+        temporary = []
+        for i in self.summaries[alpha]:
+            temporary += i.timeStamps
+        return temporary
+
+    @staticmethod
+    def getSupportAndPeriod(timeStamps, pattern):
+        """To calculate the periodicity and support
+
+        :param timeStamps: Timestamps of an item set
+        :type timeStamps: list
+        :param pattern: pattern to evaluate the weighted frequent regular or not
+        :type pattern: list
+        :return: support, periodicity
+        """
+
+        global _WS, _regularity, _lno, _weights
+        timeStamps.sort()
+        cur = 0
+        per = list()
+        sup = 0
+        for j in range(len(timeStamps)):
+            per.append(timeStamps[j] - cur)
+            cur = timeStamps[j]
+            sup += 1
+        per.append(_lno - cur)
+        l = int()
+        for i in pattern:
+            l = l + _weights[i]
+        wf = (l / (len(pattern))) * sup
+        if len(per) == 0:
+            return [0, 0]
+        return [sup, max(per), wf]
+
+    def conditionalDatabases(self, conditionalPatterns, conditionalTimeStamps, pattern):
+        """ It generates the conditional patterns with periodic-frequent items
+
+            :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
+            :type conditionalPatterns: list
+            :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
+            :type conditionalTimeStamps: list
+            :param pattern: prefix of the pattern
+            :type pattern: list
+            :returns: Returns conditional transactions by removing non-periodic and non-frequent items
         """
-        global _minSup, _miniWeight
+
+        global _WS, _regularity
         pat = []
-        freq = []
+        timeStamps = []
         data1 = {}
-        for i in range(len(ConditionalPatterns)):
-            for j in ConditionalPatterns[i]:
+        for i in range(len(conditionalPatterns)):
+            for j in conditionalPatterns[i]:
                 if j in data1:
-                    data1[j] += conditionalFreq[i]
+                    data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
-                    data1[j] = conditionalFreq[i]
-        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+                    data1[j] = conditionalTimeStamps[i]
+        updatedDictionary = {}
+        for m in data1:
+            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
         count = 0
-        for p in ConditionalPatterns:
-            p1 = [v for v in p if v in up_dict]
-            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+        for p in conditionalPatterns:
+            p1 = [v for v in p if v in updatedDictionary]
+            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                freq.append(conditionalFreq[count])
+                timeStamps.append(conditionalTimeStamps[count])
             count += 1
-        return pat, freq, up_dict
+        return pat, timeStamps, updatedDictionary
 
     def generatePatterns(self, prefix):
+        """ Generates the patterns
+
+            :param prefix: Forms the combination of items
+            :type prefix: list
+            :returns: yields patterns with their support and periodicity
         """
-        To generate the frequent patterns
-        Parameters
-        ----------
-        prefix: an empty list
-        Returns
-        -------
-        Frequent patterns that are extracted from fp-tree
-        """
-        global _miniWeight, _maxWeight, _minWeight, _minSup
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+        global _WS
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
             pattern = prefix[:]
             pattern.append(i)
-            yield pattern, self.info[i]
-            patterns, freq, info = self.getFinalConditionalPatterns(i)
-            conditionalTree = _Tree()
-            conditionalTree.info = info.copy()
-            for pat in range(len(patterns)):
-                conditionalTree.addTransaction(patterns[pat], freq[pat])
-            if len(patterns) > 0:
-                for q in conditionalTree.generatePatterns(pattern):
-                    yield q
+            if self.info[i][2] >= _WS:
+                yield pattern, self.info[i]
+                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+                conditionalTree = _Tree()
+                conditionalTree.info = info.copy()
+                for pat in range(len(patterns)):
+                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                if len(patterns) > 0:
+                    for q in conditionalTree.generatePatterns(pattern):
+                        yield q
+            self.removeNode(i)
 
 
-class WFIM(_fp._weightedFrequentPatterns):
+class WFRIMiner(_fp._weightedFrequentRegularPatterns):
     """
-    Description:
-    -------------
-       WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
-       It stores the database in compressed fp-tree decreasing the memory usage and extracts the
+       WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
+       It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the
        patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+
     Reference :
-    -----------
-           U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
-           in Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
-           https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+    ---------
+           K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
+           2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
+           doi: 10.1109/KST.2017.7886090.
+
     Attributes :
-    ------------
+    ----------
         iFile : file
             Input file name or path of the input file
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        WS: float or int or str
+            The user can specify WS either in count or proportion of database size.
+            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        minWeight: float or int or str
-            The user can specify minWeight either in count or proportion of database size.
-            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
+        regularity: float or int or str
+            The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
         oFile : file
             Name of the output file or the path of the output file
         startTime:float
             To record the start time of the mining process
@@ -273,16 +351,17 @@
             To maintain the information of item and their frequency
         lno : int
             it represents the total no of transactions
         tree : class
             it represents the Tree class
         finalPatterns : dict
             it represents to store the patterns
+
     Methods :
-    ---------
+    -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -293,42 +372,44 @@
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets()
             Scans the dataset or dataframes and stores in list format
         frequentOneItem()
             Extracts the one-frequent patterns from transactions
-    Methods to execute code on terminal
-    ------------------------------------
-        Format:
-                  >>>  python3 WFIM.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
-        Example:
-                  >>>  python3 WFIM.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
 
-                 .. note:: minSup and maxPer will be considered in support count or frequency
+
+    **Methods to execute code on terminal**
+
+            Format:
+                      >>> python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
+            Example:
+                      >>>  python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
+
+                     .. note:: WS & regularity will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
-    --------------------------------------------------
+
     .. code-block:: python
 
-            from PAMI.weightFrequentPattern.basic import WFIM as alg
+            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 
-            obj = alg.WFIM(iFile, wFile, minSup, minWeight)
+            obj = alg.WFRIMiner(iFile, WS, regularity)
 
             obj.startMine()
 
-            frequentPatterns = obj.getPatterns()
+            weightedFrequentRegularPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 
             obj.savePatterns(oFile)
 
-            Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getmemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
@@ -336,308 +417,349 @@
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
              The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
-  """
+        """
 
-    __startTime = float()
-    __endTime = float()
-    _minSup = str()
-    __finalPatterns = {}
+    _startTime = float()
+    _endTime = float()
+    _WS = str()
+    _regularity = str()
+    _weight = {}
+    _finalPatterns = {}
+    _wFile = " "
     _iFile = " "
     _oFile = " "
     _sep = " "
-    __memoryUSS = float()
-    __memoryRSS = float()
-    __Database = []
-    __mapSupport = {}
-    __lno = 0
-    __tree = _Tree()
-    __rank = {}
-    __rankDup = {}
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _mapSupport = {}
+    _lno = 0
+    _tree = _Tree()
+    _rank = {}
+    _rankDup = {}
 
-    def __init__(self, iFile, wFile, minSup, minWeight, sep='\t'):
-        super().__init__(iFile, wFile, minSup, minWeight, sep)
+    def __init__(self, iFile, _wFile, WS, regularity, sep='\t'):
+        super().__init__(iFile, _wFile, WS, regularity, sep)
 
-    def __creatingItemSets(self):
+    def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
+
+
         """
-        self.__Database = []
+        self._Database = []
+        self._weight = {}
         if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self.__Database = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
+
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            _items, _weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                _items = self._wFile['items'].tolist()
+            if 'weight' in i:
+                _weights = self._wFile['weight'].tolist()
+            for i in range(len(_items)):
+                self._weight[_items[i]] = _weights[i]
 
             # print(self.Database)
         if isinstance(self._iFile, str):
             if _fp._validators.url(self._iFile):
                 data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self.__Database.append(temp)
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            # print(len(temp))
-                            self.__Database.append(temp)
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _scanningWeights(self):
-        """
-            Storing the weights of the variables in input file in a weights variable
-        """
-        global _weights
-        _weights = {}
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            items, weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                items = self._wFile['items'].tolist()
-            if 'weights' in i:
-                weights = self._wFile['weights'].tolist()
-            for i in range(len(weights)):
-                _weights[items[i]] = weights[i]
-
-            # print(self.Database)
         if isinstance(self._wFile, str):
             if _fp._validators.url(self._wFile):
                 data = _fp._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    _weights[temp[0]] = temp[1]
+                    self._weight[temp[0]] = float(temp[1])
             else:
                 try:
                     with open(self._wFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            s = int(float(temp[1]))
-                            _weights[temp[0]] = s
+                            self._weight[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def __convert(self, value):
+    def _convert(self, value):
         """
         to convert the type of user specified minSup value
+
         :param value: user specified minSup value
+
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self.__Database) * value)
+            value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self.__Database) * value)
+                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def __frequentOneItem(self):
+    def _frequentOneItem(self):
         """
         Generating One frequent items sets
+
         """
-        global _maxWeight
-        self.__mapSupport = {}
-        for tr in self.__Database:
-            for i in range(0, len(tr)):
-                if tr[i] not in self.__mapSupport:
-                    self.__mapSupport[tr[i]] = 1
+        global _lno, _wf, _weights
+        self._mapSupport = {}
+        _owf = {}
+        for tr in self._Database:
+            for i in range(1, len(tr)):
+                if tr[i] not in self._mapSupport:
+                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
                 else:
-                    self.__mapSupport[tr[i]] += 1
-        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
-        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
+                    self._mapSupport[tr[i]][1] = int(tr[0])
+                    self._mapSupport[tr[i]][2] += 1
+        for key in self._mapSupport:
+            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
+        _lno = len(self._Database)
+        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
+        for x, y in self._mapSupport.items():
+            if self._weight.get(x) is None:
+                self._weight[x] = 0
+        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
+        for x, y in self._mapSupport.items():
+            _owf[x] = y[0] * gmax
+        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
+        for x, y in self._mapSupport.items():
+            temp = self._weight[x] * y[0]
+            _wf[x] = temp
+            self._mapSupport[x].append(temp)
+        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
+        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        for x, y in self._rank.items():
+            _weights[y] = self._weight[x]
         return genList
 
-    def __updateTransactions(self, itemSet):
+    def _updateTransactions(self, itemSet):
         """
         Updates the items in transactions with rank of items according to their support
+
         :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
                     rank = {'a':0, 'b':1, 'c':2, 'd':3}
+
         Parameters
         ----------
         itemSet: list of one-frequent items
+
         -------
+
         """
         list1 = []
-        for tr in self.__Database:
-            list2 = []
-            for i in range(len(tr)):
+        for tr in self._Database:
+            list2 = [int(tr[0])]
+            for i in range(1, len(tr)):
                 if tr[i] in itemSet:
-                    list2.append(self.__rank[tr[i]])
-            if len(list2) >= 1:
-                list2.sort()
+                    list2.append(self._rank[tr[i]])
+            if len(list2) >= 2:
+                basket = list2[1:]
+                basket.sort()
+                list2[1:] = basket[0:]
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def __buildTree(transactions, info):
+    def _buildTree(transactions, info):
         """
         Builds the tree with updated transactions
         Parameters:
         ----------
             transactions: updated transactions
             info: support details of each item in transactions
+
         Returns:
         -------
             transactions compressed in fp-tree
+
         """
         rootNode = _Tree()
         rootNode.info = info.copy()
         for i in range(len(transactions)):
-            rootNode.addTransaction(transactions[i], 1)
+            set1 = [transactions[i][0]]
+            rootNode.addTransaction(transactions[i][1:], set1)
         return rootNode
 
-    def __savePeriodic(self, itemSet):
+    def _savePeriodic(self, itemSet):
         """
         The duplication items and their ranks
         Parameters:
         ----------
             itemSet: frequent itemSet that generated
+
         Returns:
         -------
             patterns with original item names.
+
         """
         temp = str()
         for i in itemSet:
-            temp = temp + self.__rankDup[i] + "\t"
+            temp = temp + self._rankDup[i] + "\t"
         return temp
 
     def startMine(self):
         """
             main program to start the operation
+
         """
-        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
-        self.__startTime = _fp._time.time()
+        global _WS, _regularity, _weights
+        self._startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._WS is None:
             raise Exception("Please enter the Minimum Support")
-        self.__creatingItemSets()
-        self._scanningWeights()
-        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
-        _maxWeight = max([s for s in _weights.values()])
-        _miniWeight = min([s for s in _weights.values()])
-        self._minSup = self.__convert(self._minSup)
-        _minSup = self._minSup
-        itemSet = self.__frequentOneItem()
-        updatedTransactions = self.__updateTransactions(itemSet)
-        for x, y in self.__rank.items():
-            self.__rankDup[y] = x
-        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
-        __Tree = self.__buildTree(updatedTransactions, info)
-        patterns = __Tree.generatePatterns([])
-        self.__finalPatterns = {}
+        self._creatingItemSets()
+        self._WS = self._convert(self._WS)
+        self._regularity = self._convert(self._regularity)
+        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
+        itemSet = self._frequentOneItem()
+        updatedTransactions = self._updateTransactions(itemSet)
+        for x, y in self._rank.items():
+            self._rankDup[y] = x
+        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
+        _Tree = self._buildTree(updatedTransactions, info)
+        patterns = _Tree.generatePatterns([])
+        self._finalPatterns = {}
         for k in patterns:
-            s = self.__savePeriodic(k[0])
-            self.__finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent patterns were generated successfully using WFIM algorithm")
-        self.__endTime = _fp._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
+            s = self._savePeriodic(k[0])
+            self._finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
+        self._endTime = _fp._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
-        return self.__memoryUSS
+        return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
-        return self.__memoryRSS
+        return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
-        return self.__endTime - self.__startTime
+        return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self.__finalPatterns.items():
+        for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
+
         :param outFile: name of the output file
+
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
-        for x, y in self.__finalPatterns.items():
+        for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
-        return self.__finalPatterns
+        return self._finalPatterns
 
     def printResults(self):
-        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
-        
-
 
 if __name__ == "__main__":
     _ap = str()
     if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
         if len(_fp._sys.argv) == 7:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 6:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 5:
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
         _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.27/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,28 +38,31 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _weightedFrequentPatterns(_ABC):
+class _weightedFrequentRegularPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
-        minSup: integer or float or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
+            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
+        :param regularity: The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -87,34 +90,39 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, wFile, minSup, minWeight, sep="\t"):
+    def __init__(self, iFile, wFile, weightSupport, regularity, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
-        :param wFile: Input file name or path of the input file
+        :param wFile: Input weight file name or path of the input file
         :type wFile: str or DataFrame
-        :param minSup: The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
+            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
+        :type weightSupport: int or float or str
+        :param regularity: The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        :type minSup: int or float or str
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+        :type regularity: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._wFile = wFile
         self._sep = sep
-        self._minSup = minSup
-        self._minWeight = minWeight
+        self._regularity = regularity
+        self._WS = weightSupport
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
@@ -164,9 +172,8 @@
 
         pass
 
     @_abstractmethod
     def printResults(self):
         """ To print all the results of execution"""
 
-
         pass
```

### Comparing `pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
+#     from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
 #
-#     obj = alg.WFRIMiner(iFile, WS, regularity)
+#     obj = alg.WFIM(iFile, wFile, expSup, expWSup)
 #
 #     obj.startMine()
 #
-#     weightedFrequentRegularPatterns = obj.getPatterns()
+#     Patterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+#     print("Total number of  Patterns:", len(Patterns))
 #
 #     obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
@@ -44,722 +44,722 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
+from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
 
-_WS = str()
-_regularity = str()
-_lno = int()
+_expSup = str()
+_expWSup = str()
 _weights = {}
-_wf = {}
-_fp._sys.setrecursionlimit(20000)
+_finalPatterns = {}
+_ab._sys.setrecursionlimit(20000)
 
 
-class _Node:
+class _Item:
     """
-        A class used to represent the node of frequentPatternTree
+    A class used to represent the item with probability in transaction of dataset
+    ...
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
+
 
+class _Node(object):
+    """
+    A class used to represent the node of frequentPatternTree
+        ...
     Attributes:
     ----------
-        itemId: int
+        item : int
             storing item of a node
-        counter: int
-            To maintain the support of node
-        parent: node
-            To maintain the parent of node
-        children: list
+        probability : int
+            To maintain the expected support of node
+        parent : node
+            To maintain the parent of every node
+        children : list
             To maintain the children of node
-
     Methods:
     -------
-
-        addChild(node)
-            Updates the nodes children list and parent for the given node
-
+        addChild(itemName)
+            storing the children to their respective parent nodes
     """
 
     def __init__(self, item, children):
-        """ Initializing the Node class
-
-        :param item: Storing the item of a node
-        :type item: int or None
-        :param children: To maintain the children of a node
-        :type children: dict
-        """
-
         self.item = item
+        self.probability = 1
         self.children = children
         self.parent = None
-        self.timeStamps = []
 
     def addChild(self, node):
-        """ To add the children to a node
-
-            :param node: parent node in the tree
-        """
-
         self.children[node.item] = node
         node.parent = self
 
 
-class _Tree:
+class _Tree(object):
     """
     A class used to represent the frequentPatternGrowth tree structure
-
+    ...
     Attributes:
     ----------
         root : Node
-            The first node of the tree set to Null.
+            Represents the root node of the tree
         summaries : dictionary
-            Stores the nodes itemId which shares same itemId
+            storing the nodes with same item name
         info : dictionary
-            frequency of items in the transactions
-
+            stores the support of items
     Methods:
     -------
-        addTransaction(transaction, freq)
-            adding items of  transactions into the tree as nodes and freq is the count of nodes
-        getFinalConditionalPatterns(node)
-            getting the conditional patterns from fp-tree for a node
-        getConditionalPatterns(patterns, frequencies)
-            sort the patterns by removing the items with lower minSup
-        generatePatterns(prefix)
-            generating the patterns from fp-tree
+        addTransaction(transaction)
+            creating transaction as a branch in frequentPatternTree
+        addConditionalPattern(prefixPaths, supportOfItems)
+            construct the conditional tree for prefix paths
+        conditionalPatterns(Node)
+            generates the conditional patterns from tree for specific node
+        conditionalTransactions(prefixPaths,Support)
+            takes the prefixPath of a node and support at child of the path and extract the frequent items from
+            prefixPaths and generates prefixPaths with items which are frequent
+        remove(Node)
+            removes the node from tree once after generating all the patterns respective to the node
+        generatePatterns(Node)
+            starts from the root node of the tree and mines the frequent patterns
     """
 
     def __init__(self):
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction, tid):
-        """     Adding a transaction into tree
+    def addTransaction(self, transaction):
+        """adding transaction into tree
+            :param transaction : it represents the one self.Database in database
+            :type transaction : list
+        """
 
-                :param transaction: To represent the complete database
-                :type transaction: list
-                :param tid: To represent the timestamp of a database
-                :type tid: list
-                :return: pfp-growth tree
+        currentNode = self.root
+        for i in range(len(transaction)):
+            if transaction[i].item not in currentNode.children:
+                newNode = _Node(transaction[i].item, {})
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    newNode.probability = transaction[i].probability
+                else:
+                    newNode.probability = max(lp) * transaction[i].probability
+                currentNode.addChild(newNode)
+                if transaction[i].item in self.summaries:
+                    self.summaries[transaction[i].item].append(newNode)
+                else:
+                    self.summaries[transaction[i].item] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i].item]
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    currentNode.probability += transaction[i].probability
+                else:
+                    currentNode.probability += max(lp) * transaction[i].probability
+
+    def addConditionalPattern(self, transaction, sup):
+        """constructing conditional tree from prefixPaths
+            :param transaction : it represents the one self.Database in database
+            :type transaction : list
+            :param sup : support of prefixPath taken at last child of the path
+            :type sup : int
         """
 
+        # This method takes transaction, support and constructs the conditional tree
         currentNode = self.root
         for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
+                newNode.probability = sup
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-        currentNode.timeStamps = currentNode.timeStamps + tid
-
-    def getConditionalPatterns(self, alpha, pattern):
-        """Generates all the conditional patterns of a respective node
+                currentNode.probability += sup
 
-            :param alpha: To represent a Node in the tree
-            :type alpha: Node
-            :param pattern: prefix of the pattern
-            :type alpha: list
-            :return: A tuple consisting of finalPatterns, conditional pattern base and information
+    def conditionalPatterns(self, alpha):
+        """generates all the conditional patterns of respective node
+            :param alpha : it represents the Node in tree
+            :type alpha : _Node
         """
+
+        # This method generates conditional patterns of node by traversing the tree
         finalPatterns = []
-        finalSets = []
+        sup = []
         for i in self.summaries[alpha]:
-            set1 = i.timeStamps
+            s = i.probability
             set2 = []
             while i.parent.item is not None:
                 set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalSets.append(set1)
-        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
-        return finalPatterns, finalSets, info
-
-    @staticmethod
-    def generateTimeStamps(node):
-        """To get the timestamps of a node
-
-        :param node: A node in the tree
-        :return: Timestamps of a node
-        """
-
-        finalTimeStamps = node.timeStamps
-        return finalTimeStamps
+                sup.append(s)
+        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
+        return finalPatterns, support, info
 
     def removeNode(self, nodeValue):
-        """ Removing the node from tree
-
-            :param nodeValue: To represent a node in the tree
-            :type nodeValue: node
-            :return: Tree with their nodes updated with timestamps
+        """removing the node from tree
+            :param nodeValue : it represents the node in tree
+            :type nodeValue : node
         """
 
         for i in self.summaries[nodeValue]:
-            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
             del i.parent.children[nodeValue]
 
-    def getTimeStamps(self, alpha):
-        """ To get all the timestamps of the nodes which share same item name
-
-            :param alpha: Node in a tree
-            :return: Timestamps of a  node
-        """
-        temporary = []
-        for i in self.summaries[alpha]:
-            temporary += i.timeStamps
-        return temporary
-
-    @staticmethod
-    def getSupportAndPeriod(timeStamps, pattern):
-        """To calculate the periodicity and support
-
-        :param timeStamps: Timestamps of an item set
-        :type timeStamps: list
-        :param pattern: pattern to evaluate the weighted frequent regular or not
-        :type pattern: list
-        :return: support, periodicity
-        """
-
-        global _WS, _regularity, _lno, _weights
-        timeStamps.sort()
-        cur = 0
-        per = list()
-        sup = 0
-        for j in range(len(timeStamps)):
-            per.append(timeStamps[j] - cur)
-            cur = timeStamps[j]
-            sup += 1
-        per.append(_lno - cur)
-        l = int()
-        for i in pattern:
-            l = l + _weights[i]
-        wf = (l / (len(pattern))) * sup
-        if len(per) == 0:
-            return [0, 0]
-        return [sup, max(per), wf]
-
-    def conditionalDatabases(self, conditionalPatterns, conditionalTimeStamps, pattern):
-        """ It generates the conditional patterns with periodic-frequent items
-
-            :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
-            :type conditionalPatterns: list
-            :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
-            :type conditionalTimeStamps: list
-            :param pattern: prefix of the pattern
-            :type pattern: list
-            :returns: Returns conditional transactions by removing non-periodic and non-frequent items
+    def conditionalTransactions(self, condPatterns, support):
+        """ It generates the conditional patterns with frequent items
+                :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
+                :type condPatterns : list
+                :support : the support of conditional pattern in tree
+                :support : int
         """
 
-        global _WS, _regularity
+        global _expSup, _expWSup
         pat = []
-        timeStamps = []
-        data1 = {}
-        for i in range(len(conditionalPatterns)):
-            for j in conditionalPatterns[i]:
-                if j in data1:
-                    data1[j] = data1[j] + conditionalTimeStamps[i]
+        sup = []
+        count = {}
+        for i in range(len(condPatterns)):
+            for j in condPatterns[i]:
+                if j in count:
+                    count[j] += support[i]
                 else:
-                    data1[j] = conditionalTimeStamps[i]
-        updatedDictionary = {}
-        for m in data1:
-            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
+                    count[j] = support[i]
+        updatedDict = {}
+        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
         count = 0
-        for p in conditionalPatterns:
-            p1 = [v for v in p if v in updatedDictionary]
-            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
+        for p in condPatterns:
+            p1 = [v for v in p if v in updatedDict]
+            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                timeStamps.append(conditionalTimeStamps[count])
-            count += 1
-        return pat, timeStamps, updatedDictionary
+                sup.append(support[count])
+                count += 1
+        return pat, sup, updatedDict
 
     def generatePatterns(self, prefix):
-        """ Generates the patterns
-
-            :param prefix: Forms the combination of items
-            :type prefix: list
-            :returns: yields patterns with their support and periodicity
+        """generates the patterns
+            :param prefix : forms the combination of items
+            :type prefix : list
         """
-        global _WS
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
+
+        global _finalPatterns, _expSup, _expWSup, _weights
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
             pattern = prefix[:]
             pattern.append(i)
-            if self.info[i][2] >= _WS:
-                yield pattern, self.info[i]
-                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+            weight = 0
+            for k in pattern:
+                weight = weight + _weights[k]
+            weight = weight/len(pattern)
+            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
+                _finalPatterns[tuple(pattern)] = self.info.get(i)
+                patterns, support, info = self.conditionalPatterns(i)
                 conditionalTree = _Tree()
                 conditionalTree.info = info.copy()
                 for pat in range(len(patterns)):
-                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
                 if len(patterns) > 0:
-                    for q in conditionalTree.generatePatterns(pattern):
-                        yield q
+                    conditionalTree.generatePatterns(pattern)
             self.removeNode(i)
 
 
-class WFRIMiner(_fp._weightedFrequentRegularPatterns):
+class WUFIM(_ab._weightedFrequentPatterns):
     """
-       WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
-       It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the
-       patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
-
-    Reference :
-    ---------
-           K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
-           2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
-           doi: 10.1109/KST.2017.7886090.
+    Description:
+    -------------
+        It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database
+        using PUF-Tree.
+
+    Reference:
+    ------------
+        Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases, In book: Machine Learning and Data Mining in Pattern Recognition
+        Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
 
-    Attributes :
-    ----------
+    Attributes:
+    ------------
         iFile : file
-            Input file name or path of the input file
-        WS: float or int or str
-            The user can specify WS either in count or proportion of database size.
-            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
-        regularity: float or int or str
-            The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+            Name of the Input file or path of the input file
+        wFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup: float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
-        oFile : file
-            Name of the output file or the path of the output file
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
         tree : class
-            it represents the Tree class
+            To represents the Tree class
+        itemSetCount : int
+            To represents the total no of patterns
         finalPatterns : dict
-            it represents to store the patterns
-
-    Methods :
-    -------
+            To store the complete patterns
+    Methods:
+    ---------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets()
-            Scans the dataset or dataframes and stores in list format
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
         frequentOneItem()
-            Extracts the one-frequent patterns from transactions
-
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
     **Methods to execute code on terminal**
 
-            Format:
-                      >>> python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
-            Example:
-                      >>>  python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
+        Format:
+                  >>>  python3 WUFIM.py <inputFile> <outputFile> <minSup>
+        Example:
+                  >>>  python3 WUFIM.py sampleTDB.txt patterns.txt 3
 
-                     .. note:: WS & regularity will be considered in support count or frequency
+                 .. note:: minSup  will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
-    .. code-block:: python
-
-            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
+.. code-block:: python
 
-            obj = alg.WFRIMiner(iFile, WS, regularity)
+        from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
 
-            obj.startMine()
+        obj = alg.WFIM(iFile, wFile, expSup, expWSup)
 
-            weightedFrequentRegularPatterns = obj.getPatterns()
+        obj.startMine()
 
-            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+        Patterns = obj.getPatterns()
 
-            obj.savePatterns(oFile)
+        print("Total number of  Patterns:", len(Patterns))
 
-            Df = obj.getPatternInDataFrame()
+        obj.savePatterns(oFile)
 
-            memUSS = obj.getMemoryUSS()
+        Df = obj.getPatternsAsDataFrame()
 
-            print("Total Memory in USS:", memUSS)
+        memUSS = obj.getMemoryUSS()
 
-            memRSS = obj.getMemoryRSS()
+        print("Total Memory in USS:", memUSS)
 
-            print("Total Memory in RSS", memRSS)
+        memRSS = obj.getMemoryRSS()
 
-            run = obj.getRuntime()
+        print("Total Memory in RSS", memRSS)
 
-            print("Total ExecutionTime in seconds:", run)
-
-    **Credits:**
-
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
-
-        """
+        run = obj.getRuntime()
 
+        print("Total ExecutionTime in seconds:", run)
+   """
     _startTime = float()
     _endTime = float()
-    _WS = str()
-    _regularity = str()
-    _weight = {}
+    _minSup = str()
     _finalPatterns = {}
-    _wFile = " "
     _iFile = " "
+    _wFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
-    _lno = 0
-    _tree = _Tree()
     _rank = {}
-    _rankDup = {}
+    _expSup = float()
+    _expWSup = float()
 
-    def __init__(self, iFile, _wFile, WS, regularity, sep='\t'):
-        super().__init__(iFile, _wFile, WS, regularity, sep)
+    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t'):
+        super().__init__(iFile, wFile, expSup, expWSup, sep)
 
     def _creatingItemSets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
-
-
+            Scans the uncertain transactional dataset
         """
         self._Database = []
-        self._weight = {}
-        if isinstance(self._iFile, _fp._pd.DataFrame):
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            _items, _weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                _items = self._wFile['items'].tolist()
-            if 'weight' in i:
-                _weights = self._wFile['weight'].tolist()
-            for i in range(len(_items)):
-                self._weight[_items[i]] = _weights[i]
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _fp._validators.url(self._iFile):
-                data = _fp._urlopen(self._iFile)
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line.strip()
                     line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    line = line.strip()
+                    line = [i for i in line.split(':')]
+                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                    temp1 = [x for x in temp1 if x]
+                    temp2 = [x for x in temp2 if x]
+                    tr = []
+                    for i in range(len(temp1)):
+                        item = temp1[i]
+                        probability = float(temp2[i])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(tr)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            line = line.strip()
+                            line = [i for i in line.split(':')]
+                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                            temp1 = [x for x in temp1 if x]
+                            temp2 = [x for x in temp2 if x]
+                            tr = []
+                            for i in range(len(temp1)):
+                                item = temp1[i]
+                                probability = float(temp2[i])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
 
+    def _scanningWeights(self):
+        """
+            Scans the uncertain transactional dataset
+        """
+        self._weights = {}
+        if isinstance(self._wFile, _ab._pd.DataFrame):
+            weights, data = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                data = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for k in range(len(data)):
+                self._weights[data[k]] = int(float(weights[k]))
+
+            # print(self.Database)
         if isinstance(self._wFile, str):
-            if _fp._validators.url(self._wFile):
-                data = _fp._urlopen(self._wFile)
+            if _ab._validators.url(self._wFile):
+                data = _ab._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._weight[temp[0]] = float(temp[1])
+                    self._weights[temp[0]] = int(float(temp[1]))
             else:
                 try:
-                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                    with open(self._wFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._weight[temp[0]] = float(temp[1])
+                            self._weights[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
-                    quit()
 
-    def _convert(self, value):
+    def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
+                :param self.Database : it represents the one self.Database in database
+                :type self.Database : list
         """
-        to convert the type of user specified minSup value
 
-        :param value: user specified minSup value
+        mapSupport = {}
+        for i in self._Database:
+            for j in i:
+                if j.item not in mapSupport:
+                    if self._weights.get(j.item) is not None:
+                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
+                else:
+                    mapSupport[j.item][0] += j.probability
+        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
+        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
+        return mapSupport, plist
 
-        :return: converted type
+    @staticmethod
+    def _buildTree(data, info):
+        """it takes the self.Database and support of each item and construct the main tree with setting root
+            node as null
+                :param data : it represents the one self.Database in database
+                :type data : list
+                :param info : it represents the support of each item
+                :type info : dictionary
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
 
-    def _frequentOneItem(self):
-        """
-        Generating One frequent items sets
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(data)):
+            rootNode.addTransaction(data[i])
+        return rootNode
 
+    def _updateTransactions(self, dict1):
+        """remove the items which are not frequent from self.Database and updates the self.Database with rank of items
+            :param dict1 : frequent items with support
+            :type dict1 : dictionary
         """
-        global _lno, _wf, _weights
-        self._mapSupport = {}
-        _owf = {}
-        for tr in self._Database:
-            for i in range(1, len(tr)):
-                if tr[i] not in self._mapSupport:
-                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
-                else:
-                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
-                    self._mapSupport[tr[i]][1] = int(tr[0])
-                    self._mapSupport[tr[i]][2] += 1
-        for key in self._mapSupport:
-            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
-        _lno = len(self._Database)
-        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
-        for x, y in self._mapSupport.items():
-            if self._weight.get(x) is None:
-                self._weight[x] = 0
-        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
-        for x, y in self._mapSupport.items():
-            _owf[x] = y[0] * gmax
-        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
-        for x, y in self._mapSupport.items():
-            temp = self._weight[x] * y[0]
-            _wf[x] = temp
-            self._mapSupport[x].append(temp)
-        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
-        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
-        for x, y in self._rank.items():
-            _weights[y] = self._weight[x]
-        return genList
-
-    def _updateTransactions(self, itemSet):
-        """
-        Updates the items in transactions with rank of items according to their support
-
-        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
-                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
-
-        Parameters
-        ----------
-        itemSet: list of one-frequent items
-
-        -------
 
-        """
         list1 = []
         for tr in self._Database:
-            list2 = [int(tr[0])]
-            for i in range(1, len(tr)):
-                if tr[i] in itemSet:
-                    list2.append(self._rank[tr[i]])
+            list2 = []
+            for i in range(0, len(tr)):
+                if tr[i].item in dict1:
+                    list2.append(tr[i])
             if len(list2) >= 2:
-                basket = list2[1:]
-                basket.sort()
-                list2[1:] = basket[0:]
+                basket = list2
+                basket.sort(key=lambda val: self.rank[val.item])
+                list2 = basket
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def _buildTree(transactions, info):
-        """
-        Builds the tree with updated transactions
-        Parameters:
-        ----------
-            transactions: updated transactions
-            info: support details of each item in transactions
-
-        Returns:
-        -------
-            transactions compressed in fp-tree
+    def _check(i, x):
+        """To check the presence of item or pattern in transaction
+                :param x: it represents the pattern
+                :type x : list
+                :param i : represents the uncertain self.Database
+                :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
+    def _convert(self, value):
         """
-        rootNode = _Tree()
-        rootNode.info = info.copy()
-        for i in range(len(transactions)):
-            set1 = [transactions[i][0]]
-            rootNode.addTransaction(transactions[i][1:], set1)
-        return rootNode
-
-    def _savePeriodic(self, itemSet):
+        To convert the type of user specified minSup value
+            :param value: user specified minSup value
+            :return: converted type minSup value
         """
-        The duplication items and their ranks
-        Parameters:
-        ----------
-            itemSet: frequent itemSet that generated
-
-        Returns:
-        -------
-            patterns with original item names.
-
-        """
-        temp = str()
-        for i in itemSet:
-            temp = temp + self._rankDup[i] + "\t"
-        return temp
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-    def startMine(self):
+    def _removeFalsePositives(self):
+        """
+            To remove the false positive patterns generated in frequent patterns
+            :return: patterns with accurate probability
         """
-            main program to start the operation
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            weight = 0
+            for i in x:
+                weight += self._weights[i]
+            weight = weight / len(x)
+            if weight * y >= self._expWSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
 
+    def startMine(self):
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
         """
-        global _WS, _regularity, _weights
-        self._startTime = _fp._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._WS is None:
-            raise Exception("Please enter the Minimum Support")
+        global _expSup, _expWSup, _weights, _finalPatterns
+        self._startTime = _ab._time.time()
+        self._Database, self._weights = [], {}
         self._creatingItemSets()
-        self._WS = self._convert(self._WS)
-        self._regularity = self._convert(self._regularity)
-        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
-        itemSet = self._frequentOneItem()
-        updatedTransactions = self._updateTransactions(itemSet)
-        for x, y in self._rank.items():
-            self._rankDup[y] = x
-        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
-        _Tree = self._buildTree(updatedTransactions, info)
-        patterns = _Tree.generatePatterns([])
+        self._scanningWeights()
+        _weights = self._weights
+        self._expSup = float(self._expSup)
+        self._expWSup = float(self._expWSup)
+        _expSup = self._expSup
+        _expWSup = self._expWSup
         self._finalPatterns = {}
-        for k in patterns:
-            s = self._savePeriodic(k[0])
-            self._finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
-        self._endTime = _fp._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        process = _fp._psutil.Process(_fp._os.getpid())
-        self._memoryRSS = float()
+        mapSupport, plist = self._frequentOneItem()
+        self.Database1 = self._updateTransactions(mapSupport)
+        info = {k: v for k, v in mapSupport.items()}
+        Tree1 = self._buildTree(self.Database1, info)
+        Tree1.generatePatterns([])
+        self._removeFalsePositives()
+        print("Weighted Frequent patterns were generated  successfully using WUFIM algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
+        self.memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            s = str()
+            for i in a:
+                s = s + i + " "
+            data.append([s, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
-
         :param outFile: name of the output file
-
         :type outFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s = str()
+            for i in x:
+                s = s + i + "\t"
+            s1 = s.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
-
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
-        if len(_fp._sys.argv) == 7:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 5:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+        if len(_ab._sys.argv) == 6:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
-        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
-        _ap.save(_fp._sys.argv[2])
-        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        for k in [120, 140, 160, 180, 200]:
+            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
+                        k, 500, '\t')
+            _ap.startMine()
+            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
+            print("Total Memory in USS:", _ap.getMemoryUSS())
+            print("Total Memory in RSS", _ap.getMemoryRSS())
+            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+__copyright__ = """
 #  Copyright (C)  2021 Rage Uday Kiran
 #
 #      This program is free software: you can redistribute it and/or modify
 #      it under the terms of the GNU General Public License as published by
 #      the Free Software Foundation, either version 3 of the License, or
 #      (at your option) any later version.
 #
@@ -21,16 +22,16 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
@@ -38,31 +39,28 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _weightedFrequentRegularPatterns(_ABC):
+class _frequentPatternsStream(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
-        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
-            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
+        minSup: integer or float or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
-        :param regularity: The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -90,46 +88,93 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, wFile, weightSupport, regularity, sep="\t"):
+    def __init__(self, iFile, minSup, windowSize, paneSize, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
-        :param wFile: Input weight file name or path of the input file
-        :type wFile: str or DataFrame
-        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
-            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
-        :type weightSupport: int or float or str
-        :param regularity: The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+        :param minSup: The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
-        :type regularity: int or float or str
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
-        self._wFile = wFile
         self._sep = sep
-        self._regularity = regularity
-        self._WS = weightSupport
+        self._minSup = minSup
+        self._windowSize = windowSize
+        self._paneSize = paneSize
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
+    '''@abstractmethod
+    def iFile(self):
+        """Variable to store the input file path/file name"""
+
+        pass
+
+    @abstractmethod
+    def minSup(self):
+        """Variable to store the user-specified minimum support value"""
+
+        pass
+
+    @abstractmethod
+    def sep(self):
+        """Variable to store the user-specified minimum support value"""
+
+        pass
+
+    @abstractmethod
+    def startTime(self):
+        """Variable to store the start time of the mining process"""
+
+        pass
+
+    @abstractmethod
+    def endTime(self):
+        """Variable to store the end time of the complete program"""
+
+        pass
+
+    @abstractmethod
+    def memoryUSS(self):
+        """Variable to store USS memory consumed by the program"""
+
+        pass
+
+    @abstractmethod
+    def memoryRSS(self):
+        """Variable to store RSS memory consumed by the program"""
+
+        pass
+
+    @abstractmethod
+    def finalPatterns(self):
+        """Variable to store the complete set of patterns in a dictionary"""
+
+        pass
+
+    @abstractmethod
+    def oFile(self):
+        """Variable to store the name of the output file to store the complete set of frequent patterns"""
+
+        pass'''
+
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
@@ -170,10 +215,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print result of the execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,765 +1,879 @@
-# **Importing this algorithm into a python program**
-# --------------------------------------------------------
-#
-#
-#     from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
-#
-#     obj = alg.WFIM(iFile, wFile, expSup, expWSup)
-#
-#     obj.startMine()
-#
-#     Patterns = obj.getPatterns()
-#
-#     print("Total number of  Patterns:", len(Patterns))
-#
-#     obj.savePatterns(oFile)
-#
-#     Df = obj.getPatternsAsDataFrame()
-#
-#     memUSS = obj.getMemoryUSS()
-#
-#     print("Total Memory in USS:", memUSS)
-#
-#     memRSS = obj.getMemoryRSS()
-#
-#     print("Total Memory in RSS", memRSS)
+__copyright__ = """
+#  Copyright (C)  2021 Rage Uday Kiran
 #
-#     run = obj.getRuntime()
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
 #
-#     print("Total ExecutionTime in seconds:", run)
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 
 
-__copyright__ = """
- Copyright (C)  2021 Rage Uday Kiran
+import abstract as _fp
 
-     This program is free software: you can redistribute it and/or modify
-     it under the terms of the GNU General Public License as published by
-     the Free Software Foundation, either version 3 of the License, or
-     (at your option) any later version.
-
-     This program is distributed in the hope that it will be useful,
-     but WITHOUT ANY WARRANTY; without even the implied warranty of
-     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-     GNU General Public License for more details.
-
-     You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-     Copyright (C)  2021 Rage Uday Kiran
+_fp._sys.setrecursionlimit(20000)
 
-"""
+class _Node:
+    """
+    This class represents a node in the FP-tree
 
-from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
+    Attributes:
+    ----------
+        itemId : str
+            The item name of the node
 
-_expSup = str()
-_expWSup = str()
-_weights = {}
-_finalPatterns = {}
-_ab._sys.setrecursionlimit(20000)
+        counter : int
+            The support count of the item
 
+        parent : Node
+            The parent node of the current node
 
-class _Item:
-    """
-    A class used to represent the item with probability in transaction of dataset
-    ...
-    Attributes:
-    __________
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
-    """
+        children : dict
+            The dictionary of children of the current node
 
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
+        tail : list
+            The tail of the current node denoting the support count in each batch
 
+        next : Node
+            The next node of the current node
 
-class _Node(object):
-    """
-    A class used to represent the node of frequentPatternTree
-        ...
-    Attributes:
-    ----------
-        item : int
-            storing item of a node
-        probability : int
-            To maintain the expected support of node
-        parent : node
-            To maintain the parent of every node
-        children : list
-            To maintain the children of node
-    Methods:
-    -------
-        addChild(itemName)
-            storing the children to their respective parent nodes
-    """
+        
+        Methods:
+        -------
+
+        addChild(node) 
+            Adds a child node to the current node
+
+        shiftTail()
+            Shifts the tail of the current node during the removal of the batch
 
-    def __init__(self, item, children):
-        self.item = item
-        self.probability = 1
-        self.children = children
+        addSupportCount(count)
+            Adds the support count to the current node
+
+    """
+    def __init__(self, item, supportCount):
+        self.itemId = item
+        self.counter = supportCount
         self.parent = None
+        self.children = {}
+        self.tail = None
+        self.next = None
 
     def addChild(self, node):
-        self.children[node.item] = node
+        """
+            Adds a child node to the current node
+
+            :param node: The child node to be added
+            :type node: Node
+        """
+        self.children[node.itemId] = node
         node.parent = self
 
+    def shiftTail(self):
+        """
+            Shifts the tail of the current node during the removal of the batch
+        """
+        self.tail.pop(0)
+        self.tail.append(0)
+
+    def addSupportCount(self, count):
+        """
+            Adds the support count to the current node
+
+            :param count: The support count to be added
+            :type count: int
+        """
+        self.counter += count
+
+class _HeaderTable:
 
-class _Tree(object):
     """
-    A class used to represent the frequentPatternGrowth tree structure
-    ...
-    Attributes:
-    ----------
-        root : Node
-            Represents the root node of the tree
-        summaries : dictionary
-            storing the nodes with same item name
-        info : dictionary
-            stores the support of items
-    Methods:
-    -------
-        addTransaction(transaction)
-            creating transaction as a branch in frequentPatternTree
-        addConditionalPattern(prefixPaths, supportOfItems)
-            construct the conditional tree for prefix paths
-        conditionalPatterns(Node)
-            generates the conditional patterns from tree for specific node
-        conditionalTransactions(prefixPaths,Support)
-            takes the prefixPath of a node and support at child of the path and extract the frequent items from
-            prefixPaths and generates prefixPaths with items which are frequent
-        remove(Node)
-            removes the node from tree once after generating all the patterns respective to the node
-        generatePatterns(Node)
-            starts from the root node of the tree and mines the frequent patterns
+        This class represents the header table of the FP-tree
+
+        Attributes:
+        ----------
+            table : dict
+                The dictionary of items and their support count with node pointer
+
+            orderedItems : list
+                The list of items in the header table in the order of their support count
+
+        Methods:
+        -------
+            updateSupportCount(item, count, node)
+                Updates the support count with the node pointer of the item in the header table
+
+            addSupportCount(item, count)
+                Adds the support count of the item in the header table
+
+            removeSupportCount(item, count)
+                Removes the support count of the item in the header table
+
+            itemOrdering()
+                Orders the items in the header table in the order of their support count
+
+            orderTransaction(transaction)
+                Orders the items in the transaction in the order of their support count
+
     """
 
     def __init__(self):
-        self.root = _Node(None, {})
-        self.summaries = {}
-        self.info = {}
-
-    def addTransaction(self, transaction):
-        """adding transaction into tree
-            :param transaction : it represents the one self.Database in database
-            :type transaction : list
-        """
-
-        currentNode = self.root
-        for i in range(len(transaction)):
-            if transaction[i].item not in currentNode.children:
-                newNode = _Node(transaction[i].item, {})
-                l1 = i - 1
-                lp = []
-                while l1 >= 0:
-                    lp.append(transaction[l1].probability)
-                    l1 -= 1
-                if len(lp) == 0:
-                    newNode.probability = transaction[i].probability
-                else:
-                    newNode.probability = max(lp) * transaction[i].probability
-                currentNode.addChild(newNode)
-                if transaction[i].item in self.summaries:
-                    self.summaries[transaction[i].item].append(newNode)
+        self.table = {}
+        self.orderedItems = []
+
+    def updateSupportCount(self, item, count, node):
+        """
+            Updates the support count with the node pointer of the item in the header table
+
+            :param item: The item whose support count is to be updated
+            :type item: str
+            :param count: The support count to be added
+            :type count: int
+            :param node: The node pointer to be added
+            :type node: Node
+        """
+        if item in self.table:
+            self.table[item][0] += count
+            tempNode = self.table[item][1]
+            while tempNode.next != None:
+                tempNode = tempNode.next
+            tempNode.next = node
+        else:
+            self.table[item] = [count, node]
+
+        self.itemOrdering()
+
+    def addSupportCount(self, item, count):
+        """
+            Adds the support count of the item in the header table
+
+            :param item: The item whose support count is to be added
+            :type item: str
+            :param count: The support count to be added
+            :type count: int
+        """
+        if item in self.table:
+            self.table[item][0] += count
+    
+    def removeSupportCount(self, item, count):
+        """
+            Removes the support count of the item in the header table
+
+            :param item: The item whose support count is to be removed
+            :type item: str
+            :param count: The support count to be removed
+            :type count: int
+        """
+        if item in self.table:
+            self.table[item][0] -= count
+            if(self.table[item][0] == 0):
+                del self.table[item]
+    
+    def itemOrdering(self):
+        """
+            Orders the items in the header table in the order of their support count
+        """
+        self.orderedItems = list(sorted(self.table.keys(), key=lambda x: self.table[x][0]))
+
+    def orderTransaction(self, transaction):
+        """
+            Orders the items in the transaction in the order of their support count
+
+            :param transaction: The transaction to be ordered
+            :type transaction: list
+
+            :return: The ordered transaction
+            :rtype: list
+        """
+        return sorted(transaction, key=lambda x: self.table[x][0] if x in self.table else 1, reverse=True)
+
+class _CPSTree:
+    """
+        Class representing the CPSTree
+
+        Attributes:
+        ----------
+            root : Node
+                The root node of the CPSTree
+
+            headerTable : HeaderTable
+                The header table of the CPSTree
+
+            windowSize : int
+                The window size used for analyzing the data stream
+
+            paneSize : int
+                The pane size used in each window for analyzing the data stream
+
+            curBatchIndex : int
+                The current batch index of the data stream
+
+        Methods:
+        -------
+
+            addTransaction(transaction, restructuring = False, supportValue = None, tailNode = None)
+                Adds the transaction to the CPSTree
+
+            updateBranch(node, count)
+                Updates the branch of the node with the support count useful while removing the oldest batch
+
+            removeBatch()
+                Removes the oldest batch from the CPSTree
+
+    """
+
+    def __init__(self, windowSize, paneSize):
+        self.root = _Node(None, 0)
+        self.headerTable = _HeaderTable()
+        self.windowSize = windowSize
+        self.paneSize = paneSize
+        self.curBatchIndex = 0
+
+    def addTransaction(self, transaction, restructuring = False, supportValue = None, tailNode = None):
+        """
+            Adds the transaction to the CPSTree
+
+            :param transaction: The transaction to be added
+            :type transaction: list
+            :param restructuring: Flag to indicate whether the transaction is added during restructuring
+            :type restructuring: bool
+            :param supportValue: The support count of the items in the transaction useful during restructuring
+            :type supportValue: dict
+            :param tailNode: The tail node of the transaction useful during restructuring
+            :type tailNode: Node
+        """
+        curNode = self.root
+
+        if restructuring is False:
+            transaction = self.headerTable.orderTransaction(transaction)
+
+        for item in transaction:
+            if item in curNode.children:
+
+                if supportValue is None:
+                    curNode.children[item].addSupportCount(1)
+                    self.headerTable.addSupportCount(item, 1)
                 else:
-                    self.summaries[transaction[i].item] = [newNode]
-                currentNode = newNode
+                    curNode.children[item].addSupportCount(supportValue[item])
+                    self.headerTable.addSupportCount(item, supportValue[item])
+                
+                curNode = curNode.children[item]
             else:
-                currentNode = currentNode.children[transaction[i].item]
-                l1 = i - 1
-                lp = []
-                while l1 >= 0:
-                    lp.append(transaction[l1].probability)
-                    l1 -= 1
-                if len(lp) == 0:
-                    currentNode.probability += transaction[i].probability
-                else:
-                    currentNode.probability += max(lp) * transaction[i].probability
 
-    def addConditionalPattern(self, transaction, sup):
-        """constructing conditional tree from prefixPaths
-            :param transaction : it represents the one self.Database in database
-            :type transaction : list
-            :param sup : support of prefixPath taken at last child of the path
-            :type sup : int
-        """
-
-        # This method takes transaction, support and constructs the conditional tree
-        currentNode = self.root
-        for i in range(len(transaction)):
-            if transaction[i] not in currentNode.children:
-                newNode = _Node(transaction[i], {})
-                newNode.probability = sup
-                currentNode.addChild(newNode)
-                if transaction[i] in self.summaries:
-                    self.summaries[transaction[i]].append(newNode)
+                if supportValue is None:
+                    newNode = _Node(item, 1)
+                    self.headerTable.updateSupportCount(item, 1, newNode)
+
                 else:
-                    self.summaries[transaction[i]] = [newNode]
-                currentNode = newNode
+                    newNode = _Node(item, supportValue[item])
+                    self.headerTable.updateSupportCount(item, supportValue[item], newNode)
+
+                curNode.addChild(newNode)
+                newNode.parent = curNode
+                curNode = newNode
+
+        if curNode.tail is None:
+            curNode.tail = [0] * self.windowSize
+
+        if restructuring is False:
+            if supportValue is None:
+                curNode.tail[self.curBatchIndex] = 1
             else:
-                currentNode = currentNode.children[transaction[i]]
-                currentNode.probability += sup
+                curNode.tail[self.curBatchIndex] = supportValue[item]
 
-    def conditionalPatterns(self, alpha):
-        """generates all the conditional patterns of respective node
-            :param alpha : it represents the Node in tree
-            :type alpha : _Node
-        """
-
-        # This method generates conditional patterns of node by traversing the tree
-        finalPatterns = []
-        sup = []
-        for i in self.summaries[alpha]:
-            s = i.probability
-            set2 = []
-            while i.parent.item is not None:
-                set2.append(i.parent.item)
-                i = i.parent
-            if len(set2) > 0:
-                set2.reverse()
-                finalPatterns.append(set2)
-                sup.append(s)
-        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
-        return finalPatterns, support, info
-
-    def removeNode(self, nodeValue):
-        """removing the node from tree
-            :param nodeValue : it represents the node in tree
-            :type nodeValue : node
-        """
-
-        for i in self.summaries[nodeValue]:
-            del i.parent.children[nodeValue]
-
-    def conditionalTransactions(self, condPatterns, support):
-        """ It generates the conditional patterns with frequent items
-                :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
-                :type condPatterns : list
-                :support : the support of conditional pattern in tree
-                :support : int
-        """
-
-        global _expSup, _expWSup
-        pat = []
-        sup = []
-        count = {}
-        for i in range(len(condPatterns)):
-            for j in condPatterns[i]:
-                if j in count:
-                    count[j] += support[i]
-                else:
-                    count[j] = support[i]
-        updatedDict = {}
-        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
-        count = 0
-        for p in condPatterns:
-            p1 = [v for v in p if v in updatedDict]
-            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
-            if len(trans) > 0:
-                pat.append(trans)
-                sup.append(support[count])
-                count += 1
-        return pat, sup, updatedDict
-
-    def generatePatterns(self, prefix):
-        """generates the patterns
-            :param prefix : forms the combination of items
-            :type prefix : list
-        """
-
-        global _finalPatterns, _expSup, _expWSup, _weights
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
-            pattern = prefix[:]
-            pattern.append(i)
-            weight = 0
-            for k in pattern:
-                weight = weight + _weights[k]
-            weight = weight/len(pattern)
-            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
-                _finalPatterns[tuple(pattern)] = self.info.get(i)
-                patterns, support, info = self.conditionalPatterns(i)
-                conditionalTree = _Tree()
-                conditionalTree.info = info.copy()
-                for pat in range(len(patterns)):
-                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
-                if len(patterns) > 0:
-                    conditionalTree.generatePatterns(pattern)
-            self.removeNode(i)
 
+        if tailNode is not None and curNode.tail is None:
+            curNode.tail = tailNode.copy()
+
+        if tailNode is not None and curNode.tail is not None:
+            for i in range(len(tailNode)):
+                curNode.tail[i] += tailNode[i]
+            
 
-class WUFIM(_ab._weightedFrequentPatterns):
+    def updateBranch(self, curNode, curSupport):
+        """
+            Updates the branch of the node with the support count useful while removing the oldest batch
+
+            :param curNode: The node whose branch is to be updated
+            :type curNode: Node
+            :param curSupport: The support count of the node to be updated
+            :type curSupport: int
+        """
+        if(curNode.itemId is None):
+            return
+
+        curNode.addSupportCount(-curSupport)
+        parentNode = curNode.parent
+
+        if(curNode.counter == 0):
+            if(self.headerTable.table[curNode.itemId][1] == curNode):
+                self.headerTable.table[curNode.itemId][1] = curNode.next
+
+            else:
+                prev = self.headerTable.table[curNode.itemId][1]
+                while(prev is not None and prev.next != curNode):
+                    prev = prev.next
+
+                prev.next = curNode.next
+
+            del curNode.parent.children[curNode.itemId]
+
+        self.headerTable.removeSupportCount(curNode.itemId, curSupport)
+        self.updateBranch(parentNode, curSupport)
+
+
+    def removeBatch(self):
+        """
+            Removes the oldest batch from the CPSTree by recursively iterating over the tree
+        """
+        root = self.root
+        curItems = list(self.headerTable.table.keys())
+        for item in curItems:
+            curNode = self.headerTable.table[item][1]
+            while curNode is not None:
+                if curNode.tail is not None:
+                    curSupport = curNode.tail[0]
+
+                    if(curSupport != 0):
+                        self.updateBranch(curNode, curSupport)
+                    curNode.shiftTail()
+
+                curNode = curNode.next
+
+
+class FrequentPatternStreamMining(_fp._frequentPatternsStream):
     """
-    Description:
-    -------------
-        It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database
-        using PUF-Tree.
-
-    Reference:
-    ------------
-        Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases, In book: Machine Learning and Data Mining in Pattern Recognition
-        Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
+        Description:
+        -------------
 
-    Attributes:
-    ------------
-        iFile : file
-            Name of the Input file or path of the input file
-        wFile : file
-            Name of the Input file or path of the input file
-        oFile : file
-            Name of the output file or path of the output file
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator.
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
-        Database : list
-            To store the transactions of a database in list
-        mapSupport : Dictionary
-            To maintain the information of item and their frequency
-        lno : int
-            To represent the total no of transaction
-        tree : class
-            To represents the Tree class
-        itemSetCount : int
-            To represents the total no of patterns
-        finalPatterns : dict
-            To store the complete patterns
-    Methods:
-    ---------
-        startMine()
-            Mining process will start from here
-        getPatterns()
-            Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
-        getPatternsAsDataFrame()
-            Complete set of frequent patterns will be loaded in to a dataframe
-        getMemoryUSS()
-            Total amount of USS memory consumed by the mining process will be retrieved from this function
-        getMemoryRSS()
-            Total amount of RSS memory consumed by the mining process will be retrieved from this function
-        getRuntime()
-            Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
-        frequentOneItem()
-            Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
+            Sliding window-based frequent pattern mining over data streams is one of basic data stream mining tasks.
+            The goal is to find all frequent patterns in a sliding window over a data stream. It stores the complete
+            database in form of FP-Tree but adjusts the tree structure based on the upcoming transactions and removes
+            the oldest batch from the tree. This creates a sliding window over the data stream. The adjusting FP-tree
+            structure is called CPSTree. It is a modified version of the existing FP-Tree structure.
+
+        Reference : 
+        ------------
+            Syed Khairuzzaman Tanbeer and Chowdhury Farhan Ahmed and Byeong-Soo Jeong and Young-Koo Lee : Sliding 
+            window-based frequent pattern mining over data streams. Information Sciences Vol 179, 3843 - 3865, 2009.
+            https://doi.org/10.1016/j.ins.2009.07.012
+
+        Attributes : 
+        ------------
+            iFile : str
+                The input file name or path
+
+            minSup : float or int or str
+                The user can specify minSup either in count or proportion of database size.
+                If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+                Otherwise, it will be treated as float.
+                Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+
+            sep : str
+                This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
+                However, the users can override their default separator.
+
+            windowSize : int
+                The size of the sliding window. It specifies the number of panes to be considered for mining frequent patterns.
+
+            paneSize : int
+                The size of the pane. It specifies the number of transactions to be considered for mining frequent patterns in each pane.
+
+            oFile : str
+                The output file name or path
+
+            startTime : float
+                The start time of the mining process
+
+            endTime : float
+                The end time of the mining process
+
+            finalPatterns : dict
+                The dictionary containing the mined frequent patterns from each window.
+
+            memoryUSS : float
+                The memory usage of the program in User Space
+
+            memoryRSS : float
+                The memory usage of the program in Resident Set Size
 
-    **Methods to execute code on terminal**
+            Database : list
+                The list containing the complete transactions of the database/input file
 
-        Format:
-                  >>>  python3 WUFIM.py <inputFile> <outputFile> <minSup>
-        Example:
-                  >>>  python3 WUFIM.py sampleTDB.txt patterns.txt 3
+            tree : CPSTree
+                The CPSTree structure used to mine frequent patterns from the data stream
 
-                 .. note:: minSup  will be considered in support count or frequency
 
-    **Importing this algorithm into a python program**
+        Methods :
+        ---------
+            creatingItemSets()
+                Loads the complete transactions of the database/input file in a database variable.
 
-.. code-block:: python
+            convert(value):
+                Converts the minSup from different formats in absolute count.
 
-        from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
+            getRestructuredTree(tree):
+                Restructures the tree by removing the oldest batch from the tree and updating the new batch in the tree.
 
-        obj = alg.WFIM(iFile, wFile, expSup, expWSup)
+            getBranches(root, restructuredTree, originalTree, curBranch):
+                Gets the branches of the tree and updates it to the restructured tree.
 
-        obj.startMine()
+            printTree():
+                Prints the CPSTree structure.
 
-        Patterns = obj.getPatterns()
+            createPrefixBranch(root):
+                Creates the branches of the prefix tree.
 
-        print("Total number of  Patterns:", len(Patterns))
+            createConditionalTree(root, transactions, minSup):
+                Creates the conditional tree from the prefix tree by removing items with support less than minSup.
 
-        obj.savePatterns(oFile)
+            itemSetGeneration(root, minSup, candidatePattern, curItemset):
+                Generates the frequent itemsets by creating a conditional tree and mining patterns from it.
 
-        Df = obj.getPatternsAsDataFrame()
+            
+            getMemoryRSS():
+                Gets the memory usage of the program in Resident Set Size.
 
-        memUSS = obj.getMemoryUSS()
+            getMemoryUSS():
+                Gets the memory usage of the program in User Space.
 
-        print("Total Memory in USS:", memUSS)
+            getPatterns():
+                Gets the mined frequent patterns from each window.
 
-        memRSS = obj.getMemoryRSS()
+            getPatternsAsDataFrame():
+                Gets the mined frequent patterns from each window as a pandas dataframe.
 
-        print("Total Memory in RSS", memRSS)
+            getRuntime():
+                Gets the runtime of the program.
 
-        run = obj.getRuntime()
+            printResults():
+                Prints the overall stasticts of the mining process.
 
-        print("Total ExecutionTime in seconds:", run)
-   """
-    _startTime = float()
-    _endTime = float()
+            save():
+                Saves the mined frequent patterns in a file.
+
+            startMine():
+                Starts the mining process by loading the input database and creating CPS Tree over each window.
+
+        
+        Executing the code on terminal:
+        -------------------------------
+
+            Format:
+            --------
+                python3 CPSTree.py <inputFile> <outputFile> <minSup> <windowSize> <paneSize> <separator>
+
+            Example:
+            ---------
+
+                python3 CPSTree.py retail.txt output.txt 0.5 100 1000 ',' (Here minimum support is 50% of the database size
+
+        Credits:
+        --------
+
+            The code is written by Vipul Chhabra under the supervision of Prof. Rage Uday Kiran.
+
+    """
+
+    __startTime = float()
+    __endTime = float()
     _minSup = str()
-    _finalPatterns = {}
+    __finalPatterns = {}
     _iFile = " "
-    _wFile = " "
     _oFile = " "
     _sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _Database = []
-    _rank = {}
-    _expSup = float()
-    _expWSup = float()
-
-    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t'):
-        super().__init__(iFile, wFile, expSup, expWSup, sep)
-
-    def _creatingItemSets(self):
-        """
-            Scans the uncertain transactional dataset
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __tree = None
+    __windowSize = 0
+    __paneSize = 0
+
+    def __init__(self, iFile, oFile, minSup, windowSize, paneSize, sep='\t'):
+        super().__init__(iFile, minSup, windowSize, paneSize, sep)
+        self._oFile = oFile
+
+    def __creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+        """
+        self.__Database = []
+        if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
+                self.__Database = self._iFile['Transactions'].tolist()
 
-            # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
-                for line in data:
-                    line = line.decode("utf-8")
-                    line = line.strip()
-                    line = [i for i in line.split(':')]
-                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
-                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
-                    temp1 = [x for x in temp1 if x]
-                    temp2 = [x for x in temp2 if x]
-                    tr = []
-                    for i in range(len(temp1)):
-                        item = temp1[i]
-                        probability = float(temp2[i])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(tr)
-            else:
-                try:
-                    with open(self._iFile, 'r') as f:
-                        for line in f:
-                            line = line.strip()
-                            line = [i for i in line.split(':')]
-                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
-                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
-                            temp1 = [x for x in temp1 if x]
-                            temp2 = [x for x in temp2 if x]
-                            tr = []
-                            for i in range(len(temp1)):
-                                item = temp1[i]
-                                probability = float(temp2[i])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
-                except IOError:
-                    print("File Not Found")
-
-    def _scanningWeights(self):
-        """
-            Scans the uncertain transactional dataset
-        """
-        self._weights = {}
-        if isinstance(self._wFile, _ab._pd.DataFrame):
-            weights, data = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                data = self._wFile['items'].tolist()
-            if 'weights' in i:
-                weights = self._wFile['weights'].tolist()
-            for k in range(len(data)):
-                self._weights[data[k]] = int(float(weights[k]))
-
-            # print(self.Database)
-        if isinstance(self._wFile, str):
-            if _ab._validators.url(self._wFile):
-                data = _ab._urlopen(self._wFile)
+            if _fp._validators.url(self._iFile):
+                data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._weights[temp[0]] = int(float(temp[1]))
+                    self.__Database.append(temp)
             else:
                 try:
-                    with open(self._wFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._weights[temp[0]] = float(temp[1])
+                            self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
-        """takes the self.Database and calculates the support of each item in the dataset and assign the
-            ranks to the items by decreasing support and returns the frequent items list
-                :param self.Database : it represents the one self.Database in database
-                :type self.Database : list
+    def __convert(self, value):
         """
+            to convert the type of user specified minSup value
 
-        mapSupport = {}
-        for i in self._Database:
-            for j in i:
-                if j.item not in mapSupport:
-                    if self._weights.get(j.item) is not None:
-                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
-                else:
-                    mapSupport[j.item][0] += j.probability
-        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
-        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
-        return mapSupport, plist
-
-    @staticmethod
-    def _buildTree(data, info):
-        """it takes the self.Database and support of each item and construct the main tree with setting root
-            node as null
-                :param data : it represents the one self.Database in database
-                :type data : list
-                :param info : it represents the support of each item
-                :type info : dictionary
-        """
-
-        rootNode = _Tree()
-        rootNode.info = info.copy()
-        for i in range(len(data)):
-            rootNode.addTransaction(data[i])
-        return rootNode
-
-    def _updateTransactions(self, dict1):
-        """remove the items which are not frequent from self.Database and updates the self.Database with rank of items
-            :param dict1 : frequent items with support
-            :type dict1 : dictionary
-        """
-
-        list1 = []
-        for tr in self._Database:
-            list2 = []
-            for i in range(0, len(tr)):
-                if tr[i].item in dict1:
-                    list2.append(tr[i])
-            if len(list2) >= 2:
-                basket = list2
-                basket.sort(key=lambda val: self.rank[val.item])
-                list2 = basket
-                list1.append(list2)
-        return list1
-
-    @staticmethod
-    def _check(i, x):
-        """To check the presence of item or pattern in transaction
-                :param x: it represents the pattern
-                :type x : list
-                :param i : represents the uncertain self.Database
-                :type i : list
-        """
-
-        # This method taken a transaction as input and returns the tree
-        for m in x:
-            k = 0
-            for n in i:
-                if m == n.item:
-                    k += 1
-            if k == 0:
-                return 0
-        return 1
-
-    def _convert(self, value):
-        """
-        To convert the type of user specified minSup value
             :param value: user specified minSup value
-            :return: converted type minSup value
+
+            :return: converted type
         """
+
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self._Database) * value)
+            value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
-                value = (len(self._Database) * value)
+                value = float(value)
+                value = (self.__paneSize * self.__windowSize * value)
             else:
                 value = int(value)
         return value
+    
+    def getRestructuredTree(self,tree):
+        """
+            Restructures the tree by removing the oldest batch from the tree and updating the new batch in the tree.
 
-    def _removeFalsePositives(self):
+            :param tree: Existing CPSTree object to be restructured
+            
+            :return: restructuredTree: CPSTree object after performing branch sorting
         """
-            To remove the false positive patterns generated in frequent patterns
-            :return: patterns with accurate probability
+        restructuredTree = _CPSTree(tree.windowSize, tree.paneSize)
+        self.getBranches(tree.root, restructuredTree, tree)
+        restructuredTree.curBatchIndex = tree.curBatchIndex
+        return restructuredTree
+
+    def getBranches(self,root, restructuredTree, origTree, curBranch = []):
         """
-        global _finalPatterns
-        periods = {}
-        for i in self._Database:
-            for x, y in _finalPatterns.items():
-                if len(x) == 1:
-                    periods[x] = y
-                else:
-                    s = 1
-                    check = self._check(i, x)
-                    if check == 1:
-                        for j in i:
-                            if j.item in x:
-                                s *= j.probability
-                        if x in periods:
-                            periods[x] += s
-                        else:
-                            periods[x] = s
-        for x, y in periods.items():
-            weight = 0
-            for i in x:
-                weight += self._weights[i]
-            weight = weight / len(x)
-            if weight * y >= self._expWSup:
-                sample = str()
-                for i in x:
-                    sample = sample + i + "\t"
-                self._finalPatterns[sample] = y
+            Gets the branches of the tree and updates it to the restructured tree.
 
-    def startMine(self):
-        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
-            by counting the original support of a patterns
+            :param root: CPSTreeNode object for the root of the original tree
+            :param restructuredTree: CPSTree object
+            :param origTree: CPSTree object for the original tree
+            :param curBranch: list of CPSTreeNode objects that needs to be sorted
         """
-        global _expSup, _expWSup, _weights, _finalPatterns
-        self._startTime = _ab._time.time()
-        self._Database, self._weights = [], {}
-        self._creatingItemSets()
-        self._scanningWeights()
-        _weights = self._weights
-        self._expSup = float(self._expSup)
-        self._expWSup = float(self._expWSup)
-        _expSup = self._expSup
-        _expWSup = self._expWSup
-        self._finalPatterns = {}
-        mapSupport, plist = self._frequentOneItem()
-        self.Database1 = self._updateTransactions(mapSupport)
-        info = {k: v for k, v in mapSupport.items()}
-        Tree1 = self._buildTree(self.Database1, info)
-        Tree1.generatePatterns([])
-        self._removeFalsePositives()
-        print("Weighted Frequent patterns were generated  successfully using WUFIM algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
-        self.memoryRSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self.memoryRSS = process.memory_info().rss
 
-    def getMemoryUSS(self):
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
-        :return: returning USS memory consumed by the mining process
-        :rtype: float
+        if(root is None):
+            return
+
+        for childItem in root.children:
+            updatedBranch = curBranch.copy()
+            updatedBranch.append(root.children[childItem])
+            self.getBranches(root.children[childItem], restructuredTree, origTree, updatedBranch)
+
+        if(len(root.children) == 0 or root.tail is not None):
+            finalBranch = curBranch.copy()
+            supportCount = {}
+
+            for node in finalBranch:
+                supportCount[node.itemId] = sum(finalBranch[-1].tail)
+
+            curTrans = [node.itemId for node in finalBranch]
+            curTrans = origTree.headerTable.orderTransaction(curTrans)
+            restructuredTree.addTransaction(curTrans, restructuring=True, supportValue=supportCount, tailNode = finalBranch[-1].tail)
+    
+    def printTree(self, root, level = 0):
+        """
+            Prints the tree in a readable format.
+
+            :param root: CPSTreeNode object for the root of the tree
+            :param level: Current level of the root node
+        """
+
+        print('  ' * level, level, root.itemId, root.counter, root.parent.itemId if root.parent else None )
+        
+        if(len(root.children) == 0 or root.tail != None):
+            print('  ' * (level + 1), level + 1, root.tail)
+        
+        for child in root.children.values():
+            self.printTree(child, level + 1)
+
+    def createPrefixBranch(self, root):
+        """
+            Creates the prefix branch for the given node.
+
+            :param root: CPSTreeNode object for the root of the tree
+
+            :return: prefixBranch: list of CPSTreeNode objects for the prefix branch
+        """
+
+        stack = []
+        while(root is not None):
+            stack.append(root)
+            root = root.parent
+
+        chosenItemset = stack[0]
+        lastSupport = chosenItemset.counter
+        return stack, lastSupport
+
+    def createConditionalTree(self, root, transactions, minSupport):
+        """
+            Creates the conditional tree for the given node.
+
+            :param root: CPSTreeNode object for the root of the tree for which conditional tree needs to be created
+            :param transactions: list of transactions which needs to be added to the conditional tree
+            :param minSupport: minimum support value for the conditional tree
+
+            :return: conditionalTree: CPSTree object for the conditional tree
+        """    
+    
+        for transaction in transactions:
+            for item in transaction["transaction"]:
+                if root.headerTable.table[item][0] < minSupport:
+                    transaction["transaction"].remove(item)
+
+        conditionalTree = _CPSTree(1, 1)
+
+        for transaction in transactions:
+            if(len(transaction["transaction"]) > 0):
+                conditionalTree.addTransaction(transaction["transaction"], restructuring=True, supportValue=transaction["support"])
+
+        return conditionalTree      
+
+    def itemSetGeneration(self, root, minSupport, candidatePattern, curItem = []):
+
+        """
+            Generates the candidate patterns for the given CPS Tree.
+
+            :param root: CPSTreeNode object for the root of the tree for which itemset needs to be generated
+            :param minSupport: minimum support value for the conditional tree
+            :param candidatePattern: list of candidate patterns generated
+            :param curItem: list of CPSTreeNode objects for the current itemset
+
+            :return: candidatePattern: list of candidate patterns
         """
+        if(root is None or root.root is None):
+            return
+
+        for item in root.headerTable.orderedItems:
+            if root.headerTable.table[item][0] >= minSupport:
+                prefixBranches = []
+                tempNode = root.headerTable.table[item][1]
+
+                while(tempNode is not None):
+                    curPrefixBranch, netSupport = self.createPrefixBranch(tempNode)
+                    tempBranch = [node.itemId for node in curPrefixBranch]
+                    supportCount = {}
+                    for each_item_node in curPrefixBranch:
+                        supportCount[each_item_node.itemId] = netSupport
+
+                    prefixBranches.append([tempBranch, supportCount])
+                    tempNode = tempNode.next
+
+                prefixTree = _CPSTree(1, 1)
+                completeTransactions = []
+
+                for branch in prefixBranches:
+                    transaction = []
+                    for nodeIndex in range(len(branch[0])-2,0,-1):
+                        transaction.append(branch[0][nodeIndex])
+                    
+                    prefixTree.addTransaction(transaction, restructuring=True, supportValue=branch[1])
+                    completeTransactions.append({"transaction": transaction, "support": branch[1]})
+
+                conditionalTree = self.createConditionalTree(prefixTree, completeTransactions, minSupport)
+                newItemset = curItem.copy()
+                newItemset.append(item)
+
+                if(len(newItemset) not in candidatePattern):
+                    candidatePattern[len(newItemset)] = [{"pattern" : newItemset, "support" : root.headerTable.table[item][0]}]
+
+                else:
+                    candidatePattern[len(newItemset)].append({"pattern" : newItemset, "support" : root.headerTable.table[item][0]})
+
+                if(len(conditionalTree.headerTable.table) > 0):
+                    self.itemSetGeneration(conditionalTree, minSupport, candidatePattern, newItemset)
 
-        return self._memoryUSS
 
     def getMemoryRSS(self):
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-        :return: returning RSS memory consumed by the mining process
-        :rtype: float
         """
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
-        return self.memoryRSS
+            :return: returning RSS memory consumed by the mining process
 
-    def getRuntime(self):
-        """Calculating the total amount of runtime taken by the mining process
-        :return: returning total amount of runtime taken by the mining process
-        :rtype: float
+            :rtype: float
         """
+        return self.__memoryRSS
+
+    def getMemoryUSS(self):
+        """
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-        return self._endTime - self._startTime
+            :return: returning USS memory consumed by the mining process
+
+            :rtype: float
+        """
+        return self.__memoryUSS
+
+    def getPatterns(self):
+        """
+            Returns the frequent patterns generated by the mining process over the complete datastream.
+
+            :return: returning frequent patterns generated by the mining process
+
+            :rtype: dict
+        """
+        return self.__finalPatterns
 
     def getPatternsAsDataFrame(self):
-        """Storing final frequent patterns in a dataframe
-        :return: returning frequent patterns in a dataframe
-        :rtype: pd.DataFrame
+        """
+            Stores the final patterns generated by the mining process in a dataframe.
+
+            :return: returning dataframe containing the final patterns generated by the mining process
+
+            :rtype: pandas.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
-            s = str()
-            for i in a:
-                s = s + i + " "
-            data.append([s, b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        for x, y in self.__finalPatterns.items():
+            for pattern in y:
+                patternString = ' '.join(pattern[0])
+                data.append([x[0], x[1], patternString, pattern[1]])
+        dataframe = _fp._pd.DataFrame(data, columns=['Window Start Index', 'Window End Index', 'Pattern', 'Support'])
         return dataframe
 
-    def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
-        :param outFile: name of the output file
-        :type outFile: file
-        """
-        self.oFile = outFile
-        writer = open(self.oFile, 'w+')
-        for x, y in self._finalPatterns.items():
-            s = str()
-            for i in x:
-                s = s + i + "\t"
-            s1 = s.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+    def getRuntime(self):
+        """
+            Total amount of time taken by the mining process will be retrieved from this function
 
-    def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
-        :return: returning frequent patterns
-        :rtype: dict
+            :return: returning time taken by the mining process
+
+            :rtype: float
         """
-        return self._finalPatterns
+
+        return self.__endTime - self.__startTime
 
     def printResults(self):
-        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
+        """
+            Prints the stats of the mining process
+
+        """
+        print("Total number of Windows Processed:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
+
+
+    def save(self):
+        """
+        Complete set of frequent patterns will be loaded in to a output file
+        """
+
+        writer = open(self._oFile, 'w+')
+        for x, y in self.__finalPatterns.items():
+            writer.write("Window Start Index : %s , End Index : %s \n" % (x[0], x[1]))
+            for pattern in y:
+                patternString = '\t'.join(pattern[0])
+                patternString += '\t' + ":" + '\t' + str(pattern[1])
+                writer.write("%s \n" % patternString)
+
+    def startMine(self):
+        """
+            This function will start the mining process
+        """
+        global _minSup
+        self.__startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        if self._windowSize is None:
+            raise Exception("Please enter the Window Size")
+        if self._paneSize is None:
+            raise Exception("Please enter the Pane Size")
+        self.__windowSize = int(self._windowSize)
+        self.__paneSize = int(self._paneSize)
+
+        self.__creatingItemSets()
+        self._minSup = self.__convert(self._minSup)
+        self.__tree = _CPSTree(self.__windowSize, self.__paneSize)
+
+        for i in range(0, self.__windowSize):
+            self.__tree.curBatchIndex = i
+            for j in range(0, self.__paneSize):
+                    self.__tree.addTransaction(self.__Database[i * self.__paneSize + j])
+            self.__tree = self.getRestructuredTree(self.__tree)
+
+
+        startIndex = 0
+        endIndex = self.__windowSize * self.__paneSize
+
+        while endIndex <= len(self.__Database):
+            print("Start Index: ", startIndex, "End Index: ", endIndex)
+            self.printTree(self.__tree.root)
+
+            patterns = {}
+            self.itemSetGeneration(self.__tree, self._minSup, patterns)
+
+            for patternLength in patterns:
+                for pattern in patterns[patternLength]:
+
+                    if((startIndex, endIndex) not in self.__finalPatterns):
+                        self.__finalPatterns[(startIndex, endIndex)] = []
+                    self.__finalPatterns[(startIndex, endIndex)].append((pattern["pattern"], pattern["support"]))
+
+            if(endIndex == len(self.__Database)):
+                break
+
+            self.__tree.removeBatch()
+
+            for i in range(0, self.__paneSize):
+                    self.__tree.addTransaction(self.__Database[endIndex + i])
+
+            self.__tree = self.getRestructuredTree(self.__tree)
+            startIndex += self.__paneSize
+            endIndex += self.__paneSize
+
+
+
+        self.__endTime = _fp._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
+
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
-        if len(_ab._sys.argv) == 7:
-            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
-        if len(_ab._sys.argv) == 6:
-            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
+        if len(_fp._sys.argv) == 7:
+            _ap = FrequentPatternStreamMining(_fp._sys.argv[1], _fp._sys.argv[2], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 6:
+            _ap = FrequentPatternStreamMining(_fp._sys.argv[1], _fp._sys.argv[2], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
+        print("Total number of Frequent Patterns:", len( _ap.getPatterns()))
+
+        print(_ap.getPatternsAsDataFrame().to_csv("result.csv", index = False, sep='\t'))
+        _ap.save()
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        for k in [120, 140, 160, 180, 200]:
-            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
-                        k, 500, '\t')
-            _ap.startMine()
-            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
-            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
-            print("Total Memory in USS:", _ap.getMemoryUSS())
-            print("Total Memory in RSS", _ap.getMemoryRSS())
-            print("Total ExecutionTime in ms:", _ap.getRuntime())
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.27/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.27/PKG-INFO` & `pami-2023.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.7.27
+Version: 2023.7.7
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayLab/PAMI
+Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: spark
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -39,21 +37,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -79,112 +77,112 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                               |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md) |
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
 | RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
@@ -314,36 +312,20 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__   
      
      
+
+
```

### Comparing `pami-2023.7.27/README.md` & `pami-2023.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -19,21 +18,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -59,112 +58,112 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                               |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md) |
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
 | RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
@@ -294,36 +293,18 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__
```

### Comparing `pami-2023.7.27/pami.egg-info/PKG-INFO` & `pami-2023.7.7/pami.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.7.27
+Version: 2023.7.7
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayLab/PAMI
+Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: spark
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -39,21 +37,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -79,112 +77,112 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                               |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md) |
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
 | RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
@@ -314,36 +312,20 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__   
      
      
+
+
```

### Comparing `pami-2023.7.27/pami.egg-info/SOURCES.txt` & `pami-2023.7.7/pami.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 PAMI/AssociationRules/basic/ARWithConfidence.py
 PAMI/AssociationRules/basic/ARWithLeverage.py
 PAMI/AssociationRules/basic/ARWithLift.py
 PAMI/AssociationRules/basic/RuleMiner.py
 PAMI/AssociationRules/basic/__init__.py
 PAMI/AssociationRules/basic/abstract.py
 PAMI/correlatedPattern/__init__.py
-PAMI/correlatedPattern/basic/CoMine.py
-PAMI/correlatedPattern/basic/CoMinePlus.py
+PAMI/correlatedPattern/basic/CPGrowth.py
+PAMI/correlatedPattern/basic/CPGrowthPlus.py
 PAMI/correlatedPattern/basic/__init__.py
 PAMI/correlatedPattern/basic/abstract.py
-PAMI/coveragePattern/__init__.py
-PAMI/coveragePattern/basic/CMine.py
-PAMI/coveragePattern/basic/CPPG.py
-PAMI/coveragePattern/basic/__init__.py
-PAMI/coveragePattern/basic/abstract.py
+PAMI/coveragePatterns/__init__.py
+PAMI/coveragePatterns/basic/CMine.py
+PAMI/coveragePatterns/basic/CPPG.py
+PAMI/coveragePatterns/basic/__init__.py
+PAMI/coveragePatterns/basic/abstract.py
 PAMI/extras/__init__.py
 PAMI/extras/generateLatexGraphFile.py
 PAMI/extras/plotPointOnMap.py
 PAMI/extras/plotPointOnMap_dump.py
 PAMI/extras/scatterPlotSpatialPoints.py
 PAMI/extras/topKPatterns.py
 PAMI/extras/uncertaindb_convert.py
@@ -61,27 +61,27 @@
 PAMI/extras/graph/plotLineGraphsFromDataFrame.py
 PAMI/extras/graph/visualizePatterns.py
 PAMI/extras/image2Database/__init__.py
 PAMI/extras/imageProcessing/__init__.py
 PAMI/extras/imageProcessing/imagery2Databases.py
 PAMI/extras/neighbours/__init__.py
 PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
-PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
 PAMI/extras/syntheticDatabaseGenerator/__init__.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
 PAMI/faultTolerantFrequentPattern/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
 PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
 PAMI/faultTolerantFrequentPattern/basic/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/abstract.py
 PAMI/frequentPattern/__init__.py
 PAMI/frequentPattern/basic/Apriori.py
 PAMI/frequentPattern/basic/ECLAT.py
 PAMI/frequentPattern/basic/ECLATDiffset.py
 PAMI/frequentPattern/basic/ECLATbitset.py
@@ -107,74 +107,73 @@
 PAMI/frequentPattern/pyspark/abstract.py
 PAMI/frequentPattern/pyspark/parallelApriori.py
 PAMI/frequentPattern/pyspark/parallelECLAT.py
 PAMI/frequentPattern/pyspark/parallelFPGrowth.py
 PAMI/frequentPattern/topk/FAE.py
 PAMI/frequentPattern/topk/__init__.py
 PAMI/frequentPattern/topk/abstract.py
+PAMI/frequentSpatialPattern/__init__.py
+PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+PAMI/frequentSpatialPattern/basic/__init__.py
+PAMI/frequentSpatialPattern/basic/abstract.py
 PAMI/fuzzyCorrelatedPattern/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
 PAMI/fuzzyCorrelatedPattern/basic/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-PAMI/fuzzyFrequentPattern/__init__.py
-PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
-PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
-PAMI/fuzzyFrequentPattern/basic/__init__.py
-PAMI/fuzzyFrequentPattern/basic/abstract.py
+PAMI/fuzzyFrequentPatterns/__init__.py
+PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+PAMI/fuzzyFrequentPatterns/basic/__init__.py
+PAMI/fuzzyFrequentPatterns/basic/abstract.py
 PAMI/fuzzyFrequentSpatialPattern/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
 PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-PAMI/fuzzyPartialPeriodicPattern/__init__.py
-PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/__init__.py
-PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py
+PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
 PAMI/fuzzyPeriodicFrequentPattern/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+PAMI/geoReferencedFrequentPattern/__init__.py
+PAMI/geoReferencedFrequentPattern/abstract.py
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
-PAMI/highUtilityFrequentPattern/__init__.py
-PAMI/highUtilityFrequentPattern/basic/HUFIM.py
-PAMI/highUtilityFrequentPattern/basic/__init__.py
-PAMI/highUtilityFrequentPattern/basic/abstract.py
+PAMI/highUtilityFrequentPatterns/__init__.py
+PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+PAMI/highUtilityFrequentPatterns/basic/__init__.py
+PAMI/highUtilityFrequentPatterns/basic/abstract.py
 PAMI/highUtilityFrequentSpatialPattern/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
 PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-PAMI/highUtilityPattern/__init__.py
-PAMI/highUtilityPattern/basic/EFIM.py
-PAMI/highUtilityPattern/basic/HMiner.py
-PAMI/highUtilityPattern/basic/UPGrowth.py
-PAMI/highUtilityPattern/basic/__init__.py
-PAMI/highUtilityPattern/basic/abstract.py
-PAMI/highUtilityPattern/basic/efimParallel.py
-PAMI/highUtilityPattern/parallel/__init__.py
-PAMI/highUtilityPattern/parallel/abstract.py
-PAMI/highUtilityPattern/parallel/efimparallel.py
-PAMI/highUtilityPatternsInStreams/HUPMS.py
-PAMI/highUtilityPatternsInStreams/SHUGrowth.py
-PAMI/highUtilityPatternsInStreams/__init__.py
-PAMI/highUtilityPatternsInStreams/abstract.py
+PAMI/highUtilityPatterns/__init__.py
+PAMI/highUtilityPatterns/basic/EFIM.py
+PAMI/highUtilityPatterns/basic/HMiner.py
+PAMI/highUtilityPatterns/basic/UPGrowth.py
+PAMI/highUtilityPatterns/basic/__init__.py
+PAMI/highUtilityPatterns/basic/abstract.py
+PAMI/highUtilityPatterns/basic/efimParallel.py
+PAMI/highUtilityPatterns/parallel/__init__.py
+PAMI/highUtilityPatterns/parallel/abstract.py
+PAMI/highUtilityPatterns/parallel/efimparallel.py
 PAMI/highUtilitySpatialPattern/__init__.py
 PAMI/highUtilitySpatialPattern/abstract.py
 PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
 PAMI/highUtilitySpatialPattern/basic/SHUIM.py
 PAMI/highUtilitySpatialPattern/basic/__init__.py
 PAMI/highUtilitySpatialPattern/basic/abstract.py
 PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
@@ -248,23 +247,22 @@
 PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
 PAMI/recurringPattern/__init__.py
 PAMI/recurringPattern/basic/RPGrowth.py
 PAMI/recurringPattern/basic/__init__.py
 PAMI/recurringPattern/basic/abstract.py
-PAMI/relativeFrequentPattern/__init__.py
-PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
-PAMI/relativeFrequentPattern/basic/__init__.py
-PAMI/relativeFrequentPattern/basic/abstract.py
-PAMI/relativeHighUtilityPattern/__init__.py
-PAMI/relativeHighUtilityPattern/basic/RHUIM.py
-PAMI/relativeHighUtilityPattern/basic/__init__.py
-PAMI/relativeHighUtilityPattern/basic/abstract.py
-PAMI/sequence/__init__.py
+PAMI/relativeFrequentPatterns/__init__.py
+PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+PAMI/relativeFrequentPatterns/basic/__init__.py
+PAMI/relativeFrequentPatterns/basic/abstract.py
+PAMI/relativeHighUtilityPatterns/__init__.py
+PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+PAMI/relativeHighUtilityPatterns/basic/__init__.py
+PAMI/relativeHighUtilityPatterns/basic/abstract.py
 PAMI/sequentialPatternMining/__init__.py
 PAMI/sequentialPatternMining/basic/SPADE.py
 PAMI/sequentialPatternMining/basic/__init__.py
 PAMI/sequentialPatternMining/basic/abstract.py
 PAMI/sequentialPatternMining/basic/prefixSpan.py
 PAMI/sequentialPatternMining/closed/__init__.py
 PAMI/sequentialPatternMining/closed/abstract.py
@@ -274,31 +272,33 @@
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
 PAMI/stablePeriodicFrequentPattern/basic/__init__.py
 PAMI/stablePeriodicFrequentPattern/basic/abstract.py
 PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
 PAMI/stablePeriodicFrequentPattern/topK/__init__.py
 PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
-PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
-PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+PAMI/streams/__init__.py
+PAMI/streams/frequentPatterns/__init__.py
+PAMI/streams/frequentPatterns/basic/FPStream.py
+PAMI/streams/frequentPatterns/basic/__init__.py
+PAMI/streams/frequentPatterns/basic/abstract.py
+PAMI/streams/highUtility/HUPMS.py
+PAMI/streams/highUtility/SHUGrowth.py
+PAMI/streams/highUtility/__init__.py
+PAMI/streams/highUtility/abstract.py
 PAMI/uncertainFrequentPattern/__init__.py
 PAMI/uncertainFrequentPattern/basic/CUFPTree.py
 PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
 PAMI/uncertainFrequentPattern/basic/TUFP.py
 PAMI/uncertainFrequentPattern/basic/TubeP.py
 PAMI/uncertainFrequentPattern/basic/TubeS.py
 PAMI/uncertainFrequentPattern/basic/UFGrowth.py
 PAMI/uncertainFrequentPattern/basic/UVECLAT.py
 PAMI/uncertainFrequentPattern/basic/__init__.py
 PAMI/uncertainFrequentPattern/basic/abstract.py
-PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
-PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
-PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
 PAMI/uncertainPeriodicFrequentPattern/__init__.py
 PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
 PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
 PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
 PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
 PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
 PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
```

### Comparing `pami-2023.7.27/setup.py` & `pami-2023.7.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='pami',
-    version='2023.07.27',
-    author='Rage Uday Kiran',
-    author_email='uday.rage@gmail.com',
-    description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    name = 'pami',
+    version = '2023.07.07',
+    author = 'Rage Uday Kiran',
+    author_email = 'uday.rage@gmail.com',
+    description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
     packages=setuptools.find_packages(),
-    url='https://github.com/udayLab/PAMI',
+    url = 'https://github.com/udayRage/PAMI',
     license='GPLv3',
     install_requires=[            # All necessary packages utilized by our PAMI software
         'psutil',
         'pandas',
         'plotly',
         'matplotlib',
         'resource',
         'validators',
         'urllib3',
         'Pillow',
         'numpy',
     ],
-    extras_require={
-        'gpu':  ['cupy', 'pycuda'],
+    extras_require = {
+        'gpu':  ['cupy'],
         'spark': ['pyspark'],
-        'dev': ['twine', 'setuptools', 'build'],
-        'all': ['cupy', 'pycuda', 'pyspark', 'twine', 'setuptools', 'build']
     },
-    classifiers=[
+    classifiers = [
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.5',
+    python_requires = '>=3.5',
 )
```

