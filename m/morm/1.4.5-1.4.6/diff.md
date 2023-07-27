# Comparing `tmp/morm-1.4.5-py3-none-any.whl.zip` & `tmp/morm-1.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 40707 bytes, number of entries: 23
+Zip file size: 40705 bytes, number of entries: 23
 -rw-r--r--  2.0 unx       50 b- defN 21-Apr-08 08:46 morm/__init__.py
 -rw-r--r--  2.0 unx     1893 b- defN 21-Apr-08 08:46 morm/admin.py
 -rw-r--r--  2.0 unx      636 b- defN 21-Apr-08 08:54 morm/datetime.py
 -rw-r--r--  2.0 unx    37130 b- defN 21-Apr-15 13:20 morm/db.py
 -rw-r--r--  2.0 unx      470 b- defN 21-Apr-08 08:46 morm/exceptions.py
 -rw-r--r--  2.0 unx     2915 b- defN 21-Apr-08 08:46 morm/meta.py
 -rw-r--r--  2.0 unx    22039 b- defN 21-Jul-21 14:32 morm/migration.py
 -rw-r--r--  2.0 unx    20820 b- defN 21-Jul-21 14:32 morm/model.py
 -rw-r--r--  2.0 unx     1015 b- defN 21-Apr-08 08:54 morm/pg_models.py
 -rw-r--r--  2.0 unx      681 b- defN 21-Apr-08 08:46 morm/q.py
 -rw-r--r--  2.0 unx     2097 b- defN 21-Apr-08 08:46 morm/types.py
 -rw-r--r--  2.0 unx      960 b- defN 21-Jul-21 14:59 morm/utils.py
--rw-r--r--  2.0 unx       89 b- defN 23-Jul-27 06:25 morm/version.py
+-rw-r--r--  2.0 unx       89 b- defN 23-Jul-27 06:29 morm/version.py
 -rw-r--r--  2.0 unx       26 b- defN 21-Apr-08 08:46 morm/fields/__init__.py
 -rw-r--r--  2.0 unx     1968 b- defN 21-Apr-08 08:54 morm/fields/common.py
 -rw-r--r--  2.0 unx    15604 b- defN 21-Jul-21 14:32 morm/fields/field.py
--rwxr-xr-x  2.0 unx     2357 b- defN 23-Jul-27 06:10 morm-1.4.5.data/scripts/init_fap
--rwxr-xr-x  2.0 unx       78 b- defN 23-Jul-27 06:26 morm-1.4.5.data/scripts/morm_admin
--rw-rw-r--  2.0 unx     1703 b- defN 23-Jul-27 06:26 morm-1.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    13464 b- defN 23-Jul-27 06:26 morm-1.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 06:26 morm-1.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 06:26 morm-1.4.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1701 b- defN 23-Jul-27 06:26 morm-1.4.5.dist-info/RECORD
-23 files, 127793 bytes uncompressed, 38025 bytes compressed:  70.2%
+-rwxr-xr-x  2.0 unx     2353 b- defN 23-Jul-27 06:28 morm-1.4.6.data/scripts/init_fap
+-rwxr-xr-x  2.0 unx       78 b- defN 23-Jul-27 06:29 morm-1.4.6.data/scripts/morm_admin
+-rw-rw-r--  2.0 unx     1703 b- defN 23-Jul-27 06:29 morm-1.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13464 b- defN 23-Jul-27 06:29 morm-1.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 06:29 morm-1.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 06:29 morm-1.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1701 b- defN 23-Jul-27 06:29 morm-1.4.6.dist-info/RECORD
+23 files, 127789 bytes uncompressed, 38023 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -42,29 +42,29 @@
 
 Filename: morm/fields/common.py
 Comment: 
 
 Filename: morm/fields/field.py
 Comment: 
 
-Filename: morm-1.4.5.data/scripts/init_fap
+Filename: morm-1.4.6.data/scripts/init_fap
 Comment: 
 
-Filename: morm-1.4.5.data/scripts/morm_admin
+Filename: morm-1.4.6.data/scripts/morm_admin
 Comment: 
 
-Filename: morm-1.4.5.dist-info/LICENSE
+Filename: morm-1.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: morm-1.4.5.dist-info/METADATA
+Filename: morm-1.4.6.dist-info/METADATA
 Comment: 
 
-Filename: morm-1.4.5.dist-info/WHEEL
+Filename: morm-1.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: morm-1.4.5.dist-info/top_level.txt
+Filename: morm-1.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: morm-1.4.5.dist-info/RECORD
+Filename: morm-1.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## morm/version.py

```diff
@@ -1,3 +1,3 @@
 
-__version_info__ = (1, 4, 5)
+__version_info__ = (1, 4, 6)
 __version__ = '.'.join([str(x) for x in __version_info__])
```

## Comparing `morm-1.4.5.data/scripts/init_fap` & `morm-1.4.6.data/scripts/init_fap`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 app.include_router(
     routers.router,
     prefix='/v1',
     tags=['v1'],
 )
 "
     ["$root/core/settings.py"]="
-    DEBUG = True
+DEBUG = True
 "
     ["$root/v1/routers/__init__.py"]="
 '''Make a single APIRouter that contains all the routers.
 
 We will automatically include all routers in this directory
 sequentially. You should give sequential names to your router modules
 such as route_0001_admin.py, route_0002_user.py, etc...
```

## Comparing `morm-1.4.5.dist-info/LICENSE` & `morm-1.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `morm-1.4.5.dist-info/METADATA` & `morm-1.4.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morm
-Version: 1.4.5
+Version: 1.4.6
 Summary: A minimal asynchronous database object relational mapper
 Home-page: https://github.com/neurobin/python-morm
 Author: Md. Jahidul Hamid
 Author-email: jahidulhamid@yahoo.com
 License: BSD
 Keywords: async,orm,postgresql
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `morm-1.4.5.dist-info/RECORD` & `morm-1.4.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 morm/meta.py,sha256=8jcofKp250ytmSMLQmAnQgaPOyRwoMF5pm-jiJO-zss,2915
 morm/migration.py,sha256=DQfqOiaj-3yxrN0C75XBorJhsloeLYi_R4Zy0NF6HVs,22039
 morm/model.py,sha256=Ov4ObPkFZxs4qfczrszdGZrhKzEjDC8AhWJ1HbJWbPs,20820
 morm/pg_models.py,sha256=cTCTNYjCf2-JFaYV6Bht9dY-Wm-3O-H1Idw0d13V0HA,1015
 morm/q.py,sha256=ipZaqyxwsdXgXikBN7JxNBIXznB8XECIxfVHuXTLuxk,681
 morm/types.py,sha256=buCW-iDTDJsFQWAd0oInZUa2MftGPx61KPovKU4os6U,2097
 morm/utils.py,sha256=SLM2knYiTVq7QovL7FbBxdPfkfG5ZDFAg2UKe7WjgxE,960
-morm/version.py,sha256=miUYc2vbUkZsvmzXKUgzfNRPwyTaJ9t_VieS16XBJX0,89
+morm/version.py,sha256=XLNa1mSYR9VgycogSL1Yx-r7lTGADDwwtKksXkGI_08,89
 morm/fields/__init__.py,sha256=HACSMMQWPGMwYB-jl2AecsRJHdnXOK3nvJHCGrEa32g,26
 morm/fields/common.py,sha256=1fs7GCFTm5M_YfEY0IT6w9skmmQuNqo8fzw5YupOyb4,1968
 morm/fields/field.py,sha256=J39hrmNzsj4byTDMvdkZQSG4j9ZQL3R4NbzJuWVaFos,15604
-morm-1.4.5.data/scripts/init_fap,sha256=2lmQu-WLbIjqHNfPRlRXgiTm6LrPdsgX6mt_Q8Wtr6M,2357
-morm-1.4.5.data/scripts/morm_admin,sha256=Vhm_CVeKh1cQIF9AaJYi7ZLZC-raw8TuocxHBn6Ch08,78
-morm-1.4.5.dist-info/LICENSE,sha256=VWsTvZmFtlW7LLhvk9XpQdjLPCaZ4GMvYv26vEg3BwQ,1703
-morm-1.4.5.dist-info/METADATA,sha256=lLhaudOZEEkB4YRs_MKSDmaHtRDVXwi2xnJa8XQLrgI,13464
-morm-1.4.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-morm-1.4.5.dist-info/top_level.txt,sha256=wsIs6ERlp_Vjva-48tzfpa_gYuoyYYqKa_YhPUQIXd4,5
-morm-1.4.5.dist-info/RECORD,,
+morm-1.4.6.data/scripts/init_fap,sha256=AMsYi3Fj9NY1K3p-LAVyV-3NOiOR9m6hHtHrioZ4eAA,2353
+morm-1.4.6.data/scripts/morm_admin,sha256=Vhm_CVeKh1cQIF9AaJYi7ZLZC-raw8TuocxHBn6Ch08,78
+morm-1.4.6.dist-info/LICENSE,sha256=VWsTvZmFtlW7LLhvk9XpQdjLPCaZ4GMvYv26vEg3BwQ,1703
+morm-1.4.6.dist-info/METADATA,sha256=m4HmoAINw_aqLkj6DMVKVKFCDCoC-W4ffF64lu31Bj0,13464
+morm-1.4.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+morm-1.4.6.dist-info/top_level.txt,sha256=wsIs6ERlp_Vjva-48tzfpa_gYuoyYYqKa_YhPUQIXd4,5
+morm-1.4.6.dist-info/RECORD,,
```

