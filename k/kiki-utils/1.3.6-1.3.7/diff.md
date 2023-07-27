# Comparing `tmp/kiki_utils-1.3.6-py3-none-any.whl.zip` & `tmp/kiki_utils-1.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 11048 bytes, number of entries: 22
+Zip file size: 11733 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx       13 b- defN 22-Nov-28 02:36 kikiutils/__init__.py
 -rw-rw-r--  2.0 unx     1936 b- defN 23-Jul-20 05:43 kikiutils/aes.py
+-rw-rw-r--  2.0 unx     1177 b- defN 23-Jul-27 14:29 kikiutils/aio.py
 -rw-rw-r--  2.0 unx     1863 b- defN 23-Jul-20 07:26 kikiutils/aiofile.py
 -rw-rw-r--  2.0 unx     1901 b- defN 23-Jul-21 11:16 kikiutils/check.py
 -rw-rw-r--  2.0 unx      188 b- defN 22-Nov-28 02:36 kikiutils/cookie.py
 -rw-rw-r--  2.0 unx     4130 b- defN 23-Jul-20 10:58 kikiutils/decorators.py
 -rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-20 07:48 kikiutils/file.py
 -rw-rw-r--  2.0 unx      795 b- defN 23-Jul-20 06:43 kikiutils/hash.py
 -rw-rw-r--  2.0 unx      152 b- defN 22-Nov-28 02:36 kikiutils/import_utils.py
 -rw-rw-r--  2.0 unx      979 b- defN 23-Feb-04 08:44 kikiutils/json.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-28 02:36 kikiutils/log.py
 -rw-rw-r--  2.0 unx      528 b- defN 23-Jul-20 05:28 kikiutils/network.py
 -rw-rw-r--  2.0 unx     1314 b- defN 23-Jul-20 07:02 kikiutils/string.py
 -rw-rw-r--  2.0 unx     1599 b- defN 23-Jul-20 05:39 kikiutils/time.py
 -rw-rw-r--  2.0 unx      198 b- defN 23-Jul-20 10:58 kikiutils/typehint.py
 -rw-rw-r--  2.0 unx      592 b- defN 23-Feb-04 08:36 kikiutils/uuid.py
--rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      523 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1698 b- defN 23-Jul-21 11:17 kiki_utils-1.3.6.dist-info/RECORD
-22 files, 22415 bytes uncompressed, 8322 bytes compressed:  62.9%
+-rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      523 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1771 b- defN 23-Jul-27 14:30 kiki_utils-1.3.7.dist-info/RECORD
+23 files, 23665 bytes uncompressed, 8899 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: kikiutils/__init__.py
 Comment: 
 
 Filename: kikiutils/aes.py
 Comment: 
 
+Filename: kikiutils/aio.py
+Comment: 
+
 Filename: kikiutils/aiofile.py
 Comment: 
 
 Filename: kikiutils/check.py
 Comment: 
 
 Filename: kikiutils/cookie.py
@@ -42,26 +45,26 @@
 
 Filename: kikiutils/typehint.py
 Comment: 
 
 Filename: kikiutils/uuid.py
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/LICENSE.txt
+Filename: kiki_utils-1.3.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/METADATA
+Filename: kiki_utils-1.3.7.dist-info/METADATA
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/WHEEL
+Filename: kiki_utils-1.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/top_level.txt
+Filename: kiki_utils-1.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/zip-safe
+Filename: kiki_utils-1.3.7.dist-info/zip-safe
 Comment: 
 
-Filename: kiki_utils-1.3.6.dist-info/RECORD
+Filename: kiki_utils-1.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `kiki_utils-1.3.6.dist-info/LICENSE.txt` & `kiki_utils-1.3.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kiki_utils-1.3.6.dist-info/METADATA` & `kiki_utils-1.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiki-utils
-Version: 1.3.6
+Version: 1.3.7
 Summary: Utils decorators and functions.
 Author: kiki-kanri
 Author-email: a470666@gmail.com
 Keywords: Utils
 Classifier: License :: Freely Distributable
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

## Comparing `kiki_utils-1.3.6.dist-info/RECORD` & `kiki_utils-1.3.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 kikiutils/__init__.py,sha256=da1PTClDMl-IBkrSvq6JC1lnS-K_BASzCvxVhNxN5Ls,13
 kikiutils/aes.py,sha256=urxcDD2UdTVMoV6DAOCxlHKsOizwvPNU3u_OIUksmQU,1936
+kikiutils/aio.py,sha256=-CT6Q4r1vVNFS4HBYwtNczCmSNqyjxncraJ66PLxHkQ,1177
 kikiutils/aiofile.py,sha256=98j0FrCaymm39tg1QE_U-6wYYeuSzPK5AG75NQtX78U,1863
 kikiutils/check.py,sha256=RQRs_1jjQS1wfyBKTejjl3vwhJS11uO3MSlz_gSqG4g,1901
 kikiutils/cookie.py,sha256=8Jc89wG4Pc3qNvJ-wKK013H90Z4Xpu0Zms-wYuO9j1w,188
 kikiutils/decorators.py,sha256=bwtiRPohIwSpW65S4FuKfWcJd7oumzDcoxmXqbOHkm4,4130
 kikiutils/file.py,sha256=_Jqhl5F9zHQ9GtPqYpzDrlwMvFS9f2TpIVSJThIUBGk,2524
 kikiutils/hash.py,sha256=xGenudRNROQsv6mRDWHNVMYmmCBd-fpLFCvA9EdRs64,795
 kikiutils/import_utils.py,sha256=5beGSUNbLgVPeNFHhx4mtHd_ZfaToA30x1e-egVYWq8,152
 kikiutils/json.py,sha256=Kyx8gzBcZlNrkF5s-JIH6PY0Er18-yQepkyD432atFg,979
 kikiutils/log.py,sha256=6WRAJHjHZjy5x9VfZDf2eWYKJeKSMq3REVJFcYldaMg,313
 kikiutils/network.py,sha256=HuhfdXuDVurGnK1jUwI3iDjcOZsp0t1LraTyh4Y52t8,528
 kikiutils/string.py,sha256=ip-KqIlYlQ2fQEAA0N7I08UfCSLanWlD_LnC1ltu4qg,1314
 kikiutils/time.py,sha256=ohSx7bOJpKaEwjTn0u1KOPZnL1N3fbg2JtLBOOWTzQk,1599
 kikiutils/typehint.py,sha256=csMxrDzL6iriowsU3gHenh226J2jeJi8NIBz-xNUCoM,198
 kikiutils/uuid.py,sha256=_yyp066EcV50ntnQ6BPIp13iQ_BZ0-nUTZQWhtF3lZk,592
-kiki_utils-1.3.6.dist-info/LICENSE.txt,sha256=dUmbJv0OZ9sNGEU_yKnUKiveA25barKmv-QMSqgLZE4,1066
-kiki_utils-1.3.6.dist-info/METADATA,sha256=NREyfdDr0BD-G48vlRoZT0NEZhBtN8A47k69ELRdPL0,523
-kiki_utils-1.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kiki_utils-1.3.6.dist-info/top_level.txt,sha256=jEtWoUBSu5QZTt0S7gB72vYd_uXbvJcs9MhF2enTwoQ,10
-kiki_utils-1.3.6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kiki_utils-1.3.6.dist-info/RECORD,,
+kiki_utils-1.3.7.dist-info/LICENSE.txt,sha256=dUmbJv0OZ9sNGEU_yKnUKiveA25barKmv-QMSqgLZE4,1066
+kiki_utils-1.3.7.dist-info/METADATA,sha256=svMzqi4os_97JXBDcUXP5lYlStEwU0iLWFteiaSRXOU,523
+kiki_utils-1.3.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kiki_utils-1.3.7.dist-info/top_level.txt,sha256=jEtWoUBSu5QZTt0S7gB72vYd_uXbvJcs9MhF2enTwoQ,10
+kiki_utils-1.3.7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+kiki_utils-1.3.7.dist-info/RECORD,,
```

