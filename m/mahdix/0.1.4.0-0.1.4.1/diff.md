# Comparing `tmp/mahdix-0.1.4.0.tar.gz` & `tmp/mahdix-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahdix-0.1.4.0.tar", last modified: Sat Jul 22 13:48:14 2023, max compression
+gzip compressed data, was "mahdix-0.1.4.1.tar", last modified: Thu Jul 27 10:26:33 2023, max compression
```

## Comparing `mahdix-0.1.4.0.tar` & `mahdix-0.1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:14.712346 mahdix-0.1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-22 13:48:14.712346 mahdix-0.1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 13:48:03.000000 mahdix-0.1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:14.712346 mahdix-0.1.4.0/mahdix/
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-07-22 13:48:03.000000 mahdix-0.1.4.0/mahdix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:14.712346 mahdix-0.1.4.0/mahdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-22 13:48:14.000000 mahdix-0.1.4.0/mahdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-22 13:48:14.000000 mahdix-0.1.4.0/mahdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:48:14.000000 mahdix-0.1.4.0/mahdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 13:48:14.000000 mahdix-0.1.4.0/mahdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 13:48:14.712346 mahdix-0.1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-22 13:48:03.000000 mahdix-0.1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:33.448624 mahdix-0.1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 10:26:33.448624 mahdix-0.1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 10:26:23.000000 mahdix-0.1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:33.448624 mahdix-0.1.4.1/mahdix/
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-27 10:26:23.000000 mahdix-0.1.4.1/mahdix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:33.448624 mahdix-0.1.4.1/mahdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 10:26:33.000000 mahdix-0.1.4.1/mahdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 10:26:33.000000 mahdix-0.1.4.1/mahdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:26:33.000000 mahdix-0.1.4.1/mahdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 10:26:33.000000 mahdix-0.1.4.1/mahdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:26:33.448624 mahdix-0.1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-27 10:26:23.000000 mahdix-0.1.4.1/setup.py
```

### Comparing `mahdix-0.1.4.0/PKG-INFO` & `mahdix-0.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahdix
-Version: 0.1.4.0
+Version: 0.1.4.1
 Summary: this is a simple pip modul and test
 
 
 # pip install mahdix
 
 # ----[USE]-------
```

### Comparing `mahdix-0.1.4.0/README.md` & `mahdix-0.1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mahdix-0.1.4.0/mahdix/__init__.py` & `mahdix-0.1.4.1/mahdix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -797,43 +797,40 @@
 000031c0: 7273 696f 6e2c 2066 6262 6b5f 7665 7273  rsion, fbbk_vers
 000031d0: 696f 6e2c 2066 6263 615f 6162 6929 0d0a  ion, fbca_abi)..
 000031e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
 000031f0: 2061 670d 0a0d 0a0d 0a0d 0a64 6566 2063   ag........def c
 00003200: 6c65 6172 2829 3a0d 0a20 2020 206f 732e  lear():..    os.
 00003210: 7379 7374 656d 2822 636c 6561 7222 290d  system("clear").
 00003220: 0a20 2020 206f 732e 7379 7374 656d 2822  .    os.system("
-00003230: 636c 7322 290d 0a75 7365 7261 6765 6e74  cls")..useragent
-00003240: 3d5b 5d0d 0a64 6566 2057 5f75 6572 6167  =[]..def W_uerag
-00003250: 6e74 2829 3a0d 0a20 2020 200d 0a20 2020  nt():..    ..   
-00003260: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00003270: 3130 3030 3029 3a0d 0a20 2020 2020 2020  10000):..       
-00003280: 2063 6872 6f6d 655f 7665 7273 696f 6e20   chrome_version 
-00003290: 3d20 7261 6e64 6f6d 2e72 616e 6469 6e74  = random.randint
-000032a0: 2838 302c 2039 3929 0d0a 2020 2020 2020  (80, 99)..      
-000032b0: 2020 7765 626b 6974 5f76 6572 7369 6f6e    webkit_version
-000032c0: 203d 2072 616e 646f 6d2e 7261 6e64 696e   = random.randin
-000032d0: 7428 3530 302c 2035 3939 290d 0a20 2020  t(500, 599)..   
-000032e0: 2020 2020 2073 6166 6172 695f 7665 7273       safari_vers
-000032f0: 696f 6e20 3d20 7261 6e64 6f6d 2e72 616e  ion = random.ran
-00003300: 6469 6e74 2834 3030 2c20 3439 3929 0d0a  dint(400, 499)..
-00003310: 2020 2020 2020 2020 7769 6e64 6f77 735f          windows_
-00003320: 7665 7273 696f 6e20 3d20 7261 6e64 6f6d  version = random
-00003330: 2e72 616e 6469 6e74 2838 2c20 3130 290d  .randint(8, 10).
-00003340: 0a20 2020 2020 2020 2069 735f 7769 6e36  .        is_win6
-00003350: 3420 3d20 7261 6e64 6f6d 2e63 686f 6963  4 = random.choic
-00003360: 6528 5b54 7275 652c 2046 616c 7365 5d29  e([True, False])
-00003370: 0d0a 2020 2020 2020 2020 7573 6572 5f61  ..        user_a
-00003380: 6765 6e74 203d 2066 224d 6f7a 696c 6c61  gent = f"Mozilla
-00003390: 2f35 2e30 2028 5769 6e64 6f77 7320 4e54  /5.0 (Windows NT
-000033a0: 207b 7769 6e64 6f77 735f 7665 7273 696f   {windows_versio
-000033b0: 6e7d 2e7b 6973 5f77 696e 3634 2061 6e64  n}.{is_win64 and
-000033c0: 2027 574f 5736 343b 2720 6f72 2027 277d   'WOW64;' or ''}
-000033d0: 5769 6e36 343b 2078 3634 2920 4170 706c  Win64; x64) Appl
-000033e0: 6557 6562 4b69 742f 7b77 6562 6b69 745f  eWebKit/{webkit_
-000033f0: 7665 7273 696f 6e7d 2e30 2028 4b48 544d  version}.0 (KHTM
-00003400: 4c2c 206c 696b 6520 4765 636b 6f29 2043  L, like Gecko) C
-00003410: 6872 6f6d 652f 7b63 6872 6f6d 655f 7665  hrome/{chrome_ve
-00003420: 7273 696f 6e7d 2e30 2e30 2e30 2053 6166  rsion}.0.0.0 Saf
-00003430: 6172 692f 7b73 6166 6172 695f 7665 7273  ari/{safari_vers
-00003440: 696f 6e7d 2e30 220d 0a20 2020 2020 2020  ion}.0"..       
-00003450: 2075 7365 7261 6765 6e74 2e61 7070 656e   useragent.appen
-00003460: 6428 7573 6572 5f61 6765 6e74 290d 0a    d(user_agent)..
+00003230: 636c 7322 290d 0a64 6566 2057 5f75 6572  cls")..def W_uer
+00003240: 6167 6e74 2829 3a0d 0a20 2020 2020 2020  agnt():..       
+00003250: 2063 6872 6f6d 655f 7665 7273 696f 6e20   chrome_version 
+00003260: 3d20 7261 6e64 6f6d 2e72 616e 6469 6e74  = random.randint
+00003270: 2838 302c 2039 3929 0d0a 2020 2020 2020  (80, 99)..      
+00003280: 2020 7765 626b 6974 5f76 6572 7369 6f6e    webkit_version
+00003290: 203d 2072 616e 646f 6d2e 7261 6e64 696e   = random.randin
+000032a0: 7428 3530 302c 2035 3939 290d 0a20 2020  t(500, 599)..   
+000032b0: 2020 2020 2073 6166 6172 695f 7665 7273       safari_vers
+000032c0: 696f 6e20 3d20 7261 6e64 6f6d 2e72 616e  ion = random.ran
+000032d0: 6469 6e74 2834 3030 2c20 3439 3929 0d0a  dint(400, 499)..
+000032e0: 2020 2020 2020 2020 7769 6e64 6f77 735f          windows_
+000032f0: 7665 7273 696f 6e20 3d20 7261 6e64 6f6d  version = random
+00003300: 2e72 616e 6469 6e74 2838 2c20 3130 290d  .randint(8, 10).
+00003310: 0a20 2020 2020 2020 2069 735f 7769 6e36  .        is_win6
+00003320: 3420 3d20 7261 6e64 6f6d 2e63 686f 6963  4 = random.choic
+00003330: 6528 5b54 7275 652c 2046 616c 7365 5d29  e([True, False])
+00003340: 0d0a 2020 2020 2020 2020 7573 6572 5f61  ..        user_a
+00003350: 6765 6e74 203d 2066 224d 6f7a 696c 6c61  gent = f"Mozilla
+00003360: 2f35 2e30 2028 5769 6e64 6f77 7320 4e54  /5.0 (Windows NT
+00003370: 207b 7769 6e64 6f77 735f 7665 7273 696f   {windows_versio
+00003380: 6e7d 2e7b 6973 5f77 696e 3634 2061 6e64  n}.{is_win64 and
+00003390: 2027 574f 5736 343b 2720 6f72 2027 277d   'WOW64;' or ''}
+000033a0: 5769 6e36 343b 2078 3634 2920 4170 706c  Win64; x64) Appl
+000033b0: 6557 6562 4b69 742f 7b77 6562 6b69 745f  eWebKit/{webkit_
+000033c0: 7665 7273 696f 6e7d 2e30 2028 4b48 544d  version}.0 (KHTM
+000033d0: 4c2c 206c 696b 6520 4765 636b 6f29 2043  L, like Gecko) C
+000033e0: 6872 6f6d 652f 7b63 6872 6f6d 655f 7665  hrome/{chrome_ve
+000033f0: 7273 696f 6e7d 2e30 2e30 2e30 2053 6166  rsion}.0.0.0 Saf
+00003400: 6172 692f 7b73 6166 6172 695f 7665 7273  ari/{safari_vers
+00003410: 696f 6e7d 2e30 220d 0a20 2020 2020 2020  ion}.0"..       
+00003420: 2072 6574 7572 6e20 7573 6572 5f61 6765   return user_age
+00003430: 6e74 0d0a                                nt..
```

### Comparing `mahdix-0.1.4.0/mahdix.egg-info/PKG-INFO` & `mahdix-0.1.4.1/mahdix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahdix
-Version: 0.1.4.0
+Version: 0.1.4.1
 Summary: this is a simple pip modul and test
 
 
 # pip install mahdix
 
 # ----[USE]-------
```

### Comparing `mahdix-0.1.4.0/setup.py` & `mahdix-0.1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='mahdix',
-version='0.1.4.0',
+version='0.1.4.1',
 description='this is a simple pip modul and test',
 long_description='''
 # pip install mahdix
 
 # ----[USE]-------
 
 # print Sumthiong = mahdix.p('YOUR TXT')
```

