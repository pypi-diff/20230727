# Comparing `tmp/isyatirimhisse-0.1.0.tar.gz` & `tmp/isyatirimhisse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyatirimhisse-0.1.0.tar", last modified: Tue Jul 25 13:12:49 2023, max compression
+gzip compressed data, was "isyatirimhisse-0.1.1.tar", last modified: Thu Jul 27 13:22:29 2023, max compression
```

## Comparing `isyatirimhisse-0.1.0.tar` & `isyatirimhisse-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:12:49.886782 isyatirimhisse-0.1.0/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5917 2023-07-25 13:12:49.884789 isyatirimhisse-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5347 2023-07-25 13:11:25.000000 isyatirimhisse-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 13:12:49.790532 isyatirimhisse-0.1.0/isyatirimhisse/
--rw-rw-rw-   0        0        0     3543 2023-07-25 10:22:17.000000 isyatirimhisse-0.1.0/isyatirimhisse/VeriCek.py
--rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyatirimhisse-0.1.0/isyatirimhisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:12:49.871823 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/
--rw-rw-rw-   0        0        0     5917 2023-07-25 13:12:49.000000 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-07-25 13:12:49.000000 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:12:49.000000 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-25 13:12:49.000000 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-25 13:12:49.000000 isyatirimhisse-0.1.0/isyatirimhisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:12:49.886782 isyatirimhisse-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-07-25 13:04:48.000000 isyatirimhisse-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:12:49.882799 isyatirimhisse-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4279 2023-07-25 13:09:24.000000 isyatirimhisse-0.1.0/tests/test_veri_cek.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.873397 isyatirimhisse-0.1.1/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 13:01:25.000000 isyatirimhisse-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6230 2023-07-27 13:22:29.871401 isyatirimhisse-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5660 2023-07-27 13:19:21.000000 isyatirimhisse-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.799600 isyatirimhisse-0.1.1/isyatirimhisse/
+-rw-rw-rw-   0        0        0     3736 2023-07-27 12:57:06.000000 isyatirimhisse-0.1.1/isyatirimhisse/VeriCek.py
+-rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyatirimhisse-0.1.1/isyatirimhisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.861465 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/
+-rw-rw-rw-   0        0        0     6230 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 13:22:29.873397 isyatirimhisse-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-07-27 13:04:08.000000 isyatirimhisse-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.869409 isyatirimhisse-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4279 2023-07-25 13:09:24.000000 isyatirimhisse-0.1.1/tests/test_veri_cek.py
```

### Comparing `isyatirimhisse-0.1.0/LICENSE.txt` & `isyatirimhisse-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.1.0/PKG-INFO` & `isyatirimhisse-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: isyatirimhisse
-Version: 0.1.0
+Version: 0.1.1
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyatirimhisse
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# isyatirimhisse v0.1.0
+# isyatirimhisse v0.1.1
 
 ## Aciklama
 
 `isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
 
 *** UYARI ***
 
@@ -190,10 +190,20 @@
 
 ## Degisiklikler
 
 ### v0.1.0 - 25/07/2023
 
 * Ilk surum yayinlandi.
 
+### v0.1.1 - 27/07/2023
+
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
+* `json` kutuphanesi kaldirildi.
+* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+
 ## Lisans
 
 Bu proje MIT Lisansi altinda lisanslanmistir.
+
+## Katkida Bulunanlar
+
+- [Sinan Erdinc](https://github.com/sinanerdinc)
```

### Comparing `isyatirimhisse-0.1.0/README.md` & `isyatirimhisse-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# isyatirimhisse v0.1.0
+# isyatirimhisse v0.1.1
 
 ## Aciklama
 
 `isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
 
 *** UYARI ***
 
@@ -175,10 +175,20 @@
 
 ## Degisiklikler
 
 ### v0.1.0 - 25/07/2023
 
 * Ilk surum yayinlandi.
 
+### v0.1.1 - 27/07/2023
+
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
+* `json` kutuphanesi kaldirildi.
+* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir.
+Bu proje MIT Lisansi altinda lisanslanmistir.
+
+## Katkida Bulunanlar
+
+- [Sinan Erdinc](https://github.com/sinanerdinc)
```

### Comparing `isyatirimhisse-0.1.0/isyatirimhisse/VeriCek.py` & `isyatirimhisse-0.1.1/isyatirimhisse/VeriCek.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-import json
 import pandas as pd
 import numpy as np
 from datetime import datetime
 
 def veri_cek(sembol=None, baslangic_tarih=None, bitis_tarih=None, frekans='1g', gozlem='son', getiri_hesapla=True, logaritmik_getiri=True, na_kaldir=True):
     """
     Belirtilen tarih aralığında, belirtilen hisse senedi sembolleri için veri çeker. Çıktı özelleştirilebilir.
@@ -19,32 +18,35 @@
         logaritmik_getiri (bool, varsayılan True): Logaritmik getiri mi hesaplanacak?
         na_kaldir (bool, varsayılan True): Eksik değerler kaldırılacak mı?
 
     Dönen değer:
         pandas.DataFrame: İstenilen tarih aralığındaki hisse senedi verileri ve gerekirse getiri değerleri içeren DataFrame.
     """
 
-    if sembol is None:
+    if not sembol or sembol is None:
         raise KeyError("Hisse senedi sembolü girilmedi. 'sembol' parametresi zorunludur.")
 
-    if baslangic_tarih is None:
+    if not baslangic_tarih or baslangic_tarih is None:
         raise KeyError("Başlangıç tarihi girilmedi. 'baslangic_tarih' parametresi zorunludur.")
 
-    if bitis_tarih is None:
+    if not bitis_tarih or bitis_tarih is None:
         bitis_tarih = datetime.now().strftime('%d-%m-%Y')
 
     if not isinstance(sembol, list):
         sembol = [sembol]
 
     liste = []
 
     for s in sembol:
         url = f"https://www.isyatirim.com.tr/_layouts/15/Isyatirim.Website/Common/Data.aspx/HisseTekil?"
         url += f"hisse={s}&startdate={baslangic_tarih}&enddate={bitis_tarih}&frequency={frekans}.json"
-        result = json.loads(requests.get(url).text)
+        res = requests.get(url)
+        if not res.status_code == 200:
+            raise ConnectionError("Gönderdiğiniz istek İş Yatırım tarafından reddedildi.")
+        result = res.json()
         historical = (
             pd.DataFrame(result['value'])
             .loc[:, ['HGDG_TARIH', 'HGDG_KAPANIS']]
             .rename(columns={'HGDG_TARIH': 'Tarih', 'HGDG_KAPANIS': f'{s}'})
         )
         liste.append(historical)
 
@@ -71,8 +73,8 @@
             df_final = df_final.apply(lambda x: x / x.shift(1) - 1)
 
     if na_kaldir:
         df_final = df_final.dropna()
 
     df_final = df_final.reset_index()
 
-    return df_final
+    return df_final
```

### Comparing `isyatirimhisse-0.1.0/isyatirimhisse.egg-info/PKG-INFO` & `isyatirimhisse-0.1.1/isyatirimhisse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: isyatirimhisse
-Version: 0.1.0
+Version: 0.1.1
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyatirimhisse
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# isyatirimhisse v0.1.0
+# isyatirimhisse v0.1.1
 
 ## Aciklama
 
 `isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
 
 *** UYARI ***
 
@@ -190,10 +190,20 @@
 
 ## Degisiklikler
 
 ### v0.1.0 - 25/07/2023
 
 * Ilk surum yayinlandi.
 
+### v0.1.1 - 27/07/2023
+
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
+* `json` kutuphanesi kaldirildi.
+* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+
 ## Lisans
 
 Bu proje MIT Lisansi altinda lisanslanmistir.
+
+## Katkida Bulunanlar
+
+- [Sinan Erdinc](https://github.com/sinanerdinc)
```

### Comparing `isyatirimhisse-0.1.0/setup.py` & `isyatirimhisse-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="isyatirimhisse",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     author="Uraz Akgül",
     author_email="urazdev@gmail.com",
     description="İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/urazakgul/isyatirimhisse",
```

### Comparing `isyatirimhisse-0.1.0/tests/test_veri_cek.py` & `isyatirimhisse-0.1.1/tests/test_veri_cek.py`

 * *Files identical despite different names*

