# Comparing `tmp/atk_training_rin_chatlink-0.1.0.tar.gz` & `tmp/atk_training_rin_chatlink-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atk_training_rin_chatlink-0.1.0.tar", max compression
+gzip compressed data, was "atk_training_rin_chatlink-0.1.1.tar", max compression
```

## Comparing `atk_training_rin_chatlink-0.1.0.tar` & `atk_training_rin_chatlink-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      680 2023-07-27 12:24:45.193744 atk_training_rin_chatlink-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-26 10:26:04.796787 atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-27 12:26:30.762809 atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/auth_commands.py
--rw-r--r--   0        0        0      410 2023-07-27 11:38:59.353831 atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/client_secrets.json
--rw-r--r--   0        0        0      563 2023-07-27 11:16:58.025802 atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/main.py
--rw-r--r--   0        0        0      349 2023-07-27 10:56:58.754669 atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/processing.py
--rw-r--r--   0        0        0      444 2023-07-27 10:59:43.764928 atk_training_rin_chatlink-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 atk_training_rin_chatlink-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      755 2023-07-27 12:31:58.947281 atk_training_rin_chatlink-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 10:26:04.796787 atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-27 12:26:30.762809 atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/auth_commands.py
+-rw-r--r--   0        0        0      410 2023-07-27 11:38:59.353831 atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/client_secrets.json
+-rw-r--r--   0        0        0      563 2023-07-27 11:16:58.025802 atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/main.py
+-rw-r--r--   0        0        0      349 2023-07-27 10:56:58.754669 atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/processing.py
+-rw-r--r--   0        0        0      472 2023-07-27 12:30:57.994120 atk_training_rin_chatlink-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 atk_training_rin_chatlink-0.1.1/PKG-INFO
```

### Comparing `atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/auth_commands.py` & `atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/auth_commands.py`

 * *Files identical despite different names*

### Comparing `atk_training_rin_chatlink-0.1.0/atk_training_rin_chatlink/main.py` & `atk_training_rin_chatlink-0.1.1/atk_training_rin_chatlink/main.py`

 * *Files identical despite different names*

### Comparing `atk_training_rin_chatlink-0.1.0/PKG-INFO` & `atk_training_rin_chatlink-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6174 6b2d  : 2.1.Name: atk-
 00000020: 7472 6169 6e69 6e67 2d72 696e 2d63 6861  training-rin-cha
 00000030: 746c 696e 6b0a 5665 7273 696f 6e3a 2030  tlink.Version: 0
-00000040: 2e31 2e30 0a53 756d 6d61 7279 3a20 0a41  .1.0.Summary: .A
-00000050: 7574 686f 723a 206e 7863 6575 7269 6e0a  uthor: nxceurin.
-00000060: 4175 7468 6f72 2d65 6d61 696c 3a20 6532  Author-email: e2
-00000070: 3063 7365 3337 3640 6265 6e6e 6574 742e  0cse376@bennett.
-00000080: 6564 752e 696e 0a52 6571 7569 7265 732d  edu.in.Requires-
-00000090: 5079 7468 6f6e 3a20 3e3d 332e 3130 2c3c  Python: >=3.10,<
-000000a0: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
-000000b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000000c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000000d0: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-000000e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000000f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000100: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-00000110: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000120: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000130: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
-00000140: 6573 2d44 6973 743a 2070 7979 616d 6c20  es-Dist: pyyaml 
-00000150: 283e 3d36 2e30 2e31 2c3c 372e 302e 3029  (>=6.0.1,<7.0.0)
-00000160: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000170: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000180: 6d61 726b 646f 776e 0a0a 3c68 313e 3c2f  markdown..<h1></
-00000190: 6831 3e0a 4765 7473 2061 6c6c 206c 696e  h1>.Gets all lin
-000001a0: 6b73 2066 726f 6d20 6120 6769 7665 6e20  ks from a given 
-000001b0: 476f 6f67 6c65 2053 7061 6365 2061 6e64  Google Space and
-000001c0: 2073 746f 7265 7320 7468 656d 2069 6e20   stores them in 
-000001d0: 6120 7465 7874 2066 696c 652e 0a3c 6872  a text file..<hr
-000001e0: 3e0a 3c68 313e 5573 6167 653c 2f68 313e  >.<h1>Usage</h1>
-000001f0: 0a54 6f20 696e 7374 616c 6c20 7468 6520  .To install the 
-00000200: 7061 636b 6167 652c 2072 756e 200a 0a60  package, run ..`
-00000210: 6060 0a70 6970 2069 6e73 7461 6c6c 2061  ``.pip install a
-00000220: 746b 2d74 7261 696e 696e 672d 7269 6e2d  tk-training-rin-
-00000230: 6368 6174 6c69 6e6b 0a60 6060 0a0a 5468  chatlink.```..Th
-00000240: 6520 636f 6d6d 616e 6420 6361 6e20 6265  e command can be
-00000250: 2075 7365 6420 6279 2072 756e 6e69 6e67   used by running
-00000260: 2074 6865 2066 6f6c 6c6f 7769 6e67 2069   the following i
-00000270: 6e20 6120 7465 726d 696e 616c 2e0a 6060  n a terminal..``
-00000280: 600a 6174 6b2d 7472 6169 6e69 6e67 2d72  `.atk-training-r
-00000290: 696e 2d63 6861 746c 696e 6b20 7061 7468  in-chatlink path
-000002a0: 2f74 6f2f 636f 6e66 6967 2e79 616d 6c0a  /to/config.yaml.
-000002b0: 6060 600a 0a45 6e73 7572 6520 796f 7572  ```..Ensure your
-000002c0: 2063 6f6e 6669 672e 7961 6d6c 2068 6173   config.yaml has
-000002d0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-000002e0: 6965 6c64 733a 0a60 6060 7961 6d6c 0a73  ields:.```yaml.s
-000002f0: 7061 6365 3a20 6e61 6d65 206f 6620 7370  pace: name of sp
-00000300: 6163 6520 746f 2067 6574 206c 696e 6b73  ace to get links
-00000310: 2066 726f 6d0a 7361 7665 5f74 6f3a 2066   from.save_to: f
-00000320: 6f6c 6465 722f 746f 2f73 6176 652f 7572  older/to/save/ur
-00000330: 6c2e 7478 742f 746f 2f0a 6060 600a 0a41  l.txt/to/.```..A
-00000340: 6464 2079 6f75 7220 6060 6063 6c69 656e  dd your ```clien
-00000350: 745f 7365 6372 6574 732e 6a73 6f6e 6060  t_secrets.json``
-00000360: 6020 6669 6c65 2066 726f 6d20 476f 6f67  ` file from Goog
-00000370: 6c65 2043 6c6f 7564 2043 6f6e 736f 6c65  le Cloud Console
-00000380: 2074 6f20 6060 6061 746b 5f74 7261 696e   to ```atk_train
-00000390: 696e 675f 7269 6e5f 6368 6174 6c69 6e6b  ing_rin_chatlink
-000003a0: 6060 602e 204d 616b 6520 7375 7265 2069  ```. Make sure i
-000003b0: 7420 6861 7320 7468 6520 666f 6c6c 6f77  t has the follow
-000003c0: 696e 6720 7363 6f70 6573 2065 6e61 626c  ing scopes enabl
-000003d0: 6564 3a3c 6272 3e0a 3c75 6c3e 0a3c 6c69  ed:<br>.<ul>.<li
-000003e0: 3e2e 2e2e 2f61 7574 682f 6368 6174 2e73  >.../auth/chat.s
-000003f0: 7061 6365 732e 7265 6164 6f6e 6c79 3c2f  paces.readonly</
-00000400: 6c69 3e0a 3c6c 693e 2e2e 2e2f 6175 7468  li>.<li>.../auth
-00000410: 2f63 6861 742e 6d65 7373 6167 6573 2e72  /chat.messages.r
-00000420: 6561 646f 6e6c 793c 2f6c 693e 0a3c 2f75  eadonly</li>.</u
-00000430: 6c3e 0a                                  l>.
+00000040: 2e31 2e31 0a53 756d 6d61 7279 3a20 4765  .1.1.Summary: Ge
+00000050: 7420 5552 4c73 2066 726f 6d20 6120 476f  t URLs from a Go
+00000060: 6f67 6c65 2053 7061 6365 0a41 7574 686f  ogle Space.Autho
+00000070: 723a 206e 7863 6575 7269 6e0a 4175 7468  r: nxceurin.Auth
+00000080: 6f72 2d65 6d61 696c 3a20 6532 3063 7365  or-email: e20cse
+00000090: 3337 3640 6265 6e6e 6574 742e 6564 752e  376@bennett.edu.
+000000a0: 696e 0a52 6571 7569 7265 732d 5079 7468  in.Requires-Pyth
+000000b0: 6f6e 3a20 3e3d 332e 3130 2c3c 342e 300a  on: >=3.10,<4.0.
+000000c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000000d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000000e0: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+000000f0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000100: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000110: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000120: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000130: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000140: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000150: 2033 2e31 310a 5265 7175 6972 6573 2d44   3.11.Requires-D
+00000160: 6973 743a 2070 7979 616d 6c20 283e 3d36  ist: pyyaml (>=6
+00000170: 2e30 2e31 2c3c 372e 302e 3029 0a44 6573  .0.1,<7.0.0).Des
+00000180: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000190: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000001a0: 646f 776e 0a0a 3c68 313e 3c2f 6831 3e0a  down..<h1></h1>.
+000001b0: 4765 7473 2061 6c6c 206c 696e 6b73 2066  Gets all links f
+000001c0: 726f 6d20 6120 6769 7665 6e20 476f 6f67  rom a given Goog
+000001d0: 6c65 2053 7061 6365 2061 6e64 2073 746f  le Space and sto
+000001e0: 7265 7320 7468 656d 2069 6e20 6120 7465  res them in a te
+000001f0: 7874 2066 696c 652e 0a3c 6872 3e0a 3c68  xt file..<hr>.<h
+00000200: 313e 5573 6167 653c 2f68 313e 0a54 6f20  1>Usage</h1>.To 
+00000210: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00000220: 6167 652c 2072 756e 200a 0a60 6060 0a70  age, run ..```.p
+00000230: 6970 2069 6e73 7461 6c6c 2061 746b 2d74  ip install atk-t
+00000240: 7261 696e 696e 672d 7269 6e2d 6368 6174  raining-rin-chat
+00000250: 6c69 6e6b 0a60 6060 0a0a 5468 6520 636f  link.```..The co
+00000260: 6d6d 616e 6420 6361 6e20 6265 2075 7365  mmand can be use
+00000270: 6420 6279 2072 756e 6e69 6e67 2074 6865  d by running the
+00000280: 2066 6f6c 6c6f 7769 6e67 2069 6e20 6120   following in a 
+00000290: 7465 726d 696e 616c 2e0a 6060 600a 6174  terminal..```.at
+000002a0: 6b2d 7472 6169 6e69 6e67 2d72 696e 2d63  k-training-rin-c
+000002b0: 6861 746c 696e 6b20 7061 7468 2f74 6f2f  hatlink path/to/
+000002c0: 636f 6e66 6967 2e79 616d 6c0a 6060 600a  config.yaml.```.
+000002d0: 0a45 6e73 7572 6520 796f 7572 2063 6f6e  .Ensure your con
+000002e0: 6669 672e 7961 6d6c 2068 6173 2074 6865  fig.yaml has the
+000002f0: 2066 6f6c 6c6f 7769 6e67 2066 6965 6c64   following field
+00000300: 733a 0a60 6060 7961 6d6c 0a73 7061 6365  s:.```yaml.space
+00000310: 3a20 6e61 6d65 206f 6620 7370 6163 6520  : name of space 
+00000320: 746f 2067 6574 206c 696e 6b73 2066 726f  to get links fro
+00000330: 6d0a 7361 7665 5f74 6f3a 2066 6f6c 6465  m.save_to: folde
+00000340: 722f 746f 2f73 6176 652f 7572 6c2e 7478  r/to/save/url.tx
+00000350: 742f 746f 2f0a 6060 600a 0a49 6620 646f  t/to/.```..If do
+00000360: 776e 6c6f 6164 6564 2066 726f 6d20 4769  wnloaded from Gi
+00000370: 7448 7562 2c20 6164 6420 796f 7572 2060  tHub, add your `
+00000380: 6060 636c 6965 6e74 5f73 6563 7265 7473  ``client_secrets
+00000390: 2e6a 736f 6e60 6060 2066 696c 6520 6672  .json``` file fr
+000003a0: 6f6d 203c 6120 6872 6566 3d22 6874 7470  om <a href="http
+000003b0: 733a 2f2f 636f 6e73 6f6c 652e 636c 6f75  s://console.clou
+000003c0: 642e 676f 6f67 6c65 2e63 6f6d 2f22 3e47  d.google.com/">G
+000003d0: 6f6f 676c 6520 436c 6f75 6420 436f 6e73  oogle Cloud Cons
+000003e0: 6f6c 653c 2f61 3e20 746f 2060 6060 6174  ole</a> to ```at
+000003f0: 6b5f 7472 6169 6e69 6e67 5f72 696e 5f63  k_training_rin_c
+00000400: 6861 746c 696e 6b60 6060 2e20 4d61 6b65  hatlink```. Make
+00000410: 2073 7572 6520 6974 2068 6173 2074 6865   sure it has the
+00000420: 2066 6f6c 6c6f 7769 6e67 2073 636f 7065   following scope
+00000430: 7320 656e 6162 6c65 643a 3c62 723e 0a3c  s enabled:<br>.<
+00000440: 756c 3e0a 3c6c 693e 2e2e 2e2f 6175 7468  ul>.<li>.../auth
+00000450: 2f63 6861 742e 7370 6163 6573 2e72 6561  /chat.spaces.rea
+00000460: 646f 6e6c 793c 2f6c 693e 0a3c 6c69 3e2e  donly</li>.<li>.
+00000470: 2e2e 2f61 7574 682f 6368 6174 2e6d 6573  ../auth/chat.mes
+00000480: 7361 6765 732e 7265 6164 6f6e 6c79 3c2f  sages.readonly</
+00000490: 6c69 3e0a 3c2f 756c 3e0a                 li>.</ul>.
```

