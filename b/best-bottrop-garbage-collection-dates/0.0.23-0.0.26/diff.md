# Comparing `tmp/best_bottrop_garbage_collection_dates-0.0.23.tar.gz` & `tmp/best_bottrop_garbage_collection_dates-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best_bottrop_garbage_collection_dates-0.0.23.tar", last modified: Sun Feb 27 14:33:20 2022, max compression
+gzip compressed data, was "best_bottrop_garbage_collection_dates-0.0.26.tar", last modified: Thu Jul 27 17:23:02 2023, max compression
```

## Comparing `best_bottrop_garbage_collection_dates-0.0.23.tar` & `best_bottrop_garbage_collection_dates-0.0.26.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-02-27 14:33:20.731894 best_bottrop_garbage_collection_dates-0.0.23/
--rw-rw-rw-   0        0        0     1083 2022-02-19 14:52:49.000000 best_bottrop_garbage_collection_dates-0.0.23/LICENSE
--rw-rw-rw-   0        0        0      833 2022-02-27 14:33:20.732895 best_bottrop_garbage_collection_dates-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0      192 2022-02-19 15:35:37.000000 best_bottrop_garbage_collection_dates-0.0.23/README.md
--rw-rw-rw-   0        0        0      108 2022-02-19 16:52:07.000000 best_bottrop_garbage_collection_dates-0.0.23/pyproject.toml
--rw-rw-rw-   0        0        0      738 2022-02-27 14:33:20.734895 best_bottrop_garbage_collection_dates-0.0.23/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-02-27 14:33:20.646894 best_bottrop_garbage_collection_dates-0.0.23/src/
-drwxrwxrwx   0        0        0        0 2022-02-27 14:33:20.710897 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates/
--rw-rw-rw-   0        0        0      168 2022-02-26 14:45:18.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates/__init__.py
--rw-rw-rw-   0        0        0     2512 2022-02-27 14:32:52.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py
--rw-rw-rw-   0        0        0    27602 2022-02-20 19:57:23.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates/const.py
-drwxrwxrwx   0        0        0        0 2022-02-27 14:33:20.728896 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates.egg-info/
--rw-rw-rw-   0        0        0      833 2022-02-27 14:33:19.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2022-02-27 14:33:20.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-27 14:33:20.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-02-27 14:33:20.000000 best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates.egg-info/top_level.txt
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.981380 best_bottrop_garbage_collection_dates-0.0.26/
+-rw-r--r--   0 denis      (501) staff       (20)     1062 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/LICENSE
+-rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-27 17:23:02.981439 best_bottrop_garbage_collection_dates-0.0.26/PKG-INFO
+-rw-r--r--   0 denis      (501) staff       (20)      188 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/README.md
+-rw-r--r--   0 denis      (501) staff       (20)      103 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/pyproject.toml
+-rw-r--r--   0 denis      (501) staff       (20)      710 2023-07-27 17:23:02.982081 best_bottrop_garbage_collection_dates-0.0.26/setup.cfg
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.969448 best_bottrop_garbage_collection_dates-0.0.26/src/
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.974651 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/
+-rw-r--r--   0 denis      (501) staff       (20)      167 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/__init__.py
+-rw-r--r--   0 denis      (501) staff       (20)     2673 2023-07-27 17:18:26.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py
+-rw-r--r--   0 denis      (501) staff       (20)    26841 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/const.py
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.979779 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/
+-rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO
+-rw-r--r--   0 denis      (501) staff       (20)      509 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/SOURCES.txt
+-rw-r--r--   0 denis      (501) staff       (20)        1 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/dependency_links.txt
+-rw-r--r--   0 denis      (501) staff       (20)       38 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/top_level.txt
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.981037 best_bottrop_garbage_collection_dates-0.0.26/tests/
+-rw-r--r--   0 denis      (501) staff       (20)     2899 2023-07-27 16:56:31.000000 best_bottrop_garbage_collection_dates-0.0.26/tests/test_best.py
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.23/LICENSE` & `best_bottrop_garbage_collection_dates-0.0.26/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Nazze
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Nazze
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.23/setup.cfg` & `best_bottrop_garbage_collection_dates-0.0.26/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2062 6573 745f 626f 7474 726f 705f   = best_bottrop_
-00000020: 6761 7262 6167 655f 636f 6c6c 6563 7469  garbage_collecti
-00000030: 6f6e 5f64 6174 6573 0d0a 7665 7273 696f  on_dates..versio
-00000040: 6e20 3d20 302e 302e 3233 0d0a 6175 7468  n = 0.0.23..auth
-00000050: 6f72 203d 204e 617a 7a65 0d0a 6465 7363  or = Nazze..desc
-00000060: 7269 7074 696f 6e20 3d20 4120 7061 636b  ription = A pack
-00000070: 6167 6520 746f 2066 696e 6420 7468 6520  age to find the 
-00000080: 6761 7262 6167 6520 636f 6c6c 6563 7469  garbage collecti
-00000090: 6f6e 2064 6174 6573 2069 6e20 7468 6520  on dates in the 
-000000a0: 6369 7479 206f 6620 426f 7474 726f 702c  city of Bottrop,
-000000b0: 2047 6572 6d61 6e79 0d0a 6c6f 6e67 5f64   Germany..long_d
-000000c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000d0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000100: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000110: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000120: 622e 636f 6d2f 4e61 7a7a 652f 6265 7374  b.com/Nazze/best
-00000130: 5f62 6f74 7472 6f70 5f67 6172 6261 6765  _bottrop_garbage
-00000140: 5f63 6f6c 6c65 6374 696f 6e5f 6461 7465  _collection_date
-00000150: 730d 0a70 726f 6a65 6374 5f75 726c 7320  s..project_urls 
-00000160: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-00000170: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000180: 622e 636f 6d2f 4e61 7a7a 652f 6265 7374  b.com/Nazze/best
-00000190: 5f62 6f74 7472 6f70 5f67 6172 6261 6765  _bottrop_garbage
-000001a0: 5f63 6f6c 6c65 6374 696f 6e5f 6461 7465  _collection_date
-000001b0: 732f 6973 7375 6573 0d0a 636c 6173 7369  s/issues..classi
-000001c0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
-000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001f0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000200: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000210: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-00000220: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000230: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000240: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000250: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000260: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-00000270: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000280: 6972 6573 203d 203e 3d33 2e36 0d0a 0d0a  ires = >=3.6....
-00000290: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-000002a0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000002b0: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-000002c0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002d0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002e0: 0d0a                                     ..
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6265 7374 5f62 6f74 7472 6f70 5f67  = best_bottrop_g
+00000020: 6172 6261 6765 5f63 6f6c 6c65 6374 696f  arbage_collectio
+00000030: 6e5f 6461 7465 730a 7665 7273 696f 6e20  n_dates.version 
+00000040: 3d20 302e 302e 3236 0a61 7574 686f 7220  = 0.0.26.author 
+00000050: 3d20 4e61 7a7a 650a 6465 7363 7269 7074  = Nazze.descript
+00000060: 696f 6e20 3d20 4120 7061 636b 6167 6520  ion = A package 
+00000070: 746f 2066 696e 6420 7468 6520 6761 7262  to find the garb
+00000080: 6167 6520 636f 6c6c 6563 7469 6f6e 2064  age collection d
+00000090: 6174 6573 2069 6e20 7468 6520 6369 7479  ates in the city
+000000a0: 206f 6620 426f 7474 726f 702c 2047 6572   of Bottrop, Ger
+000000b0: 6d61 6e79 0a6c 6f6e 675f 6465 7363 7269  many.long_descri
+000000c0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+000000d0: 4144 4d45 2e6d 640a 6c6f 6e67 5f64 6573  ADME.md.long_des
+000000e0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+000000f0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000100: 6b64 6f77 6e0a 7572 6c20 3d20 6874 7470  kdown.url = http
+00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
+00000120: 617a 7a65 2f62 6573 745f 626f 7474 726f  azze/best_bottro
+00000130: 705f 6761 7262 6167 655f 636f 6c6c 6563  p_garbage_collec
+00000140: 7469 6f6e 5f64 6174 6573 0a70 726f 6a65  tion_dates.proje
+00000150: 6374 5f75 726c 7320 3d20 0a09 4275 6720  ct_urls = ..Bug 
+00000160: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 617a  //github.com/Naz
+00000180: 7a65 2f62 6573 745f 626f 7474 726f 705f  ze/best_bottrop_
+00000190: 6761 7262 6167 655f 636f 6c6c 6563 7469  garbage_collecti
+000001a0: 6f6e 5f64 6174 6573 2f69 7373 7565 730a  on_dates/issues.
+000001b0: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
+000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001e0: 3a20 330a 094c 6963 656e 7365 203a 3a20  : 3..License :: 
+000001f0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000200: 4d49 5420 4c69 6365 6e73 650a 094f 7065  MIT License..Ope
+00000210: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000220: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000230: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+00000240: 6765 5f64 6972 203d 200a 093d 2073 7263  ge_dir = ..= src
+00000250: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000260: 3a0a 7079 7468 6f6e 5f72 6571 7569 7265  :.python_require
+00000270: 7320 3d20 3e3d 332e 360a 0a5b 6f70 7469  s = >=3.6..[opti
+00000280: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000290: 645d 0a77 6865 7265 203d 2073 7263 0a0a  d].where = src..
+000002a0: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+000002b0: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+000002c0: 203d 2030 0a0a                            = 0..
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.23/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py` & `best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-
 from dataclasses import dataclass
 from .const import STREET_ID_DICT
 import enum
 import requests
 import datetime
 import aiohttp
 import asyncio
 
 @dataclass
 class BESTBottropGarbageCollectionDates:
     """ Class for managing connection and data to the BEST Bottrop garbage collection dates"""
 
     trash_types_json : list[dict] = ""
-    HTTPSession : aiohttp.ClientSession() = None
+    session_timeout = aiohttp.ClientTimeout (total = 10)
 
     def _get_name_for_id(self, x, json):
         for i in json:
             if i.get("id") == x:
                 return i.get("name")
         return x
 
@@ -36,35 +35,35 @@
 
     def get_id_for_name(self, x):
         return STREET_ID_DICT.get(x)
 
     async def get_trash_types (self):
         # Load the trashtypes
         try:
-            async with aiohttp.ClientSession() as session:
+            async with aiohttp.ClientSession(timeout = self.session_timeout) as session:
                 async with session.get('https://www.best-bottrop.de/api/trashtype') as trash_types_response:
                     self.trash_types_json = await trash_types_response.json()
-        except aiohttp.ClientError as e:
+        except (aiohttp.ClientError, aiohttp.ClientConnectionError, TimeoutError) as e:
             print ("Could not load dates! Exception: {0}".format(e))
             raise e
             return ""
 
     async def get_dates_as_json(self, street_code, number) -> list[dict]:
         # Get the BEST street id code for a given street
         #street_code = STREET_ID_DICT.get(street)
 
         dates_json = ""
 
         if (street_code != None and self.trash_types_json != None):
             try:
-                async with aiohttp.ClientSession() as session:
+                async with aiohttp.ClientSession(timeout = self.session_timeout) as session:
                     async with session.get('https://www.best-bottrop.de/api/street/{0}/house/{1}/collection'.format(street_code, number)) as dates:
                         dates_json = await dates.json()
                         dates_json = list(filter(self._today_or_later, dates_json))
-            except aiohttp.ClientError as e:
+            except (aiohttp.ClientError, aiohttp.ClientConnectionError, TimeoutError) as e:
                 print ("Could not load dates! Exception: {0}".format(e))
                 raise e
 
             for date_item in dates_json:
                 date_item.update({"trashType": self._get_name_for_id(date_item.get("trashType"), self.trash_types_json)})
 
         return dates_json
```

