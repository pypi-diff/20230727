# Comparing `tmp/python3-capsolver-0.6.1.tar.gz` & `tmp/python3-capsolver-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-capsolver-0.6.1.tar", last modified: Fri Apr 28 23:51:26 2023, max compression
+gzip compressed data, was "python3-capsolver-0.7.1.tar", last modified: Thu Jul 27 20:08:15 2023, max compression
```

## Comparing `python3-capsolver-0.6.1.tar` & `python3-capsolver-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/
--rw-r--r--   0 homea     (1000) homea     (1000)     5065 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/PKG-INFO
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.6.1/python3_capsolver/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-04-28 23:51:22.000000 python3-capsolver-0.6.1/python3_capsolver/__version__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4919 2023-04-28 23:01:33.000000 python3-capsolver-0.6.1/python3_capsolver/cloudflare.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1958 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/control.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.6.1/python3_capsolver/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.6.1/python3_capsolver/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.6.1/python3_capsolver/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3398 2023-04-28 23:03:36.000000 python3-capsolver-0.6.1/python3_capsolver/core/enum.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4381 2023-04-28 23:23:41.000000 python3-capsolver-0.6.1/python3_capsolver/core/serializer.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3923 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/datadome_slider.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.6.1/python3_capsolver/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4322 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/gee_test.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4830 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6349 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/image_to_text.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4972 2023-04-28 22:33:29.000000 python3-capsolver-0.6.1/python3_capsolver/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6394 2023-04-28 22:02:43.000000 python3-capsolver-0.6.1/python3_capsolver/recaptcha.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver.egg-info/
--rw-rw-r--   0 homea     (1000) homea     (1000)     5065 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/PKG-INFO
--rw-rw-r--   0 homea     (1000) homea     (1000)      771 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:33:01.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/not-zip-safe
--rw-rw-r--   0 homea     (1000) homea     (1000)       60 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/requires.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)       18 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/top_level.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4137 2023-04-28 23:50:54.000000 python3-capsolver-0.6.1/setup.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/
+-rw-r--r--   0 homea     (1000) homea     (1000)     5300 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/PKG-INFO
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/python3_capsolver/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.7.1/python3_capsolver/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-07-27 19:50:36.000000 python3-capsolver-0.7.1/python3_capsolver/__version__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4538 2023-07-26 15:58:01.000000 python3-capsolver-0.7.1/python3_capsolver/aws_waf.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4907 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/cloudflare.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1958 2023-07-26 15:32:58.000000 python3-capsolver-0.7.1/python3_capsolver/control.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/python3_capsolver/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.7.1/python3_capsolver/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.7.1/python3_capsolver/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1018 2023-07-27 12:52:57.000000 python3-capsolver-0.7.1/python3_capsolver/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3418 2023-07-27 19:12:48.000000 python3-capsolver-0.7.1/python3_capsolver/core/enum.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4546 2023-07-27 19:31:24.000000 python3-capsolver-0.7.1/python3_capsolver/core/serializer.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     5247 2023-07-27 14:27:52.000000 python3-capsolver-0.7.1/python3_capsolver/cyber_si_ara.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3938 2023-07-27 19:48:25.000000 python3-capsolver-0.7.1/python3_capsolver/datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)    10707 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4310 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7684 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6271 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/image_to_text.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4948 2023-07-27 20:03:15.000000 python3-capsolver-0.7.1/python3_capsolver/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6374 2023-07-27 19:48:09.000000 python3-capsolver-0.7.1/python3_capsolver/recaptcha.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/python3_capsolver.egg-info/
+-rw-r--r--   0 homea     (1000) homea     (1000)     5300 2023-07-27 20:08:15.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)      834 2023-07-27 20:08:15.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-07-27 20:08:15.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-07-27 20:07:44.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/not-zip-safe
+-rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-07-27 20:08:15.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/requires.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-07-27 20:08:15.000000 python3-capsolver-0.7.1/python3_capsolver.egg-info/top_level.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-07-27 20:08:15.361885 python3-capsolver-0.7.1/setup.cfg
+-rw-r--r--   0 homea     (1000) homea     (1000)     4167 2023-07-27 20:08:06.000000 python3-capsolver-0.7.1/setup.py
```

### Comparing `python3-capsolver-0.6.1/PKG-INFO` & `python3-capsolver-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7468  : 2.1.Name: pyth
 00000020: 6f6e 332d 6361 7073 6f6c 7665 720a 5665  on3-capsolver.Ve
-00000030: 7273 696f 6e3a 2030 2e36 2e31 0a53 756d  rsion: 0.6.1.Sum
-00000040: 6d61 7279 3a20 5079 7468 6f6e 2033 2e37  mary: Python 3.7
+00000030: 7273 696f 6e3a 2030 2e37 2e31 0a53 756d  rsion: 0.7.1.Sum
+00000040: 6d61 7279 3a20 5079 7468 6f6e 2033 2e38  mary: Python 3.8
 00000050: 2b20 4361 7073 6f6c 7665 7220 6c69 6272  + Capsolver libr
 00000060: 6172 7920 7769 7468 2041 494f 206d 6f64  ary with AIO mod
 00000070: 756c 652e 0a48 6f6d 652d 7061 6765 3a20  ule..Home-page: 
 00000080: 6874 7470 733a 2f2f 616e 6472 6569 6472  https://andreidr
 00000090: 616e 672e 6769 7468 7562 2e69 6f2f 7079  ang.github.io/py
 000000a0: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
 000000b0: 0a41 7574 686f 723a 2041 6e64 7265 6944  .Author: AndreiD
@@ -18,15 +18,15 @@
 00000110: 2068 7474 7073 3a2f 2f61 6e64 7265 6964   https://andreid
 00000120: 7261 6e67 2e67 6974 6875 622e 696f 2f70  rang.github.io/p
 00000130: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
 00000140: 2f0a 5072 6f6a 6563 742d 5552 4c3a 2053  /.Project-URL: S
 00000150: 6f75 7263 652c 2068 7474 7073 3a2f 2f67  ource, https://g
 00000160: 6974 6875 622e 636f 6d2f 416e 6472 6569  ithub.com/Andrei
 00000170: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
-00000180: 7074 6368 6161 690a 4b65 7977 6f72 6473  ptchaai.Keywords
+00000180: 7073 6f6c 7665 720a 4b65 7977 6f72 6473  psolver.Keywords
 00000190: 3a20 6361 7074 6368 6120 0a20 2020 2020  : captcha .     
 000001a0: 2020 2020 2020 2020 2020 2072 6563 6170             recap
 000001b0: 7463 6861 0a20 2020 2020 2020 2020 2020  tcha.           
 000001c0: 2020 2020 2067 6565 7465 7374 0a20 2020       geetest.   
 000001d0: 2020 2020 2020 2020 2020 2020 2068 6361               hca
 000001e0: 7074 6368 610a 2020 2020 2020 2020 2020  ptcha.          
 000001f0: 2020 2020 2020 6361 7079 7075 7a7a 6c65        capypuzzle
@@ -68,250 +68,265 @@
 00000430: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000440: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 00000450: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000460: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000470: 203a 3a20 4f6e 6c79 0a43 6c61 7373 6966   :: Only.Classif
 00000480: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 00000490: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000004a0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
+000004a0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
 000004b0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000004c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000004d0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+000004d0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
 000004e0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 000004f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000500: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00000510: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000520: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000530: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000540: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000550: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000560: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000570: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000580: 2046 7261 6d65 776f 726b 203a 3a20 4173   Framework :: As
-00000590: 796e 6349 4f0a 436c 6173 7369 6669 6572  yncIO.Classifier
-000005a0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000005b0: 656d 203a 3a20 556e 6978 0a43 6c61 7373  em :: Unix.Class
-000005c0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-000005d0: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-000005e0: 736f 6674 203a 3a20 5769 6e64 6f77 730a  soft :: Windows.
-000005f0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000600: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000610: 4d61 634f 530a 5265 7175 6972 6573 2d50  MacOS.Requires-P
-00000620: 7974 686f 6e3a 203e 3d33 2e37 2e30 0a44  ython: >=3.7.0.D
-00000630: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-00000640: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000650: 726b 646f 776e 0a0a 0a23 2070 7974 686f  rkdown...# pytho
-00000660: 6e33 2d63 6170 736f 6c76 6572 0a21 5b50  n3-capsolver.![P
-00000670: 7974 686f 6e33 2d43 6170 736f 6c76 6572  ython3-Capsolver
-00000680: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000690: 2e63 6f6d 2f41 6e64 7265 6944 7261 6e67  .com/AndreiDrang
-000006a0: 2f70 7974 686f 6e33 2d63 6170 736f 6c76  /python3-capsolv
-000006b0: 6572 2f62 6c6f 622f 6d61 696e 2f66 696c  er/blob/main/fil
-000006c0: 6573 2f43 6170 736f 6c76 6572 536d 2e70  es/CapsolverSm.p
-000006d0: 6e67 290a 0a5b 215b 4361 7073 6f6c 7665  ng)..[![Capsolve
-000006e0: 725d 2868 7474 7073 3a2f 2f75 7365 722d  r](https://user-
-000006f0: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000700: 7263 6f6e 7465 6e74 2e63 6f6d 2f31 3639  rcontent.com/169
-00000710: 3931 3336 352f 3233 3438 3532 3232 392d  91365/234852229-
-00000720: 3665 3462 3366 3363 2d66 3439 382d 3466  6e4b3f3c-f498-4f
-00000730: 6435 2d39 6136 622d 6637 6632 3639 6464  d5-9a6b-f7f269dd
-00000740: 3462 6663 2e67 6966 295d 2868 7474 7073  4bfc.gif)](https
-00000750: 3a2f 2f64 6173 6862 6f61 7264 2e63 6170  ://dashboard.cap
-00000760: 736f 6c76 6572 2e63 6f6d 2f70 6173 7370  solver.com/passp
-00000770: 6f72 742f 7265 6769 7374 6572 3f69 6e76  ort/register?inv
-00000780: 6974 6543 6f64 653d 6b51 546e 2d74 4730  iteCode=kQTn-tG0
-00000790: 374a 6231 290a 0a5b 215b 5079 5049 2076  7Jb1)..[![PyPI v
-000007a0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000007b0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-000007c0: 2f70 7974 686f 6e33 2d63 6170 736f 6c76  /python3-capsolv
-000007d0: 6572 2e73 7667 295d 2868 7474 7073 3a2f  er.svg)](https:/
-000007e0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-000007f0: 792f 7079 7468 6f6e 332d 6361 7073 6f6c  y/python3-capsol
-00000800: 7665 7229 0a5b 215b 5079 7468 6f6e 2076  ver).[![Python v
-00000810: 6572 7369 6f6e 735d 2868 7474 7073 3a2f  ersions](https:/
-00000820: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000830: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000840: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
-00000850: 722e 7376 673f 6c6f 676f 3d70 7974 686f  r.svg?logo=pytho
-00000860: 6e26 6c6f 676f 436f 6c6f 723d 4642 4530  n&logoColor=FBE0
-00000870: 3732 295d 2868 7474 7073 3a2f 2f62 6164  72)](https://bad
-00000880: 6765 2e66 7572 792e 696f 2f70 792f 7079  ge.fury.io/py/py
-00000890: 7468 6f6e 332d 6361 7073 6f6c 7665 7229  thon3-capsolver)
-000008a0: 0a5b 215b 446f 776e 6c6f 6164 735d 2868  .[![Downloads](h
-000008b0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000008c0: 2f62 6164 6765 2f70 7974 686f 6e33 2d63  /badge/python3-c
-000008d0: 6170 736f 6c76 6572 2f6d 6f6e 7468 295d  apsolver/month)]
-000008e0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-000008f0: 6368 2f70 726f 6a65 6374 2f70 7974 686f  ch/project/pytho
-00000900: 6e33 2d63 6170 736f 6c76 6572 290a 0a5b  n3-capsolver)..[
-00000910: 215b 4d61 696e 7461 696e 6162 696c 6974  ![Maintainabilit
-00000920: 795d 2868 7474 7073 3a2f 2f61 7069 2e63  y](https://api.c
-00000930: 6f64 6563 6c69 6d61 7465 2e63 6f6d 2f76  odeclimate.com/v
-00000940: 312f 6261 6467 6573 2f33 6333 3031 3637  1/badges/3c30167
-00000950: 6235 6662 3337 6130 3737 3565 612f 6d61  b5fb37a0775ea/ma
-00000960: 696e 7461 696e 6162 696c 6974 7929 5d28  intainability)](
-00000970: 6874 7470 733a 2f2f 636f 6465 636c 696d  https://codeclim
-00000980: 6174 652e 636f 6d2f 6769 7468 7562 2f41  ate.com/github/A
-00000990: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
-000009a0: 6e33 2d63 6170 736f 6c76 6572 2f6d 6169  n3-capsolver/mai
-000009b0: 6e74 6169 6e61 6269 6c69 7479 290a 5b21  ntainability).[!
-000009c0: 5b43 6f64 6163 7920 4261 6467 655d 2868  [Codacy Badge](h
-000009d0: 7474 7073 3a2f 2f61 7070 2e63 6f64 6163  ttps://app.codac
-000009e0: 792e 636f 6d2f 7072 6f6a 6563 742f 6261  y.com/project/ba
-000009f0: 6467 652f 4772 6164 652f 3332 3364 3465  dge/Grade/323d4e
-00000a00: 6461 3066 6531 3437 3762 6265 6138 6665  da0fe1477bbea8fe
-00000a10: 3839 3032 6239 6539 3765 295d 2868 7474  8902b9e97e)](htt
-00000a20: 7073 3a2f 2f77 7777 2e63 6f64 6163 792e  ps://www.codacy.
-00000a30: 636f 6d2f 6768 2f41 6e64 7265 6944 7261  com/gh/AndreiDra
-00000a40: 6e67 2f70 7974 686f 6e33 2d63 6170 736f  ng/python3-capso
-00000a50: 6c76 6572 2f64 6173 6862 6f61 7264 3f75  lver/dashboard?u
-00000a60: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
-00000a70: 2e63 6f6d 2661 6d70 3b75 746d 5f6d 6564  .com&amp;utm_med
-00000a80: 6975 6d3d 7265 6665 7272 616c 2661 6d70  ium=referral&amp
-00000a90: 3b75 746d 5f63 6f6e 7465 6e74 3d41 6e64  ;utm_content=And
-00000aa0: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
-00000ab0: 2d63 6170 736f 6c76 6572 2661 6d70 3b75  -capsolver&amp;u
-00000ac0: 746d 5f63 616d 7061 6967 6e3d 4261 6467  tm_campaign=Badg
-00000ad0: 655f 4772 6164 6529 0a5b 215b 636f 6465  e_Grade).[![code
-00000ae0: 636f 765d 2868 7474 7073 3a2f 2f63 6f64  cov](https://cod
-00000af0: 6563 6f76 2e69 6f2f 6768 2f41 6e64 7265  ecov.io/gh/Andre
-00000b00: 6944 7261 6e67 2f70 7974 686f 6e33 2d63  iDrang/python3-c
-00000b10: 6170 736f 6c76 6572 2f62 7261 6e63 682f  apsolver/branch/
-00000b20: 6d61 696e 2f67 7261 7068 2f62 6164 6765  main/graph/badge
-00000b30: 2e73 7667 3f74 6f6b 656e 3d32 4c34 5656  .svg?token=2L4VV
-00000b40: 4946 3447 3829 5d28 6874 7470 733a 2f2f  IF4G8)](https://
-00000b50: 636f 6465 636f 762e 696f 2f67 682f 416e  codecov.io/gh/An
-00000b60: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
-00000b70: 332d 6361 7073 6f6c 7665 7229 0a0a 5b21  3-capsolver)..[!
-00000b80: 5b53 7068 696e 7820 6275 696c 645d 2868  [Sphinx build](h
-00000b90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ba0: 6d2f 416e 6472 6569 4472 616e 672f 7079  m/AndreiDrang/py
-00000bb0: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
-00000bc0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000bd0: 732f 7370 6869 6e78 2e79 6d6c 2f62 6164  s/sphinx.yml/bad
-00000be0: 6765 2e73 7667 3f62 7261 6e63 683d 7265  ge.svg?branch=re
-00000bf0: 6c65 6173 6529 5d28 6874 7470 733a 2f2f  lease)](https://
-00000c00: 6769 7468 7562 2e63 6f6d 2f41 6e64 7265  github.com/Andre
-00000c10: 6944 7261 6e67 2f70 7974 686f 6e33 2d63  iDrang/python3-c
-00000c20: 6170 736f 6c76 6572 2f61 6374 696f 6e73  apsolver/actions
-00000c30: 2f77 6f72 6b66 6c6f 7773 2f73 7068 696e  /workflows/sphin
-00000c40: 782e 796d 6c29 0a5b 215b 4275 696c 645d  x.yml).[![Build]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
-00000c70: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
-00000c80: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
-00000c90: 6f77 732f 6275 696c 642e 796d 6c2f 6261  ows/build.yml/ba
-00000ca0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000cb0: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-00000cc0: 7468 7562 2e63 6f6d 2f41 6e64 7265 6944  thub.com/AndreiD
-00000cd0: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
-00000ce0: 736f 6c76 6572 2f61 6374 696f 6e73 2f77  solver/actions/w
-00000cf0: 6f72 6b66 6c6f 7773 2f62 7569 6c64 2e79  orkflows/build.y
-00000d00: 6d6c 290a 5b21 5b49 6e73 7461 6c6c 6174  ml).[![Installat
-00000d10: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-00000d20: 6875 622e 636f 6d2f 416e 6472 6569 4472  hub.com/AndreiDr
-00000d30: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
-00000d40: 6f6c 7665 722f 6163 7469 6f6e 732f 776f  olver/actions/wo
-00000d50: 726b 666c 6f77 732f 696e 7374 616c 6c2e  rkflows/install.
-00000d60: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
-00000d70: 616e 6368 3d6d 6169 6e29 5d28 6874 7470  anch=main)](http
-00000d80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000d90: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
-00000da0: 6e33 2d63 6170 736f 6c76 6572 2f61 6374  n3-capsolver/act
-00000db0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f69  ions/workflows/i
-00000dc0: 6e73 7461 6c6c 2e79 6d6c 290a 5b21 5b54  nstall.yml).[![T
-00000dd0: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
-00000de0: 7468 7562 2e63 6f6d 2f41 6e64 7265 6944  thub.com/AndreiD
-00000df0: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
-00000e00: 736f 6c76 6572 2f61 6374 696f 6e73 2f77  solver/actions/w
-00000e10: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
-00000e20: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-00000e30: 6368 3d6d 6169 6e29 5d28 6874 7470 733a  ch=main)](https:
-00000e40: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6e64  //github.com/And
-00000e50: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
-00000e60: 2d63 6170 736f 6c76 6572 2f61 6374 696f  -capsolver/actio
-00000e70: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-00000e80: 742e 796d 6c29 0a5b 215b 4c69 6e74 5d28  t.yml).[![Lint](
-00000e90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ea0: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
-00000eb0: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
-00000ec0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000ed0: 7773 2f6c 696e 742e 796d 6c2f 6261 6467  ws/lint.yml/badg
-00000ee0: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-00000ef0: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
-00000f00: 7562 2e63 6f6d 2f41 6e64 7265 6944 7261  ub.com/AndreiDra
-00000f10: 6e67 2f70 7974 686f 6e33 2d63 6170 736f  ng/python3-capso
-00000f20: 6c76 6572 2f61 6374 696f 6e73 2f77 6f72  lver/actions/wor
-00000f30: 6b66 6c6f 7773 2f6c 696e 742e 796d 6c29  kflows/lint.yml)
-00000f40: 0a0a 0a50 7974 686f 6e20 3320 6c69 6272  ...Python 3 libr
-00000f50: 6172 7920 666f 7220 5b43 6170 736f 6c76  ary for [Capsolv
-00000f60: 6572 5d28 6874 7470 733a 2f2f 6461 7368  er](https://dash
-00000f70: 626f 6172 642e 6361 7073 6f6c 7665 722e  board.capsolver.
-00000f80: 636f 6d2f 7061 7373 706f 7274 2f72 6567  com/passport/reg
-00000f90: 6973 7465 723f 696e 7669 7465 436f 6465  ister?inviteCode
-00000fa0: 3d6b 5154 6e2d 7447 3037 4a62 3129 2073  =kQTn-tG07Jb1) s
-00000fb0: 6572 7669 6365 2041 5049 2e0a 0a54 6573  ervice API...Tes
-00000fc0: 7465 6420 6f6e 2055 4e49 5820 6261 7365  ted on UNIX base
-00000fd0: 6420 4f53 2e0a 0a54 6865 206c 6962 7261  d OS...The libra
-00000fe0: 7279 2069 7320 696e 7465 6e64 6564 2066  ry is intended f
-00000ff0: 6f72 2073 6f66 7477 6172 6520 6465 7665  or software deve
-00001000: 6c6f 7065 7273 2061 6e64 2069 7320 7573  lopers and is us
-00001010: 6564 2074 6f20 776f 726b 2077 6974 6820  ed to work with 
-00001020: 7468 6520 5b43 6170 736f 6c76 6572 5d28  the [Capsolver](
-00001030: 6874 7470 733a 2f2f 6461 7368 626f 6172  https://dashboar
-00001040: 642e 6361 7073 6f6c 7665 722e 636f 6d2f  d.capsolver.com/
-00001050: 7061 7373 706f 7274 2f72 6567 6973 7465  passport/registe
-00001060: 723f 696e 7669 7465 436f 6465 3d6b 5154  r?inviteCode=kQT
-00001070: 6e2d 7447 3037 4a62 3129 2073 6572 7669  n-tG07Jb1) servi
-00001080: 6365 2041 5049 2e0a 0a2a 2a2a 0a0a 4966  ce API...***..If
-00001090: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-000010a0: 6573 7469 6f6e 732c 2070 6c65 6173 6520  estions, please 
-000010b0: 7365 6e64 2061 206d 6573 7361 6765 2074  send a message t
-000010c0: 6f20 7468 6520 5b54 656c 6567 7261 6d5d  o the [Telegram]
-000010d0: 2868 7474 7073 3a2f 2f74 2e6d 652f 7079  (https://t.me/py
-000010e0: 7468 6f6e 6361 7074 6368 6129 2063 6861  thoncaptcha) cha
-000010f0: 7420 726f 6f6d 2e0a 0a4f 7220 656d 6169  t room...Or emai
-00001100: 6c20 7079 7468 6f6e 2d63 6170 7463 6861  l python-captcha
-00001110: 4070 6d2e 6d65 0a0a 2a2a 2a0a 0a23 2320  @pm.me..***..## 
-00001120: 486f 7720 746f 2069 6e73 7461 6c6c 3f0a  How to install?.
-00001130: 0a57 6520 7265 636f 6d6d 656e 6420 7573  .We recommend us
-00001140: 696e 6720 7468 6520 6c61 7465 7374 2076  ing the latest v
-00001150: 6572 7369 6f6e 206f 6620 5079 7468 6f6e  ersion of Python
-00001160: 2e20 6070 7974 686f 6e33 2d63 6170 736f  . `python3-capso
-00001170: 6c76 6572 6020 7375 7070 6f72 7473 2050  lver` supports P
-00001180: 7974 686f 6e20 332e 372b 2e0a 0a23 2323  ython 3.7+...###
-00001190: 2070 6970 0a0a 6060 6062 6173 680a 7069   pip..```bash.pi
-000011a0: 7020 696e 7374 616c 6c20 7079 7468 6f6e  p install python
-000011b0: 332d 6361 7073 6f6c 7665 720a 6060 600a  3-capsolver.```.
-000011c0: 0a23 2320 486f 7720 746f 2075 7365 3f0a  .## How to use?.
-000011d0: 0a49 7320 6465 7363 7269 6265 6420 696e  .Is described in
-000011e0: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
-000011f0: 696f 6e2d 7765 6273 6974 655d 2868 7474  ion-website](htt
-00001200: 7073 3a2f 2f61 6e64 7265 6964 7261 6e67  ps://andreidrang
-00001210: 2e67 6974 6875 622e 696f 2f70 7974 686f  .github.io/pytho
-00001220: 6e33 2d63 6170 736f 6c76 6572 2f29 2e0a  n3-capsolver/)..
-00001230: 0a0a 2323 2048 6f77 2074 6f20 7465 7374  ..## How to test
-00001240: 3f0a 0a31 2e20 596f 7520 6e65 6564 2073  ?..1. You need s
-00001250: 6574 2060 6041 5049 5f4b 4559 6060 2069  et ``API_KEY`` i
-00001260: 6e20 796f 7572 2065 6e76 6972 6f6e 6d65  n your environme
-00001270: 6e74 2867 6574 2074 6869 7320 7661 6c75  nt(get this valu
-00001280: 6520 6672 6f6d 2079 6f75 2061 6363 6f75  e from you accou
-00001290: 6e74 292e 0a32 2e20 5275 6e20 636f 6d6d  nt)..2. Run comm
-000012a0: 616e 6420 6060 6d61 6b65 2074 6573 7473  and ``make tests
-000012b0: 6060 2c20 6672 6f6d 2072 6f6f 7420 6469  ``, from root di
-000012c0: 7265 6374 6f72 792e 0a0a 0a23 2323 2043  rectory....### C
-000012d0: 6861 6e67 656c 6f67 0a0a 4368 6563 6b20  hangelog..Check 
-000012e0: 5b72 656c 6561 7365 7320 7061 6765 5d28  [releases page](
-000012f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001300: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
-00001310: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
-00001320: 2f72 656c 6561 7365 7329 2e0a 0a23 2323  /releases)...###
-00001330: 2048 6f77 2074 6f20 6765 7420 4150 4920   How to get API 
-00001340: 4b65 7920 746f 2077 6f72 6b20 7769 7468  Key to work with
-00001350: 2074 6865 206c 6962 7261 7279 0a31 2e20   the library.1. 
-00001360: 4f6e 2074 6865 2070 6167 6520 2d20 6874  On the page - ht
-00001370: 7470 733a 2f2f 6461 7368 626f 6172 642e  tps://dashboard.
-00001380: 6361 7073 6f6c 7665 722e 636f 6d2f 6f76  capsolver.com/ov
-00001390: 6572 7669 6577 2f75 7365 722d 6365 6e74  erview/user-cent
-000013a0: 6572 0a32 2e20 4669 6e64 2069 743a 2021  er.2. Find it: !
-000013b0: 5b69 6d67 2e70 6e67 5d28 6669 6c65 732f  [img.png](files/
-000013c0: 696d 672e 706e 6729 0a                   img.png).
+00000500: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000510: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000520: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000530: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000540: 3131 0a43 6c61 7373 6966 6965 723a 2046  11.Classifier: F
+00000550: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
+00000560: 6349 4f0a 436c 6173 7369 6669 6572 3a20  cIO.Classifier: 
+00000570: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000580: 203a 3a20 556e 6978 0a43 6c61 7373 6966   :: Unix.Classif
+00000590: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
+000005a0: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
+000005b0: 6674 203a 3a20 5769 6e64 6f77 730a 436c  ft :: Windows.Cl
+000005c0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000005d0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+000005e0: 634f 530a 5265 7175 6972 6573 2d50 7974  cOS.Requires-Pyt
+000005f0: 686f 6e3a 203e 3d33 2e38 2e30 0a44 6573  hon: >=3.8.0.Des
+00000600: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000610: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000620: 646f 776e 0a0a 0a23 2070 7974 686f 6e33  down...# python3
+00000630: 2d63 6170 736f 6c76 6572 0a21 5b50 7974  -capsolver.![Pyt
+00000640: 686f 6e33 2d43 6170 736f 6c76 6572 5d28  hon3-Capsolver](
+00000650: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000660: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
+00000670: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
+00000680: 2f62 6c6f 622f 6d61 696e 2f66 696c 6573  /blob/main/files
+00000690: 2f43 6170 736f 6c76 6572 536d 2e70 6e67  /CapsolverSm.png
+000006a0: 290a 0a3c 6120 6872 6566 3d22 6874 7470  )..<a href="http
+000006b0: 733a 2f2f 6461 7368 626f 6172 642e 6361  s://dashboard.ca
+000006c0: 7073 6f6c 7665 722e 636f 6d2f 7061 7373  psolver.com/pass
+000006d0: 706f 7274 2f72 6567 6973 7465 723f 696e  port/register?in
+000006e0: 7669 7465 436f 6465 3d6b 5154 6e2d 7447  viteCode=kQTn-tG
+000006f0: 3037 4a62 3122 3e0a 2020 2020 3c69 6d67  07Jb1">.    <img
+00000700: 2073 7263 3d22 6874 7470 733a 2f2f 6364   src="https://cd
+00000710: 6e2e 6469 7363 6f72 6461 7070 2e63 6f6d  n.discordapp.com
+00000720: 2f61 7474 6163 686d 656e 7473 2f31 3130  /attachments/110
+00000730: 3531 3732 3339 3436 3535 3632 3533 3036  5172394655625306
+00000740: 2f31 3130 3531 3830 3130 3138 3032 3437  /110518010180247
+00000750: 3135 3735 2f32 3032 3231 3230 372d 3136  1575/20221207-16
+00000760: 3037 3439 2e67 6966 2220 616c 743d 2243  0749.gif" alt="C
+00000770: 6170 736f 6c76 6572 2773 2042 616e 6e65  apsolver's Banne
+00000780: 7222 3e0a 3c2f 613e 0a3c 6272 3e0a 4174  r">.</a>.<br>.At
+00000790: 2074 6865 206c 6f77 6573 7420 7072 6963   the lowest pric
+000007a0: 6520 6f6e 2074 6865 206d 6172 6b65 742c  e on the market,
+000007b0: 2079 6f75 206d 6179 2072 6563 6569 7665   you may receive
+000007c0: 2061 2076 6172 6965 7479 206f 6620 736f   a variety of so
+000007d0: 6c75 7469 6f6e 732c 2069 6e63 6c75 6469  lutions, includi
+000007e0: 6e67 2072 6543 4150 5443 4841 2056 322c  ng reCAPTCHA V2,
+000007f0: 2072 6543 4150 5443 4841 2056 332c 2068   reCAPTCHA V3, h
+00000800: 4361 7074 6368 612c 2068 4361 7074 6368  Captcha, hCaptch
+00000810: 6120 436c 6963 6b2c 2046 756e 4361 7074  a Click, FunCapt
+00000820: 6368 612c 2070 6963 7475 7265 2d74 6f2d  cha, picture-to-
+00000830: 7465 7874 2c20 616e 6420 6d6f 7265 2e20  text, and more. 
+00000840: 5769 7468 2074 6869 7320 7365 7276 6963  With this servic
+00000850: 652c 2030 2e31 7320 6973 2074 6865 2073  e, 0.1s is the s
+00000860: 6c6f 7765 7374 2073 7065 6564 2065 7665  lowest speed eve
+00000870: 7220 6d65 6173 7572 6564 2e0a 3c68 723e  r measured..<hr>
+00000880: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
+00000890: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+000008a0: 2e66 7572 792e 696f 2f70 792f 7079 7468  .fury.io/py/pyth
+000008b0: 6f6e 332d 6361 7073 6f6c 7665 722e 7376  on3-capsolver.sv
+000008c0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+000008d0: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+000008e0: 686f 6e33 2d63 6170 736f 6c76 6572 290a  hon3-capsolver).
+000008f0: 5b21 5b50 7974 686f 6e20 7665 7273 696f  [![Python versio
+00000900: 6e73 5d28 6874 7470 733a 2f2f 696d 672e  ns](https://img.
+00000910: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000920: 7079 7665 7273 696f 6e73 2f70 7974 686f  pyversions/pytho
+00000930: 6e33 2d63 6170 736f 6c76 6572 2e73 7667  n3-capsolver.svg
+00000940: 3f6c 6f67 6f3d 7079 7468 6f6e 266c 6f67  ?logo=python&log
+00000950: 6f43 6f6c 6f72 3d46 4245 3037 3229 5d28  oColor=FBE072)](
+00000960: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000970: 7279 2e69 6f2f 7079 2f70 7974 686f 6e33  ry.io/py/python3
+00000980: 2d63 6170 736f 6c76 6572 290a 5b21 5b44  -capsolver).[![D
+00000990: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+000009a0: 2f2f 7065 7079 2e74 6563 682f 6261 6467  //pepy.tech/badg
+000009b0: 652f 7079 7468 6f6e 332d 6361 7073 6f6c  e/python3-capsol
+000009c0: 7665 722f 6d6f 6e74 6829 5d28 6874 7470  ver/month)](http
+000009d0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000009e0: 6f6a 6563 742f 7079 7468 6f6e 332d 6361  oject/python3-ca
+000009f0: 7073 6f6c 7665 7229 0a0a 5b21 5b4d 6169  psolver)..[![Mai
+00000a00: 6e74 6169 6e61 6269 6c69 7479 5d28 6874  ntainability](ht
+00000a10: 7470 733a 2f2f 6170 692e 636f 6465 636c  tps://api.codecl
+00000a20: 696d 6174 652e 636f 6d2f 7631 2f62 6164  imate.com/v1/bad
+00000a30: 6765 732f 3363 3330 3136 3762 3566 6233  ges/3c30167b5fb3
+00000a40: 3761 3037 3735 6561 2f6d 6169 6e74 6169  7a0775ea/maintai
+00000a50: 6e61 6269 6c69 7479 295d 2868 7474 7073  nability)](https
+00000a60: 3a2f 2f63 6f64 6563 6c69 6d61 7465 2e63  ://codeclimate.c
+00000a70: 6f6d 2f67 6974 6875 622f 416e 6472 6569  om/github/Andrei
+00000a80: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
+00000a90: 7073 6f6c 7665 722f 6d61 696e 7461 696e  psolver/maintain
+00000aa0: 6162 696c 6974 7929 0a5b 215b 436f 6461  ability).[![Coda
+00000ab0: 6379 2042 6164 6765 5d28 6874 7470 733a  cy Badge](https:
+00000ac0: 2f2f 6170 702e 636f 6461 6379 2e63 6f6d  //app.codacy.com
+00000ad0: 2f70 726f 6a65 6374 2f62 6164 6765 2f47  /project/badge/G
+00000ae0: 7261 6465 2f33 3233 6434 6564 6130 6665  rade/323d4eda0fe
+00000af0: 3134 3737 6262 6561 3866 6538 3930 3262  1477bbea8fe8902b
+00000b00: 3965 3937 6529 5d28 6874 7470 733a 2f2f  9e97e)](https://
+00000b10: 7777 772e 636f 6461 6379 2e63 6f6d 2f67  www.codacy.com/g
+00000b20: 682f 416e 6472 6569 4472 616e 672f 7079  h/AndreiDrang/py
+00000b30: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
+00000b40: 6461 7368 626f 6172 643f 7574 6d5f 736f  dashboard?utm_so
+00000b50: 7572 6365 3d67 6974 6875 622e 636f 6d26  urce=github.com&
+00000b60: 616d 703b 7574 6d5f 6d65 6469 756d 3d72  amp;utm_medium=r
+00000b70: 6566 6572 7261 6c26 616d 703b 7574 6d5f  eferral&amp;utm_
+00000b80: 636f 6e74 656e 743d 416e 6472 6569 4472  content=AndreiDr
+00000b90: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
+00000ba0: 6f6c 7665 7226 616d 703b 7574 6d5f 6361  olver&amp;utm_ca
+00000bb0: 6d70 6169 676e 3d42 6164 6765 5f47 7261  mpaign=Badge_Gra
+00000bc0: 6465 290a 5b21 5b63 6f64 6563 6f76 5d28  de).[![codecov](
+00000bd0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000be0: 696f 2f67 682f 416e 6472 6569 4472 616e  io/gh/AndreiDran
+00000bf0: 672f 7079 7468 6f6e 332d 6361 7073 6f6c  g/python3-capsol
+00000c00: 7665 722f 6272 616e 6368 2f6d 6169 6e2f  ver/branch/main/
+00000c10: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000c20: 746f 6b65 6e3d 324c 3456 5649 4634 4738  token=2L4VVIF4G8
+00000c30: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000c40: 6f76 2e69 6f2f 6768 2f41 6e64 7265 6944  ov.io/gh/AndreiD
+00000c50: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
+00000c60: 736f 6c76 6572 290a 0a5b 215b 5370 6869  solver)..[![Sphi
+00000c70: 6e78 2062 7569 6c64 5d28 6874 7470 733a  nx build](https:
+00000c80: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6e64  //github.com/And
+00000c90: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
+00000ca0: 2d63 6170 736f 6c76 6572 2f61 6374 696f  -capsolver/actio
+00000cb0: 6e73 2f77 6f72 6b66 6c6f 7773 2f73 7068  ns/workflows/sph
+00000cc0: 696e 782e 796d 6c2f 6261 6467 652e 7376  inx.yml/badge.sv
+00000cd0: 673f 6272 616e 6368 3d72 656c 6561 7365  g?branch=release
+00000ce0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000cf0: 622e 636f 6d2f 416e 6472 6569 4472 616e  b.com/AndreiDran
+00000d00: 672f 7079 7468 6f6e 332d 6361 7073 6f6c  g/python3-capsol
+00000d10: 7665 722f 6163 7469 6f6e 732f 776f 726b  ver/actions/work
+00000d20: 666c 6f77 732f 7370 6869 6e78 2e79 6d6c  flows/sphinx.yml
+00000d30: 290a 5b21 5b42 7569 6c64 5d28 6874 7470  ).[![Build](http
+00000d40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000d50: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
+00000d60: 6e33 2d63 6170 736f 6c76 6572 2f61 6374  n3-capsolver/act
+00000d70: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+00000d80: 7569 6c64 2e79 6d6c 2f62 6164 6765 2e73  uild.yml/badge.s
+00000d90: 7667 3f62 7261 6e63 683d 6d61 696e 295d  vg?branch=main)]
+00000da0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000db0: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
+00000dc0: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
+00000dd0: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000de0: 6f77 732f 6275 696c 642e 796d 6c29 0a5b  ows/build.yml).[
+00000df0: 215b 496e 7374 616c 6c61 7469 6f6e 5d28  ![Installation](
+00000e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000e10: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
+00000e20: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
+00000e30: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000e40: 7773 2f69 6e73 7461 6c6c 2e79 6d6c 2f62  ws/install.yml/b
+00000e50: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
+00000e60: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
+00000e70: 6974 6875 622e 636f 6d2f 416e 6472 6569  ithub.com/Andrei
+00000e80: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
+00000e90: 7073 6f6c 7665 722f 6163 7469 6f6e 732f  psolver/actions/
+00000ea0: 776f 726b 666c 6f77 732f 696e 7374 616c  workflows/instal
+00000eb0: 6c2e 796d 6c29 0a5b 215b 5465 7374 735d  l.yml).[![Tests]
+00000ec0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000ed0: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
+00000ee0: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
+00000ef0: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000f00: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+00000f10: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000f20: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000f30: 6875 622e 636f 6d2f 416e 6472 6569 4472  hub.com/AndreiDr
+00000f40: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
+00000f50: 6f6c 7665 722f 6163 7469 6f6e 732f 776f  olver/actions/wo
+00000f60: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
+00000f70: 290a 5b21 5b4c 696e 745d 2868 7474 7073  ).[![Lint](https
+00000f80: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+00000f90: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
+00000fa0: 332d 6361 7073 6f6c 7665 722f 6163 7469  3-capsolver/acti
+00000fb0: 6f6e 732f 776f 726b 666c 6f77 732f 6c69  ons/workflows/li
+00000fc0: 6e74 2e79 6d6c 2f62 6164 6765 2e73 7667  nt.yml/badge.svg
+00000fd0: 3f62 7261 6e63 683d 6d61 696e 295d 2868  ?branch=main)](h
+00000fe0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ff0: 6d2f 416e 6472 6569 4472 616e 672f 7079  m/AndreiDrang/py
+00001000: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
+00001010: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00001020: 732f 6c69 6e74 2e79 6d6c 290a 0a0a 5079  s/lint.yml)...Py
+00001030: 7468 6f6e 2033 206c 6962 7261 7279 2066  thon 3 library f
+00001040: 6f72 205b 4361 7073 6f6c 7665 725d 2868  or [Capsolver](h
+00001050: 7474 7073 3a2f 2f64 6173 6862 6f61 7264  ttps://dashboard
+00001060: 2e63 6170 736f 6c76 6572 2e63 6f6d 2f70  .capsolver.com/p
+00001070: 6173 7370 6f72 742f 7265 6769 7374 6572  assport/register
+00001080: 3f69 6e76 6974 6543 6f64 653d 6b51 546e  ?inviteCode=kQTn
+00001090: 2d74 4730 374a 6231 2920 7365 7276 6963  -tG07Jb1) servic
+000010a0: 6520 4150 492e 0a0a 5465 7374 6564 206f  e API...Tested o
+000010b0: 6e20 554e 4958 2062 6173 6564 204f 532e  n UNIX based OS.
+000010c0: 0a0a 5468 6520 6c69 6272 6172 7920 6973  ..The library is
+000010d0: 2069 6e74 656e 6465 6420 666f 7220 736f   intended for so
+000010e0: 6674 7761 7265 2064 6576 656c 6f70 6572  ftware developer
+000010f0: 7320 616e 6420 6973 2075 7365 6420 746f  s and is used to
+00001100: 2077 6f72 6b20 7769 7468 2074 6865 205b   work with the [
+00001110: 4361 7073 6f6c 7665 725d 2868 7474 7073  Capsolver](https
+00001120: 3a2f 2f64 6173 6862 6f61 7264 2e63 6170  ://dashboard.cap
+00001130: 736f 6c76 6572 2e63 6f6d 2f70 6173 7370  solver.com/passp
+00001140: 6f72 742f 7265 6769 7374 6572 3f69 6e76  ort/register?inv
+00001150: 6974 6543 6f64 653d 6b51 546e 2d74 4730  iteCode=kQTn-tG0
+00001160: 374a 6231 2920 7365 7276 6963 6520 4150  7Jb1) service AP
+00001170: 492e 0a0a 2a2a 2a0a 0a49 6620 796f 7520  I...***..If you 
+00001180: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
+00001190: 6e73 2c20 706c 6561 7365 2073 656e 6420  ns, please send 
+000011a0: 6120 6d65 7373 6167 6520 746f 2074 6865  a message to the
+000011b0: 205b 5465 6c65 6772 616d 5d28 6874 7470   [Telegram](http
+000011c0: 733a 2f2f 742e 6d65 2f70 7974 686f 6e63  s://t.me/pythonc
+000011d0: 6170 7463 6861 2920 6368 6174 2072 6f6f  aptcha) chat roo
+000011e0: 6d2e 0a0a 4f72 2065 6d61 696c 2070 7974  m...Or email pyt
+000011f0: 686f 6e2d 6361 7074 6368 6140 706d 2e6d  hon-captcha@pm.m
+00001200: 650a 0a2a 2a2a 0a0a 2323 2048 6f77 2074  e..***..## How t
+00001210: 6f20 696e 7374 616c 6c3f 0a0a 5765 2072  o install?..We r
+00001220: 6563 6f6d 6d65 6e64 2075 7369 6e67 2074  ecommend using t
+00001230: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
+00001240: 6e20 6f66 2050 7974 686f 6e2e 2060 7079  n of Python. `py
+00001250: 7468 6f6e 332d 6361 7073 6f6c 7665 7260  thon3-capsolver`
+00001260: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
+00001270: 2033 2e37 2b2e 0a0a 2323 2320 7069 700a   3.7+...### pip.
+00001280: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+00001290: 7461 6c6c 2070 7974 686f 6e33 2d63 6170  tall python3-cap
+000012a0: 736f 6c76 6572 0a60 6060 0a0a 2323 2048  solver.```..## H
+000012b0: 6f77 2074 6f20 7573 653f 0a0a 4973 2064  ow to use?..Is d
+000012c0: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+000012d0: 5b64 6f63 756d 656e 7461 7469 6f6e 2d77  [documentation-w
+000012e0: 6562 7369 7465 5d28 6874 7470 733a 2f2f  ebsite](https://
+000012f0: 616e 6472 6569 6472 616e 672e 6769 7468  andreidrang.gith
+00001300: 7562 2e69 6f2f 7079 7468 6f6e 332d 6361  ub.io/python3-ca
+00001310: 7073 6f6c 7665 722f 292e 0a0a 0a23 2320  psolver/)....## 
+00001320: 486f 7720 746f 2074 6573 743f 0a0a 312e  How to test?..1.
+00001330: 2059 6f75 206e 6565 6420 7365 7420 6060   You need set ``
+00001340: 4150 495f 4b45 5960 6020 696e 2079 6f75  API_KEY`` in you
+00001350: 7220 656e 7669 726f 6e6d 656e 7428 6765  r environment(ge
+00001360: 7420 7468 6973 2076 616c 7565 2066 726f  t this value fro
+00001370: 6d20 796f 7520 6163 636f 756e 7429 2e0a  m you account)..
+00001380: 322e 2052 756e 2063 6f6d 6d61 6e64 2060  2. Run command `
+00001390: 606d 616b 6520 7465 7374 7360 602c 2066  `make tests``, f
+000013a0: 726f 6d20 726f 6f74 2064 6972 6563 746f  rom root directo
+000013b0: 7279 2e0a 0a0a 2323 2320 4368 616e 6765  ry....### Change
+000013c0: 6c6f 670a 0a43 6865 636b 205b 7265 6c65  log..Check [rele
+000013d0: 6173 6573 2070 6167 655d 2868 7474 7073  ases page](https
+000013e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+000013f0: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
+00001400: 332d 6361 7073 6f6c 7665 722f 7265 6c65  3-capsolver/rele
+00001410: 6173 6573 292e 0a0a 2323 2320 486f 7720  ases)...### How 
+00001420: 746f 2067 6574 2041 5049 204b 6579 2074  to get API Key t
+00001430: 6f20 776f 726b 2077 6974 6820 7468 6520  o work with the 
+00001440: 6c69 6272 6172 790a 312e 204f 6e20 7468  library.1. On th
+00001450: 6520 7061 6765 202d 2068 7474 7073 3a2f  e page - https:/
+00001460: 2f64 6173 6862 6f61 7264 2e63 6170 736f  /dashboard.capso
+00001470: 6c76 6572 2e63 6f6d 2f6f 7665 7276 6965  lver.com/overvie
+00001480: 772f 7573 6572 2d63 656e 7465 720a 322e  w/user-center.2.
+00001490: 2046 696e 6420 6974 3a20 215b 696d 672e   Find it: ![img.
+000014a0: 706e 675d 2866 696c 6573 2f69 6d67 2e70  png](files/img.p
+000014b0: 6e67 290a                                ng).
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/cloudflare.py` & `python3-capsolver-0.7.1/python3_capsolver/cloudflare.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,45 +22,45 @@
         >>> Cloudflare(api_key="CAI-1324...",
         ...             captcha_type=CloudflareTypeEnm.AntiCloudflareTask,
         ...             websiteURL="https://bck.websiteurl.com/registry",
         ...             websiteKey='4ac25d',
         ...             proxy="socks5:158.120.100.23:334:user:pass",
         ...             metadata={'type': 'turnstile', 'acton':'login', 'cdata': '0000-1111-2222-3333-example-cdata'}
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> Cloudflare(api_key="CAI-1324...",
         ...             captcha_type=CloudflareTypeEnm.AntiCloudflareTask,
         ...             websiteURL="https://bck.websiteurl.com/registry",
         ...             proxy="socks5:158.120.100.23:334:user:pass",
         ...             metadata={'type': 'challenge'}
         ...             html="<your challenge html source code>",
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> await Cloudflare(api_key="CAI-1324...",
         ...             captcha_type=CloudflareTypeEnm.AntiCloudflareTask,
         ...             websiteURL="https://bck.websiteurl.com/registry",
         ...             websiteKey='4ac25d',
         ...             proxy="socks5:158.120.100.23:334:user:pass",
         ...             metadata={'type': 'challenge', 'acton':'login', 'cdata': '0000-1111-2222-3333-example-cdata'}
         ...          ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/control.py` & `python3-capsolver-0.7.1/python3_capsolver/control.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6.1/python3_capsolver/core/base.py` & `python3-capsolver-0.7.1/python3_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6.1/python3_capsolver/core/config.py` & `python3-capsolver-0.7.1/python3_capsolver/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tenacity import AsyncRetrying, wait_fixed, stop_after_attempt
 from requests.adapters import Retry
 
 RETRIES = Retry(total=5, backoff_factor=0.9, status_forcelist=[500, 502, 503, 504])
 ASYNC_RETRIES = AsyncRetrying(wait=wait_fixed(5), stop=stop_after_attempt(5), reraise=True)
 
 REQUEST_URL = "https://api.capsolver.com"
-VALID_STATUS_CODES = (200, 400, 401)
+VALID_STATUS_CODES = (200, 202, 400, 401, 405)
 
 APP_ID = "3E36E3CD-7EB5-4CAF-AA15-91011E652321"
 
 
 # Connection retry generator
 def attempts_generator(amount: int = 16) -> Generator:
     """
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/core/enum.py` & `python3-capsolver-0.7.1/python3_capsolver/core/enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,56 +30,47 @@
         """
         return self._value_
 
 
 class EndpointPostfixEnm(str, MyEnum):
     """
     Enum stored URL postfixes for API endpoints
-
-    Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426042
     """
 
     GET_BALANCE = "getBalance"
     CREATE_TASK = "createTask"
     GET_TASK_RESULT = "getTaskResult"
 
 
-class CaptchaTypeEnmXXX(str, MyEnum):
-    """
-    Enum with all available captcha types
-
-    Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/393295
-    """
-
+class ImageToTextTaskTypeEnm(str, MyEnum):
     ImageToTextTask = "ImageToTextTask"
-    # HCaptcha
-    HCaptchaClassification = "HCaptchaClassification"
-    # FunCaptcha
-    FunCaptchaClassification = "FunCaptchaClassification"
-    # Other types
-    AntiKasadaTask = "AntiKasadaTask"
-    AntiAkamaiBMPTask = "AntiAkamaiBMPTask"
 
 
 class HCaptchaTypeEnm(str, MyEnum):
     HCaptchaTask = "HCaptchaTask"
     HCaptchaTaskProxyless = "HCaptchaTaskProxyless"
     HCaptchaEnterpriseTask = "HCaptchaEnterpriseTask"
     HCaptchaEnterpriseTaskProxyLess = "HCaptchaEnterpriseTaskProxyLess"
     HCaptchaTurboTask = "HCaptchaTurboTask"
-    HCaptchaTurboTaskProxyLess = "HCaptchaTurboTaskProxyLess"
+    HCaptchaClassification = "HCaptchaClassification"
+
+
+class HCaptchaClassificationTypeEnm(str, MyEnum):
+    HCaptchaClassification = "HCaptchaClassification"
 
 
 class FunCaptchaTypeEnm(str, MyEnum):
     FunCaptchaTask = "FunCaptchaTask"
     FunCaptchaTaskProxyLess = "FunCaptchaTaskProxyLess"
 
 
+class FunCaptchaClassificationTypeEnm(str, MyEnum):
+    FunCaptchaClassification = "FunCaptchaClassification"
+
+
 class GeeTestCaptchaTypeEnm(str, MyEnum):
     GeeTestTask = "GeeTestTask"
     GeeTestTaskProxyLess = "GeeTestTaskProxyLess"
 
 
 class ReCaptchaV2TypeEnm(str, MyEnum):
     # V2
@@ -105,19 +96,29 @@
     DatadomeSliderTask = "DatadomeSliderTask"
 
 
 class CloudflareTypeEnm(str, MyEnum):
     AntiCloudflareTask = "AntiCloudflareTask"
 
 
+class AntiAwsWafTaskTypeEnm(str, MyEnum):
+    AntiAwsWafTask = "AntiAwsWafTask"
+    AntiAwsWafTaskProxyLess = "AntiAwsWafTaskProxyLess"
+
+
+class AntiCyberSiAraTaskTypeEnm(str, MyEnum):
+    AntiCyberSiAraTask = "AntiCyberSiAraTask"
+    AntiCyberSiAraTaskProxyLess = "AntiCyberSiAraTaskProxyLess"
+
+
 class ResponseStatusEnm(str, MyEnum):
     """
     Enum store results `status` field variants
 
     Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426124
+        https://docs.capsolver.com/guide/api-createtask.html
     """
 
     Idle = "idle"  # Task created
     Processing = "processing"  # Task is not ready yet
     Ready = "ready"  # Task completed, solution object can be found in solution property
     Failed = "failed"  # Task failed, check the errorDescription to know why failed.
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/core/serializer.py` & `python3-capsolver-0.7.1/python3_capsolver/core/serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,14 +83,22 @@
 class HCaptchaClassificationOptionsSer(BaseModel):
     queries: List[str] = Field(..., description="Base64-encoded images, do not include 'data:image/***;base64,'")
     question: str = Field(
         ..., description="Question ID. Support English and Chinese, other languages please convert yourself"
     )
 
 
+class FunCaptchaClassificationOptionsSer(BaseModel):
+    images: List[str] = Field(..., description="Base64-encoded images, do not include 'data:image/***;base64,'")
+    question: str = Field(
+        ...,
+        description="Question name. this param value from API response game_variant field. Exmaple: maze,maze2,flockCompass,3d_rollball_animals",
+    )
+
+
 class GeeTestSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with Geetest")
     gt: str = Field(..., description="The domain public key, rarely updated")
     challenge: Optional[str] = Field(
         "",
         description="If you need to solve Geetest V3 you must use this parameter, don't need if you need to solve GeetestV4",
     )
@@ -105,26 +113,22 @@
         "Most FunCaptcha installations work from shared domains.",
     )
 
 
 class DatadomeSliderSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with DatadomeSlider")
     captchaUrl: str = Field(..., description="Captcha Url where is the captcha")
-    proxy: str = Field(..., description="Proxy data")
     userAgent: str = Field(..., description="Browser's User-Agent which is used in emulation")
 
 
-class KasadaOptionsSer(BaseModel):
-    pageURL: str = Field(..., description="Address of a webpage with Kasada")
-    proxyLogin: str = Field(
-        ...,
-        description="Login for proxy which requires authorizaiton (basic)."
-        "This isn’t required if you are using proxies authenticated by IP",
-    )
-    proxyPassword: str = Field(..., description="This isn’t required if you are using proxies authenticated by IP")
-
-
 class CloudflareTurnstileSer(WebsiteDataOptionsSer):
     metadata: dict = Field(..., description="Extra data")
     html: Optional[str] = Field(
         None, description="You can pass in the entire html source code for the challenge directly."
     )
+
+
+class CyberSiAraSer(WebsiteDataOptionsSer):
+    SlideMasterUrlId: str = Field(
+        ..., description="You can get MasterUrlId param form `api/CyberSiara/GetCyberSiara` endpoint request"
+    )
+    UserAgent: str = Field(..., description="Browser userAgent, you need submit your userAgent")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/datadome_slider.py` & `python3-capsolver-0.7.1/python3_capsolver/datadome_slider.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,30 +20,30 @@
         >>> DatadomeSlider(api_key="CAI-1324...",
         ...         captcha_type=DatadomeSliderTypeEnm.DatadomeSliderTask,
         ...         websiteURL="https://www.some-url.com/",
         ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
         ...         proxy="socks5:158.120.100.23:334:user:pass",
         ...         userAgent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
         ...        ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> await DatadomeSlider(api_key="CAI-1324...",
         ...         captcha_type="DatadomeSliderTask",
         ...         websiteURL="https://www.some-url.com/",
         ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
         ...         proxy="socks5:158.120.100.23:334:user:pass",
         ...         userAgent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
         ...        ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
@@ -52,19 +52,18 @@
 
     Notes:
         https://docs.capsolver.com/guide/antibots/datadome.html
     """
 
     def __init__(
         self,
-        captcha_type: Union[DatadomeSliderTypeEnm, str],
         websiteURL: str,
         captchaUrl: str,
-        proxy: str,
         userAgent: str,
+        captcha_type: Union[DatadomeSliderTypeEnm, str] = DatadomeSliderTypeEnm.DatadomeSliderTask,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         if captcha_type in DatadomeSliderTypeEnm.list():
             self.task_params = DatadomeSliderSer(**locals()).dict()
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/fun_captcha.py` & `python3-capsolver-0.7.1/python3_capsolver/fun_captcha.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Union
+from typing import List, Union
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import FunCaptchaTypeEnm
-from python3_capsolver.core.serializer import FunCaptchaSer, CaptchaResponseSer
+from python3_capsolver.core.enum import FunCaptchaTypeEnm, FunCaptchaClassificationTypeEnm
+from python3_capsolver.core.serializer import FunCaptchaSer, CaptchaResponseSer, FunCaptchaClassificationOptionsSer
 
 
 class FunCaptcha(BaseCaptcha):
     """
     The class is used to work with Capsolver FuncaptchaTask methods.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``FuncaptchaTaskProxyless`` and etc.
+        captcha_type: Captcha type name, like ``FunCaptchaTaskProxyLess`` and etc.
         websiteURL: Address of a webpage with Geetest.
         websitePublicKey: Funcaptcha website key.
 
     Examples:
         >>> with FunCaptcha(api_key="CAI-1324...",
-        ...             captcha_type="FuncaptchaTaskProxyless",
+        ...             captcha_type="FunCaptchaTaskProxyLess",
         ...             websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
         ...             websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
         ...             funcaptchaApiJSSubdomain="https://api.funcaptcha.com/"
         ...         ) as instance:
         >>>     instance.captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'token': '44795sds...'}
                           )
 
         >>> with FunCaptcha(api_key="CAI-1324...",
-        ...             captcha_type="FuncaptchaTaskProxyless",
+        ...             captcha_type="FunCaptchaTaskProxyLess",
         ...             websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
         ...             websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
         ...             funcaptchaApiJSSubdomain="https://api.funcaptcha.com/"
         ...         ) as instance:
         >>>     await instance.aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'token': '44795sds...'}
                           )
 
@@ -50,15 +50,15 @@
         CaptchaResponseSer model with full server response
 
     Notes:
         https://docs.capsolver.com/guide/captcha/FunCaptcha.html
     """
 
     def __init__(
-        self, captcha_type: Union[FunCaptchaSer, str], websiteURL: str, websitePublicKey: str, *args, **kwargs
+        self, captcha_type: Union[FunCaptchaTypeEnm, str], websiteURL: str, websitePublicKey: str, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
 
         if captcha_type in FunCaptchaTypeEnm.list():
             self.task_params = FunCaptchaSer(**locals()).dict()
         else:
             raise ValueError(
@@ -70,20 +70,20 @@
 
     def captcha_handler(self) -> CaptchaResponseSer:
         """
         Sync solving method
 
         Examples:
             >>> FunCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
-            ...         captcha_type="FuncaptchaTaskProxyless",
+            ...         captcha_type="FunCaptchaTaskProxyLess",
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
             ...         websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
             ...         funcaptchaApiJSSubdomain="https://api.funcaptcha.com/"
             ...        ).captcha_handler()
-            CaptchaResponseSer(errorId=False,
+            CaptchaResponseSer(errorId=0,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'token': '44795sds...'}
                               )
 
@@ -92,15 +92,15 @@
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
             ...         websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
             ...         funcaptchaApiJSSubdomain="https://api.funcaptcha.com/",
             ...         proxyType="http",
             ...         proxyAddress="0.0.0.0",
             ...         proxyPort=9090,
             ...        ).captcha_handler()
-            CaptchaResponseSer(errorId=False,
+            CaptchaResponseSer(errorId=0,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'token': '44795sds...'}
                               )
 
@@ -114,20 +114,20 @@
 
     async def aio_captcha_handler(self) -> CaptchaResponseSer:
         """
         Async method for captcha solving
 
         Examples:
             >>> await FunCaptcha(api_key="CAI-1324...",
-            ...         captcha_type="FuncaptchaTaskProxyless",
+            ...         captcha_type="FunCaptchaTaskProxyLess",
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
             ...         websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
             ...         funcaptchaApiJSSubdomain="https://api.funcaptcha.com/"
             ...        ).aio_captcha_handler()
-            CaptchaResponseSer(errorId=False,
+            CaptchaResponseSer(errorId=0,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'token': '44795sds...'}
                               )
 
@@ -136,15 +136,15 @@
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
             ...         websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
             ...         funcaptchaApiJSSubdomain="https://api.funcaptcha.com/",
             ...         proxyType="http",
             ...         proxyAddress="0.0.0.0",
             ...         proxyPort=9090,
             ...        ).aio_captcha_handler()
-            CaptchaResponseSer(errorId=False,
+            CaptchaResponseSer(errorId=0,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'token': '44795sds...'}
                               )
 
@@ -152,22 +152,100 @@
             ...    img_data = img_file.read()
             >>> body = base64.b64encode(img_data).decode("utf-8")
             >>> await FunCaptcha(api_key="CAI-1324...",
             ...         captcha_type="FunCaptchaClassification"
             ...        ).aio_captcha_handler(
             ...                     image=body,
             ...                     question="Ask your question")
-            CaptchaResponseSer(errorId=False,
+            CaptchaResponseSer(errorId=0,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'token': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
             Check class docstring for more info
         """
+        return await self._aio_processing_captcha(create_params=self.task_params)
+
+
+class FunCaptchaClassification(BaseCaptcha):
+    """
+    The class is used to work with Capsolver FunCaptchaClassification methods.
+
+    Args:
+        api_key: Capsolver API key
+        captcha_type: Captcha type name, like ``FunCaptchaClassification`` and etc.
+        images: Base64 encoded image, can be a screenshot (pass only the hexagonal image, do not pass the rest of the content)
+        question: Question name. this param value from API response game_variant field. Exmaple: maze,maze2,flockCompass,3d_rollball_animals
+
+    Examples:
+        >>> FunCaptchaClassification(api_key="CAI-1324...",
+        ...             captcha_type="FunCaptchaClassification",
+        ...             images=["image payload"],
+        ...             question="maze2",
+        ...         ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={"objects": [ 4 ]}
+                          )
+
+    Returns:
+        CaptchaResponseSer model with full server response
+
+    Notes:
+        https://docs.capsolver.com/guide/recognition/FunCaptchaClassification.html
+    """
+
+    def __init__(
+        self,
+        images: List[str],
+        question: str,
+        captcha_type: Union[
+            FunCaptchaClassificationTypeEnm, str
+        ] = FunCaptchaClassificationTypeEnm.FunCaptchaClassification,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+
+        if captcha_type in FunCaptchaClassificationTypeEnm.list():
+            self.task_params = FunCaptchaClassificationOptionsSer(**locals()).dict()
+        else:
+            raise ValueError(
+                f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
+                available - {FunCaptchaClassificationTypeEnm.list()}"""
+            )
+        for key in kwargs:
+            self.task_params.update({key: kwargs[key]})
+
+    def captcha_handler(self) -> CaptchaResponseSer:
+        """
+        Sync solving method
+
+        Returns:
+            CaptchaResponseSer model with full service response
+
+        Notes:
+            Check class docstring for more info
+        """
+        return self._processing_captcha(create_params=self.task_params)
+
+    async def aio_captcha_handler(self) -> CaptchaResponseSer:
+        """
+        Async method for captcha solving
+
+        Returns:
+            CaptchaResponseSer model with full service response
+
+        Notes:
+            Check class docstring for more info
+        """
         return await self._aio_processing_captcha(create_params=self.task_params)
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/gee_test.py` & `python3-capsolver-0.7.1/python3_capsolver/gee_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,60 +3,60 @@
 from python3_capsolver.core.base import BaseCaptcha
 from python3_capsolver.core.enum import GeeTestCaptchaTypeEnm
 from python3_capsolver.core.serializer import GeeTestSer, CaptchaResponseSer
 
 
 class GeeTest(BaseCaptcha):
     """
-    The class is used to work with Capsolver GeetestTask methods.
+    The class is used to work with Capsolver GeeTestTask methods.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``GeetestTaskProxyless`` and etc.
+        captcha_type: Captcha type name, like ``GeeTestTaskProxyLess`` and etc.
         websiteURL: Address of a webpage with Geetest
         gt: The domain public key, rarely updated
         challenge: If you need to solve Geetest V3 you must use this parameter, don't need if you need to solve GeetestV4
 
     Examples:
         >>> GeeTest(api_key="CAI-1324...",
         ...         captcha_type=GeeTestCaptchaTypeEnm.GeeTestTaskProxyLess,
         ...         websiteURL="https://www.geetest.com/en/demo",
         ...         gt="022397c99c9f646f6477822485f30404",
         ...         challenge='12345678abc90123d45678ef90123a456b'
         ...        ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> GeeTest(api_key="CAI-1324...",
         ...         captcha_type=GeeTestCaptchaTypeEnm.GeeTestTask,
         ...         websiteURL="https://www.geetest.com/en/demo",
         ...         gt="022397c99c9f646f6477822485f30404",
         ...         challenge='12345678abc90123d45678ef90123a456b'
         ...         proxy="socks5:192.191.100.10:4780:user:pwd"
         ...        ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> await GeeTest(api_key="CAI-1324...",
         ...         captcha_type="GeetestTaskProxyless",
         ...         websiteURL="https://www.geetest.com/en/demo",
         ...         gt="022397c99c9f646f6477822485f30404",
         ...         challenge='12345678abc90123d45678ef90123a456b'
         ...        ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/hcaptcha.py` & `python3-capsolver-0.7.1/python3_capsolver/mt_captcha.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,103 +1,110 @@
 from typing import Union
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import HCaptchaTypeEnm
+from python3_capsolver.core.enum import MtCaptchaTypeEnm
 from python3_capsolver.core.serializer import CaptchaResponseSer, WebsiteDataOptionsSer
 
 
-class HCaptcha(BaseCaptcha):
+class MtCaptcha(BaseCaptcha):
     """
-    The class is used to work with Capsolver HCaptcha methods.
+    The class is used to work with Capsolver MtCaptcha method.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``HCaptchaTaskProxyless`` and etc.
-        websiteURL: Address of a webpage with hCaptcha
-        websiteKey: hCaptcha website key
+        captcha_type: Captcha type name, like ``MtCaptchaTask`` and etc.
+        websiteURL: Web address of the website using hcaptcha, generally it's fixed value. (Ex: https://google.com)
+        websiteKey: The domain public key, rarely updated. (Ex: sk=MTPublic-xxx public key)
 
     Examples:
-        >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
-        ...          captcha_type='HCaptchaTaskProxyless',
-        ...          websiteURL="https://accounts.hcaptcha.com/demo",
-        ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
-        ...         ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTaskProxyLess,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...        ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
-        >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
-        ...          captcha_type=HCaptchaTypeEnm.HCaptchaEnterpriseTaskProxyLess,
-        ...          websiteURL="https://accounts.hcaptcha.com/demo",
-        ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
-        ...         ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
-        >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
-        ...          captcha_type=HCaptchaTypeEnm.HCaptchaTask,
-        ...          websiteURL="https://accounts.hcaptcha.com/demo",
-        ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
-        ...          proxy="socks5:192.191.100.10:4780:user:pwd"
-        ...          isInvisible=True
-        ...         ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> await MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).aio_captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
-        >>> await HCaptcha(api_key="CAI-BA9650D2B9C2786B21120D512702E010",
-        ...          captcha_type=HCaptchaTypeEnm.HCaptchaTaskProxyless,
-        ...          websiteURL="https://accounts.hcaptcha.com/demo",
-        ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
-        ...         ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> await MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).aio_captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                            solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://docs.capsolver.com/guide/captcha/HCaptcha.html
+        https://docs.capsolver.com/guide/captcha/MtCaptcha.html
     """
 
-    def __init__(self, captcha_type: Union[HCaptchaTypeEnm, str], websiteURL: str, websiteKey: str, *args, **kwargs):
+    def __init__(
+        self,
+        captcha_type: Union[MtCaptchaTypeEnm, str],
+        websiteURL: str,
+        websiteKey: str,
+        *args,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
 
-        if captcha_type in HCaptchaTypeEnm.list():
+        if captcha_type in MtCaptchaTypeEnm.list():
             self.task_params = WebsiteDataOptionsSer(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
-                available - {HCaptchaTypeEnm.list_values()}"""
+                available - {MtCaptchaTypeEnm}"""
             )
-
         for key in kwargs:
             self.task_params.update({key: kwargs[key]})
 
     def captcha_handler(self) -> CaptchaResponseSer:
         """
-        Sync solving method
+        Sync method for captcha solving
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
             Check class docstring for more info
         """
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/image_to_text.py` & `python3-capsolver-0.7.1/python3_capsolver/image_to_text.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,147 +1,151 @@
+from typing import Union
+
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.config import REQUEST_URL
-from python3_capsolver.core.serializer import CaptchaResponseSer, RequestCreateTaskSer
+from python3_capsolver.core.enum import ImageToTextTaskTypeEnm
+from python3_capsolver.core.serializer import TaskSer, CaptchaResponseSer
 
 
-class BaseImageToText(BaseCaptcha):
+class ImageToText(BaseCaptcha):
     """
     The class is used to work with Capsolver Image captcha solving methods.
 
     Args:
         api_key: Capsolver API key
-        sleep_time: The waiting time between requests to get the result of the Captcha
-        request_url: API address for sending requests
+        captcha_type: Captcha type name, like ``ImageToTextTask`` and etc.
 
     Examples:
         >>> with open('some_image.jpeg', 'rb') as img_file:
         ...    img_data = img_file.read()
         >>> body = base64.b64encode(img_data).decode("utf-8")
         >>> ImageToText(api_key="CAI-12345....").captcha_handler(body=body)
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'confidence': 0.9585, 'text': 'gcphjd'}
+                          )
+
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> ImageToText(api_key="CAI-12345....",
+        ...             module='queueit'
+        ...            ).captcha_handler(body=body)
+        CaptchaResponseSer(errorId=0,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={'confidence': 0.9585, 'text': 'zzzzz'}
+                          )
+
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> ImageToText(api_key="CAI-12345....",
+        ...             module='dell',
+        ...             score=0.98,
+        ...             case=True,
+        ...            ).captcha_handler(body=body)
+        CaptchaResponseSer(errorId=0,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={'confidence': 0.9585, 'text': 'gcphjd'}
                           )
 
         >>> with open('some_image.jpeg', 'rb') as img_file:
         ...    img_data = img_file.read()
         >>> body = base64.b64encode(img_data).decode("utf-8")
         >>> with ImageToText(api_key="CAI-12345....") as image_to_text_inst:
         ...    image_to_text_inst.captcha_handler(body=body)
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'confidence': 0.9585, 'text': 'gcphjd'}
                           )
 
         >>> with open('some_image.jpeg', 'rb') as img_file:
         ...    img_data = img_file.read()
         >>> body = base64.b64encode(img_data).decode("utf-8")
         >>> await ImageToText(api_key="CAI-12345....").aio_captcha_handler(body=body)
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'confidence': 0.9585, 'text': 'gcphjd'}
                           )
 
         >>> with open('some_image.jpeg', 'rb') as img_file:
         ...    img_data = img_file.read()
         >>> body = base64.b64encode(img_data).decode("utf-8")
         >>> with ImageToText(api_key="CAI-12345....") as image_to_text_inst:
         ...    await image_to_text_inst.aio_captcha_handler(body=body)
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'confidence': 0.9585, 'text': 'gcphjd'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/393427
+        https://docs.capsolver.com/guide/recognition/ImageToTextTask.html
     """
 
     def __init__(
         self,
-        api_key: str,
-        sleep_time: int = 10,
-        request_url: str = REQUEST_URL,
+        captcha_type: Union[ImageToTextTaskTypeEnm, str] = ImageToTextTaskTypeEnm.ImageToTextTask,
+        *args,
+        **kwargs,
     ):
-        super().__init__(api_key=api_key, sleep_time=sleep_time, request_url=request_url)
-
-
-class ImageToText(BaseImageToText):
-    __doc__ = BaseImageToText.__doc__
+        super().__init__(*args, **kwargs)
+        if captcha_type in ImageToTextTaskTypeEnm.list():
+            self.task_params = TaskSer(**locals()).dict(exclude_none=True)
+        else:
+            raise ValueError(
+                f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
+                available - {ImageToTextTaskTypeEnm.list()}"""
+            )
+        for key in kwargs:
+            self.task_params.update({key: kwargs[key]})
 
-    def captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
+    def captcha_handler(self, body: str) -> CaptchaResponseSer:
         """
         Synchronous method for captcha solving
 
         Args:
-            body: Base64 encoded content of the image
-            additional_params: Some additional parameters that will be used in creating the task
-                                and will be passed to the payload under ``task`` key
-
-        Examples:
-            >>> with open('some_image.jpeg', 'rb') as img_file:
-            ...    img_data = img_file.read()
-            >>> body = base64.b64encode(img_data).decode("utf-8")
-            >>> ImageToText(api_key="CAI-12345....").captcha_handler(body=body)
-            CaptchaResponseSer(errorId=False,
-                               errorCode=None,
-                               errorDescription=None,
-                               taskId='73bdcd28-6c77-4414-8....',
-                               status=<ResponseStatusEnm.Ready: 'ready'>,
-                               solution={'gRecaptchaResponse': '44795sds...'}
-                              )
+            body: Base64 encoded content of the image, decoded into str
 
         Returns:
             CaptchaResponseSer model with full server response
 
         Notes:
             Check class docstring for more info
         """
-        return self._processing_captcha(
-            serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
-        )
+        self.task_params.update({"body": body})
+        return self._processing_captcha(create_params=self.task_params)
 
-    async def aio_captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
+    async def aio_captcha_handler(self, body: str) -> CaptchaResponseSer:
         """
         Asynchronous method for captcha solving
 
         Args:
-            body: Base64 encoded content of the image
-            additional_params: Some additional parameters that will be used in creating the task
-                                and will be passed to the payload under ``task`` key
-
-        Examples:
-            >>> with open('some_image.jpeg', 'rb') as img_file:
-            ...    img_data = img_file.read()
-            >>> body = base64.b64encode(img_data).decode("utf-8")
-            >>> await ImageToText(api_key="CAI-12345....").aio_captcha_handler(body=body)
-            CaptchaResponseSer(errorId=False,
-                               errorCode=None,
-                               errorDescription=None,
-                               taskId='73bdcd28-6c77-4414-8....',
-                               status=<ResponseStatusEnm.Ready: 'ready'>,
-                               solution={'gRecaptchaResponse': '44795sds...'}
-                              )
+            body: Base64 encoded content of the image, decoded into str
 
         Returns:
             CaptchaResponseSer model with full server response
 
         Notes:
             Check class docstring for more info
         """
-        return await self._aio_processing_captcha(
-            serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
-        )
+        self.task_params.update({"body": body})
+        return await self._aio_processing_captcha(create_params=self.task_params)
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/mt_captcha.py` & `python3-capsolver-0.7.1/python3_capsolver/cyber_si_ara.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,111 +1,115 @@
 from typing import Union
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import MtCaptchaTypeEnm
-from python3_capsolver.core.serializer import CaptchaResponseSer, WebsiteDataOptionsSer
+from python3_capsolver.core.enum import AntiCyberSiAraTaskTypeEnm
+from python3_capsolver.core.serializer import CyberSiAraSer, CaptchaResponseSer
 
 
-class MtCaptcha(BaseCaptcha):
+class CyberSiARA(BaseCaptcha):
     """
-    The class is used to work with Capsolver MtCaptcha method.
+    The class is used to work with Capsolver CyberSiARA methods.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``MtCaptchaTask`` and etc.
-        websiteURL: Address of a webpage with Google ReCaptcha
-        websiteKey: Recaptcha website key. <div class="g-recaptcha" data-sitekey="THAT_ONE"></div>
+        captcha_type: Captcha type name, like ``AntiCyberSiAraTask`` and etc.
+        websiteURL: Address of a webpage with CyberSiARA
+        SlideMasterUrlId: You can get MasterUrlId param form `api/CyberSiara/GetCyberSiara` endpoint request
+        UserAgent: Browser userAgent, you need submit your userAgent
 
     Examples:
-        >>> MtCaptcha(api_key="CAI-1324...",
-        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTaskProxyLess,
-        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
-        ...         websiteKey="MTPublic-tqNCRE0GS",
-        ...         proxy="198.22.3.1:10001:user:pwd"
-        ...        ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> CyberSiARA(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
+        ...          captcha_type='AntiCyberSiAraTaskProxyLess',
+        ...          websiteURL="https://www.cybersiara.com/book-a-demo",
+        ...          UserAgent="Mozilla/5.0 ....",
+        ...          SlideMasterUrlId="OXR2LVNvCuXykkZbB8KZIfh162sNT8S2",
+        ...         ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
+                           solution={'token': '44795sds...'}
                           )
 
-        >>> MtCaptcha(api_key="CAI-1324...",
-        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
-        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
-        ...         websiteKey="MTPublic-tqNCRE0GS",
-        ...         proxy="198.22.3.1:10001:user:pwd"
-        ...        ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> CyberSiARA(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
+        ...          captcha_type=AntiCyberSiAraTaskTypeEnm.AntiCyberSiAraTaskProxyLess,
+        ...          websiteURL="https://www.cybersiara.com/book-a-demo",
+        ...          UserAgent="Mozilla/5.0 ....",
+        ...          SlideMasterUrlId="OXR2LVNvCuXykkZbB8KZIfh162sNT8S2",
+        ...         ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
+                           solution={'token': '44795sds...'}
                           )
 
-        >>> await MtCaptcha(api_key="CAI-1324...",
-        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
-        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
-        ...         websiteKey="MTPublic-tqNCRE0GS",
-        ...         proxy="198.22.3.1:10001:user:pwd"
-        ...        ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> CyberSiARA(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
+        ...          captcha_type=AntiCyberSiAraTaskTypeEnm.AntiCyberSiAraTask,
+        ...          websiteURL="https://www.cybersiara.com/book-a-demo",
+        ...          UserAgent="Mozilla/5.0 ....",
+        ...          SlideMasterUrlId="OXR2LVNvCuXykkZbB8KZIfh162sNT8S2",
+        ...          proxy="socks5:192.191.100.10:4780:user:pwd",
+        ...         ).captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
-                           taskId='73bdcd28-6c77-4414-8....',
+                           taskId="87f149f4-1c....",
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
+                           solution={'token': '44795sds...'}
                           )
 
-        >>> await MtCaptcha(api_key="CAI-1324...",
-        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
-        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
-        ...         websiteKey="MTPublic-tqNCRE0GS",
-        ...         proxy="198.22.3.1:10001:user:pwd"
-        ...        ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        >>> await CyberSiARA(api_key="CAI-BA9650D2B9C2786B21120D512702E010",
+        ...          captcha_type=AntiCyberSiAraTaskTypeEnm.AntiCyberSiAraTaskProxyLess,
+        ...          websiteURL="https://www.cybersiara.com/book-a-demo",
+        ...          UserAgent="Mozilla/5.0 ....",
+        ...          SlideMasterUrlId="OXR2LVNvCuXykkZbB8KZIfh162sNT8S2",
+        ...         ).aio_captcha_handler()
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                            solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
+                           solution={'token': '44795sds...'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://docs.capsolver.com/guide/captcha/MtCaptcha.html
+        https://docs.capsolver.com/guide/captcha/CyberSiara.html
     """
 
     def __init__(
         self,
-        captcha_type: Union[MtCaptchaTypeEnm, str],
+        captcha_type: Union[AntiCyberSiAraTaskTypeEnm, str],
         websiteURL: str,
-        websiteKey: str,
+        SlideMasterUrlId: str,
+        UserAgent: str,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        if captcha_type in MtCaptchaTypeEnm.list():
-            self.task_params = WebsiteDataOptionsSer(**locals()).dict()
+        if captcha_type in AntiCyberSiAraTaskTypeEnm.list():
+            self.task_params = CyberSiAraSer(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
-                available - {MtCaptchaTypeEnm}"""
+                available - {AntiCyberSiAraTaskTypeEnm.list_values()}"""
             )
+
         for key in kwargs:
             self.task_params.update({key: kwargs[key]})
 
     def captcha_handler(self) -> CaptchaResponseSer:
         """
-        Sync method for captcha solving
+        Sync solving method
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
             Check class docstring for more info
         """
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver/recaptcha.py` & `python3-capsolver-0.7.1/python3_capsolver/recaptcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,72 +19,72 @@
 
     Examples:
         >>> ReCaptcha(api_key="CAI-1324...",
         ...           captcha_type="ReCaptchaV2TaskProxyLess",
         ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
         ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> ReCaptcha(api_key="CAI-1324...",
         ...           captcha_type=ReCaptchaV2TypeEnm.ReCaptchaV2TaskProxyLess,
         ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
         ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> ReCaptcha(api_key="CAI-1324...",
         ...           captcha_type=ReCaptchaV2TypeEnm.ReCaptchaV2Task,
         ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
         ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-",
         ...           proxy="socks5:192.191.100.10:4780:user:pwd"
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> ReCaptcha(api_key="CAI-1324...",
         ...           captcha_type=ReCaptchaV3TypeEnm.ReCaptchaV3TaskProxyLess,
         ...           websiteURL="https://2captcha.com/demo/recaptcha-v3",
         ...           websiteKey="6LfB5_IbAAAAAMCtsjEHEHKqcB9iQocwwxTiihJu",
         ...           pageAction="demo_action",
         ...           proxy="socks5:192.191.100.10:4780:user:pwd"
         ...          ).captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> await ReCaptcha(api_key="CAI-1324...",
         ...           captcha_type=ReCaptchaV3TypeEnm.ReCaptchaV3TaskProxyLess,
         ...           websiteURL="https://2captcha.com/demo/recaptcha-v3",
         ...           websiteKey="6LfB5_IbAAAAAMCtsjEHEHKqcB9iQocwwxTiihJu",
         ...           pageAction="demo_action",
         ...           proxy="socks5:192.191.100.10:4780:user:pwd"
         ...          ).aio_captcha_handler()
-        CaptchaResponseSer(errorId=False,
+        CaptchaResponseSer(errorId=0,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver.egg-info/PKG-INFO` & `python3-capsolver-0.7.1/python3_capsolver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7468  : 2.1.Name: pyth
 00000020: 6f6e 332d 6361 7073 6f6c 7665 720a 5665  on3-capsolver.Ve
-00000030: 7273 696f 6e3a 2030 2e36 2e31 0a53 756d  rsion: 0.6.1.Sum
-00000040: 6d61 7279 3a20 5079 7468 6f6e 2033 2e37  mary: Python 3.7
+00000030: 7273 696f 6e3a 2030 2e37 2e31 0a53 756d  rsion: 0.7.1.Sum
+00000040: 6d61 7279 3a20 5079 7468 6f6e 2033 2e38  mary: Python 3.8
 00000050: 2b20 4361 7073 6f6c 7665 7220 6c69 6272  + Capsolver libr
 00000060: 6172 7920 7769 7468 2041 494f 206d 6f64  ary with AIO mod
 00000070: 756c 652e 0a48 6f6d 652d 7061 6765 3a20  ule..Home-page: 
 00000080: 6874 7470 733a 2f2f 616e 6472 6569 6472  https://andreidr
 00000090: 616e 672e 6769 7468 7562 2e69 6f2f 7079  ang.github.io/py
 000000a0: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
 000000b0: 0a41 7574 686f 723a 2041 6e64 7265 6944  .Author: AndreiD
@@ -18,15 +18,15 @@
 00000110: 2068 7474 7073 3a2f 2f61 6e64 7265 6964   https://andreid
 00000120: 7261 6e67 2e67 6974 6875 622e 696f 2f70  rang.github.io/p
 00000130: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
 00000140: 2f0a 5072 6f6a 6563 742d 5552 4c3a 2053  /.Project-URL: S
 00000150: 6f75 7263 652c 2068 7474 7073 3a2f 2f67  ource, https://g
 00000160: 6974 6875 622e 636f 6d2f 416e 6472 6569  ithub.com/Andrei
 00000170: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
-00000180: 7074 6368 6161 690a 4b65 7977 6f72 6473  ptchaai.Keywords
+00000180: 7073 6f6c 7665 720a 4b65 7977 6f72 6473  psolver.Keywords
 00000190: 3a20 6361 7074 6368 6120 0a20 2020 2020  : captcha .     
 000001a0: 2020 2020 2020 2020 2020 2072 6563 6170             recap
 000001b0: 7463 6861 0a20 2020 2020 2020 2020 2020  tcha.           
 000001c0: 2020 2020 2067 6565 7465 7374 0a20 2020       geetest.   
 000001d0: 2020 2020 2020 2020 2020 2020 2068 6361               hca
 000001e0: 7074 6368 610a 2020 2020 2020 2020 2020  ptcha.          
 000001f0: 2020 2020 2020 6361 7079 7075 7a7a 6c65        capypuzzle
@@ -68,250 +68,265 @@
 00000430: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000440: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 00000450: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000460: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000470: 203a 3a20 4f6e 6c79 0a43 6c61 7373 6966   :: Only.Classif
 00000480: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 00000490: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000004a0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
+000004a0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
 000004b0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000004c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000004d0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+000004d0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
 000004e0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 000004f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000500: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00000510: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000520: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000530: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000540: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000550: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000560: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000570: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000580: 2046 7261 6d65 776f 726b 203a 3a20 4173   Framework :: As
-00000590: 796e 6349 4f0a 436c 6173 7369 6669 6572  yncIO.Classifier
-000005a0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000005b0: 656d 203a 3a20 556e 6978 0a43 6c61 7373  em :: Unix.Class
-000005c0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-000005d0: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-000005e0: 736f 6674 203a 3a20 5769 6e64 6f77 730a  soft :: Windows.
-000005f0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000600: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000610: 4d61 634f 530a 5265 7175 6972 6573 2d50  MacOS.Requires-P
-00000620: 7974 686f 6e3a 203e 3d33 2e37 2e30 0a44  ython: >=3.7.0.D
-00000630: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-00000640: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000650: 726b 646f 776e 0a0a 0a23 2070 7974 686f  rkdown...# pytho
-00000660: 6e33 2d63 6170 736f 6c76 6572 0a21 5b50  n3-capsolver.![P
-00000670: 7974 686f 6e33 2d43 6170 736f 6c76 6572  ython3-Capsolver
-00000680: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000690: 2e63 6f6d 2f41 6e64 7265 6944 7261 6e67  .com/AndreiDrang
-000006a0: 2f70 7974 686f 6e33 2d63 6170 736f 6c76  /python3-capsolv
-000006b0: 6572 2f62 6c6f 622f 6d61 696e 2f66 696c  er/blob/main/fil
-000006c0: 6573 2f43 6170 736f 6c76 6572 536d 2e70  es/CapsolverSm.p
-000006d0: 6e67 290a 0a5b 215b 4361 7073 6f6c 7665  ng)..[![Capsolve
-000006e0: 725d 2868 7474 7073 3a2f 2f75 7365 722d  r](https://user-
-000006f0: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
-00000700: 7263 6f6e 7465 6e74 2e63 6f6d 2f31 3639  rcontent.com/169
-00000710: 3931 3336 352f 3233 3438 3532 3232 392d  91365/234852229-
-00000720: 3665 3462 3366 3363 2d66 3439 382d 3466  6e4b3f3c-f498-4f
-00000730: 6435 2d39 6136 622d 6637 6632 3639 6464  d5-9a6b-f7f269dd
-00000740: 3462 6663 2e67 6966 295d 2868 7474 7073  4bfc.gif)](https
-00000750: 3a2f 2f64 6173 6862 6f61 7264 2e63 6170  ://dashboard.cap
-00000760: 736f 6c76 6572 2e63 6f6d 2f70 6173 7370  solver.com/passp
-00000770: 6f72 742f 7265 6769 7374 6572 3f69 6e76  ort/register?inv
-00000780: 6974 6543 6f64 653d 6b51 546e 2d74 4730  iteCode=kQTn-tG0
-00000790: 374a 6231 290a 0a5b 215b 5079 5049 2076  7Jb1)..[![PyPI v
-000007a0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000007b0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-000007c0: 2f70 7974 686f 6e33 2d63 6170 736f 6c76  /python3-capsolv
-000007d0: 6572 2e73 7667 295d 2868 7474 7073 3a2f  er.svg)](https:/
-000007e0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-000007f0: 792f 7079 7468 6f6e 332d 6361 7073 6f6c  y/python3-capsol
-00000800: 7665 7229 0a5b 215b 5079 7468 6f6e 2076  ver).[![Python v
-00000810: 6572 7369 6f6e 735d 2868 7474 7073 3a2f  ersions](https:/
-00000820: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000830: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000840: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
-00000850: 722e 7376 673f 6c6f 676f 3d70 7974 686f  r.svg?logo=pytho
-00000860: 6e26 6c6f 676f 436f 6c6f 723d 4642 4530  n&logoColor=FBE0
-00000870: 3732 295d 2868 7474 7073 3a2f 2f62 6164  72)](https://bad
-00000880: 6765 2e66 7572 792e 696f 2f70 792f 7079  ge.fury.io/py/py
-00000890: 7468 6f6e 332d 6361 7073 6f6c 7665 7229  thon3-capsolver)
-000008a0: 0a5b 215b 446f 776e 6c6f 6164 735d 2868  .[![Downloads](h
-000008b0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000008c0: 2f62 6164 6765 2f70 7974 686f 6e33 2d63  /badge/python3-c
-000008d0: 6170 736f 6c76 6572 2f6d 6f6e 7468 295d  apsolver/month)]
-000008e0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-000008f0: 6368 2f70 726f 6a65 6374 2f70 7974 686f  ch/project/pytho
-00000900: 6e33 2d63 6170 736f 6c76 6572 290a 0a5b  n3-capsolver)..[
-00000910: 215b 4d61 696e 7461 696e 6162 696c 6974  ![Maintainabilit
-00000920: 795d 2868 7474 7073 3a2f 2f61 7069 2e63  y](https://api.c
-00000930: 6f64 6563 6c69 6d61 7465 2e63 6f6d 2f76  odeclimate.com/v
-00000940: 312f 6261 6467 6573 2f33 6333 3031 3637  1/badges/3c30167
-00000950: 6235 6662 3337 6130 3737 3565 612f 6d61  b5fb37a0775ea/ma
-00000960: 696e 7461 696e 6162 696c 6974 7929 5d28  intainability)](
-00000970: 6874 7470 733a 2f2f 636f 6465 636c 696d  https://codeclim
-00000980: 6174 652e 636f 6d2f 6769 7468 7562 2f41  ate.com/github/A
-00000990: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
-000009a0: 6e33 2d63 6170 736f 6c76 6572 2f6d 6169  n3-capsolver/mai
-000009b0: 6e74 6169 6e61 6269 6c69 7479 290a 5b21  ntainability).[!
-000009c0: 5b43 6f64 6163 7920 4261 6467 655d 2868  [Codacy Badge](h
-000009d0: 7474 7073 3a2f 2f61 7070 2e63 6f64 6163  ttps://app.codac
-000009e0: 792e 636f 6d2f 7072 6f6a 6563 742f 6261  y.com/project/ba
-000009f0: 6467 652f 4772 6164 652f 3332 3364 3465  dge/Grade/323d4e
-00000a00: 6461 3066 6531 3437 3762 6265 6138 6665  da0fe1477bbea8fe
-00000a10: 3839 3032 6239 6539 3765 295d 2868 7474  8902b9e97e)](htt
-00000a20: 7073 3a2f 2f77 7777 2e63 6f64 6163 792e  ps://www.codacy.
-00000a30: 636f 6d2f 6768 2f41 6e64 7265 6944 7261  com/gh/AndreiDra
-00000a40: 6e67 2f70 7974 686f 6e33 2d63 6170 736f  ng/python3-capso
-00000a50: 6c76 6572 2f64 6173 6862 6f61 7264 3f75  lver/dashboard?u
-00000a60: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
-00000a70: 2e63 6f6d 2661 6d70 3b75 746d 5f6d 6564  .com&amp;utm_med
-00000a80: 6975 6d3d 7265 6665 7272 616c 2661 6d70  ium=referral&amp
-00000a90: 3b75 746d 5f63 6f6e 7465 6e74 3d41 6e64  ;utm_content=And
-00000aa0: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
-00000ab0: 2d63 6170 736f 6c76 6572 2661 6d70 3b75  -capsolver&amp;u
-00000ac0: 746d 5f63 616d 7061 6967 6e3d 4261 6467  tm_campaign=Badg
-00000ad0: 655f 4772 6164 6529 0a5b 215b 636f 6465  e_Grade).[![code
-00000ae0: 636f 765d 2868 7474 7073 3a2f 2f63 6f64  cov](https://cod
-00000af0: 6563 6f76 2e69 6f2f 6768 2f41 6e64 7265  ecov.io/gh/Andre
-00000b00: 6944 7261 6e67 2f70 7974 686f 6e33 2d63  iDrang/python3-c
-00000b10: 6170 736f 6c76 6572 2f62 7261 6e63 682f  apsolver/branch/
-00000b20: 6d61 696e 2f67 7261 7068 2f62 6164 6765  main/graph/badge
-00000b30: 2e73 7667 3f74 6f6b 656e 3d32 4c34 5656  .svg?token=2L4VV
-00000b40: 4946 3447 3829 5d28 6874 7470 733a 2f2f  IF4G8)](https://
-00000b50: 636f 6465 636f 762e 696f 2f67 682f 416e  codecov.io/gh/An
-00000b60: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
-00000b70: 332d 6361 7073 6f6c 7665 7229 0a0a 5b21  3-capsolver)..[!
-00000b80: 5b53 7068 696e 7820 6275 696c 645d 2868  [Sphinx build](h
-00000b90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ba0: 6d2f 416e 6472 6569 4472 616e 672f 7079  m/AndreiDrang/py
-00000bb0: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
-00000bc0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000bd0: 732f 7370 6869 6e78 2e79 6d6c 2f62 6164  s/sphinx.yml/bad
-00000be0: 6765 2e73 7667 3f62 7261 6e63 683d 7265  ge.svg?branch=re
-00000bf0: 6c65 6173 6529 5d28 6874 7470 733a 2f2f  lease)](https://
-00000c00: 6769 7468 7562 2e63 6f6d 2f41 6e64 7265  github.com/Andre
-00000c10: 6944 7261 6e67 2f70 7974 686f 6e33 2d63  iDrang/python3-c
-00000c20: 6170 736f 6c76 6572 2f61 6374 696f 6e73  apsolver/actions
-00000c30: 2f77 6f72 6b66 6c6f 7773 2f73 7068 696e  /workflows/sphin
-00000c40: 782e 796d 6c29 0a5b 215b 4275 696c 645d  x.yml).[![Build]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
-00000c70: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
-00000c80: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
-00000c90: 6f77 732f 6275 696c 642e 796d 6c2f 6261  ows/build.yml/ba
-00000ca0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000cb0: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-00000cc0: 7468 7562 2e63 6f6d 2f41 6e64 7265 6944  thub.com/AndreiD
-00000cd0: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
-00000ce0: 736f 6c76 6572 2f61 6374 696f 6e73 2f77  solver/actions/w
-00000cf0: 6f72 6b66 6c6f 7773 2f62 7569 6c64 2e79  orkflows/build.y
-00000d00: 6d6c 290a 5b21 5b49 6e73 7461 6c6c 6174  ml).[![Installat
-00000d10: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-00000d20: 6875 622e 636f 6d2f 416e 6472 6569 4472  hub.com/AndreiDr
-00000d30: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
-00000d40: 6f6c 7665 722f 6163 7469 6f6e 732f 776f  olver/actions/wo
-00000d50: 726b 666c 6f77 732f 696e 7374 616c 6c2e  rkflows/install.
-00000d60: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
-00000d70: 616e 6368 3d6d 6169 6e29 5d28 6874 7470  anch=main)](http
-00000d80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000d90: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
-00000da0: 6e33 2d63 6170 736f 6c76 6572 2f61 6374  n3-capsolver/act
-00000db0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f69  ions/workflows/i
-00000dc0: 6e73 7461 6c6c 2e79 6d6c 290a 5b21 5b54  nstall.yml).[![T
-00000dd0: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
-00000de0: 7468 7562 2e63 6f6d 2f41 6e64 7265 6944  thub.com/AndreiD
-00000df0: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
-00000e00: 736f 6c76 6572 2f61 6374 696f 6e73 2f77  solver/actions/w
-00000e10: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
-00000e20: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-00000e30: 6368 3d6d 6169 6e29 5d28 6874 7470 733a  ch=main)](https:
-00000e40: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6e64  //github.com/And
-00000e50: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
-00000e60: 2d63 6170 736f 6c76 6572 2f61 6374 696f  -capsolver/actio
-00000e70: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-00000e80: 742e 796d 6c29 0a5b 215b 4c69 6e74 5d28  t.yml).[![Lint](
-00000e90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ea0: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
-00000eb0: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
-00000ec0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000ed0: 7773 2f6c 696e 742e 796d 6c2f 6261 6467  ws/lint.yml/badg
-00000ee0: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-00000ef0: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
-00000f00: 7562 2e63 6f6d 2f41 6e64 7265 6944 7261  ub.com/AndreiDra
-00000f10: 6e67 2f70 7974 686f 6e33 2d63 6170 736f  ng/python3-capso
-00000f20: 6c76 6572 2f61 6374 696f 6e73 2f77 6f72  lver/actions/wor
-00000f30: 6b66 6c6f 7773 2f6c 696e 742e 796d 6c29  kflows/lint.yml)
-00000f40: 0a0a 0a50 7974 686f 6e20 3320 6c69 6272  ...Python 3 libr
-00000f50: 6172 7920 666f 7220 5b43 6170 736f 6c76  ary for [Capsolv
-00000f60: 6572 5d28 6874 7470 733a 2f2f 6461 7368  er](https://dash
-00000f70: 626f 6172 642e 6361 7073 6f6c 7665 722e  board.capsolver.
-00000f80: 636f 6d2f 7061 7373 706f 7274 2f72 6567  com/passport/reg
-00000f90: 6973 7465 723f 696e 7669 7465 436f 6465  ister?inviteCode
-00000fa0: 3d6b 5154 6e2d 7447 3037 4a62 3129 2073  =kQTn-tG07Jb1) s
-00000fb0: 6572 7669 6365 2041 5049 2e0a 0a54 6573  ervice API...Tes
-00000fc0: 7465 6420 6f6e 2055 4e49 5820 6261 7365  ted on UNIX base
-00000fd0: 6420 4f53 2e0a 0a54 6865 206c 6962 7261  d OS...The libra
-00000fe0: 7279 2069 7320 696e 7465 6e64 6564 2066  ry is intended f
-00000ff0: 6f72 2073 6f66 7477 6172 6520 6465 7665  or software deve
-00001000: 6c6f 7065 7273 2061 6e64 2069 7320 7573  lopers and is us
-00001010: 6564 2074 6f20 776f 726b 2077 6974 6820  ed to work with 
-00001020: 7468 6520 5b43 6170 736f 6c76 6572 5d28  the [Capsolver](
-00001030: 6874 7470 733a 2f2f 6461 7368 626f 6172  https://dashboar
-00001040: 642e 6361 7073 6f6c 7665 722e 636f 6d2f  d.capsolver.com/
-00001050: 7061 7373 706f 7274 2f72 6567 6973 7465  passport/registe
-00001060: 723f 696e 7669 7465 436f 6465 3d6b 5154  r?inviteCode=kQT
-00001070: 6e2d 7447 3037 4a62 3129 2073 6572 7669  n-tG07Jb1) servi
-00001080: 6365 2041 5049 2e0a 0a2a 2a2a 0a0a 4966  ce API...***..If
-00001090: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-000010a0: 6573 7469 6f6e 732c 2070 6c65 6173 6520  estions, please 
-000010b0: 7365 6e64 2061 206d 6573 7361 6765 2074  send a message t
-000010c0: 6f20 7468 6520 5b54 656c 6567 7261 6d5d  o the [Telegram]
-000010d0: 2868 7474 7073 3a2f 2f74 2e6d 652f 7079  (https://t.me/py
-000010e0: 7468 6f6e 6361 7074 6368 6129 2063 6861  thoncaptcha) cha
-000010f0: 7420 726f 6f6d 2e0a 0a4f 7220 656d 6169  t room...Or emai
-00001100: 6c20 7079 7468 6f6e 2d63 6170 7463 6861  l python-captcha
-00001110: 4070 6d2e 6d65 0a0a 2a2a 2a0a 0a23 2320  @pm.me..***..## 
-00001120: 486f 7720 746f 2069 6e73 7461 6c6c 3f0a  How to install?.
-00001130: 0a57 6520 7265 636f 6d6d 656e 6420 7573  .We recommend us
-00001140: 696e 6720 7468 6520 6c61 7465 7374 2076  ing the latest v
-00001150: 6572 7369 6f6e 206f 6620 5079 7468 6f6e  ersion of Python
-00001160: 2e20 6070 7974 686f 6e33 2d63 6170 736f  . `python3-capso
-00001170: 6c76 6572 6020 7375 7070 6f72 7473 2050  lver` supports P
-00001180: 7974 686f 6e20 332e 372b 2e0a 0a23 2323  ython 3.7+...###
-00001190: 2070 6970 0a0a 6060 6062 6173 680a 7069   pip..```bash.pi
-000011a0: 7020 696e 7374 616c 6c20 7079 7468 6f6e  p install python
-000011b0: 332d 6361 7073 6f6c 7665 720a 6060 600a  3-capsolver.```.
-000011c0: 0a23 2320 486f 7720 746f 2075 7365 3f0a  .## How to use?.
-000011d0: 0a49 7320 6465 7363 7269 6265 6420 696e  .Is described in
-000011e0: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
-000011f0: 696f 6e2d 7765 6273 6974 655d 2868 7474  ion-website](htt
-00001200: 7073 3a2f 2f61 6e64 7265 6964 7261 6e67  ps://andreidrang
-00001210: 2e67 6974 6875 622e 696f 2f70 7974 686f  .github.io/pytho
-00001220: 6e33 2d63 6170 736f 6c76 6572 2f29 2e0a  n3-capsolver/)..
-00001230: 0a0a 2323 2048 6f77 2074 6f20 7465 7374  ..## How to test
-00001240: 3f0a 0a31 2e20 596f 7520 6e65 6564 2073  ?..1. You need s
-00001250: 6574 2060 6041 5049 5f4b 4559 6060 2069  et ``API_KEY`` i
-00001260: 6e20 796f 7572 2065 6e76 6972 6f6e 6d65  n your environme
-00001270: 6e74 2867 6574 2074 6869 7320 7661 6c75  nt(get this valu
-00001280: 6520 6672 6f6d 2079 6f75 2061 6363 6f75  e from you accou
-00001290: 6e74 292e 0a32 2e20 5275 6e20 636f 6d6d  nt)..2. Run comm
-000012a0: 616e 6420 6060 6d61 6b65 2074 6573 7473  and ``make tests
-000012b0: 6060 2c20 6672 6f6d 2072 6f6f 7420 6469  ``, from root di
-000012c0: 7265 6374 6f72 792e 0a0a 0a23 2323 2043  rectory....### C
-000012d0: 6861 6e67 656c 6f67 0a0a 4368 6563 6b20  hangelog..Check 
-000012e0: 5b72 656c 6561 7365 7320 7061 6765 5d28  [releases page](
-000012f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001300: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
-00001310: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
-00001320: 2f72 656c 6561 7365 7329 2e0a 0a23 2323  /releases)...###
-00001330: 2048 6f77 2074 6f20 6765 7420 4150 4920   How to get API 
-00001340: 4b65 7920 746f 2077 6f72 6b20 7769 7468  Key to work with
-00001350: 2074 6865 206c 6962 7261 7279 0a31 2e20   the library.1. 
-00001360: 4f6e 2074 6865 2070 6167 6520 2d20 6874  On the page - ht
-00001370: 7470 733a 2f2f 6461 7368 626f 6172 642e  tps://dashboard.
-00001380: 6361 7073 6f6c 7665 722e 636f 6d2f 6f76  capsolver.com/ov
-00001390: 6572 7669 6577 2f75 7365 722d 6365 6e74  erview/user-cent
-000013a0: 6572 0a32 2e20 4669 6e64 2069 743a 2021  er.2. Find it: !
-000013b0: 5b69 6d67 2e70 6e67 5d28 6669 6c65 732f  [img.png](files/
-000013c0: 696d 672e 706e 6729 0a                   img.png).
+00000500: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000510: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000520: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000530: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000540: 3131 0a43 6c61 7373 6966 6965 723a 2046  11.Classifier: F
+00000550: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
+00000560: 6349 4f0a 436c 6173 7369 6669 6572 3a20  cIO.Classifier: 
+00000570: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000580: 203a 3a20 556e 6978 0a43 6c61 7373 6966   :: Unix.Classif
+00000590: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
+000005a0: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
+000005b0: 6674 203a 3a20 5769 6e64 6f77 730a 436c  ft :: Windows.Cl
+000005c0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000005d0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+000005e0: 634f 530a 5265 7175 6972 6573 2d50 7974  cOS.Requires-Pyt
+000005f0: 686f 6e3a 203e 3d33 2e38 2e30 0a44 6573  hon: >=3.8.0.Des
+00000600: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000610: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000620: 646f 776e 0a0a 0a23 2070 7974 686f 6e33  down...# python3
+00000630: 2d63 6170 736f 6c76 6572 0a21 5b50 7974  -capsolver.![Pyt
+00000640: 686f 6e33 2d43 6170 736f 6c76 6572 5d28  hon3-Capsolver](
+00000650: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000660: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
+00000670: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
+00000680: 2f62 6c6f 622f 6d61 696e 2f66 696c 6573  /blob/main/files
+00000690: 2f43 6170 736f 6c76 6572 536d 2e70 6e67  /CapsolverSm.png
+000006a0: 290a 0a3c 6120 6872 6566 3d22 6874 7470  )..<a href="http
+000006b0: 733a 2f2f 6461 7368 626f 6172 642e 6361  s://dashboard.ca
+000006c0: 7073 6f6c 7665 722e 636f 6d2f 7061 7373  psolver.com/pass
+000006d0: 706f 7274 2f72 6567 6973 7465 723f 696e  port/register?in
+000006e0: 7669 7465 436f 6465 3d6b 5154 6e2d 7447  viteCode=kQTn-tG
+000006f0: 3037 4a62 3122 3e0a 2020 2020 3c69 6d67  07Jb1">.    <img
+00000700: 2073 7263 3d22 6874 7470 733a 2f2f 6364   src="https://cd
+00000710: 6e2e 6469 7363 6f72 6461 7070 2e63 6f6d  n.discordapp.com
+00000720: 2f61 7474 6163 686d 656e 7473 2f31 3130  /attachments/110
+00000730: 3531 3732 3339 3436 3535 3632 3533 3036  5172394655625306
+00000740: 2f31 3130 3531 3830 3130 3138 3032 3437  /110518010180247
+00000750: 3135 3735 2f32 3032 3231 3230 372d 3136  1575/20221207-16
+00000760: 3037 3439 2e67 6966 2220 616c 743d 2243  0749.gif" alt="C
+00000770: 6170 736f 6c76 6572 2773 2042 616e 6e65  apsolver's Banne
+00000780: 7222 3e0a 3c2f 613e 0a3c 6272 3e0a 4174  r">.</a>.<br>.At
+00000790: 2074 6865 206c 6f77 6573 7420 7072 6963   the lowest pric
+000007a0: 6520 6f6e 2074 6865 206d 6172 6b65 742c  e on the market,
+000007b0: 2079 6f75 206d 6179 2072 6563 6569 7665   you may receive
+000007c0: 2061 2076 6172 6965 7479 206f 6620 736f   a variety of so
+000007d0: 6c75 7469 6f6e 732c 2069 6e63 6c75 6469  lutions, includi
+000007e0: 6e67 2072 6543 4150 5443 4841 2056 322c  ng reCAPTCHA V2,
+000007f0: 2072 6543 4150 5443 4841 2056 332c 2068   reCAPTCHA V3, h
+00000800: 4361 7074 6368 612c 2068 4361 7074 6368  Captcha, hCaptch
+00000810: 6120 436c 6963 6b2c 2046 756e 4361 7074  a Click, FunCapt
+00000820: 6368 612c 2070 6963 7475 7265 2d74 6f2d  cha, picture-to-
+00000830: 7465 7874 2c20 616e 6420 6d6f 7265 2e20  text, and more. 
+00000840: 5769 7468 2074 6869 7320 7365 7276 6963  With this servic
+00000850: 652c 2030 2e31 7320 6973 2074 6865 2073  e, 0.1s is the s
+00000860: 6c6f 7765 7374 2073 7065 6564 2065 7665  lowest speed eve
+00000870: 7220 6d65 6173 7572 6564 2e0a 3c68 723e  r measured..<hr>
+00000880: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
+00000890: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+000008a0: 2e66 7572 792e 696f 2f70 792f 7079 7468  .fury.io/py/pyth
+000008b0: 6f6e 332d 6361 7073 6f6c 7665 722e 7376  on3-capsolver.sv
+000008c0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+000008d0: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+000008e0: 686f 6e33 2d63 6170 736f 6c76 6572 290a  hon3-capsolver).
+000008f0: 5b21 5b50 7974 686f 6e20 7665 7273 696f  [![Python versio
+00000900: 6e73 5d28 6874 7470 733a 2f2f 696d 672e  ns](https://img.
+00000910: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000920: 7079 7665 7273 696f 6e73 2f70 7974 686f  pyversions/pytho
+00000930: 6e33 2d63 6170 736f 6c76 6572 2e73 7667  n3-capsolver.svg
+00000940: 3f6c 6f67 6f3d 7079 7468 6f6e 266c 6f67  ?logo=python&log
+00000950: 6f43 6f6c 6f72 3d46 4245 3037 3229 5d28  oColor=FBE072)](
+00000960: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000970: 7279 2e69 6f2f 7079 2f70 7974 686f 6e33  ry.io/py/python3
+00000980: 2d63 6170 736f 6c76 6572 290a 5b21 5b44  -capsolver).[![D
+00000990: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+000009a0: 2f2f 7065 7079 2e74 6563 682f 6261 6467  //pepy.tech/badg
+000009b0: 652f 7079 7468 6f6e 332d 6361 7073 6f6c  e/python3-capsol
+000009c0: 7665 722f 6d6f 6e74 6829 5d28 6874 7470  ver/month)](http
+000009d0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000009e0: 6f6a 6563 742f 7079 7468 6f6e 332d 6361  oject/python3-ca
+000009f0: 7073 6f6c 7665 7229 0a0a 5b21 5b4d 6169  psolver)..[![Mai
+00000a00: 6e74 6169 6e61 6269 6c69 7479 5d28 6874  ntainability](ht
+00000a10: 7470 733a 2f2f 6170 692e 636f 6465 636c  tps://api.codecl
+00000a20: 696d 6174 652e 636f 6d2f 7631 2f62 6164  imate.com/v1/bad
+00000a30: 6765 732f 3363 3330 3136 3762 3566 6233  ges/3c30167b5fb3
+00000a40: 3761 3037 3735 6561 2f6d 6169 6e74 6169  7a0775ea/maintai
+00000a50: 6e61 6269 6c69 7479 295d 2868 7474 7073  nability)](https
+00000a60: 3a2f 2f63 6f64 6563 6c69 6d61 7465 2e63  ://codeclimate.c
+00000a70: 6f6d 2f67 6974 6875 622f 416e 6472 6569  om/github/Andrei
+00000a80: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
+00000a90: 7073 6f6c 7665 722f 6d61 696e 7461 696e  psolver/maintain
+00000aa0: 6162 696c 6974 7929 0a5b 215b 436f 6461  ability).[![Coda
+00000ab0: 6379 2042 6164 6765 5d28 6874 7470 733a  cy Badge](https:
+00000ac0: 2f2f 6170 702e 636f 6461 6379 2e63 6f6d  //app.codacy.com
+00000ad0: 2f70 726f 6a65 6374 2f62 6164 6765 2f47  /project/badge/G
+00000ae0: 7261 6465 2f33 3233 6434 6564 6130 6665  rade/323d4eda0fe
+00000af0: 3134 3737 6262 6561 3866 6538 3930 3262  1477bbea8fe8902b
+00000b00: 3965 3937 6529 5d28 6874 7470 733a 2f2f  9e97e)](https://
+00000b10: 7777 772e 636f 6461 6379 2e63 6f6d 2f67  www.codacy.com/g
+00000b20: 682f 416e 6472 6569 4472 616e 672f 7079  h/AndreiDrang/py
+00000b30: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
+00000b40: 6461 7368 626f 6172 643f 7574 6d5f 736f  dashboard?utm_so
+00000b50: 7572 6365 3d67 6974 6875 622e 636f 6d26  urce=github.com&
+00000b60: 616d 703b 7574 6d5f 6d65 6469 756d 3d72  amp;utm_medium=r
+00000b70: 6566 6572 7261 6c26 616d 703b 7574 6d5f  eferral&amp;utm_
+00000b80: 636f 6e74 656e 743d 416e 6472 6569 4472  content=AndreiDr
+00000b90: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
+00000ba0: 6f6c 7665 7226 616d 703b 7574 6d5f 6361  olver&amp;utm_ca
+00000bb0: 6d70 6169 676e 3d42 6164 6765 5f47 7261  mpaign=Badge_Gra
+00000bc0: 6465 290a 5b21 5b63 6f64 6563 6f76 5d28  de).[![codecov](
+00000bd0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000be0: 696f 2f67 682f 416e 6472 6569 4472 616e  io/gh/AndreiDran
+00000bf0: 672f 7079 7468 6f6e 332d 6361 7073 6f6c  g/python3-capsol
+00000c00: 7665 722f 6272 616e 6368 2f6d 6169 6e2f  ver/branch/main/
+00000c10: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000c20: 746f 6b65 6e3d 324c 3456 5649 4634 4738  token=2L4VVIF4G8
+00000c30: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000c40: 6f76 2e69 6f2f 6768 2f41 6e64 7265 6944  ov.io/gh/AndreiD
+00000c50: 7261 6e67 2f70 7974 686f 6e33 2d63 6170  rang/python3-cap
+00000c60: 736f 6c76 6572 290a 0a5b 215b 5370 6869  solver)..[![Sphi
+00000c70: 6e78 2062 7569 6c64 5d28 6874 7470 733a  nx build](https:
+00000c80: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6e64  //github.com/And
+00000c90: 7265 6944 7261 6e67 2f70 7974 686f 6e33  reiDrang/python3
+00000ca0: 2d63 6170 736f 6c76 6572 2f61 6374 696f  -capsolver/actio
+00000cb0: 6e73 2f77 6f72 6b66 6c6f 7773 2f73 7068  ns/workflows/sph
+00000cc0: 696e 782e 796d 6c2f 6261 6467 652e 7376  inx.yml/badge.sv
+00000cd0: 673f 6272 616e 6368 3d72 656c 6561 7365  g?branch=release
+00000ce0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000cf0: 622e 636f 6d2f 416e 6472 6569 4472 616e  b.com/AndreiDran
+00000d00: 672f 7079 7468 6f6e 332d 6361 7073 6f6c  g/python3-capsol
+00000d10: 7665 722f 6163 7469 6f6e 732f 776f 726b  ver/actions/work
+00000d20: 666c 6f77 732f 7370 6869 6e78 2e79 6d6c  flows/sphinx.yml
+00000d30: 290a 5b21 5b42 7569 6c64 5d28 6874 7470  ).[![Build](http
+00000d40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000d50: 6e64 7265 6944 7261 6e67 2f70 7974 686f  ndreiDrang/pytho
+00000d60: 6e33 2d63 6170 736f 6c76 6572 2f61 6374  n3-capsolver/act
+00000d70: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+00000d80: 7569 6c64 2e79 6d6c 2f62 6164 6765 2e73  uild.yml/badge.s
+00000d90: 7667 3f62 7261 6e63 683d 6d61 696e 295d  vg?branch=main)]
+00000da0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000db0: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
+00000dc0: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
+00000dd0: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000de0: 6f77 732f 6275 696c 642e 796d 6c29 0a5b  ows/build.yml).[
+00000df0: 215b 496e 7374 616c 6c61 7469 6f6e 5d28  ![Installation](
+00000e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000e10: 6f6d 2f41 6e64 7265 6944 7261 6e67 2f70  om/AndreiDrang/p
+00000e20: 7974 686f 6e33 2d63 6170 736f 6c76 6572  ython3-capsolver
+00000e30: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000e40: 7773 2f69 6e73 7461 6c6c 2e79 6d6c 2f62  ws/install.yml/b
+00000e50: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
+00000e60: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
+00000e70: 6974 6875 622e 636f 6d2f 416e 6472 6569  ithub.com/Andrei
+00000e80: 4472 616e 672f 7079 7468 6f6e 332d 6361  Drang/python3-ca
+00000e90: 7073 6f6c 7665 722f 6163 7469 6f6e 732f  psolver/actions/
+00000ea0: 776f 726b 666c 6f77 732f 696e 7374 616c  workflows/instal
+00000eb0: 6c2e 796d 6c29 0a5b 215b 5465 7374 735d  l.yml).[![Tests]
+00000ec0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000ed0: 636f 6d2f 416e 6472 6569 4472 616e 672f  com/AndreiDrang/
+00000ee0: 7079 7468 6f6e 332d 6361 7073 6f6c 7665  python3-capsolve
+00000ef0: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000f00: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+00000f10: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000f20: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000f30: 6875 622e 636f 6d2f 416e 6472 6569 4472  hub.com/AndreiDr
+00000f40: 616e 672f 7079 7468 6f6e 332d 6361 7073  ang/python3-caps
+00000f50: 6f6c 7665 722f 6163 7469 6f6e 732f 776f  olver/actions/wo
+00000f60: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
+00000f70: 290a 5b21 5b4c 696e 745d 2868 7474 7073  ).[![Lint](https
+00000f80: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+00000f90: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
+00000fa0: 332d 6361 7073 6f6c 7665 722f 6163 7469  3-capsolver/acti
+00000fb0: 6f6e 732f 776f 726b 666c 6f77 732f 6c69  ons/workflows/li
+00000fc0: 6e74 2e79 6d6c 2f62 6164 6765 2e73 7667  nt.yml/badge.svg
+00000fd0: 3f62 7261 6e63 683d 6d61 696e 295d 2868  ?branch=main)](h
+00000fe0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ff0: 6d2f 416e 6472 6569 4472 616e 672f 7079  m/AndreiDrang/py
+00001000: 7468 6f6e 332d 6361 7073 6f6c 7665 722f  thon3-capsolver/
+00001010: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00001020: 732f 6c69 6e74 2e79 6d6c 290a 0a0a 5079  s/lint.yml)...Py
+00001030: 7468 6f6e 2033 206c 6962 7261 7279 2066  thon 3 library f
+00001040: 6f72 205b 4361 7073 6f6c 7665 725d 2868  or [Capsolver](h
+00001050: 7474 7073 3a2f 2f64 6173 6862 6f61 7264  ttps://dashboard
+00001060: 2e63 6170 736f 6c76 6572 2e63 6f6d 2f70  .capsolver.com/p
+00001070: 6173 7370 6f72 742f 7265 6769 7374 6572  assport/register
+00001080: 3f69 6e76 6974 6543 6f64 653d 6b51 546e  ?inviteCode=kQTn
+00001090: 2d74 4730 374a 6231 2920 7365 7276 6963  -tG07Jb1) servic
+000010a0: 6520 4150 492e 0a0a 5465 7374 6564 206f  e API...Tested o
+000010b0: 6e20 554e 4958 2062 6173 6564 204f 532e  n UNIX based OS.
+000010c0: 0a0a 5468 6520 6c69 6272 6172 7920 6973  ..The library is
+000010d0: 2069 6e74 656e 6465 6420 666f 7220 736f   intended for so
+000010e0: 6674 7761 7265 2064 6576 656c 6f70 6572  ftware developer
+000010f0: 7320 616e 6420 6973 2075 7365 6420 746f  s and is used to
+00001100: 2077 6f72 6b20 7769 7468 2074 6865 205b   work with the [
+00001110: 4361 7073 6f6c 7665 725d 2868 7474 7073  Capsolver](https
+00001120: 3a2f 2f64 6173 6862 6f61 7264 2e63 6170  ://dashboard.cap
+00001130: 736f 6c76 6572 2e63 6f6d 2f70 6173 7370  solver.com/passp
+00001140: 6f72 742f 7265 6769 7374 6572 3f69 6e76  ort/register?inv
+00001150: 6974 6543 6f64 653d 6b51 546e 2d74 4730  iteCode=kQTn-tG0
+00001160: 374a 6231 2920 7365 7276 6963 6520 4150  7Jb1) service AP
+00001170: 492e 0a0a 2a2a 2a0a 0a49 6620 796f 7520  I...***..If you 
+00001180: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
+00001190: 6e73 2c20 706c 6561 7365 2073 656e 6420  ns, please send 
+000011a0: 6120 6d65 7373 6167 6520 746f 2074 6865  a message to the
+000011b0: 205b 5465 6c65 6772 616d 5d28 6874 7470   [Telegram](http
+000011c0: 733a 2f2f 742e 6d65 2f70 7974 686f 6e63  s://t.me/pythonc
+000011d0: 6170 7463 6861 2920 6368 6174 2072 6f6f  aptcha) chat roo
+000011e0: 6d2e 0a0a 4f72 2065 6d61 696c 2070 7974  m...Or email pyt
+000011f0: 686f 6e2d 6361 7074 6368 6140 706d 2e6d  hon-captcha@pm.m
+00001200: 650a 0a2a 2a2a 0a0a 2323 2048 6f77 2074  e..***..## How t
+00001210: 6f20 696e 7374 616c 6c3f 0a0a 5765 2072  o install?..We r
+00001220: 6563 6f6d 6d65 6e64 2075 7369 6e67 2074  ecommend using t
+00001230: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
+00001240: 6e20 6f66 2050 7974 686f 6e2e 2060 7079  n of Python. `py
+00001250: 7468 6f6e 332d 6361 7073 6f6c 7665 7260  thon3-capsolver`
+00001260: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
+00001270: 2033 2e37 2b2e 0a0a 2323 2320 7069 700a   3.7+...### pip.
+00001280: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+00001290: 7461 6c6c 2070 7974 686f 6e33 2d63 6170  tall python3-cap
+000012a0: 736f 6c76 6572 0a60 6060 0a0a 2323 2048  solver.```..## H
+000012b0: 6f77 2074 6f20 7573 653f 0a0a 4973 2064  ow to use?..Is d
+000012c0: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+000012d0: 5b64 6f63 756d 656e 7461 7469 6f6e 2d77  [documentation-w
+000012e0: 6562 7369 7465 5d28 6874 7470 733a 2f2f  ebsite](https://
+000012f0: 616e 6472 6569 6472 616e 672e 6769 7468  andreidrang.gith
+00001300: 7562 2e69 6f2f 7079 7468 6f6e 332d 6361  ub.io/python3-ca
+00001310: 7073 6f6c 7665 722f 292e 0a0a 0a23 2320  psolver/)....## 
+00001320: 486f 7720 746f 2074 6573 743f 0a0a 312e  How to test?..1.
+00001330: 2059 6f75 206e 6565 6420 7365 7420 6060   You need set ``
+00001340: 4150 495f 4b45 5960 6020 696e 2079 6f75  API_KEY`` in you
+00001350: 7220 656e 7669 726f 6e6d 656e 7428 6765  r environment(ge
+00001360: 7420 7468 6973 2076 616c 7565 2066 726f  t this value fro
+00001370: 6d20 796f 7520 6163 636f 756e 7429 2e0a  m you account)..
+00001380: 322e 2052 756e 2063 6f6d 6d61 6e64 2060  2. Run command `
+00001390: 606d 616b 6520 7465 7374 7360 602c 2066  `make tests``, f
+000013a0: 726f 6d20 726f 6f74 2064 6972 6563 746f  rom root directo
+000013b0: 7279 2e0a 0a0a 2323 2320 4368 616e 6765  ry....### Change
+000013c0: 6c6f 670a 0a43 6865 636b 205b 7265 6c65  log..Check [rele
+000013d0: 6173 6573 2070 6167 655d 2868 7474 7073  ases page](https
+000013e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+000013f0: 6472 6569 4472 616e 672f 7079 7468 6f6e  dreiDrang/python
+00001400: 332d 6361 7073 6f6c 7665 722f 7265 6c65  3-capsolver/rele
+00001410: 6173 6573 292e 0a0a 2323 2320 486f 7720  ases)...### How 
+00001420: 746f 2067 6574 2041 5049 204b 6579 2074  to get API Key t
+00001430: 6f20 776f 726b 2077 6974 6820 7468 6520  o work with the 
+00001440: 6c69 6272 6172 790a 312e 204f 6e20 7468  library.1. On th
+00001450: 6520 7061 6765 202d 2068 7474 7073 3a2f  e page - https:/
+00001460: 2f64 6173 6862 6f61 7264 2e63 6170 736f  /dashboard.capso
+00001470: 6c76 6572 2e63 6f6d 2f6f 7665 7276 6965  lver.com/overvie
+00001480: 772f 7573 6572 2d63 656e 7465 720a 322e  w/user-center.2.
+00001490: 2046 696e 6420 6974 3a20 215b 696d 672e   Find it: ![img.
+000014a0: 706e 675d 2866 696c 6573 2f69 6d67 2e70  png](files/img.p
+000014b0: 6e67 290a                                ng).
```

### Comparing `python3-capsolver-0.6.1/python3_capsolver.egg-info/SOURCES.txt` & `python3-capsolver-0.7.1/python3_capsolver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 setup.py
 python3_capsolver/__init__.py
 python3_capsolver/__version__.py
+python3_capsolver/aws_waf.py
 python3_capsolver/cloudflare.py
 python3_capsolver/control.py
+python3_capsolver/cyber_si_ara.py
 python3_capsolver/datadome_slider.py
 python3_capsolver/fun_captcha.py
 python3_capsolver/gee_test.py
 python3_capsolver/hcaptcha.py
 python3_capsolver/image_to_text.py
 python3_capsolver/mt_captcha.py
 python3_capsolver/recaptcha.py
```

### Comparing `python3-capsolver-0.6.1/setup.py` & `python3-capsolver-0.7.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from setuptools import Command, setup
 from pkg_resources import parse_requirements
 
 from python3_capsolver.__version__ import __version__
 
 # Package meta-data.
 NAME = "python3-capsolver"
-DESCRIPTION = "Python 3.7+ Capsolver library with AIO module."
+DESCRIPTION = "Python 3.8+ Capsolver library with AIO module."
 URL = "https://andreidrang.github.io/python3-capsolver/"
 EMAIL = "python-captcha@pm.me"
 AUTHOR = "AndreiDrang"
-REQUIRES_PYTHON = ">=3.7.0"
+REQUIRES_PYTHON = ">=3.8.0"
 VERSION = __version__
 with open("requirements.txt", "rt") as requirements_txt:
     REQUIRED = [str(requirement) for requirement in parse_requirements(requirements_txt)]
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
@@ -46,14 +46,17 @@
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
+        logging.info("Prepapre wheel")
+        os.system("pip install wheel")
+
         logging.info("Building Source and Wheel distribution . . .")
         os.system("python setup.py sdist bdist_wheel")
 
         logging.info("Uploading the package to PyPI via Twin . . .")
         os.system("twine upload dist/* --verbose")
 
         logging.info("🤖 Uploaded . . .")
@@ -77,17 +80,17 @@
     install_requires=REQUIRED,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email=EMAIL,
     project_urls={
         "Documentation": URL,
-        "Source": "https://github.com/AndreiDrang/python3-captchaai",
+        "Source": "https://github.com/AndreiDrang/python3-capsolver",
     },
-    package_dir={"python3-captchaai": "python3_capsolver"},
+    package_dir={"python3-capsolver": "python3_capsolver"},
     include_package_data=True,
     py_modules=["python3_capsolver"],
     url=URL,
     license="MIT",
     keywords="""
               	captcha 
                 recaptcha
@@ -115,15 +118,14 @@
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: AsyncIO",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
```

