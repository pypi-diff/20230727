# Comparing `tmp/nonebot_plugin_mystool-1.1.0.tar.gz` & `tmp/nonebot_plugin_mystool-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-1.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-1.2.0b1.tar", max compression
```

## Comparing `nonebot_plugin_mystool-1.1.0.tar` & `nonebot_plugin_mystool-1.2.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/LICENSE
--rw-r--r--   0        0        0     3825 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/README.md
--rw-r--r--   0        0        0     1322 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2158 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     4434 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    13805 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/data_model.py
--rw-r--r--   0        0        0    22678 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    11757 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/game_sign_api.py
--rw-r--r--   0        0        0     5463 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/good_image.py
--rw-r--r--   0        0        0     1955 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0     9662 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    21935 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/myb_missions_api.py
--rw-r--r--   0        0        0    31387 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0    12627 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/plugin_data.py
--rw-r--r--   0        0        0    10171 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    70861 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/simple_api.py
--rw-r--r--   0        0        0     2630 2023-07-23 06:23:42.383677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/user_check.py
--rw-r--r--   0        0        0    11480 2023-07-23 06:23:42.387677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/user_data.py
--rw-r--r--   0        0        0     9648 2023-07-23 06:23:42.387677 nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     5199 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/LICENSE
+-rw-r--r--   0        0        0     4630 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/README.md
+-rw-r--r--   0        0        0     1382 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2139 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    14918 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/data_model.py
+-rw-r--r--   0        0        0    22981 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    11963 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/game_sign_api.py
+-rw-r--r--   0        0        0     5463 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/good_image.py
+-rw-r--r--   0        0        0     2154 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    10355 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    21935 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/myb_missions_api.py
+-rw-r--r--   0        0        0    25577 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0    15022 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plugin_data.py
+-rw-r--r--   0        0        0    11698 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    70833 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/simple_api.py
+-rw-r--r--   0        0        0    10022 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_check.py
+-rw-r--r--   0        0        0    12863 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_data.py
+-rw-r--r--   0        0        0    14402 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     6101 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.2.0b1/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-1.1.0/LICENSE` & `nonebot_plugin_mystool-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.1.0/README.md` & `nonebot_plugin_mystool-1.2.0b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,193 +48,243 @@
 000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
 00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
 00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
 00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
 00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
 00000340: b60a 0a23 2320 f09f 93a3 20e6 9bb4 e696  ...## .... .....
 00000350: b0e5 8685 e5ae b90a 2323 2320 3230 3233  ........### 2023
-00000360: 2e37 2e32 3320 2d20 7631 2e31 2e30 0a2d  .7.23 - v1.1.0.-
-00000370: 20e5 a29e e58a a0e5 b4a9 e59d 8fef bc9a   ...............
-00000380: e698 9fe7 a9b9 e993 81e9 8193 e79a 84e4  ................
-00000390: bebf e7ac bae5 8a9f e883 bd20 2331 3430  ........... #140
-000003a0: 2023 3134 3320 6279 2040 4a6f 7365 616e   #143 by @Josean
-000003b0: 646c 7575 6520 4052 656d 6944 7265 0a20  dluue @RemiDre. 
-000003c0: 2020 203e 20e8 afb4 e698 8ee6 9687 e6a1     > ...........
-000003d0: a3ef bc9a 5bf0 9f94 97e6 989f e7a9 b9e9  ....[...........
-000003e0: 9381 e981 93e5 ae9e e697 b6e4 bebf e7ac  ................
-000003f0: ba5d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-00000400: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000410: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000420: 7374 6f6f 6c2f 7769 6b69 2f49 6e66 6f72  stool/wiki/Infor
-00000430: 6d61 7469 6f6e 2d53 7461 7252 6169 6c53  mation-StarRailS
-00000440: 7461 7475 7329 0a2d 20e4 bfae e5a4 8de6  tatus).- .......
-00000450: af8f e5b0 8fe6 97b6 e983 bde5 8f91 e980  ................
-00000460: 81e4 bebf e7ac bae9 809a e79f a5e7 9a84  ................
-00000470: 4275 6720 2331 3335 0a2d 20e4 baba e69c  Bug #135.- .....
-00000480: bae9 aa8c e8af 81e6 8993 e7a0 81e5 b9b3  ................
-00000490: e58f b0e6 94af e68c 81e8 87aa e5ae 9ae4  ................
-000004a0: b989 4a53 4f4e e586 85e5 aeb9 2023 3133  ..JSON...... #13
-000004b0: 330a 2020 2020 3e20 e8af b4e6 988e e696  3.    > ........
-000004c0: 87e6 a1a3 efbc 9a5b f09f 9497 6765 6574  .......[....geet
-000004d0: 6573 745f 6a73 6f6e 5d28 6874 7470 733a  est_json](https:
-000004e0: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-000004f0: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00000500: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-00000510: 692f 436f 6e66 6967 7572 6174 696f 6e2d  i/Configuration-
-00000520: 5072 6566 6572 656e 6365 2367 6565 7465  Preference#geete
-00000530: 7374 5f6a 736f 6e29 0a2d 20e4 bfae e5a4  st_json).- .....
-00000540: 8de5 9586 e593 81e5 8591 e68d a241 5049  .............API
-00000550: 2023 3131 300a 2d20 e4b8 8de5 9ca8 e5a5   #110.- ........
-00000560: bde5 8f8b e588 97e8 a1a8 e79a 84e7 94a8  ................
-00000570: e688 b7e6 95b0 e68d aee5 9ca8 e588 a0e9  ................
-00000580: 99a4 e589 8de5 b086 e8bf 9be8 a18c e5a4  ................
-00000590: 87e4 bbbd 2023 3132 390a 2020 2020 3e20  .... #129.    > 
-000005a0: e5a4 87e4 bbbd e79b aee5 bd95 efbc 9a60  ...............`
-000005b0: 6461 7461 2f6e 6f6e 6562 6f74 5f70 6c75  data/nonebot_plu
-000005c0: 6769 6e5f 6d79 7374 6f6f 6c2f 6465 6c65  gin_mystool/dele
-000005d0: 7465 6455 7365 7273 600a 2d20 e998 b2e6  tedUsers`.- ....
-000005e0: ada2 e59b a0e6 8f92 e4bb b6e6 95b0 e68d  ................
-000005f0: aee6 9687 e4bb b6e4 b8ad e9bb 98e8 aea4  ................
-00000600: e5ad 98e5 9ca8 2064 6576 6963 655f 636f  ...... device_co
-00000610: 6e66 6967 2c20 7361 6c74 5f63 6f6e 6669  nfig, salt_confi
-00000620: 6720 e880 8ce5 afbc e887 b4e6 9bb4 e696  g ..............
-00000630: b0e5 908e e9bb 98e8 aea4 e985 8de7 bdae  ................
-00000640: e8a2 abe5 8e9f e985 8de7 bdae e8a6 86e7  ................
-00000650: 9b96 e79a 84e9 97ae e9a2 980a 2d20 e88b  ............- ..
-00000660: a5e9 9c80 e8a6 81e4 bfae e694 b920 6465  ............. de
-00000670: 7669 6365 5f63 6f6e 6669 6720 e985 8de7  vice_config ....
-00000680: bdae efbc 8ce4 bfae e694 b9e5 908e e8bf  ................
-00000690: 98e8 aebe e7bd aee6 8f92 e4bb b6e6 95b0  ................
-000006a0: e68d aee6 9687 e4bb b6e4 b8ad 2070 7265  ............ pre
-000006b0: 6665 7265 6e63 652e 6f76 6572 7269 6465  ference.override
-000006c0: 5f64 6576 6963 655f 616e 645f 7361 6c74  _device_and_salt
-000006d0: 20e4 b8ba 2074 7275 6520 e4bb a5e8 a686   ... true ......
-000006e0: e79b 96e9 bb98 e8ae a4e5 80bc 0a20 2020  .............   
-000006f0: 203e 20e8 afb4 e698 8ee6 9687 e6a1 a3ef   > .............
-00000700: bc9a 0a20 2020 203e 202d 205b f09f 9497  ...    > - [....
-00000710: e7bd 91e7 bb9c e8af b7e6 b182 e8ae bee5  ................
-00000720: a487 e4bf a1e6 81af 2060 636c 6173 7320  ........ `class 
-00000730: 4465 7669 6365 436f 6e66 6967 605d 2868  DeviceConfig`](h
-00000740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000750: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000760: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000770: 6c2f 7769 6b69 2f43 6f6e 6669 6775 7261  l/wiki/Configura
-00000780: 7469 6f6e 2d44 6576 6963 6543 6f6e 6669  tion-DeviceConfi
-00000790: 6729 0a20 2020 203e 202d 205b f09f 9497  g).    > - [....
-000007a0: 6f76 6572 7269 6465 5f64 6576 6963 655f  override_device_
-000007b0: 616e 645f 7361 6c74 5d28 6874 7470 733a  and_salt](https:
-000007c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-000007d0: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-000007e0: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-000007f0: 692f 436f 6e66 6967 7572 6174 696f 6e2d  i/Configuration-
-00000800: 5072 6566 6572 656e 6365 236f 7665 7272  Preference#overr
-00000810: 6964 655f 6465 7669 6365 5f61 6e64 5f73  ide_device_and_s
-00000820: 616c 7429 0a2d 20e5 9ca8 e585 91e6 8da2  alt).- .........
-00000830: e5bc 80e5 a78b e590 8ee7 9a84 e4b8 80e6  ................
-00000840: aeb5 e697 b6e9 97b4 e586 85e4 b88d e696  ................
-00000850: ade5 b09d e8af 95e5 8591 e68d a2ef bc8c  ................
-00000860: e79b b4e5 88b0 e688 90e5 8a9f 2023 3131  ............ #11
-00000870: 300a 2d20 e585 91e6 8da2 e5bc 80e5 a78b  0.- ............
-00000880: e590 8ee5 b086 e4b8 8de4 bc9a e5bb b6e8  ................
-00000890: bf9f e585 91e6 8da2 efbc 8ce7 94a8 e688  ................
-000008a0: b7e6 95b0 e68d aee6 9687 e4bb b6e4 b8ad  ................
-000008b0: 2060 7072 6566 6572 656e 6365 2e65 7863   `preference.exc
-000008c0: 6861 6e67 655f 6c61 7465 6e63 7960 20e5  hange_latency` .
-000008d0: b086 e4bd 9ce4 b8ba e590 8ce4 b880 e7ba  ................
-000008e0: bfe7 a88b e4b8 8be6 af8f e4b8 aae5 8591  ................
-000008f0: e68d a2e8 afb7 e6b1 82e4 b98b e997 b4e7  ................
-00000900: 9a84 e697 b6e9 97b4 e997 b4e9 9a94 2023  .............. #
-00000910: 3131 300a 2d20 e585 91e6 8da2 e8af b7e6  110.- ..........
-00000920: b182 e697 a5e5 bf97 e586 85e5 aeb9 e5a2  ................
-00000930: 9ee5 8aa0 e4ba 86e5 8f91 e980 81e8 afb7  ................
-00000940: e6b1 82e6 97b6 e79a 84e6 97b6 e997 b4e6  ................
-00000950: 88b3 0a0a 2323 2320 3230 3233 2e36 2e32  ....### 2023.6.2
-00000960: 3320 2d20 7631 2e30 2e31 0a2d 20e4 bfae  3 - v1.0.1.- ...
-00000970: e5a4 8de6 97a0 e6b3 95e5 afbc e587 ba43  ...............C
-00000980: 6f6f 6b69 6573 e79a 84e9 97ae e9a2 980a  ookies..........
-00000990: 2d20 e4bf aee5 a48d e59b a0e7 bcba e5b0  - ..............
-000009a0: 91e5 8f82 e987 8fe8 b4a8 e58f 98e4 bbaa  ................
-000009b0: e695 b0e6 8dae e880 8ce5 afbc e887 b4e4  ................
-000009c0: b88d e696 ade6 8f90 e986 92e7 9a84 4275  ..............Bu
-000009d0: 670a 2d20 e4bf aee5 a48d e8b4 a6e5 8fb7  g.- ............
-000009e0: e8ae bee7 bdae e4b8 ade6 b8b8 e688 8fe7  ................
-000009f0: adbe e588 b0e5 bc80 e590 af2f e585 b3e9  .........../....
-00000a00: 97ad e78a b6e6 8081 e5ae 9ee9 9985 e5af  ................
-00000a10: b9e5 ba94 e79a 84e6 98af e7b1 b3e6 b8b8  ................
-00000a20: e5b8 81e4 bbbb e58a a1e7 9a84 4275 6720  ............Bug 
-00000a30: 2331 3231 2062 7920 4078 7874 6736 3636  #121 by @xxtg666
-00000a40: 0a0a 2323 20e5 8a9f e883 bde5 928c e789  ..## ...........
-00000a50: b9e6 80a7 0a0a 2d20 e79f ade4 bfa1 e9aa  ......- ........
-00000a60: 8ce8 af81 e799 bbe5 bd95 efbc 8ce5 858d  ................
-00000a70: e68a 93e5 8c85 e88e b7e5 8f96 2043 6f6f  ............ Coo
-00000a80: 6b69 650a 2d20 e887 aae5 8aa8 e5ae 8ce6  kie.- ..........
-00000a90: 8890 e6af 8fe6 97a5 e7b1 b3e6 b8b8 e5b8  ................
-00000aa0: 81e4 bbbb e58a a10a 2d20 e887 aae5 8aa8  ........- ......
-00000ab0: e8bf 9be8 a18c e6b8 b8e6 888f e7ad bee5  ................
-00000ac0: 88b0 0a2d 20e5 8faf e588 b6e5 ae9a e7b1  ...- ...........
-00000ad0: b3e6 b8b8 e5b8 81e5 9586 e593 81e5 8591  ................
-00000ae0: e68d a2e8 aea1 e588 92ef bc8c e588 b0e7  ................
-00000af0: 82b9 e585 91e6 8da2 efbc 88e5 9ba0 e58a  ................
-00000b00: a0e5 85a5 e4ba 86e4 baba e69c bae9 aa8c  ................
-00000b10: e8af 81ef bc8c e688 90e5 8a9f e78e 87e8  ................
-00000b20: be83 e4bd 8eef bc89 0a2d 20e5 8faf e694  .........- .....
-00000b30: afe6 8c81 e5a4 9ae4 b8aa 2051 5120 e8b4  .......... QQ ..
-00000b40: a6e5 8fb7 efbc 8ce6 af8f e4b8 aa20 5151  ............. QQ
-00000b50: 20e8 b4a6 e58f b7e5 8faf e7bb 91e5 ae9a   ...............
-00000b60: e5a4 9ae4 b8aa e7b1 b3e5 9388 e6b8 b8e8  ................
-00000b70: b4a6 e688 b70a 2d20 5151 20e6 8ea8 e980  ......- QQ .....
-00000b80: 81e6 89a7 e8a1 8ce7 bb93 e69e 9ce9 809a  ................
-00000b90: e79f a50a 2d20 e58e 9fe7 a59e e380 81e5  ....- ..........
-00000ba0: b4a9 e59d 8fef bc9a e698 9fe7 a9b9 e993  ................
-00000bb0: 81e9 8193 e78a b6e6 8081 e4be bfe7 acba  ................
-00000bc0: e980 9ae7 9fa5 0a0a 2323 20e4 bdbf e794  ........## .....
-00000bd0: a8e8 afb4 e698 8e0a 0a23 2323 20f0 9f9b  .........### ...
-00000be0: a0ef b88f 204e 6f6e 6542 6f74 3220 e69c  .... NoneBot2 ..
-00000bf0: bae5 99a8 e4ba bae9 83a8 e7bd b2e5 928c  ................
-00000c00: e68f 92e4 bbb6 e5ae 89e8 a385 0a0a e8af  ................
-00000c10: b7e6 9fa5 e79c 8b20 2d3e 205b f09f 9497  ....... -> [....
-00000c20: 496e 7374 616c 6c61 7469 6f6e 5d28 6874  Installation](ht
-00000c30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c40: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
-00000c50: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000c60: 2f77 696b 692f 496e 7374 616c 6c61 7469  /wiki/Installati
-00000c70: 6f6e 290a 0a23 2323 20f0 9f93 9620 e68f  on)..### .... ..
-00000c80: 92e4 bbb6 e585 b7e4 bd93 e4bd bfe7 94a8  ................
-00000c90: e8af b4e6 988e 0a0a e8af b7e6 9fa5 e79c  ................
-00000ca0: 8b20 2d3e 205b f09f 9497 5769 6b69 20e6  . -> [....Wiki .
-00000cb0: 9687 e6a1 a35d 2868 7474 7073 3a2f 2f67  .....](https://g
-00000cc0: 6974 6875 622e 636f 6d2f 4c6a 7a64 2d50  ithub.com/Ljzd-P
-00000cd0: 524f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  RO/nonebot-plugi
-00000ce0: 6e2d 6d79 7374 6f6f 6c2f 7769 6b69 290a  n-mystool/wiki).
-00000cf0: 0a23 2323 20e2 9d93 20e8 8eb7 e58f 96e6  .### ... .......
-00000d00: 8f92 e4bb b6e5 b8ae e58a a9e4 bfa1 e681  ................
-00000d10: af0a 0a23 2323 2320 e68f 92e4 bbb6 e591  ...#### ........
-00000d20: bde4 bba4 0a0a 6060 600a 2fe5 b8ae e58a  ......```./.....
-00000d30: a90a 6060 600a 0a3e 20e2 9aa0 efb8 8f20  ..```..> ...... 
-00000d40: e6b3 a8e6 848f 20e6 ada4 e5a4 84e6 b2a1  ...... .........
-00000d50: e69c 89e4 bdbf e794 a820 5bf0 9f94 9720  ......... [.... 
-00000d60: e68f 92e4 bbb6 e591 bde4 bba4 e5a4 b45d  ...............]
-00000d70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d80: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-00000d90: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000da0: 6f6f 6c2f 7769 6b69 2f43 6f6e 6669 6775  ool/wiki/Configu
-00000db0: 7261 7469 6f6e 2d43 6f6e 6669 6723 636f  ration-Config#co
-00000dc0: 6d6d 616e 6473 7461 7274 290a 0a23 2320  mmandstart)..## 
-00000dd0: e585 b6e4 bb96 0a0a 2323 2320 5bf0 9f93  ........### [...
-00000de0: 83e6 ba90 e7a0 81e8 afb4 e698 8e5d 2868  .............](h
-00000df0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e00: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000e10: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000e20: 6c2f 7769 6b69 2f53 6f75 7263 652d 5374  l/wiki/Source-St
-00000e30: 7275 6374 7572 6529 0a23 2323 20e9 8082  ructure).### ...
-00000e40: e985 8d20 5be7 bbaa e5b1 b1e7 9c9f e5af  ... [...........
-00000e50: bb42 6f74 5d28 6874 7470 733a 2f2f 6769  .Bot](https://gi
-00000e60: 7468 7562 2e63 6f6d 2f48 6962 694b 6965  thub.com/HibiKie
-00000e70: 722f 7a68 656e 7875 6e5f 626f 7429 20e7  r/zhenxun_bot) .
-00000e80: 9a84 e588 86e6 94af 0a2d 2068 7474 7073  .........- https
-00000e90: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d57  ://github.com/MW
-00000ea0: 544a 432f 7a68 656e 7875 6e2d 706c 7567  TJC/zhenxun-plug
-00000eb0: 696e 2d6d 7973 746f 6f6c 0a2d 2068 7474  in-mystool.- htt
-00000ec0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ed0: 6179 616b 6173 756b 692f 6e6f 6e65 626f  ayakasuki/nonebo
-00000ee0: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000ef0: 0a                                       .
+00000360: 2e37 2e32 3820 2d20 7631 2e32 2e30 2d62  .7.28 - v1.2.0-b
+00000370: 6574 612e 310a 2d20 e5a2 9ee5 8aa0 e5af  eta.1.- ........
+00000380: b951 51e9 a291 e981 93e7 9a84 e694 afe6  .QQ.............
+00000390: 8c81 2023 3132 380a 2020 3e20 e8af b4e6  .. #128.  > ....
+000003a0: 988e e696 87e6 a1a3 efbc 9a5b f09f 9497  ...........[....
+000003b0: 5151 4775 696c 6420 e980 82e9 858d e599  QQGuild ........
+000003c0: a85d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+000003d0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000003e0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+000003f0: 7374 6f6f 6c2f 7769 6b69 2f49 6e73 7461  stool/wiki/Insta
+00000400: 6c6c 6174 696f 6e23 5151 4775 696c 642d  llation#QQGuild-
+00000410: e980 82e9 858d e599 a829 0a2d 20e5 a29e  .........).- ...
+00000420: e58a a0e7 94a8 e688 b7e6 95b0 e68d aee7  ................
+00000430: bb91 e5ae 9ae5 85b3 e881 94e5 8a9f e883  ................
+00000440: bdef bc88 e5a6 8251 51e9 a291 e981 93e8  .......QQ.......
+00000450: b4a6 e58f b7e4 b88e 5151 e881 8ae5 a4a9  ........QQ......
+00000460: e8b4 a6e5 8fb7 e79a 84e6 95b0 e68d aee7  ................
+00000470: bb91 e5ae 9aef bc89 0a20 203e 20e8 afb4  .........  > ...
+00000480: e698 8ee6 9687 e6a1 a3ef bc9a 5bf0 9f94  ............[...
+00000490: 97e7 94a8 e688 b7e6 95b0 e68d aee7 bb91  ................
+000004a0: e5ae 9ae5 85b3 e881 945d 2868 7474 7073  .........](https
+000004b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+000004c0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+000004d0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+000004e0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d55  ki/Information-U
+000004f0: 7365 7242 696e 6429 0a2d 20e5 a29e e58a  serBind).- .....
+00000500: a0e5 8e9f e7a5 9ee4 bebf e7ac bae6 a091  ................
+00000510: e884 82e6 8f90 e986 92e9 9888 e580 bce7  ................
+00000520: 9a84 e8ae bee7 bdae e980 89e9 a1b9 2023  .............. #
+00000530: 3135 3120 6279 2040 4a6f 7365 616e 646c  151 by @Joseandl
+00000540: 7575 650a 2020 3e20 e8af b4e6 988e e696  uue.  > ........
+00000550: 87e6 a1a3 efbc 9a5b f09f 9497 e5af b9e7  .......[........
+00000560: bb91 e5ae 9ae7 9a84 e69f 90e4 b8aa e7b1  ................
+00000570: b3e5 9388 e6b8 b8e8 b4a6 e688 b7e8 bf9b  ................
+00000580: e8a1 8ce8 aebe e7bd ae5d 2868 7474 7073  .........](https
+00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+000005a0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+000005b0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+000005c0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d53  ki/Information-S
+000005d0: 6574 7469 6e67 2325 4535 2541 4625 4239  etting#%E5%AF%B9
+000005e0: 2545 3725 4242 2539 3125 4535 2541 4525  %E7%BB%91%E5%AE%
+000005f0: 3941 2545 3725 3941 2538 3425 4536 2539  9A%E7%9A%84%E6%9
+00000600: 4625 3930 2545 3425 4238 2541 4125 4537  F%90%E4%B8%AA%E7
+00000610: 2542 3125 4233 2545 3525 3933 2538 3825  %B1%B3%E5%93%88%
+00000620: 4536 2542 3825 4238 2545 3825 4234 2541  E6%B8%B8%E8%B4%A
+00000630: 3625 4536 2538 3825 4237 2545 3825 4246  6%E6%88%B7%E8%BF
+00000640: 2539 4225 4538 2541 3125 3843 2545 3825  %9B%E8%A1%8C%E8%
+00000650: 4145 2542 4525 4537 2542 4425 4145 290a  AE%BE%E7%BD%AE).
+00000660: 2d20 e4bf aee5 a48d 2060 7072 6566 6572  - ...... `prefer
+00000670: 656e 6365 2e6f 7665 7272 6964 655f 6465  ence.override_de
+00000680: 7669 6365 5f61 6e64 5f73 616c 7460 20e5  vice_and_salt` .
+00000690: 85b3 e997 ade6 97a0 e695 88e7 9a84 e997  ................
+000006a0: aee9 a298 0a0a 2323 2320 3230 3233 2e37  ......### 2023.7
+000006b0: 2e32 3320 2d20 7631 2e31 2e30 0a2d 20e5  .23 - v1.1.0.- .
+000006c0: a29e e58a a0e5 b4a9 e59d 8fef bc9a e698  ................
+000006d0: 9fe7 a9b9 e993 81e9 8193 e79a 84e4 bebf  ................
+000006e0: e7ac bae5 8a9f e883 bd20 2331 3430 2023  ......... #140 #
+000006f0: 3134 3320 6279 2040 4a6f 7365 616e 646c  143 by @Joseandl
+00000700: 7575 6520 4052 656d 6944 7265 0a20 2020  uue @RemiDre.   
+00000710: 203e 20e8 afb4 e698 8ee6 9687 e6a1 a3ef   > .............
+00000720: bc9a 5bf0 9f94 97e6 989f e7a9 b9e9 9381  ..[.............
+00000730: e981 93e5 ae9e e697 b6e4 bebf e7ac ba5d  ...............]
+00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000750: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000760: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000770: 6f6f 6c2f 7769 6b69 2f49 6e66 6f72 6d61  ool/wiki/Informa
+00000780: 7469 6f6e 2d53 7461 7252 6169 6c53 7461  tion-StarRailSta
+00000790: 7475 7329 0a2d 20e4 bfae e5a4 8de6 af8f  tus).- .........
+000007a0: e5b0 8fe6 97b6 e983 bde5 8f91 e980 81e4  ................
+000007b0: bebf e7ac bae9 809a e79f a5e7 9a84 4275  ..............Bu
+000007c0: 6720 2331 3335 0a2d 20e4 baba e69c bae9  g #135.- .......
+000007d0: aa8c e8af 81e6 8993 e7a0 81e5 b9b3 e58f  ................
+000007e0: b0e6 94af e68c 81e8 87aa e5ae 9ae4 b989  ................
+000007f0: 4a53 4f4e e586 85e5 aeb9 2023 3133 330a  JSON...... #133.
+00000800: 2020 2020 3e20 e8af b4e6 988e e696 87e6      > ..........
+00000810: a1a3 efbc 9a5b f09f 9497 6765 6574 6573  .....[....geetes
+00000820: 745f 6a73 6f6e 5d28 6874 7470 733a 2f2f  t_json](https://
+00000830: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000840: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000850: 696e 2d6d 7973 746f 6f6c 2f77 696b 692f  in-mystool/wiki/
+00000860: 436f 6e66 6967 7572 6174 696f 6e2d 5072  Configuration-Pr
+00000870: 6566 6572 656e 6365 2367 6565 7465 7374  eference#geetest
+00000880: 5f6a 736f 6e29 0a2d 20e4 bfae e5a4 8de5  _json).- .......
+00000890: 9586 e593 81e5 8591 e68d a241 5049 2023  ...........API #
+000008a0: 3131 300a 2d20 e4b8 8de5 9ca8 e5a5 bde5  110.- ..........
+000008b0: 8f8b e588 97e8 a1a8 e79a 84e7 94a8 e688  ................
+000008c0: b7e6 95b0 e68d aee5 9ca8 e588 a0e9 99a4  ................
+000008d0: e589 8de5 b086 e8bf 9be8 a18c e5a4 87e4  ................
+000008e0: bbbd 2023 3132 390a 2020 2020 3e20 e5a4  .. #129.    > ..
+000008f0: 87e4 bbbd e79b aee5 bd95 efbc 9a60 6461  .............`da
+00000900: 7461 2f6e 6f6e 6562 6f74 5f70 6c75 6769  ta/nonebot_plugi
+00000910: 6e5f 6d79 7374 6f6f 6c2f 6465 6c65 7465  n_mystool/delete
+00000920: 6455 7365 7273 600a 2d20 e998 b2e6 ada2  dUsers`.- ......
+00000930: e59b a0e6 8f92 e4bb b6e6 95b0 e68d aee6  ................
+00000940: 9687 e4bb b6e4 b8ad e9bb 98e8 aea4 e5ad  ................
+00000950: 98e5 9ca8 2060 6465 7669 6365 5f63 6f6e  .... `device_con
+00000960: 6669 6760 2c20 6073 616c 745f 636f 6e66  fig`, `salt_conf
+00000970: 6967 6020 e880 8ce5 afbc e887 b4e6 9bb4  ig` ............
+00000980: e696 b0e5 908e e9bb 98e8 aea4 e985 8de7  ................
+00000990: bdae e8a2 abe5 8e9f e985 8de7 bdae e8a6  ................
+000009a0: 86e7 9b96 e79a 84e9 97ae e9a2 980a 2d20  ..............- 
+000009b0: e88b a5e9 9c80 e8a6 81e4 bfae e694 b920  ............... 
+000009c0: 6064 6576 6963 655f 636f 6e66 6967 6020  `device_config` 
+000009d0: e985 8de7 bdae efbc 8ce4 bfae e694 b9e5  ................
+000009e0: 908e e8bf 98e8 aebe e7bd aee6 8f92 e4bb  ................
+000009f0: b6e6 95b0 e68d aee6 9687 e4bb b6e4 b8ad  ................
+00000a00: 2060 7072 6566 6572 656e 6365 2e6f 7665   `preference.ove
+00000a10: 7272 6964 655f 6465 7669 6365 5f61 6e64  rride_device_and
+00000a20: 5f73 616c 7460 20e4 b8ba 2074 7275 6520  _salt` ... true 
+00000a30: e4bb a5e8 a686 e79b 96e9 bb98 e8ae a4e5  ................
+00000a40: 80bc 0a20 2020 203e 20e8 afb4 e698 8ee6  ...    > .......
+00000a50: 9687 e6a1 a3ef bc9a 0a20 2020 203e 202d  .........    > -
+00000a60: 205b f09f 9497 e7bd 91e7 bb9c e8af b7e6   [..............
+00000a70: b182 e8ae bee5 a487 e4bf a1e6 81af 2060  .............. `
+00000a80: 636c 6173 7320 4465 7669 6365 436f 6e66  class DeviceConf
+00000a90: 6967 605d 2868 7474 7073 3a2f 2f67 6974  ig`](https://git
+00000aa0: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
+00000ab0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000ac0: 6d79 7374 6f6f 6c2f 7769 6b69 2f43 6f6e  mystool/wiki/Con
+00000ad0: 6669 6775 7261 7469 6f6e 2d44 6576 6963  figuration-Devic
+00000ae0: 6543 6f6e 6669 6729 0a20 2020 203e 202d  eConfig).    > -
+00000af0: 205b f09f 9497 6f76 6572 7269 6465 5f64   [....override_d
+00000b00: 6576 6963 655f 616e 645f 7361 6c74 5d28  evice_and_salt](
+00000b10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b20: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000b30: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000b40: 6f6c 2f77 696b 692f 436f 6e66 6967 7572  ol/wiki/Configur
+00000b50: 6174 696f 6e2d 5072 6566 6572 656e 6365  ation-Preference
+00000b60: 236f 7665 7272 6964 655f 6465 7669 6365  #override_device
+00000b70: 5f61 6e64 5f73 616c 7429 0a2d 20e5 a29e  _and_salt).- ...
+00000b80: e58a a0e4 ba86 e698 afe5 90a6 e4bd bfe7  ................
+00000b90: 94a8 e5a4 9ae8 bf9b e7a8 8be7 949f e688  ................
+00000ba0: 90e5 9586 e593 81e5 9bbe e789 87e7 9a84  ................
+00000bb0: e985 8de7 bdae e9a1 b920 6067 6f6f 645f  ......... `good_
+00000bc0: 6c69 7374 5f69 6d61 6765 5f63 6f6e 6669  list_image_confi
+00000bd0: 6760 2e60 4d55 4c54 495f 5052 4f43 4553  g`.`MULTI_PROCES
+00000be0: 5360 efbc 8ce5 a682 e69e 9ce9 8187 e588  S`..............
+00000bf0: b0e7 949f e688 90e5 9bbe e789 87e5 a4b1  ................
+00000c00: e8b4 a5e5 8faf e4bb a5e5 b09d e8af 95e5  ................
+00000c10: 85b3 e997 ade8 afa5 e9a1 b90a 2d20 e59c  ............- ..
+00000c20: a8e5 8591 e68d a2e5 bc80 e5a7 8be5 908e  ................
+00000c30: e79a 84e4 b880 e6ae b5e6 97b6 e997 b4e5  ................
+00000c40: 8685 e4b8 8de6 96ad e5b0 9de8 af95 e585  ................
+00000c50: 91e6 8da2 efbc 8ce7 9bb4 e588 b0e6 8890  ................
+00000c60: e58a 9f20 2331 3130 0a2d 20e5 8591 e68d  ... #110.- .....
+00000c70: a2e5 bc80 e5a7 8be5 908e e5b0 86e4 b88d  ................
+00000c80: e4bc 9ae5 bbb6 e8bf 9fe5 8591 e68d a2ef  ................
+00000c90: bc8c e794 a8e6 88b7 e695 b0e6 8dae e696  ................
+00000ca0: 87e4 bbb6 e4b8 ad20 6070 7265 6665 7265  ....... `prefere
+00000cb0: 6e63 652e 6578 6368 616e 6765 5f6c 6174  nce.exchange_lat
+00000cc0: 656e 6379 6020 e5b0 86e4 bd9c e4b8 bae5  ency` ..........
+00000cd0: 908c e4b8 80e7 babf e7a8 8be4 b88b e6af  ................
+00000ce0: 8fe4 b8aa e585 91e6 8da2 e8af b7e6 b182  ................
+00000cf0: e4b9 8be9 97b4 e79a 84e6 97b6 e997 b4e9  ................
+00000d00: 97b4 e99a 9420 2331 3130 0a2d 20e5 8591  ..... #110.- ...
+00000d10: e68d a2e8 afb7 e6b1 82e6 97a5 e5bf 97e5  ................
+00000d20: 8685 e5ae b9e5 a29e e58a a0e4 ba86 e58f  ................
+00000d30: 91e9 8081 e8af b7e6 b182 e697 b6e7 9a84  ................
+00000d40: e697 b6e9 97b4 e688 b30a 0a23 2320 e58a  ...........## ..
+00000d50: 9fe8 83bd e592 8ce7 89b9 e680 a70a 0a2d  ...............-
+00000d60: 20e6 94af e68c 8151 51e8 818a e5a4 a9e5   ......QQ.......
+00000d70: 928c 5151 e9a2 91e9 8193 0a2d 20e7 9fad  ..QQ.......- ...
+00000d80: e4bf a1e9 aa8c e8af 81e7 99bb e5bd 95ef  ................
+00000d90: bc8c e585 8de6 8a93 e58c 85e8 8eb7 e58f  ................
+00000da0: 9620 436f 6f6b 6965 0a2d 20e8 87aa e58a  . Cookie.- .....
+00000db0: a8e5 ae8c e688 90e6 af8f e697 a5e7 b1b3  ................
+00000dc0: e6b8 b8e5 b881 e4bb bbe5 8aa1 0a2d 20e8  .............- .
+00000dd0: 87aa e58a a8e8 bf9b e8a1 8ce6 b8b8 e688  ................
+00000de0: 8fe7 adbe e588 b00a 2d20 e58f afe5 88b6  ........- ......
+00000df0: e5ae 9ae7 b1b3 e6b8 b8e5 b881 e595 86e5  ................
+00000e00: 9381 e585 91e6 8da2 e8ae a1e5 8892 efbc  ................
+00000e10: 8ce5 88b0 e782 b9e5 8591 e68d a2ef bc88  ................
+00000e20: e59b a0e5 8aa0 e585 a5e4 ba86 e4ba bae6  ................
+00000e30: 9cba e9aa 8ce8 af81 efbc 8ce6 8890 e58a  ................
+00000e40: 9fe7 8e87 e8be 83e4 bd8e efbc 890a 2d20  ..............- 
+00000e50: e58f afe6 94af e68c 81e5 a49a e4b8 aa20  ............... 
+00000e60: 5151 20e8 b4a6 e58f b7ef bc8c e6af 8fe4  QQ .............
+00000e70: b8aa 2051 5120 e8b4 a6e5 8fb7 e58f afe7  .. QQ ..........
+00000e80: bb91 e5ae 9ae5 a49a e4b8 aae7 b1b3 e593  ................
+00000e90: 88e6 b8b8 e8b4 a6e6 88b7 0a2d 2051 5120  ...........- QQ 
+00000ea0: e68e a8e9 8081 e689 a7e8 a18c e7bb 93e6  ................
+00000eb0: 9e9c e980 9ae7 9fa5 0a2d 20e5 8e9f e7a5  .........- .....
+00000ec0: 9ee3 8081 e5b4 a9e5 9d8f efbc 9ae6 989f  ................
+00000ed0: e7a9 b9e9 9381 e981 93e7 8ab6 e680 81e4  ................
+00000ee0: bebf e7ac bae9 809a e79f a50a 0a23 2320  .............## 
+00000ef0: e4bd bfe7 94a8 e8af b4e6 988e 0a0a 2323  ..............##
+00000f00: 2320 f09f 9ba0 efb8 8f20 4e6f 6e65 426f  # ....... NoneBo
+00000f10: 7432 20e6 9cba e599 a8e4 baba e983 a8e7  t2 .............
+00000f20: bdb2 e592 8ce6 8f92 e4bb b6e5 ae89 e8a3  ................
+00000f30: 850a 0ae8 afb7 e69f a5e7 9c8b 202d 3e20  ............ -> 
+00000f40: 5bf0 9f94 9749 6e73 7461 6c6c 6174 696f  [....Installatio
+00000f50: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+00000f60: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000f70: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000f80: 7374 6f6f 6c2f 7769 6b69 2f49 6e73 7461  stool/wiki/Insta
+00000f90: 6c6c 6174 696f 6e29 0a0a 2323 2320 f09f  llation)..### ..
+00000fa0: 9396 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4  .. .............
+00000fb0: bdbf e794 a8e8 afb4 e698 8e0a 0ae8 afb7  ................
+00000fc0: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9757  ...... -> [....W
+00000fd0: 696b 6920 e696 87e6 a1a3 5d28 6874 7470  iki ......](http
+00000fe0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000ff0: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00001000: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00001010: 696b 6929 0a0a 2323 2320 e29d 9320 e88e  iki)..### ... ..
+00001020: b7e5 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9  ................
+00001030: e4bf a1e6 81af 0a0a 2323 2323 20e6 8f92  ........#### ...
+00001040: e4bb b6e5 91bd e4bb a40a 0a60 6060 0a2f  ...........```./
+00001050: e5b8 aee5 8aa9 0a60 6060 0a0a 3e20 e29a  .......```..> ..
+00001060: a0ef b88f 20e6 b3a8 e684 8f20 e6ad a4e5  .... ...... ....
+00001070: a484 e6b2 a1e6 9c89 e4bd bfe7 94a8 205b  .............. [
+00001080: f09f 9497 20e6 8f92 e4bb b6e5 91bd e4bb  .... ...........
+00001090: a4e5 a4b4 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+000010a0: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
+000010b0: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
+000010c0: 2d6d 7973 746f 6f6c 2f77 696b 692f 436f  -mystool/wiki/Co
+000010d0: 6e66 6967 7572 6174 696f 6e2d 436f 6e66  nfiguration-Conf
+000010e0: 6967 2363 6f6d 6d61 6e64 7374 6172 7429  ig#commandstart)
+000010f0: 0a0a 2323 20e5 85b6 e4bb 960a 0a23 2323  ..## ........###
+00001100: 205b f09f 9383 e6ba 90e7 a081 e8af b4e6   [..............
+00001110: 988e 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
+00001120: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+00001130: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00001140: 7973 746f 6f6c 2f77 696b 692f 536f 7572  ystool/wiki/Sour
+00001150: 6365 2d53 7472 7563 7475 7265 290a 2323  ce-Structure).##
+00001160: 2320 e980 82e9 858d 205b e7bb aae5 b1b1  # ...... [......
+00001170: e79c 9fe5 afbb 426f 745d 2868 7474 7073  ......Bot](https
+00001180: 3a2f 2f67 6974 6875 622e 636f 6d2f 4869  ://github.com/Hi
+00001190: 6269 4b69 6572 2f7a 6865 6e78 756e 5f62  biKier/zhenxun_b
+000011a0: 6f74 2920 e79a 84e5 8886 e694 af0a 2d20  ot) ..........- 
+000011b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000011c0: 6f6d 2f4d 5754 4a43 2f7a 6865 6e78 756e  om/MWTJC/zhenxun
+000011d0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c0a  -plugin-mystool.
+000011e0: 2d20 6874 7470 733a 2f2f 6769 7468 7562  - https://github
+000011f0: 2e63 6f6d 2f61 7961 6b61 7375 6b69 2f6e  .com/ayakasuki/n
+00001200: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00001210: 7374 6f6f 6c0a                           stool.
```

### Comparing `nonebot_plugin_mystool-1.1.0/pyproject.toml` & `nonebot_plugin_mystool-1.2.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v1.1.0"
+version = "v1.2.0-beta.1"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
@@ -26,15 +26,17 @@
 python = ">=3.9,<4.0"
 httpx = "^0.24.1"
 nonebot_plugin_apscheduler = ">=0.2.0"
 ntplib = "^0.4.0"
 Pillow = ">=9.5,<11.0"
 requests = "^2.31.0"
 nonebot_adapter_onebot = "^2.2.3"
+nonebot-adapter-qqguild = "^0.2.3"
 tenacity = "^8.2.2"
+qrcode = "^7.4.2"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/address.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,94 @@
-"""
-### 米游社收货地址相关
-"""
-import asyncio
-from typing import Union
-
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import PrivateMessageEvent, GroupMessageEvent
-from nonebot.adapters.onebot.v11.message import Message
-from nonebot.matcher import Matcher
-from nonebot.params import Arg, ArgPlainText, T_State
-
-from .plugin_data import PluginDataManager, write_plugin_data
-from .simple_api import get_address
-from .user_data import UserAccount
-from .utils import COMMAND_BEGIN
-
-_conf = PluginDataManager.plugin_data
-
-address_matcher = on_command(_conf.preference.command_start + '地址', priority=4, block=True)
-
-address_matcher.name = '地址'
-address_matcher.usage = '跟随指引，获取地址ID，用于兑换米游币商品。在获取地址ID前，如果你还没有设置米游社收获地址，请前往官网或App设置'
-
-
-@address_matcher.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher):
-    if isinstance(event, GroupMessageEvent):
-        await address_matcher.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行地址设置。")
-    user = _conf.users.get(event.user_id)
-    user_account = user.accounts if user else None
-    if not user_account:
-        await address_matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
-    else:
-        await address_matcher.send(
-            "请跟随指引设置收货地址ID，如果你还没有设置米游社收获地址，请前往官网或App设置。\n🚪过程中发送“退出”即可退出")
-    if len(user_account) == 1:
-        account = next(iter(user_account.values()))
-        matcher.set_arg('bbs_uid', Message(account.bbs_uid))
-    else:
-        msg = "您有多个账号，您要设置以下哪个账号的收货地址？\n"
-        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
-        await matcher.send(msg)
-
-
-@address_matcher.got('bbs_uid')
-async def _(event: PrivateMessageEvent, state: T_State, uid=Arg("bbs_uid")):
-    if isinstance(uid, Message):
-        uid = uid.extract_plain_text().strip()
-    if uid == '退出':
-        await address_matcher.finish('🚪已成功退出')
-
-    user_account = _conf.users[event.user_id].accounts
-    if uid not in user_account:
-        await address_matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
-    account = user_account[uid]
-    state['account'] = account
-
-    address_status, address_list = await get_address(account)
-    state['address_list'] = address_list
-    if not address_status:
-        if address_status.login_expired:
-            await address_matcher.finish(f"⚠️账户 {account.bbs_uid} 登录失效，请重新登录")
-        await address_matcher.finish("⚠️获取失败，请稍后重新尝试")
-
-    if address_list:
-        address_text = map(
-            lambda x: f"省 ➢ {x.province_name}" \
-                      f"\n市 ➢ {x.city_name}" \
-                      f"\n区/县 ➢ {x.county_name}" \
-                      f"\n详细地址 ➢ {x.addr_ext}" \
-                      f"\n联系电话 ➢ {x.phone}" \
-                      f"\n联系人 ➢ {x.connect_name}" \
-                      f"\n地址ID ➢ {x.id}",
-            address_list
-        )
-        msg = "以下为查询结果：" \
-              "\n\n" + "\n- - -\n".join(address_text)
-        await address_matcher.send(msg)
-        await asyncio.sleep(0.2)
-    else:
-        await address_matcher.finish("⚠️您还没有配置地址，请先前往米游社配置地址！")
-
-
-@address_matcher.got('address_id', prompt='请发送你要选择的地址ID')
-async def _(_: PrivateMessageEvent, state: T_State, address_id=ArgPlainText()):
-    if address_id == "退出":
-        await address_matcher.finish("🚪已成功退出")
-
-    address_filter = filter(lambda x: x.id == address_id, state['address_list'])
-    address = next(address_filter, None)
-    if address is not None:
-        account: UserAccount = state["account"]
-        account.address = address
-        write_plugin_data()
-        await address_matcher.finish(f"🎉已成功设置账户 {account.bbs_uid} 的地址")
-    else:
-        await address_matcher.reject("⚠️您发送的地址ID与查询结果不匹配，请重新发送")
+"""
+### 米游社收货地址相关
+"""
+import asyncio
+
+from nonebot import on_command
+from nonebot.internal.params import ArgStr
+from nonebot.matcher import Matcher
+from nonebot.params import T_State
+
+from .plugin_data import PluginDataManager, write_plugin_data
+from .simple_api import get_address
+from .user_data import UserAccount
+from .utils import COMMAND_BEGIN, GeneralMessageEvent, GeneralPrivateMessageEvent, GeneralGroupMessageEvent
+
+_conf = PluginDataManager.plugin_data
+
+address_matcher = on_command(_conf.preference.command_start + '地址', priority=4, block=True)
+
+address_matcher.name = '地址'
+address_matcher.usage = '跟随指引，获取地址ID，用于兑换米游币商品。在获取地址ID前，如果你还没有设置米游社收获地址，请前往官网或App设置'
+
+
+@address_matcher.handle()
+async def _(event: GeneralMessageEvent, matcher: Matcher, state: T_State):
+    if isinstance(event, GeneralGroupMessageEvent):
+        await address_matcher.finish("⚠️为了保护您的隐私，请私聊进行地址设置。")
+    user = _conf.users.get(event.user_id)
+    user_account = user.accounts if user else None
+    if not user_account:
+        await address_matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
+    else:
+        await address_matcher.send(
+            "请跟随指引设置收货地址ID，如果你还没有设置米游社收获地址，请前往官网或App设置。\n🚪过程中发送“退出”即可退出")
+    if len(user_account) == 1:
+        account = next(iter(user_account.values()))
+        state["bbs_uid"] = account.bbs_uid
+    else:
+        msg = "您有多个账号，您要设置以下哪个账号的收货地址？\n"
+        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
+        await matcher.send(msg)
+
+
+@address_matcher.got('bbs_uid')
+async def _(event: GeneralPrivateMessageEvent, state: T_State, bbs_uid=ArgStr()):
+    if bbs_uid == '退出':
+        await address_matcher.finish('🚪已成功退出')
+
+    user_account = _conf.users[event.user_id].accounts
+    if bbs_uid not in user_account:
+        await address_matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
+    account = user_account[bbs_uid]
+    state['account'] = account
+
+    address_status, address_list = await get_address(account)
+    state['address_list'] = address_list
+    if not address_status:
+        if address_status.login_expired:
+            await address_matcher.finish(f"⚠️账户 {account.bbs_uid} 登录失效，请重新登录")
+        await address_matcher.finish("⚠️获取失败，请稍后重新尝试")
+
+    if address_list:
+        address_text = map(
+            lambda x: f"省 ➢ {x.province_name}" \
+                      f"\n市 ➢ {x.city_name}" \
+                      f"\n区/县 ➢ {x.county_name}" \
+                      f"\n详细地址 ➢ {x.addr_ext}" \
+                      f"\n联系电话 ➢ {x.phone}" \
+                      f"\n联系人 ➢ {x.connect_name}" \
+                      f"\n地址ID ➢ {x.id}",
+            address_list
+        )
+        msg = "以下为查询结果：" \
+              "\n\n" + "\n- - -\n".join(address_text)
+        await address_matcher.send(msg)
+        await asyncio.sleep(0.2)
+    else:
+        await address_matcher.finish("⚠️您还没有配置地址，请先前往米游社配置地址！")
+
+
+@address_matcher.got('address_id', prompt='请发送你要选择的地址ID')
+async def _(_: GeneralPrivateMessageEvent, state: T_State, address_id=ArgStr()):
+    if address_id == "退出":
+        await address_matcher.finish("🚪已成功退出")
+
+    address_filter = filter(lambda x: x.id == address_id, state['address_list'])
+    address = next(address_filter, None)
+    if address is not None:
+        account: UserAccount = state["account"]
+        account.address = address
+        write_plugin_data()
+        await address_matcher.finish(f"🎉已成功设置账户 {account.bbs_uid} 的地址")
+    else:
+        await address_matcher.reject("⚠️您发送的地址ID与查询结果不匹配，请重新发送")
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/data_model.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -357,14 +357,16 @@
     """探索派遣 最多派遣数"""
     current_home_coin: int
     """洞天财瓮 未收取的宝钱数"""
     max_home_coin: int
     """洞天财瓮 最多可容纳宝钱数"""
     transformer: Optional[Dict[str, Any]]
     """参量质变仪相关数据"""
+    resin_recovery_time: int
+    """剩余树脂恢复时间"""
 
     @property
     def transformer_text(self):
         """
         参量质变仪状态文本
         """
         try:
@@ -374,14 +376,31 @@
                 return '已准备就绪'
             else:
                 return f"{self.transformer['recovery_time']['Day']} 天" \
                        f"{self.transformer['recovery_time']['Hour']} 小时 {self.transformer['recovery_time']['Minute']} 分钟"
         except KeyError:
             return None
 
+    @property
+    def resin_recovery_text(self):
+        """
+        剩余树脂恢复文本
+        """
+        try:
+            if not self.resin_recovery_time:
+                return ':未获得时间数据'
+            elif self.resin_recovery_time == 0:
+                return '已准备就绪'
+            else:
+                recovery_timestamp = int(time.time()) + self.resin_recovery_time
+                recovery_datetime = datetime.fromtimestamp(recovery_timestamp)
+                return f"将在{recovery_datetime.strftime('%m-%d %H:%M')}回满"
+        except KeyError:
+            return None
+
 
 class StarRailBoard(BaseModel):
     """
     崩铁实时便笺数据 (从米游社内相关页面API的返回数据初始化)
     """
     current_stamina: int
     """当前开拓力"""
@@ -407,22 +426,21 @@
     @property
     def stamina_recover_text(self):
         """
         剩余体力恢复文本
         """
         try:
             if not self.stamina_recover_time:
-                return '体力未获得'
+                return ':未获得时间数据'
             elif self.stamina_recover_time == 0:
-                return '体力已准备就绪'
+                return '已准备就绪'
             else:
-                return datetime.fromtimestamp(int(time.time()) + self.stamina_recover_time)
-                # m, s = divmod(self.stamina_recover_time, 60)
-                # h, m = divmod(m, 60) 
-                # return f"{h} 小时 {m} 分钟 {s} 秒"
+                recovery_timestamp = int(time.time()) + self.stamina_recover_time
+                recovery_datetime = datetime.fromtimestamp(recovery_timestamp)
+                return f"将在{recovery_datetime.strftime('%m-%d %H:%M')}回满"
         except KeyError:
             return None
 
 
 class BaseApiStatus(BaseModel):
     """
     API返回结果基类
@@ -442,14 +460,24 @@
 
     def __bool__(self):
         if self.success:
             return True
         else:
             return False
 
+    @property
+    def error_type(self):
+        """
+        返回错误类型
+        """
+        for key, field in self.__fields__.items():
+            if field and key != "success":
+                return key
+        return None
+
 
 class CreateMobileCaptchaStatus(BaseApiStatus):
     """
     发送短信验证码 返回结果
     """
     incorrect_geetest = False
     """人机验证结果数据无效"""
@@ -518,23 +546,33 @@
     """
     兑换操作 返回结果
     """
     invalid_arguments = False
     """参数错误"""
 
 
-class GenshinBoardStatus(BaseApiStatus):
+class BoardStatus(BaseApiStatus):
+    """
+    实时便笺 返回结果
+    """
+    game_record_failed = False
+    """获取用户游戏数据失败"""
+    game_list_failed = False
+    """获取游戏列表失败"""
+
+
+class GenshinBoardStatus(BoardStatus):
     """
     原神实时便笺 返回结果
     """
     no_genshin_account = False
     """用户没有任何原神账户"""
 
 
-class StarRailBoardStatus(BaseApiStatus):
+class StarRailBoardStatus(BoardStatus):
     """
     星铁实时便笺 返回结果
     """
     no_starrail_account = False
     """用户没有任何星铁账户"""
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/exchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,91 +7,103 @@
 import random
 import threading
 import time
 from datetime import datetime
 from multiprocessing import Manager
 from multiprocessing.pool import Pool
 from multiprocessing.synchronize import Lock
-from typing import List, Union, Callable, Any, Tuple, Optional, Dict
+from typing import List, Callable, Any, Tuple, Optional, Dict
 
 import nonebot
 from apscheduler.events import JobExecutionEvent, EVENT_JOB_EXECUTED
-from nonebot import on_command, get_bot
-from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
-                                         PrivateMessageEvent, GroupMessageEvent)
-from nonebot.adapters.onebot.v11.message import Message
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import MessageEvent as OnebotV11MessageEvent, MessageSegment as OnebotV11MessageSegment
+from nonebot.adapters.qqguild import MessageEvent as QQGuildMessageEvent, MessageSegment as QQGuildMessageSegment
+from nonebot.internal.params import ArgStr
 from nonebot.matcher import Matcher
-from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
+from nonebot.params import ArgPlainText, T_State, CommandArg, Command
 from nonebot_plugin_apscheduler import scheduler
 
 from .data_model import Good, GameRecord, ExchangeStatus
 from .good_image import game_list_to_image
 from .plugin_data import PluginDataManager, write_plugin_data
 from .simple_api import get_game_record, get_good_detail, get_good_list, good_exchange_sync, get_device_fp, \
     good_exchange
 from .user_data import UserAccount, ExchangePlan, ExchangeResult
-from .utils import COMMAND_BEGIN, logger, get_last_command_sep
+from .utils import COMMAND_BEGIN, logger, get_last_command_sep, GeneralMessageEvent, send_private_msg
 
 _conf = PluginDataManager.plugin_data
 _driver = nonebot.get_driver()
 
-myb_exchange_plan = on_command(f"{_conf.preference.command_start}兑换",
-                               aliases={(f"{_conf.preference.command_start}兑换", "+"),
-                                        (f"{_conf.preference.command_start}兑换", "-")},
-                               priority=5, block=True)
+myb_exchange_plan = on_command(
+    f"{_conf.preference.command_start}兑换",
+    aliases={
+        (f"{_conf.preference.command_start}兑换", "+"),
+        (f"{_conf.preference.command_start}兑换", "-")
+    },
+    priority=5,
+    block=True
+)
 myb_exchange_plan.name = "兑换"
 myb_exchange_plan.usage = "跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，" \
                           "并使用『{HEAD}地址』选择你要使用的地址。" \
                           "所需的商品ID可通过命令『{HEAD}商品』获取。" \
                           "注意，不限兑换时间的商品将不会在此处显示。 "
 myb_exchange_plan.extra_usage = """\
 具体用法：
-{HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
-{HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
-{HEAD}商品 ➢ 查看米游社商品
+🛒 {HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
+🗑️ {HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
+🎁 {HEAD}商品 ➢ 查看米游社商品
 『{SEP}』为分隔符，使用NoneBot配置中的其他分隔符亦可\
 """
 
 
 @myb_exchange_plan.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, command=Command(),
-            command_arg=CommandArg()):
+async def _(
+        event: GeneralMessageEvent,
+        matcher: Matcher,
+        state: T_State,
+        command=Command(),
+        command_arg=CommandArg()
+):
     """
     主命令触发
 
     :command: 主命令和二级命令的元组
     :command_arg: 二级命令的参数，即商品ID，为Message
     """
     if command_arg and len(command) == 1:
         # 如果没有二级命令，但是有参数，则说明用户没有意向使用本功能。
         # 例如：/兑换码获取，识别到的参数为"码获取"，而用户可能有意使用其他插件。
         await matcher.finish()
-    elif len(command) > 1 and command[1] in ["+", "-"]:
+    elif len(command) > 1:
         if not command_arg:
             await matcher.reject(
-                '⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
-                                                                                        SEP=get_last_command_sep()))
+                '⚠️您的输入有误，缺少商品ID，请重新输入\n\n'
+                f'{myb_exchange_plan.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep())}'
+            )
         elif not str(command_arg).isdigit():
             await matcher.reject(
-                '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
-                                                                                 SEP=get_last_command_sep()))
+                '⚠️商品ID必须为数字，请重新输入\n\n'
+                f'{myb_exchange_plan.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep())}'
+            )
 
-    user = _conf.users.get(event.user_id)
+    user = _conf.users.get(event.get_user_id())
     user_account = user.accounts if user else None
     if not user_account:
         await matcher.finish(
             f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
 
     # 如果使用了二级命令 + - 则跳转进下一步，通过phone选择账户进行设置
     if len(command) > 1:
         state['command_2'] = command[1]
         matcher.set_arg("good_id", command_arg)
         if len(user_account) == 1:
             uid = next(iter(user_account.values())).bbs_uid
-            matcher.set_arg('bbs_uid', Message(uid))
+            state["bbs_uid"] = uid
         else:
             msg = "您有多个账号，您要配置以下哪个账号的兑换计划？\n"
             msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
             msg += "\n🚪发送“退出”即可退出"
             await matcher.send(msg)
     # 如果未使用二级命令，则进行查询操作，并结束交互
     else:
@@ -104,35 +116,43 @@
                    f"\n- 🔢商品ID：{good.goods_id}" \
                    f"\n- 💰商品价格：{good.price} 米游币" \
                    f"\n- 📅兑换时间：{good.time_text}" \
                    f"\n- 🆔账户：{plan.account.bbs_uid}"
             msg += "\n\n"
         if not msg:
             msg = '您还没有兑换计划哦~\n\n'
-        await matcher.finish(msg + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+        await matcher.finish(msg + myb_exchange_plan.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
 
 
 @myb_exchange_plan.got('bbs_uid')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
-            uid=ArgStr('bbs_uid')):
+async def _(
+        event: GeneralMessageEvent,
+        matcher: Matcher,
+        state: T_State,
+        bbs_uid=ArgStr()
+):
     """
     请求用户输入手机号以对账户设置兑换计划
     """
-    user_account = _conf.users[event.user_id].accounts
-    if uid == '退出':
+    if bbs_uid == '退出':
         await matcher.finish('🚪已成功退出')
-    if uid in user_account:
-        state["account"] = user_account[uid]
+    user_account = _conf.users[event.get_user_id()].accounts
+    if bbs_uid in user_account:
+        state["account"] = user_account[bbs_uid]
     else:
         await matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
 
 
 @myb_exchange_plan.got('good_id')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
-            good_id=ArgPlainText('good_id')):
+async def _(
+        event: GeneralMessageEvent,
+        matcher: Matcher,
+        state: T_State,
+        good_id=ArgPlainText('good_id')
+):
     """
     处理三级命令，即商品ID
     """
     account: UserAccount = state['account']
     command_2 = state['command_2']
     if command_2 == '+':
         good_dict = {
@@ -158,72 +178,77 @@
         if flag:
             await matcher.finish('⚠️您发送的商品ID不在可兑换的商品列表内，程序已退出')
         state['good'] = good
         if good.time:
             # 若为实物商品，也进入下一步骤，但是传入uid为None
             if good.is_virtual:
                 game_records_status, records = await get_game_record(account)
-
                 if game_records_status:
                     if len(records) == 0:
-                        matcher.set_arg('uid', Message(records[0].game_role_id))
+                        state['game_uid'] = records[0].game_role_id
                     else:
                         msg = f'您米游社账户下的游戏账号：'
                         for record in records:
                             msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.game_role_id}'
                         if records:
                             state['records'] = records
                             await matcher.send(
                                 "您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
                             await asyncio.sleep(0.5)
                             await matcher.send(msg)
                         else:
                             await matcher.finish(
                                 f"您的米游社账户下还没有绑定游戏账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
+                else:
+                    await matcher.finish('⚠️获取游戏账号列表失败，无法继续')
             else:
                 if not account.address:
                     await matcher.finish('⚠️您还没有配置地址哦，请先配置地址')
-                matcher.set_arg('uid', Message())
+                state['game_uid'] = ''
         else:
             await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
 
     elif command_2 == '-':
-        plans = _conf.users[event.user_id].exchange_plans
+        plans = _conf.users[event.get_user_id()].exchange_plans
         if plans:
             for plan in plans:
                 if plan.good.goods_id == good_id:
                     plans.remove(plan)
                     write_plugin_data()
                     for i in range(_conf.preference.exchange_thread_count):
                         scheduler.remove_job(job_id=f"exchange-plan-{hash(plan)}-{i}")
                     await matcher.finish('兑换计划删除成功')
             await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
         else:
             await matcher.finish("您还没有配置兑换计划哦~")
 
     else:
         await matcher.reject(
-            '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
-                                                                         SEP=get_last_command_sep()))
+            '⚠️您的输入有误，请重新输入\n\n' + myb_exchange_plan.extra_usage.format(HEAD=COMMAND_BEGIN,
+                                                                                   SEP=get_last_command_sep()))
 
 
-@myb_exchange_plan.got('uid')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
-            uid=ArgPlainText('uid')):
+@myb_exchange_plan.got('game_uid')
+async def _(
+        event: GeneralMessageEvent,
+        matcher: Matcher,
+        state: T_State,
+        game_uid=ArgStr()
+):
     """
     初始化商品兑换任务，如果传入UID为None则为实物商品，仍可继续
     """
-    user = _conf.users[event.user_id]
+    user = _conf.users[event.get_user_id()]
     account: UserAccount = state['account']
     good: Good = state['good']
     if good.is_virtual:
         records: List[GameRecord] = state['records']
-        if uid == '退出':
+        if game_uid == '退出':
             await matcher.finish('🚪已成功退出')
-        record_filter = filter(lambda x: x.game_role_id == uid, records)
+        record_filter = filter(lambda x: x.game_role_id == game_uid, records)
         record = next(record_filter, None)
         if not record:
             await matcher.reject('⚠️您输入的UID不在上述账号内，请重新输入')
         plan = ExchangePlan(good=good, address=account.address, game_record=record, account=account)
     else:
         plan = ExchangePlan(good=good, address=account.address, account=account)
     if plan in user.exchange_plans:
@@ -257,35 +282,35 @@
 
 get_good_image = on_command(_conf.preference.command_start + '商品', priority=5, block=True)
 get_good_image.name = "商品"
 get_good_image.usage = "获取当日米游币商品信息。添加自动兑换计划需要商品ID，请记下您要兑换的商品的ID。"
 
 
 @get_good_image.handle()
-async def _(_: MessageEvent, matcher: Matcher, arg=CommandArg()):
+async def _(_: GeneralMessageEvent, matcher: Matcher, arg=CommandArg()):
     # 若有使用二级命令，即传入了想要查看的商品类别，则跳过询问
     if arg:
         matcher.set_arg("content", arg)
 
 
 @get_good_image.got("content", prompt="请发送您要查看的商品类别:"
                                       "\n- 崩坏3"
                                       "\n- 原神"
                                       "\n- 崩坏2"
                                       "\n- 崩坏：星穹铁道"
                                       "\n- 未定事件簿"
                                       "\n- 米游社"
                                       "\n若是商品图片与米游社商品不符或报错 请发送“更新”哦~"
                                       "\n—— 🚪发送“退出”以结束")
-async def _(_: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
+async def _(event: GeneralMessageEvent, arg=ArgPlainText("content")):
     """
     根据传入的商品类别，发送对应的商品列表图片
     """
     if arg == '退出':
-        await matcher.finish('🚪已成功退出')
+        await get_good_image.finish('🚪已成功退出')
     elif arg in ['原神', 'ys']:
         arg = ('hk4e', '原神')
     elif arg in ['崩坏3', '崩坏三', '崩3', '崩三', '崩崩崩', '蹦蹦蹦', 'bh3']:
         arg = ('bh3', '崩坏3')
     elif arg in ['崩坏2', '崩坏二', '崩2', '崩二', '崩崩', '蹦蹦', 'bh2']:
         arg = ('bh2', '崩坏2')
     elif arg in ['崩坏：星穹铁道', '星铁', '星穹铁道', '铁道', '轨子', '星穹', 'xq']:
@@ -301,15 +326,20 @@
         await get_good_image.reject('⚠️您的输入有误，请重新输入')
 
     img_path = time.strftime(
         f'{_conf.good_list_image_config.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
     if os.path.exists(img_path):
         with open(img_path, 'rb') as f:
             image_bytes = io.BytesIO(f.read())
-        await get_good_image.finish(MessageSegment.image(image_bytes))
+        message_segment = None
+        if isinstance(event, OnebotV11MessageEvent):
+            message_segment = OnebotV11MessageSegment.image(image_bytes)
+        elif isinstance(event, QQGuildMessageEvent):
+            message_segment = QQGuildMessageSegment.file_image(image_bytes)
+        await get_good_image.finish(message_segment)
     else:
         await get_good_image.finish(
             f'{arg[1]} 分区暂时没有可兑换的限时商品。如果这与实际不符，你可以尝试用『{COMMAND_BEGIN}商品 更新』进行更新。')
 
 
 lock = threading.Lock()
 finished: Dict[ExchangePlan, List[bool]] = {}
@@ -317,15 +347,14 @@
 
 @lambda func: scheduler.add_listener(func, EVENT_JOB_EXECUTED)
 def exchange_notice(event: JobExecutionEvent):
     """
     接收兑换结果
     """
     if event.job_id.startswith("exchange-plan"):
-        bot = get_bot()
         loop = asyncio.get_event_loop()
 
         thread_id = int(event.job_id.split('-')[-1]) + 1
         result: Tuple[ExchangeStatus, Optional[ExchangeResult]] = event.retval
         exchange_status, exchange_result = result
 
         if not exchange_status:
@@ -333,15 +362,15 @@
             plans = map(lambda x: x.exchange_plans, _conf.users.values())
             plan_filter = filter(lambda x: hash(x[0]) == hash_value, zip(plans, _conf.users.keys()))
             plan_tuple = next(plan_filter)
             plan, user_id = plan_tuple
             with lock:
                 finished[plan].append(False)
                 loop.create_task(
-                    bot.send_private_msg(
+                    send_private_msg(
                         user_id=user_id,
                         message=f"⚠️账户 {plan.account.bbs_uid}"
                                 f"\n- {plan.good.general_name}"
                                 f"\n- 线程 {thread_id}"
                                 f"\n- 兑换请求发送失败"
                     )
                 )
@@ -355,26 +384,26 @@
             user_id, user = next(user_filter)
             with lock:
                 # 如果已经有一个线程兑换成功，就不再接收结果
                 if True not in finished[plan]:
                     if exchange_result.result:
                         finished[plan].append(True)
                         loop.create_task(
-                            bot.send_private_msg(
+                            send_private_msg(
                                 user_id=user_id,
                                 message=f"🎉账户 {plan.account.bbs_uid}"
                                         f"\n- {plan.good.general_name}"
                                         f"\n- 线程 {thread_id}"
                                         f"\n- 兑换成功"
                             )
                         )
                     else:
                         finished[plan].append(False)
                         loop.create_task(
-                            bot.send_private_msg(
+                            send_private_msg(
                                 user_id=user_id,
                                 message=f"💦账户 {plan.account.bbs_uid}"
                                         f"\n- {plan.good.general_name}"
                                         f"\n- 线程 {thread_id}"
                                         f"\n- 兑换失败"
                             )
                         )
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/game_sign_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/game_sign_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ### 米游社的游戏签到相关API
 """
-from typing import List, Optional, Tuple, Literal, Set, Type, Callable, Any
+from typing import List, Optional, Tuple, Literal, Set, Type, Callable, Any, Coroutine
 from urllib.parse import urlencode
 
 import httpx
 import tenacity
 
 from .data_model import GameRecord, BaseApiStatus, Award, GameSignInfo, GeetestResult
 from .plugin_data import PluginDataManager
@@ -204,15 +204,18 @@
                         logger.debug(f"{_conf.preference.log_head}网络请求返回: {res.text}")
                         gt = api_result.data.get("gt", None)
                         challenge = api_result.data.get("challenge", None)
                         if gt and challenge:
                             geetest_result = await get_validate(gt, challenge)
                             if _conf.preference.geetest_url:
                                 if on_geetest_callback and attempt.retry_state.attempt_number == 1:
-                                    on_geetest_callback()
+                                    if isinstance(on_geetest_callback, Coroutine):
+                                        await on_geetest_callback
+                                    else:
+                                        on_geetest_callback()
                                 continue
                             else:
                                 return BaseApiStatus(need_verify=True)
             return BaseApiStatus(success=True)
 
         except tenacity.RetryError as e:
             if is_incorrect_return(e):
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/good_image.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/help.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 """
 ### 帮助相关
 #### 参考了`nonebot-plugin-help`
 """
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageEvent
-from nonebot.adapters.onebot.v11.message import Message
+from nonebot.adapters.qqguild.exception import ActionFailed as QQGuildActionFailed
+from nonebot.internal.params import ArgStr
 from nonebot.matcher import Matcher
-from nonebot.params import Arg, CommandArg
+from nonebot.params import CommandArg
 
 from .plugin_data import PluginDataManager
-from .utils import PLUGIN, COMMAND_BEGIN
+from .utils import PLUGIN, COMMAND_BEGIN, GeneralMessageEvent, logger
 
 _conf = PluginDataManager.plugin_data
 
-helper = on_command(_conf.preference.command_start + "help",
-                    priority=1,
-                    aliases={_conf.preference.command_start + "帮助"},
-                    block=True)
+helper = on_command(
+    f"{_conf.preference.command_start}帮助",
+    priority=1,
+    aliases={f"{_conf.preference.command_start}help"},
+    block=True
+)
 
 helper.name = '帮助'
-helper.usage = '''\
-    🍺欢迎使用米游社小助手帮助系统！\
-    \n{HEAD}帮助 ➢ 查看米游社小助手使用说明\
-    \n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明\
-'''.strip()
+helper.usage = "🍺欢迎使用米游社小助手帮助系统！" \
+               "\n{HEAD}帮助 ➢ 查看米游社小助手使用说明" \
+               "\n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明"
 
 
 @helper.handle()
-async def _(_: MessageEvent, matcher: Matcher, args: Message = CommandArg()):
+async def _(_: GeneralMessageEvent, matcher: Matcher, args=CommandArg()):
     """
     主命令触发
     """
     # 二级命令
     if args:
         matcher.set_arg("content", args)
     # 只有主命令“帮助”
     else:
-        await matcher.finish(
-            PLUGIN.metadata.name +
-            PLUGIN.metadata.description +
-            "\n具体用法：\n" +
-            PLUGIN.metadata.usage.format(HEAD=COMMAND_BEGIN))
+        try:
+            await matcher.finish(
+                f"{PLUGIN.metadata.name}"
+                f"{PLUGIN.metadata.description}\n"
+                "具体用法：\n"
+                f"{PLUGIN.metadata.usage.format(HEAD=COMMAND_BEGIN)}"
+            )
+        except QQGuildActionFailed as e:
+            if e.code == 304003:
+                logger.exception(f"{_conf.preference.log_head}帮助命令的文本发送失败，原因是频道禁止发送URL")
 
 
 @helper.got('content')
-async def _(_: MessageEvent, content: Message = Arg()):
+async def _(_: GeneralMessageEvent, content=ArgStr()):
     """
     二级命令触发。功能详细说明查询
     """
-    arg = content.extract_plain_text().strip()
-
     # 相似词
-    if arg == '登陆':
-        arg = '登录'
+    if content == '登陆':
+        content = '登录'
 
     matchers = PLUGIN.matcher
     for matcher in matchers:
         try:
-            if arg.lower() == matcher.name:
+            if content.lower() == matcher.name:
                 await helper.finish(
-                    f"『{COMMAND_BEGIN}{matcher.name}』- 使用说明\n{matcher.usage.format(HEAD=COMMAND_BEGIN)}")
+                    f"『{COMMAND_BEGIN}{matcher.name}』- 使用说明\n{matcher.usage}")
         except AttributeError:
             continue
     await helper.finish("⚠️未查询到相关功能，请重新尝试")
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 """
 ### 米游社登录获取Cookie相关
 """
 import json
-from typing import Union
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import PrivateMessageEvent, GroupMessageEvent, Message
+from nonebot.adapters.qqguild import MessageEvent as QQGuildMessageEvent, \
+    MessageSegment as QQGuildMessageSegment, DirectMessageCreateEvent
 from nonebot.internal.matcher import Matcher
-from nonebot.internal.params import Arg
+from nonebot.internal.params import ArgStr
 from nonebot.params import ArgPlainText, T_State
 
 from .plugin_data import PluginDataManager, write_plugin_data
 from .simple_api import get_login_ticket_by_captcha, get_multi_token_by_login_ticket, get_stoken_v2_by_v1, \
     get_ltoken_by_stoken, get_cookie_token_by_stoken, get_device_fp
 from .user_data import UserAccount, UserData
-from .utils import logger, COMMAND_BEGIN
+from .utils import logger, COMMAND_BEGIN, GeneralMessageEvent, GeneralPrivateMessageEvent, GeneralGroupMessageEvent, \
+    generate_qr_img
 
 _conf = PluginDataManager.plugin_data
 
 get_cookie = on_command(_conf.preference.command_start + '登录', priority=4, block=True)
 get_cookie.name = '登录'
 get_cookie.usage = '跟随指引，通过电话获取短信方式绑定米游社账户，配置完成后会自动开启签到、米游币任务，后续可制定米游币自动兑换计划。'
 
 
 @get_cookie.handle()
-async def handle_first_receive(event: Union[GroupMessageEvent, PrivateMessageEvent]):
-    if isinstance(event, GroupMessageEvent):
-        await get_cookie.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行登录。")
+async def handle_first_receive(event: GeneralMessageEvent):
+    if isinstance(event, GeneralGroupMessageEvent):
+        await get_cookie.finish("⚠️为了保护您的隐私，请私聊进行登录。")
     user_num = len(_conf.users)
     if user_num < _conf.preference.max_user or _conf.preference.max_user in [-1, 0]:
-        await get_cookie.send("""\
-        登录过程概览：\
-        \n1.发送手机号\
-        \n2.前往 https://user.mihoyo.com/#/login/captcha，输入手机号并获取验证码（网页上不要登录）\
-        \n3.发送验证码给QQ机器人，完成登录\
-        \n🚪过程中发送“退出”即可退出\
-            """.strip())
+        # QQ频道可能无法发送链接，需要发送二维码
+        login_url = "https://user.mihoyo.com/#/login/captcha"
+        msg = "登录过程概览：\n" \
+              "1.发送手机号\n" \
+              "2.扫描二维码，进入米哈游官方登录页，输入手机号并获取验证码（网页上不要登录）\n" \
+            if isinstance(event, QQGuildMessageEvent) else \
+            f"2.前往 {login_url}，输入手机号并获取验证码（网页上不要登录）\n" \
+            "3.发送验证码给QQ机器人，完成登录\n" \
+            "🚪过程中发送“退出”即可退出"
+        if isinstance(event, QQGuildMessageEvent):
+            msg += QQGuildMessageSegment.file_image(generate_qr_img(login_url))
+        await get_cookie.send(msg)
     else:
         await get_cookie.finish('⚠️目前可支持使用用户数已经满啦~')
 
 
 @get_cookie.got('phone', prompt='1.请发送您的手机号：')
-async def _(_: PrivateMessageEvent, state: T_State, phone: str = ArgPlainText('phone')):
+async def _(_: GeneralPrivateMessageEvent, state: T_State, phone: str = ArgPlainText('phone')):
     if phone == '退出':
         await get_cookie.finish("🚪已成功退出")
     if not phone.isdigit():
         await get_cookie.reject("⚠️手机号应为数字，请重新输入")
     if len(phone) != 11:
         await get_cookie.reject("⚠️手机号应为11位数字，请重新输入")
     else:
         state['phone'] = phone
 
 
 @get_cookie.handle()
-async def _(_: PrivateMessageEvent):
+async def _(_: GeneralPrivateMessageEvent):
     await get_cookie.send('2.前往 https://user.mihoyo.com/#/login/captcha，获取验证码（不要登录！）')
 
 
 @get_cookie.got("captcha", prompt='3.请发送验证码：')
-async def _(event: PrivateMessageEvent, state: T_State, captcha: str = ArgPlainText('captcha')):
+async def _(event: GeneralPrivateMessageEvent, state: T_State, captcha: str = ArgPlainText('captcha')):
     phone_number: str = state['phone']
     if captcha == '退出':
         await get_cookie.finish("🚪已成功退出")
     if not captcha.isdigit():
         await get_cookie.reject("⚠️验证码应为数字，请重新输入")
     else:
-        _conf.users.setdefault(event.user_id, UserData())
-        user = _conf.users[event.user_id]
+        user_id = event.get_user_id()
+        _conf.users.setdefault(user_id, UserData())
+        user = _conf.users[user_id]
+        # 如果是QQ频道，需要记录频道ID
+        if isinstance(event, DirectMessageCreateEvent):
+            user.qq_guilds.setdefault(user_id, set())
+            user.qq_guilds[user_id].add(event.channel_id)
         # 1. 通过短信验证码获取 login_ticket / 使用已有 login_ticket
         login_status, cookies = await get_login_ticket_by_captcha(phone_number, int(captcha))
         if login_status:
             # logger.info(f"用户 {phone_number} 成功获取 login_ticket: {cookies.login_ticket}")
-            account = _conf.users[event.user_id].accounts.get(cookies.bbs_uid)
+            account = _conf.users[user_id].accounts.get(cookies.bbs_uid)
             """当前的账户数据对象"""
             if not account or not account.cookies:
                 user.accounts.update({
                     cookies.bbs_uid: UserAccount(phone_number=phone_number, cookies=cookies)
                 })
                 account = user.accounts[cookies.bbs_uid]
             else:
@@ -155,40 +166,38 @@
              _conf.preference.command_start + '导出cookie', _conf.preference.command_start + '导出cookies'}, priority=4,
     block=True)
 output_cookies.name = '导出Cookies'
 output_cookies.usage = '导出绑定的米游社账号的Cookies数据'
 
 
 @output_cookies.handle()
-async def handle_first_receive(event: Union[GroupMessageEvent, PrivateMessageEvent], matcher: Matcher):
+async def handle_first_receive(event: GeneralMessageEvent, state: T_State):
     """
     Cookies导出命令触发
     """
-    if isinstance(event, GroupMessageEvent):
-        await output_cookies.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行Cookies导出。")
-    user_account = _conf.users[event.user_id].accounts
+    if isinstance(event, GeneralGroupMessageEvent):
+        await output_cookies.finish("⚠️为了保护您的隐私，请私聊进行Cookies导出。")
+    user_account = _conf.users[event.get_user_id()].accounts
     if not user_account:
         await output_cookies.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     elif len(user_account) == 1:
         account = next(iter(user_account.values()))
-        matcher.set_arg('bbs_uid', Message(account.bbs_uid))
+        state["bbs_uid"] = account.bbs_uid
     else:
         msg = "您有多个账号，您要导出哪个账号的Cookies数据？\n"
         msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
         msg += "\n🚪发送“退出”即可退出"
         await output_cookies.send(msg)
 
 
 @output_cookies.got('bbs_uid')
-async def _(event: PrivateMessageEvent, matcher: Matcher, uid=Arg("bbs_uid")):
+async def _(event: GeneralPrivateMessageEvent, matcher: Matcher, state: T_State, bbs_uid=ArgStr()):
     """
     根据手机号设置导出相应的账户的Cookies
     """
-    if isinstance(uid, Message):
-        uid = uid.extract_plain_text().strip()
-    if uid == '退出':
+    if bbs_uid == '退出':
         await matcher.finish('🚪已成功退出')
-    user_account = _conf.users[event.user_id].accounts
-    if uid in user_account:
-        await output_cookies.finish(json.dumps(user_account[uid].cookies.dict(cookie_type=True), indent=4))
+    user_account = _conf.users[event.get_user_id()].accounts
+    if bbs_uid in user_account:
+        await output_cookies.finish(json.dumps(user_account[bbs_uid].cookies.dict(cookie_type=True), indent=4))
     else:
         await matcher.reject('⚠️您输入的账号不在以上账号内，请重新输入')
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/myb_missions_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/myb_missions_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plan.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 """
 ### 计划任务相关
 """
 import asyncio
 import random
 import threading
-from typing import Union
 
-from nonebot import get_bot, on_command
-from nonebot.adapters.onebot.v11 import (Bot, MessageSegment,
-                                         PrivateMessageEvent, GroupMessageEvent)
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import (MessageSegment)
+from nonebot.internal.matcher import Matcher
 from nonebot_plugin_apscheduler import scheduler
 
 from .exchange import generate_image
 from .game_sign_api import BaseGameSign
 from .myb_missions_api import BaseMission, get_missions_state
 from .plugin_data import PluginDataManager, write_plugin_data
 from .simple_api import genshin_board, get_game_record, StarRail_board
-from .utils import get_file, logger, COMMAND_BEGIN
+from .utils import get_file, logger, COMMAND_BEGIN, GeneralMessageEvent, send_private_msg
 
 _conf = PluginDataManager.plugin_data
 
 manually_game_sign = on_command(_conf.preference.command_start + '签到', priority=5, block=True)
 manually_game_sign.name = '签到'
 manually_game_sign.usage = '手动进行游戏签到，查看本次签到奖励及本月签到天数'
 
 
 @manually_game_sign.handle()
-async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
+async def _(event: GeneralMessageEvent, matcher: Matcher):
     """
     手动游戏签到函数
     """
-    bot = get_bot(str(event.self_id))
-    user = _conf.users.get(event.user_id)
+    user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await manually_game_sign.send("⏳开始游戏签到...")
-    await perform_game_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
+    await perform_game_sign(user_id=event.get_user_id(), matcher=matcher)
 
 
 manually_bbs_sign = on_command(_conf.preference.command_start + '任务', priority=5, block=True)
 manually_bbs_sign.name = '任务'
 manually_bbs_sign.usage = '手动执行米游币每日任务，可以查看米游币任务完成情况'
 
 
 @manually_bbs_sign.handle()
-async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
+async def _(event: GeneralMessageEvent, matcher: Matcher):
     """
     手动米游币任务函数
     """
-    bot = get_bot(str(event.self_id))
-    user = _conf.users.get(event.user_id)
+    user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await manually_game_sign.send("⏳开始执行米游币任务...")
-    await perform_bbs_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
+    await perform_bbs_sign(user_id=event.get_user_id(), matcher=matcher)
 
 
 manually_resin_check = on_command(
     _conf.preference.command_start + '原神便笺',
     aliases={
         _conf.preference.command_start + '便笺',
         _conf.preference.command_start + '便签',
@@ -73,23 +70,22 @@
     for account in user.accounts.values():
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"resin": False, "coin": False, "transformer": False})
 
 
 @manually_resin_check.handle()
-async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
+async def _(event: GeneralMessageEvent, matcher: Matcher):
     """
     手动查看原神便笺
     """
-    bot = get_bot(str(event.self_id))
-    user = _conf.users.get(event.user_id)
+    user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
-    await resin_check(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
+    await resin_check(user_id=event.get_user_id(), matcher=matcher)
 
 
 manually_resin_check_sr = on_command(
     _conf.preference.command_start + '星穹铁道便笺',
     aliases={
         _conf.preference.command_start + '铁道便笺',
         _conf.preference.command_start + '铁道便签',
@@ -104,97 +100,98 @@
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"stamina": False, "train_score": False,
                                                             "rogue_score": False})
 
 
 @manually_resin_check_sr.handle()
-async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
+async def _(event: GeneralMessageEvent, matcher: Matcher):
     """
     手动查看星穹铁道便笺（sr）
     """
-    bot = get_bot(str(event.self_id))
-    user = _conf.users.get(event.user_id)
+    user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
-    await resin_check_sr(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
+    await resin_check_sr(user_id=event.get_user_id(), matcher=matcher)
 
 
-async def perform_game_sign(bot: Bot, qq: int, is_auto: bool,
-                            group_event: Union[GroupMessageEvent, PrivateMessageEvent, None] = None):
+async def perform_game_sign(user_id: str, matcher: Matcher = None):
     """
     执行游戏签到函数，并发送给用户签到消息。
 
-    :param bot: Bot实例
-    :param qq: 用户QQ号
-    :param is_auto: `True`为当日自动签到，`False`为用户手动调用签到功能
-    :param group_event: 若为群消息触发，则为群消息事件，否则为None
+    :param user_id: 用户QQ号
+    :param matcher: 事件响应器
     """
-    if isinstance(group_event, PrivateMessageEvent):
-        group_event = None
     failed_accounts = []
-    user = _conf.users[qq]
-    for account in _conf.users.get(qq).accounts.values():
+    user = _conf.users[user_id]
+    for account in _conf.users.get(user_id).accounts.values():
+        # 自动签到时，要求用户打开了签到功能；手动签到时都可以调用执行。
+        if not matcher and not account.enable_game_sign:
+            continue
         signed = False
         """是否已经完成过签到"""
         game_record_status, records = await get_game_record(account)
         if not game_record_status:
-            if group_event:
-                await bot.send(event=group_event, at_sender=True,
-                               message=f"⚠️账户 {account.bbs_uid} 获取游戏账号信息失败，请重新尝试")
+            if matcher:
+                await matcher.send(f"⚠️账户 {account.bbs_uid} 获取游戏账号信息失败，请重新尝试")
             else:
-                await bot.send_private_msg(user_id=qq,
-                                           message=f"⚠️账户 {account.bbs_uid} 获取游戏账号信息失败，请重新尝试")
+                await send_private_msg(
+                    user_id=user_id,
+                    message=f"⚠️账户 {account.bbs_uid} 获取游戏账号信息失败，请重新尝试"
+                )
             continue
         games_has_record = []
         for class_type in BaseGameSign.AVAILABLE_GAME_SIGNS:
             signer = class_type(account, records)
             if not signer.has_record:
                 continue
             else:
                 games_has_record.append(signer)
             get_info_status, info = await signer.get_info(account.platform)
             if not get_info_status:
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True,
-                                   message=f"⚠️账户 {account.bbs_uid} 获取签到记录失败")
-                else:
-                    await bot.send_private_msg(user_id=qq, message=f"⚠️账户 {account.bbs_uid} 获取签到记录失败")
-
-            # 自动签到时，要求用户打开了签到功能；手动签到时都可以调用执行。若没签到，则进行签到功能。
-            # 若获取今日签到情况失败，仍可继续
-            if ((account.enable_game_sign and is_auto) or not is_auto) and (
-                    (info and not info.is_sign) or not get_info_status):
-                sign_status = await signer.sign(
-                    account.platform,
-                    lambda: bot.send_private_msg(user_id=qq, message=f"⏳正在尝试完成人机验证，请稍后...")
-                )
-                if not sign_status:
+                if matcher:
+                    await matcher.send(f"⚠️账户 {account.bbs_uid} 获取签到记录失败")
+                else:
+                    await send_private_msg(
+                        user_id=user_id,
+                        message=f"⚠️账户 {account.bbs_uid} 获取签到记录失败"
+                    )
+            else:
+                signed = info.is_sign
+
+            # 若没签到，则进行签到功能；若获取今日签到情况失败，仍可继续
+            if (get_info_status and not info.is_sign) or not get_info_status:
+                if matcher:
+                    sign_status = await signer.sign(
+                        account.platform,
+                        lambda: matcher.send(f"⏳正在尝试完成人机验证，请稍后...")
+                    )
+                else:
+                    sign_status = await signer.sign(
+                        account.platform,
+                        lambda: send_private_msg(user_id=user_id, message=f"⏳正在尝试完成人机验证，请稍后...")
+                    )
+                if not sign_status and (user.enable_notice or matcher):
                     if sign_status.login_expired:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时服务器返回登录失效，请尝试重新登录绑定账户"
                     elif sign_status.need_verify:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时可能遇到验证码拦截，请尝试使用命令『/账号设置』更改设备平台，若仍失败请手动前往米游社签到"
                     else:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到失败，请稍后再试"
-                    if user.enable_notice or not is_auto:
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True, message=message)
-                        else:
-                            await bot.send_msg(message_type="private", user_id=qq, message=message)
+                    if matcher:
+                        await matcher.send(message)
+                    elif user.enable_notice:
+                        await send_private_msg(user_id=user_id, message=message)
                     await asyncio.sleep(_conf.preference.sleep_time)
                     continue
+
                 await asyncio.sleep(_conf.preference.sleep_time)
-            # 若用户未开启自动签到且手动签到过了，不再提醒
-            elif not account.enable_game_sign and is_auto:
-                continue
-            else:
-                signed = True
 
             # 用户打开通知或手动签到时，进行通知
-            if user.enable_notice or not is_auto:
+            if user.enable_notice or matcher:
                 img = ""
                 get_info_status, info = await signer.get_info(account.platform)
                 get_award_status, awards = await signer.get_rewards()
                 if not get_info_status or not get_award_status:
                     msg = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』获取签到结果失败！请手动前往米游社查看"
                 else:
                     award = awards[info.total_sign_day - 1]
@@ -207,213 +204,164 @@
                               "\n\n🎁今日签到奖励：" \
                               f"\n{award.name} * {award.cnt}" \
                               f"\n\n📅本月签到次数：{info.total_sign_day}"
                         img_file = await get_file(award.icon)
                         img = MessageSegment.image(img_file)
                     else:
                         msg = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到失败！请尝试重新签到，若多次失败请尝试重新登录绑定账户"
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True, message=msg + img)
+                if matcher:
+                    await matcher.send(msg + img)
                 else:
-                    await bot.send_msg(message_type="private", user_id=qq, message=msg + img)
+                    await send_private_msg(user_id=user_id, message=msg + img)
             await asyncio.sleep(_conf.preference.sleep_time)
 
         if not games_has_record:
-            if group_event:
-                await bot.send(
-                    event=group_event,
-                    at_sender=True,
-                    message=f"⚠️您的米游社账户 {account.bbs_uid} 下不存在任何游戏账号，已跳过签到"
-                )
+            if matcher:
+                await matcher.send(f"⚠️您的米游社账户 {account.bbs_uid} 下不存在任何游戏账号，已跳过签到")
             else:
-                await bot.send_msg(
-                    message_type="private",
-                    user_id=qq,
-                    message=f"⚠️您的米游社账户 {account.bbs_uid} 下不存在任何游戏账号，已跳过签到"
-                )
+                await send_private_msg(user_id=user_id,
+                                       message=f"⚠️您的米游社账户 {account.bbs_uid} 下不存在任何游戏账号，已跳过签到")
 
     # 如果全部登录失效，则关闭通知
     if len(failed_accounts) == len(user.accounts):
         user.enable_notice = False
         write_plugin_data()
 
 
-async def perform_bbs_sign(bot: Bot, qq: int, is_auto: bool,
-                           group_event: Union[GroupMessageEvent, PrivateMessageEvent, None] = None):
+async def perform_bbs_sign(user_id: str, matcher: Matcher = None):
     """
     执行米游币任务函数，并发送给用户任务执行消息。
 
-    :param bot: Bot实例
-    :param qq: 用户QQ号
-    :param is_auto: True为当日自动执行任务，False为用户手动调用任务功能
-    :param group_event: 若为群消息触发，则为群消息事件，否则为None
+    :param user_id: 用户QQ号
+    :param matcher: 事件响应器
     """
-    if isinstance(group_event, PrivateMessageEvent):
-        group_event = None
     failed_accounts = []
-    user = _conf.users[qq]
+    user = _conf.users[user_id]
     for account in user.accounts.values():
+        # 自动执行米游币任务时，要求用户打开了米游币任务功能；手动执行米游币任务时都可以调用执行。
+        if not matcher and not account.enable_mission:
+            continue
         for class_type in account.mission_games:
             mission_obj = class_type(account)
             missions_state_status, missions_state = await get_missions_state(account)
             if not missions_state_status:
                 if missions_state_status.login_expired:
-                    if group_event:
-                        await bot.send(event=group_event, at_sender=True,
-                                       message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                     else:
-                        await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
+                        await send_private_msg(user_id=user_id, message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                     continue
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True,
-                                   message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
+                if matcher:
+                    await matcher.send(f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
                 else:
-                    await bot.send_private_msg(user_id=qq,
-                                               message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
+                    await send_private_msg(user_id=user_id,
+                                           message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
                 continue
 
             myb_before_mission = missions_state.current_myb
 
-            # 自动执行米游币任务时，要求用户打开了任务功能；手动执行时都可以调用执行。
-            if (account.enable_mission and is_auto) or not is_auto:
-                if not is_auto:
-                    if not group_event:
-                        await bot.send_private_msg(user_id=qq,
-                                                   message=f'🆔账户 {account.bbs_uid} ⏳开始在分区『{class_type.NAME}』执行米游币任务...')
+            if matcher:
+                await matcher.send(f'🆔账户 {account.bbs_uid} ⏳开始在分区『{class_type.NAME}』执行米游币任务...')
 
-                # 执行任务
-                for key_name, (mission, current) in missions_state.state_dict.items():
-                    if current < mission.threshold:
-                        if key_name == BaseMission.SIGN:
-                            await mission_obj.sign()
-                        elif key_name == BaseMission.VIEW:
-                            await mission_obj.read()
-                        elif key_name == BaseMission.LIKE:
-                            await mission_obj.like()
-                        elif key_name == BaseMission.SHARE:
-                            await mission_obj.share()
-
-                # 用户打开通知或手动任务时，进行通知
-                if user.enable_notice or not is_auto:
-                    missions_state_status, missions_state = await get_missions_state(account)
-                    if not missions_state_status:
-                        if missions_state_status.login_expired:
-                            if group_event:
-                                await bot.send(event=group_event, at_sender=True,
-                                               message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
-                            else:
-                                await bot.send_private_msg(user_id=qq,
-                                                           message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
-                            continue
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True,
-                                           message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
+            # 执行任务
+            for key_name, (mission, current) in missions_state.state_dict.items():
+                if current < mission.threshold:
+                    if key_name == BaseMission.SIGN:
+                        await mission_obj.sign()
+                    elif key_name == BaseMission.VIEW:
+                        await mission_obj.read()
+                    elif key_name == BaseMission.LIKE:
+                        await mission_obj.like()
+                    elif key_name == BaseMission.SHARE:
+                        await mission_obj.share()
+
+            # 用户打开通知或手动任务时，进行通知
+            if user.enable_notice or matcher:
+                missions_state_status, missions_state = await get_missions_state(account)
+                if not missions_state_status:
+                    if missions_state_status.login_expired:
+                        if matcher:
+                            await matcher.send(f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                         else:
-                            await bot.send_private_msg(user_id=qq,
-                                                       message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
+                            await send_private_msg(user_id=user_id,
+                                                   message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                         continue
-                    if all(map(lambda x: x[1] >= x[0].threshold, missions_state.state_dict.values())):
-                        notice_string = f"🎉已完成今日米游币任务 - 分区『{class_type.NAME}』"
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
                     else:
-                        notice_string = f"⚠️今日米游币任务未全部完成 - 分区『{class_type.NAME}』"
+                        await send_private_msg(user_id=user_id,
+                                               message=f'⚠️账户 {account.bbs_uid} 获取任务完成情况请求失败，你可以手动前往App查看')
+                    continue
+                if all(map(lambda x: x[1] >= x[0].threshold, missions_state.state_dict.values())):
+                    notice_string = f"🎉已完成今日米游币任务 - 分区『{class_type.NAME}』"
+                else:
+                    notice_string = f"⚠️今日米游币任务未全部完成 - 分区『{class_type.NAME}』"
 
-                    msg = f"{notice_string}" \
-                          f"\n🆔账户 {account.bbs_uid}"
-                    for key_name, (mission, current) in missions_state.state_dict.items():
-                        if key_name == BaseMission.SIGN:
-                            mission_name = "签到"
-                        elif key_name == BaseMission.VIEW:
-                            mission_name = "阅读"
-                        elif key_name == BaseMission.LIKE:
-                            mission_name = "点赞"
-                        elif key_name == BaseMission.SHARE:
-                            mission_name = "转发"
-                        else:
-                            mission_name = mission.mission_key
-                        msg += f"\n- {mission_name} {'✓' if current >= mission.threshold else '✕'}"
-                    msg += f"\n💰获得米游币: {missions_state.current_myb - myb_before_mission}"
-                    msg += f"\n💰当前米游币: {missions_state.current_myb}"
-                    msg.strip()
-
-                    if group_event:
-                        await bot.send(event=group_event, at_sender=True, message=msg)
-                    else:
-                        await bot.send_msg(
-                            message_type="private",
-                            user_id=qq,
-                            message=msg
-                        )
+                msg = f"{notice_string}" \
+                      f"\n🆔账户 {account.bbs_uid}"
+                for key_name, (mission, current) in missions_state.state_dict.items():
+                    if key_name == BaseMission.SIGN:
+                        mission_name = "签到"
+                    elif key_name == BaseMission.VIEW:
+                        mission_name = "阅读"
+                    elif key_name == BaseMission.LIKE:
+                        mission_name = "点赞"
+                    elif key_name == BaseMission.SHARE:
+                        mission_name = "转发"
+                    else:
+                        mission_name = mission.mission_key
+                    msg += f"\n- {mission_name} {'✓' if current >= mission.threshold else '✕'}"
+                msg += f"\n💰获得米游币: {missions_state.current_myb - myb_before_mission}" \
+                       f"\n💰当前米游币: {missions_state.current_myb}"
+
+                if matcher:
+                    await matcher.send(msg)
+                else:
+                    await send_private_msg(user_id=user_id, message=msg)
 
     # 如果全部登录失效，则关闭通知
     if len(failed_accounts) == len(user.accounts):
         user.enable_notice = False
         write_plugin_data()
 
 
-async def resin_check(bot: Bot, qq: int, is_auto: bool,
-                      group_event: Union[GroupMessageEvent, PrivateMessageEvent, None] = None):
+async def resin_check(user_id: str, matcher: Matcher = None):
     """
     查看原神实时便笺函数，并发送给用户任务执行消息。
 
-    :param bot: Bot实例
-    :param qq: 用户QQ号
-    :param is_auto: True为自动检查，False为用户手动调用该功能
-    :param group_event: 若为群消息触发，则为群消息事件，否则为None
+    :param user_id: 用户QQ号
+    :param matcher: 事件响应器
     """
-    if isinstance(group_event, PrivateMessageEvent):
-        group_event = None
     global has_checked
-    user = _conf.users[qq]
+    user = _conf.users[user_id]
     for account in user.accounts.values():
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"resin": False, "coin": False, "transformer": False})
-        if (account.enable_resin and is_auto) or not is_auto:
+        if account.enable_resin or matcher:
             genshin_board_status, board = await genshin_board(account)
-            logger.info(genshin_board_status)
             if not genshin_board_status:
                 if genshin_board_status.login_expired:
-                    if not is_auto:
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True,
-                                           message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
-                        else:
-                            await bot.send_private_msg(user_id=qq,
-                                                       message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                 if genshin_board_status.no_genshin_account:
-                    if not is_auto:
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True,
-                                           message=f'⚠️账户 {account.bbs_uid} 没有绑定任何原神账户，请绑定后再重试')
-                        else:
-                            await bot.send_private_msg(user_id=qq,
-                                                       message=f'⚠️账户 {account.bbs_uid} 没有绑定任何原神账户，请绑定后再重试')
-                        account.enable_resin = False
-                        write_plugin_data()
-                        continue
-                if not is_auto:
-                    if group_event:
-                        await bot.send(event=group_event, at_sender=True,
-                                       message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
-                    else:
-                        await bot.send_private_msg(user_id=qq,
-                                                   message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 没有绑定任何原神账户，请绑定后再重试')
+                    account.enable_resin = False
+                    write_plugin_data()
+                    continue
+                if matcher:
+                    await matcher.send(f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
             if genshin_board_status.need_verify:
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True,
-                                   message=f'⚠️遇到验证码正在尝试绕过')
-                else:
-                    await bot.send_private_msg(user_id=qq,
-                                               message=f'⚠️遇到验证码正在尝试绕过')
+                if matcher:
+                    await matcher.send(f'⚠️遇到验证码正在尝试绕过')
             msg = ''
             # 手动查询体力时，无需判断是否溢出
-            if not is_auto:
-                pass
-            else:
+            if not matcher:
                 # 体力溢出提醒
                 if board.current_resin == 160:
                     # 防止重复提醒
                     if has_checked[account.bbs_uid]['resin']:
                         return
                     else:
                         has_checked[account.bbs_uid]['resin'] = True
@@ -442,86 +390,63 @@
                     else:
                         has_checked[account.bbs_uid]['transformer'] = False
                         return
                 else:
                     has_checked[account.bbs_uid]['transformer'] = True
             msg += "❖实时便笺❖" \
                    f"\n⏳树脂数量：{board.current_resin} / 160" \
+                   f"\n⏱️树脂{board.resin_recovery_text}" \
                    f"\n🕰️探索派遣：{board.current_expedition_num} / {board.max_expedition_num}" \
                    f"\n📅每日委托：{4 - board.finished_task_num} 个任务未完成" \
                    f"\n💰洞天财瓮：{board.current_home_coin} / {board.max_home_coin}" \
                    f"\n🎰参量质变仪：{board.transformer_text if board.transformer else 'N/A'}"
-            if group_event:
-                await bot.send(event=group_event, at_sender=True, message=msg)
+            if matcher:
+                await matcher.send(msg)
             else:
-                await bot.send_private_msg(user_id=qq, message=msg)
+                if board.current_resin >= account.user_resin_threshold:
+                    await send_private_msg(user_id=user_id, message=msg)
+                else:
+                    logger.info(f"原神实时便笺：账户 {account.bbs_uid} 树脂:{board.current_resin},未满足推送条件")
 
 
-async def resin_check_sr(bot: Bot, qq: int, is_auto: bool,
-                         group_event: Union[GroupMessageEvent, PrivateMessageEvent, None] = None):
+async def resin_check_sr(user_id: str, matcher: Matcher = None):
     """
     查看星铁实时便笺函数，并发送给用户任务执行消息。
 
-    :param bot: Bot实例
-    :param qq: 用户QQ号
-    :param is_auto: True为自动检查，False为用户手动调用该功能
-    :param group_event: 若为群消息触发，则为群消息事件，否则为None
+    :param user_id: 用户QQ号
+    :param matcher: 事件响应器
     """
-    if isinstance(group_event, PrivateMessageEvent):
-        group_event = None
     global has_checked
-    user = _conf.users[qq]
+    user = _conf.users[user_id]
     for account in user.accounts.values():
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"stamina": False, "train_score": False,
                                                             "rogue_score": False})
-        if (account.enable_resin and is_auto) or not is_auto:
+        if account.enable_resin or matcher:
             starrail_board_status, board = await StarRail_board(account)
-            logger.info(starrail_board_status)
             if not starrail_board_status:
                 if starrail_board_status.login_expired:
-                    if not is_auto:
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True,
-                                           message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
-                        else:
-                            await bot.send_private_msg(user_id=qq,
-                                                       message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                 if starrail_board_status.no_starrail_account:
-                    if not is_auto:
-                        if group_event:
-                            await bot.send(event=group_event, at_sender=True,
-                                           message=f'⚠️账户 {account.bbs_uid} 没有绑定任何星铁账户，请绑定后再重试')
-                        else:
-                            await bot.send_private_msg(user_id=qq,
-                                                       message=f'⚠️账户 {account.bbs_uid} 没有绑定任何星铁账户，请绑定后再重试')
-                        account.enable_resin = False
-                        write_plugin_data()
-                        continue
-                if not is_auto:
-                    if group_event:
-                        await bot.send(event=group_event, at_sender=True,
-                                       message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
-                    else:
-                        await bot.send_private_msg(user_id=qq,
-                                                   message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
+                    if matcher:
+                        await matcher.send(f'⚠️账户 {account.bbs_uid} 没有绑定任何星铁账户，请绑定后再重试')
+                    account.enable_resin = False
+                    write_plugin_data()
+                    continue
+                if matcher:
+                    await matcher.send(f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
             if starrail_board_status.need_verify:
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True,
-                                   message='⚠️遇到验证码正在尝试绕过')
-                else:
-                    await bot.send_private_msg(user_id=qq,
-                                               message='⚠️遇到验证码正在尝试绕过')
+                if matcher:
+                    await matcher.send(f'⚠️遇到验证码正在尝试绕过')
             msg = ''
             # 手动查询体力时，无需判断是否溢出
-            if not is_auto:
-                pass
-            else:
+            if not matcher:
                 # 体力溢出提醒
                 if board.current_stamina == 180:
                     # 防止重复提醒
                     if has_checked[account.bbs_uid]['stamina']:
                         return
                     else:
                         has_checked[account.bbs_uid]['stamina'] = True
@@ -547,30 +472,24 @@
                         has_checked[account.bbs_uid]['rogue_score'] = True
                         msg += '❕您的模拟宇宙积分已经打满了\n\n'
                 else:
                     has_checked[account.bbs_uid]['rogue_score'] = False
                     return
             msg += "❖星穹铁道实时便笺❖" \
                    f"\n⏳开拓力数量：{board.current_stamina} / 180" \
-                   f"\n⏱开拓力将在{board.stamina_recover_text}回满" \
+                   f"\n⏱开拓力{board.stamina_recover_text}" \
                    f"\n📒每日实训：{board.current_train_score} / {board.max_train_score}" \
                    f"\n📅每日委托：{board.accepted_expedition_num} / 4" \
                    f"\n🌌模拟宇宙：{board.current_rogue_score} / {board.max_rogue_score}"
-            if not is_auto:
-                if group_event:
-                    await bot.send(event=group_event, at_sender=True, message=msg)
-                else:
-                    await bot.send_private_msg(user_id=qq, message=msg)
+
+            if matcher:
+                await matcher.send(msg)
             else:
                 if board.current_stamina >= account.user_stamina_threshold:
-
-                    if group_event:
-                        await bot.send(event=group_event, at_sender=True, message=msg)
-                    else:
-                        await bot.send_private_msg(user_id=qq, message=msg)
+                    await send_private_msg(user_id=user_id, message=msg)
                 else:
                     logger.info(f"崩铁实时便笺：账户 {account.bbs_uid} 开拓力:{board.current_stamina},未满足推送条件")
 
 
 @scheduler.scheduled_job("cron", hour='0', minute='0', id="daily_goodImg_update")
 def daily_update():
     """
@@ -587,25 +506,23 @@
 async def daily_schedule():
     """
     自动米游币任务、游戏签到函数
     """
     # 随机延迟
     await asyncio.sleep(random.randint(0, 59))
     logger.info(f"{_conf.preference.log_head}开始执行每日自动任务")
-    bot = get_bot()
     for qq in _conf.users:
-        await perform_bbs_sign(bot=bot, qq=qq, is_auto=True)
-        await perform_game_sign(bot=bot, qq=qq, is_auto=True)
+        await perform_bbs_sign(user_id=qq)
+        await perform_game_sign(user_id=qq)
     logger.info(f"{_conf.preference.log_head}每日自动任务执行完成")
 
 
 @scheduler.scheduled_job("interval",
                          minutes=_conf.preference.resin_interval,
                          id="resin_check")
 async def auto_resin_check():
     """
     自动查看实时便笺
     """
-    bot = get_bot()
     for qq in _conf.users:
-        await resin_check(bot=bot, qq=qq, is_auto=True)
-        await resin_check_sr(bot=bot, qq=qq, is_auto=True)
+        await resin_check(user_id=qq)
+        await resin_check_sr(user_id=qq)
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/plugin_data.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plugin_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from pathlib import Path
 from typing import Union, Optional, Tuple, Any, Dict, TYPE_CHECKING, AbstractSet, \
     Mapping
 
 from loguru import logger
 from pydantic import BaseModel, ValidationError, BaseSettings, validator, Extra
 
+from . import user_data
 from .user_data import UserData, UserAccount
 
-VERSION = "v1.1.0"
+VERSION = "v1.2.0-beta.1"
 """程序当前版本"""
 
 ROOT_PATH = Path(__name__).parent.absolute()
 '''NoneBot2 机器人根目录'''
 
 DATA_PATH = ROOT_PATH / "data" / "nonebot-plugin-mystool"
 '''插件数据保存目录'''
@@ -219,40 +220,86 @@
     """偏好设置"""
     salt_config: SaltConfig = SaltConfig()
     """生成Headers - DS所用salt值"""
     device_config: DeviceConfig = DeviceConfig()
     """设备信息"""
     good_list_image_config: GoodListImageConfig = GoodListImageConfig()
     """商品列表输出图片设置"""
-    users: Dict[int, UserData] = {}
+    user_bind: Optional[Dict[str, str]] = {}
+    '''不同NoneBot适配器平台的用户数据绑定关系（如QQ聊天和QQ频道）'''
+    users: Dict[str, UserData] = {}
     '''所有用户数据'''
 
+    def do_user_bind(self, src: str = None, dst: str = None, write: bool = False):
+        """
+        执行用户数据绑定同步，将src指向dst的用户数据，即src处的数据将会被dst处的数据对象替换
+
+        :param src: 源用户数据，为空则读取 self.user_bind 并执行全部绑定
+        :param dst: 目标用户数据，为空则读取 self.user_bind 并执行全部绑定
+        :param write: 是否写入插件数据文件
+        :return: 执行是否成功
+        """
+        if None in [src, dst]:
+            for src, dst in self.user_bind.items():
+                try:
+                    self.users[src] = self.users[dst]
+                except KeyError:
+                    logger.error(f"用户数据绑定失败，目标用户 {dst} 不存在")
+                    return False
+                else:
+                    return True
+        else:
+            try:
+                self.user_bind[src] = dst
+                self.users[src] = self.users[dst]
+            except KeyError:
+                logger.error(f"用户数据绑定失败，目标用户 {dst} 不存在")
+                return False
+            else:
+                if write:
+                    write_plugin_data()
+                return True
+
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+        self.do_user_bind(write=True)
+
     class Config:
         json_encoders = UserAccount.Config.json_encoders
 
 
 class PluginDataManager:
     plugin_data = PluginData()
-    device_config = DeviceConfig()
     """加载出的插件数据对象"""
+    device_config: DeviceConfig
+    """加载出的设备信息数据对象"""
 
     @classmethod
     def load_plugin_data(cls):
         """
         加载插件数据文件
         """
         if os.path.exists(PLUGIN_DATA_PATH) and os.path.isfile(PLUGIN_DATA_PATH):
             try:
                 with open(PLUGIN_DATA_PATH, "r") as f:
-                    device_config_dict = json.load(f)["device_config"]
-                device_config_from_file = DeviceConfig.parse_obj(device_config_dict)
-                for attr in device_config_from_file.__fields__:
-                    cls.device_config.__setattr__(attr, device_config_from_file.__getattribute__(attr))
+                    plugin_data_dict = json.load(f)
+                    override_device_and_salt = plugin_data_dict["preference"].get("override_device_and_salt")
+                    # 读取 preference.override_device_and_salt 时，如果没有该配置，则默认为 False
+                    override_device_and_salt = override_device_and_salt \
+                        if override_device_and_salt is not None else False
+                    device_config_dict = plugin_data_dict["device_config"]
+
+                # 先读取设备信息配置，因为之后导入其他代码时部分变量如Headers将会使用到，一旦完成导入，再修改设备信息配置将不会生效
+                if override_device_and_salt:
+                    cls.device_config = DeviceConfig.parse_obj(device_config_dict)
+                else:
+                    cls.device_config = DeviceConfig()
 
-                plugin_data_from_file = PluginData.parse_file(PLUGIN_DATA_PATH)
+                # 读取完整的插件数据
+                plugin_data_from_file = PluginData.parse_obj(plugin_data_dict)
                 for attr in plugin_data_from_file.__fields__:
                     cls.plugin_data.__setattr__(attr, plugin_data_from_file.__getattribute__(attr))
             except (ValidationError, JSONDecodeError):
                 logger.exception(f"读取插件数据文件失败，请检查插件数据文件 {PLUGIN_DATA_PATH} 格式是否正确")
                 raise
             except:
                 logger.exception(
@@ -279,26 +326,31 @@
                     f.write(str_data)
             except (AttributeError, TypeError, ValueError, PermissionError):
                 logger.exception(f"创建插件数据文件失败，请检查是否有权限读取和写入 {PLUGIN_DATA_PATH}")
                 raise
             logger.info(f"插件数据文件 {PLUGIN_DATA_PATH} 不存在，已创建默认插件数据文件。")
 
 
-PluginDataManager.load_plugin_data()
-
-
 def write_plugin_data(data: PluginData = None):
     """
     写入插件数据文件
 
     :param data: 配置对象
+    :return: 是否成功
     """
     if data is None:
         data = PluginDataManager.plugin_data
     try:
         str_data = data.json(indent=4)
     except (AttributeError, TypeError, ValueError):
         logger.exception("数据对象序列化失败，可能是数据类型错误")
         return False
     with open(PLUGIN_DATA_PATH, "w", encoding="utf-8") as f:
         f.write(str_data)
     return True
+
+
+PluginDataManager.load_plugin_data()
+
+# 如果插件数据文件加载后，发现有用户没有UUID密钥，进行了生成，则需要保存写入
+if user_data._new_uuid_in_init:
+    write_plugin_data()
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/setting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,221 +1,256 @@
-"""
-### 用户设置相关
-"""
-from typing import Union
-
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import PrivateMessageEvent, GroupMessageEvent, MessageEvent
-from nonebot.adapters.onebot.v11.message import Message
-from nonebot.matcher import Matcher
-from nonebot.params import Arg, ArgPlainText, T_State
-
-from .myb_missions_api import BaseMission
-from .plugin_data import PluginDataManager, write_plugin_data
-from .user_data import UserAccount
-from .utils import COMMAND_BEGIN
-
-_conf = PluginDataManager.plugin_data
-
-setting = on_command(_conf.preference.command_start + '设置', priority=4, block=True)
-setting.name = "设置"
-setting.usage = '如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{HEAD}账号设置』命令。' \
-                '\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{HEAD}通知设置』命令。'
-
-
-@setting.handle()
-async def _(_: MessageEvent):
-    msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令' \
-          f'\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
-    await setting.send(msg)
-
-
-account_setting = on_command(_conf.preference.command_start + '账号设置', priority=5, block=True)
-account_setting.name = "账号设置"
-account_setting.usage = "配置游戏自动签到、米游币任务是否开启、设备平台、频道任务相关选项"
-
-
-@account_setting.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher):
-    """
-    账号设置命令触发
-    """
-    user = _conf.users.get(event.user_id)
-    user_account = user.accounts if user else None
-    if not user_account:
-        await account_setting.finish(
-            f"⚠️你尚未绑定米游社账户，请先使用『{_conf.preference.command_start}登录』进行登录")
-    if len(user_account) == 1:
-        uid = next(iter(user_account.values())).bbs_uid
-        matcher.set_arg('bbs_uid', Message(uid))
-    else:
-        msg = "您有多个账号，您要更改以下哪个账号的设置？\n"
-        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
-        msg += "\n🚪发送“退出”即可退出"
-        await matcher.send(msg)
-
-
-@account_setting.got('bbs_uid')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, uid=Arg('bbs_uid')):
-    """
-    根据手机号设置相应的账户
-    """
-    if isinstance(uid, Message):
-        uid = uid.extract_plain_text().strip()
-    if uid == '退出':
-        await matcher.finish('🚪已成功退出')
-
-    user_account = _conf.users[event.user_id].accounts
-    if uid not in user_account:
-        await account_setting.reject('⚠️您发送的账号不在以上账号内，请重新发送')
-    account = user_account[uid]
-    state['account'] = account
-    state["prepare_to_delete"] = False
-
-    user_setting = ""
-    user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.enable_mission else '关'}"
-    user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_game_sign else '关'}"
-    platform_show = "iOS" if account.platform == "ios" else "安卓"
-    user_setting += f"\n3️⃣ 设备平台：{platform_show}"
-
-    # 筛选出用户数据中的missionGame对应的游戏全称
-    user_setting += "\n\n4️⃣ 执行米游币任务的频道：" + \
-                    "\n- " + "、".join(map(lambda x: f"『{x.NAME}』", account.mission_games))
-    user_setting += f"\n\n5️⃣ 原神树脂恢复提醒：{'开' if account.enable_resin else '关'}"
-    user_setting += f"\n6️⃣更改崩铁便笺开拓力提醒阈值 \
-                            当前提醒阈值：{account.user_stamina_threshold}"
-    user_setting += "\n7️⃣⚠️删除账户数据"
-
-    await account_setting.send(user_setting + '\n\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6 / 7'
-                                              '\n🚪发送“退出”即可退出')
-
-
-@account_setting.got('arg')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], state: T_State, arg=ArgPlainText('arg')):
-    """
-    根据所选更改相应账户的相应设置
-    """
-    arg = arg.strip()
-    account: UserAccount = state['account']
-    user_account = _conf.users[event.user_id].accounts
-    if arg == '退出':
-        await account_setting.finish('🚪已成功退出')
-    elif arg == '1':
-        account.enable_mission = not account.enable_mission
-        write_plugin_data()
-        await account_setting.finish(f"📅米游币任务自动执行已 {'✅开启' if account.enable_mission else '❌关闭'}")
-    elif arg == '2':
-        account.enable_game_sign = not account.enable_game_sign
-        write_plugin_data()
-        await account_setting.finish(f"📅米哈游游戏自动签到已 {'✅开启' if account.enable_game_sign else '❌关闭'}")
-    elif arg == '3':
-        if account.platform == "ios":
-            account.platform = "android"
-            platform_show = "安卓"
-        else:
-            account.platform = "ios"
-            platform_show = "iOS"
-        write_plugin_data()
-        await account_setting.finish(f"📲设备平台已更改为 {platform_show}")
-    elif arg == '4':
-        games_show = "、".join(map(lambda x: f"『{x.NAME}』", BaseMission.AVAILABLE_GAMES))
-        await account_setting.send(
-            "请发送你想要执行米游币任务的频道："
-            "\n❕多个频道请用空格分隔，如 “原神 崩坏3 大别野”"
-            "\n\n可选的频道："
-            f"\n- {games_show}"
-            "\n\n🚪发送“退出”即可退出"
-        )
-        state["setting_item"] = "mission_games"
-    elif arg == '5':
-        account.enable_resin = not account.enable_resin
-        write_plugin_data()
-        await account_setting.finish(f"📅原神、星穹铁道便笺提醒已 {'✅开启' if account.enable_resin else '❌关闭'}")
-    elif arg == '6':
-        await account_setting.send(
-            "请输入想要所需阈值数字："
-            "支持输入[0,180]"
-            "\n\n🚪发送“退出”即可退出"
-        )
-        state["setting_item"] = "threshold"
-    elif arg == '7':
-        state["prepare_to_delete"] = True
-        await account_setting.reject(f"⚠️确认删除账号 {account.phone_number} ？发送 \"确认删除\" 以确定。")
-    elif arg == '确认删除' and state["prepare_to_delete"]:
-        user_account.pop(account.bbs_uid)
-        write_plugin_data()
-        await account_setting.finish(f"已删除账号 {account.phone_number} 的数据")
-    else:
-        await account_setting.reject("⚠️您的输入有误，请重新输入")
-
-
-@account_setting.got('setting_arg')
-async def _(_: Union[PrivateMessageEvent, GroupMessageEvent], state: T_State, arg=ArgPlainText('setting_arg')):
-    arg = arg.strip()
-    if arg == '退出':
-        await account_setting.finish('🚪已成功退出')
-    account: UserAccount = state['account']
-
-    if state["setting_item"] == "threshold":
-        try:
-            stamina_threshold = int(arg)
-        except ValueError:
-            await account_setting.reject("⚠️请输入有效的数字。")
-        else:
-            if 0 <= stamina_threshold <= 180:
-                # 输入有效的数字范围，将 stamina_threshold 赋值为输入的整数
-                account.user_stamina_threshold = stamina_threshold
-                write_plugin_data()
-                await account_setting.finish(f"更改崩铁便笺开拓力提醒阈值成功，当前提醒阈值：{stamina_threshold}")
-            else:
-                await account_setting.reject("⚠️输入的数字范围应在 0 到 180 之间。")
-
-    elif state["setting_item"] == "mission_games":
-        games_input = arg.split()
-        mission_games = set()
-        for game in games_input:
-            game_filter = filter(lambda x: x.NAME == game, BaseMission.AVAILABLE_GAMES)
-            game_obj = next(game_filter, None)
-            if game_obj is None:
-                await account_setting.reject("⚠️您的输入有误，请重新输入")
-            else:
-                mission_games.add(game_obj)
-
-        account.mission_games = mission_games
-        write_plugin_data()
-        arg = arg.replace(" ", "、")
-        await account_setting.finish(f"💬执行米游币任务的频道已更改为『{arg}』")
-
-
-global_setting = on_command(_conf.preference.command_start + '通知设置', priority=5, block=True)
-global_setting.name = "通知设置"
-global_setting.usage = "设置每日签到后是否进行QQ通知"
-
-
-@global_setting.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher):
-    """
-    通知设置命令触发
-    """
-    user = _conf.users[event.user_id]
-    await matcher.send(
-        f"自动通知每日计划任务结果：{'🔔开' if user.enable_notice else '🔕关'}"
-        "\n请问您是否需要更改呢？\n请回复“是”或“否”\n🚪发送“退出”即可退出")
-
-
-@global_setting.got('choice')
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher,
-            choice: Message = ArgPlainText('choice')):
-    """
-    根据选择变更通知设置
-    """
-    user = _conf.users[event.user_id]
-    if choice == '退出':
-        await matcher.finish("🚪已成功退出")
-    elif choice == '是':
-        user.enable_notice = not user.enable_notice
-        write_plugin_data()
-        await matcher.finish(f"自动通知每日计划任务结果 已 {'🔔开启' if user.enable_notice else '🔕关闭'}")
-    elif choice == '否':
-        await matcher.finish("没有做修改哦~")
-    else:
-        await matcher.reject("⚠️您的输入有误，请重新输入")
+"""
+### 用户设置相关
+"""
+
+from nonebot import on_command
+from nonebot.internal.params import ArgStr
+from nonebot.matcher import Matcher
+from nonebot.params import T_State
+
+from .myb_missions_api import BaseMission
+from .plugin_data import PluginDataManager, write_plugin_data
+from .user_data import UserAccount
+from .utils import COMMAND_BEGIN, GeneralMessageEvent, logger
+
+_conf = PluginDataManager.plugin_data
+
+setting = on_command(_conf.preference.command_start + '设置', priority=4, block=True)
+setting.name = "设置"
+setting.usage = '如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{HEAD}账号设置』命令。' \
+                '\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{HEAD}通知设置』命令。'
+
+
+@setting.handle()
+async def _(_: GeneralMessageEvent):
+    msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令' \
+          f'\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
+    await setting.send(msg)
+
+
+account_setting = on_command(_conf.preference.command_start + '账号设置', priority=5, block=True)
+account_setting.name = "账号设置"
+account_setting.usage = "配置游戏自动签到、米游币任务是否开启、设备平台、频道任务相关选项"
+
+
+@account_setting.handle()
+async def _(event: GeneralMessageEvent, matcher: Matcher, state: T_State):
+    """
+    账号设置命令触发
+    """
+    user = _conf.users.get(event.get_user_id())
+    user_account = user.accounts if user else None
+    if not user_account:
+        await account_setting.finish(
+            f"⚠️你尚未绑定米游社账户，请先使用『{_conf.preference.command_start}登录』进行登录")
+    if len(user_account) == 1:
+        uid = next(iter(user_account.values())).bbs_uid
+        state["bbs_uid"] = uid
+    else:
+        msg = "您有多个账号，您要更改以下哪个账号的设置？\n"
+        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
+        msg += "\n🚪发送“退出”即可退出"
+        await matcher.send(msg)
+
+
+@account_setting.got('bbs_uid')
+async def _(event: GeneralMessageEvent, matcher: Matcher, state: T_State, bbs_uid=ArgStr()):
+    """
+    根据手机号设置相应的账户
+    """
+    if bbs_uid == '退出':
+        await matcher.finish('🚪已成功退出')
+
+    user_account = _conf.users[event.get_user_id()].accounts
+    if bbs_uid not in user_account:
+        await account_setting.reject('⚠️您发送的账号不在以上账号内，请重新发送')
+    account = user_account[bbs_uid]
+    state['account'] = account
+    state["prepare_to_delete"] = False
+
+    user_setting = ""
+    user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.enable_mission else '关'}"
+    user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_game_sign else '关'}"
+    platform_show = "iOS" if account.platform == "ios" else "安卓"
+    user_setting += f"\n3️⃣ 设备平台：{platform_show}"
+
+    # 筛选出用户数据中的missionGame对应的游戏全称
+    user_setting += "\n\n4️⃣ 执行米游币任务的频道：" + \
+                    "\n- " + "、".join(map(lambda x: f"『{x.NAME}』", account.mission_games))
+    user_setting += f"\n\n5️⃣ 原神树脂恢复提醒：{'开' if account.enable_resin else '关'}"
+    user_setting += f"\n6️⃣更改便笺体力提醒阈值 \
+                      \n   当前原神提醒阈值：{account.user_resin_threshold} \
+                      \n   当前崩铁提醒阈值：{account.user_stamina_threshold}"
+    user_setting += "\n7️⃣⚠️删除账户数据"
+
+    await account_setting.send(user_setting + '\n\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6 / 7'
+                                              '\n🚪发送“退出”即可退出')
+
+
+@account_setting.got('setting_id')
+async def _(event: GeneralMessageEvent, state: T_State, setting_id=ArgStr()):
+    """
+    根据所选更改相应账户的相应设置
+    """
+    logger.debug(f"{type(setting_id)}")
+    account: UserAccount = state['account']
+    user_account = _conf.users[event.get_user_id()].accounts
+    if setting_id == '退出':
+        await account_setting.finish('🚪已成功退出')
+    elif setting_id == '1':
+        account.enable_mission = not account.enable_mission
+        write_plugin_data()
+        await account_setting.finish(f"📅米游币任务自动执行已 {'✅开启' if account.enable_mission else '❌关闭'}")
+    elif setting_id == '2':
+        account.enable_game_sign = not account.enable_game_sign
+        write_plugin_data()
+        await account_setting.finish(f"📅米哈游游戏自动签到已 {'✅开启' if account.enable_game_sign else '❌关闭'}")
+    elif setting_id == '3':
+        if account.platform == "ios":
+            account.platform = "android"
+            platform_show = "安卓"
+        else:
+            account.platform = "ios"
+            platform_show = "iOS"
+        write_plugin_data()
+        await account_setting.finish(f"📲设备平台已更改为 {platform_show}")
+    elif setting_id == '4':
+        games_show = "、".join(map(lambda x: f"『{x.NAME}』", BaseMission.AVAILABLE_GAMES))
+        await account_setting.send(
+            "请发送你想要执行米游币任务的频道："
+            "\n❕多个频道请用空格分隔，如 “原神 崩坏3 大别野”"
+            "\n\n可选的频道："
+            f"\n- {games_show}"
+            "\n\n🚪发送“退出”即可退出"
+        )
+        state["setting_item"] = "mission_games"
+    elif setting_id == '5':
+        account.enable_resin = not account.enable_resin
+        write_plugin_data()
+        await account_setting.finish(f"📅原神、星穹铁道便笺提醒已 {'✅开启' if account.enable_resin else '❌关闭'}")
+    elif setting_id == '6':
+        await account_setting.send(
+            "请发送想要修改体力提醒阈值的游戏编号："
+            "\n1. 原神"
+            "\n2. 崩坏：星穹铁道"
+            "\n\n🚪发送“退出”即可退出"
+        )
+        state["setting_item"] = "notice_value"
+    elif setting_id == '7':
+        state["prepare_to_delete"] = True
+        await account_setting.reject(f"⚠️确认删除账号 {account.phone_number} ？发送 \"确认删除\" 以确定。")
+    elif setting_id == '确认删除' and state["prepare_to_delete"]:
+        user_account.pop(account.bbs_uid)
+        write_plugin_data()
+        await account_setting.finish(f"已删除账号 {account.phone_number} 的数据")
+    else:
+        await account_setting.reject("⚠️您的输入有误，请重新输入")
+
+
+@account_setting.got('notice_game')
+async def _(_: GeneralMessageEvent, state: T_State, notice_game=ArgStr()):
+    if notice_game == '退出':
+        await account_setting.finish('🚪已成功退出')
+    if state["setting_item"] == "notice_value":
+        if notice_game == "1":
+            await account_setting.send(
+                "请输入想要所需通知阈值，树脂达到该值时将进行通知："
+                "可用范围 [0, 160]"
+                "\n\n🚪发送“退出”即可退出"
+            )
+            state["setting_item"] = "notice_value_op"
+        elif notice_game == "2":
+            await account_setting.send(
+                "请输入想要所需阈值数字，开拓力达到该值时将进行通知："
+                "可用范围 [0, 180]"
+                "\n\n🚪发送“退出”即可退出"
+            )
+            state["setting_item"] = "notice_value_sr"
+        else:
+            await account_setting.reject("⚠️您的输入有误，请重新输入")
+
+
+@account_setting.got('notice_value')
+async def _(_: GeneralMessageEvent, state: T_State, notice_value=ArgStr()):
+    if notice_value == '退出':
+        await account_setting.finish('🚪已成功退出')
+    account: UserAccount = state['account']
+
+    if state["setting_item"] == "notice_value_op":
+        try:
+            resin_threshold = int(notice_value)
+        except ValueError:
+            await account_setting.reject("⚠️请输入有效的数字。")
+        else:
+            if 0 <= resin_threshold <= 160:
+                # 输入有效的数字范围，将 resin_threshold 赋值为输入的整数
+                account.user_resin_threshold = resin_threshold
+                write_plugin_data()
+                await account_setting.finish(f"更改原神便笺树脂提醒阈值成功\n"
+                                             f"⏰当前提醒阈值：{resin_threshold}")
+            else:
+                await account_setting.reject("⚠️输入的数字范围应在 0 到 160 之间。")
+
+    elif state["setting_item"] == "notice_value_sr":
+        try:
+            stamina_threshold = int(notice_value)
+        except ValueError:
+            await account_setting.reject("⚠️请输入有效的数字。")
+        else:
+            if 0 <= stamina_threshold <= 180:
+                # 输入有效的数字范围，将 stamina_threshold 赋值为输入的整数
+                account.user_stamina_threshold = stamina_threshold
+                write_plugin_data()
+                await account_setting.finish(f"更改崩铁便笺开拓力提醒阈值成功\n"
+                                             f"⏰当前提醒阈值：{stamina_threshold}")
+            else:
+                await account_setting.reject("⚠️输入的数字范围应在 0 到 180 之间。")
+
+    elif state["setting_item"] == "mission_games":
+        games_input = notice_value.split()
+        mission_games = set()
+        for game in games_input:
+            game_filter = filter(lambda x: x.NAME == game, BaseMission.AVAILABLE_GAMES)
+            game_obj = next(game_filter, None)
+            if game_obj is None:
+                await account_setting.reject("⚠️您的输入有误，请重新输入")
+            else:
+                mission_games.add(game_obj)
+
+        account.mission_games = mission_games
+        write_plugin_data()
+        notice_value = notice_value.replace(" ", "、")
+        await account_setting.finish(f"💬执行米游币任务的频道已更改为『{notice_value}』")
+
+
+global_setting = on_command(_conf.preference.command_start + '通知设置', priority=5, block=True)
+global_setting.name = "通知设置"
+global_setting.usage = "设置每日签到后是否进行QQ通知"
+
+
+@global_setting.handle()
+async def _(event: GeneralMessageEvent, matcher: Matcher):
+    """
+    通知设置命令触发
+    """
+    user = _conf.users[event.get_user_id()]
+    await matcher.send(
+        f"自动通知每日计划任务结果：{'🔔开' if user.enable_notice else '🔕关'}"
+        "\n请问您是否需要更改呢？\n请回复“是”或“否”\n🚪发送“退出”即可退出")
+
+
+@global_setting.got('choice')
+async def _(event: GeneralMessageEvent, matcher: Matcher, choice=ArgStr()):
+    """
+    根据选择变更通知设置
+    """
+    user = _conf.users[event.get_user_id()]
+    if choice == '退出':
+        await matcher.finish("🚪已成功退出")
+    elif choice == '是':
+        user.enable_notice = not user.enable_notice
+        write_plugin_data()
+        await matcher.finish(f"自动通知每日计划任务结果 已 {'🔔开启' if user.enable_notice else '🔕关闭'}")
+    elif choice == '否':
+        await matcher.finish("没有做修改哦~")
+    else:
+        await matcher.reject("⚠️您的输入有误，请重新输入")
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/simple_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/simple_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1414,18 +1414,18 @@
     """
     获取原神实时便笺
 
     :param account: 用户账户数据
     """
     game_record_status, records = await get_game_record(account)
     if not game_record_status:
-        return game_record_status, None
+        return GenshinBoardStatus(game_record_failed=True), None
     game_list_status, game_list = await get_game_list()
     if not game_list_status:
-        return game_list_status, None
+        return GenshinBoardStatus(game_list_failed=True), None
     game_filter = filter(lambda x: x.en_name == 'ys', game_list)
     game_info = next(game_filter, None)
     if not game_info:
         return GenshinBoardStatus(no_genshin_account=True), None
     else:
         game_id = game_info.id
     flag = True
@@ -1490,21 +1490,19 @@
     Union[BaseApiStatus, StarRailBoardStatus], Optional[StarRailBoard]]:
     """
     获取崩铁实时便笺
 
     :param account: 用户账户数据
     """
     game_record_status, records = await get_game_record(account)
-    logger.info(f"genshin_board game_record_status : {game_record_status}")
-    logger.info(f"genshin_board records : {records}")
     if not game_record_status:
-        return game_record_status, None
+        return StarRailBoardStatus(game_record_failed=True), None
     game_list_status, game_list = await get_game_list()
     if not game_list_status:
-        return game_list_status, None
+        return StarRailBoardStatus(game_list_failed=True), None
     game_filter = filter(lambda x: x.en_name == 'sr', game_list)
     game_info = next(game_filter, None)
     if not game_info:
         return StarRailBoardStatus(no_starrail_account=True), None
     else:
         game_id = game_info.id
     flag = True
```

### Comparing `nonebot_plugin_mystool-1.1.0/src/nonebot_plugin_mystool/user_data.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 ### 用户数据相关
 """
 from typing import List, Union, Optional, Any, Dict, Set, TYPE_CHECKING, AbstractSet, \
     Mapping, Literal
+from uuid import uuid4, UUID
 
 from httpx import Cookies
 from pydantic import BaseModel, validator
 
 from .data_model import BaseModelWithSetter, Good, Address, GameRecord, BaseModelWithUpdate
 
 if TYPE_CHECKING:
@@ -224,16 +225,18 @@
     '''是否开启米游社游戏签到计划'''
     enable_resin: bool = True
     '''是否开启原神树脂提醒'''
     platform: Literal["ios", "android"] = "ios"
     '''设备平台'''
     mission_games: Set[type] = {}
     '''在哪些板块执行米游币任务计划'''
-    user_stamina_threshold: Optional[int] = 0
+    user_stamina_threshold: Optional[int] = 180
     '''崩铁便笺体力提醒阈值，0为一直提醒'''
+    user_resin_threshold: Optional[int] = 160
+    '''原神便笺树脂提醒阈值，0为一直提醒'''
 
     def __init__(self, **data: Any):
         if not data.get("device_id_ios") or not data.get("device_id_android"):
             from .utils import generate_device_id
             if not data.get("device_id_ios"):
                 data.setdefault("device_id_ios", generate_device_id())
             if not data.get("device_id_android"):
@@ -334,25 +337,71 @@
     """兑换结果"""
     return_data: dict
     """返回数据"""
     plan: ExchangePlan
     """兑换计划"""
 
 
+_uuid_set: Set[str] = set()
+"""已使用的用户UUID密钥集合"""
+_new_uuid_in_init = False
+"""插件反序列化用户数据时，是否生成了新的UUID密钥"""
+
+
+def uuid4_validate(v):
+    """
+    验证UUID是否为合法的UUIDv4
+
+    :param v: UUID
+    """
+    try:
+        UUID(v, version=4)
+    except:
+        return False
+    else:
+        return True
+
+
 class UserData(BaseModelWithSetter):
     """
     用户数据类
+
+    >>> _ = UserData()
     """
+    enable_notice: bool = True
+    """是否开启通知"""
+    uuid: Optional[str] = None
+    """用户UUID密钥，用于不同NoneBot适配器平台之间的数据同步，因此不可泄露"""
     exchange_plans: Union[Set[ExchangePlan], List[ExchangePlan]] = set()
     """兑换计划列表"""
     accounts: Dict[str, UserAccount] = {}
     """储存一些已绑定的账号数据"""
-    enable_notice: bool = True
-    """是否开启通知"""
+    qq_guilds: Optional[Dict[str, Set[int]]] = {}
+    """储存用户所在的QQ频道ID {用户ID : [频道ID]}"""
+
+    @validator("uuid")
+    def uuid_validator(cls, v):
+        """
+        验证UUID是否为合法的UUIDv4
+
+        :raises ValueError: UUID格式错误，不是合法的UUIDv4
+        """
+        if v is None and not uuid4_validate(v):
+            raise ValueError("UUID格式错误，不是合法的UUIDv4")
 
     def __init__(self, **data: Any):
+        global _new_uuid_in_init
         super().__init__(**data)
+
         exchange_plans = self.exchange_plans
         self.exchange_plans = set()
         for plan in exchange_plans:
             plan = ExchangePlan.parse_obj(plan)
             self.exchange_plans.add(plan)
+
+        if self.uuid is None:
+            new_uuid = uuid4()
+            while str(new_uuid) in _uuid_set:
+                new_uuid = uuid4()
+            self.uuid = str(new_uuid)
+            _new_uuid_in_init = True
+        _uuid_set.add(self.uuid)
```

### Comparing `nonebot_plugin_mystool-1.1.0/PKG-INFO` & `nonebot_plugin_mystool-1.2.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 1.1.0
+Version: 1.2.0b1
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -13,17 +13,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.5,<11.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: nonebot-adapter-qqguild (>=0.2.3,<0.3.0)
 Requires-Dist: nonebot_adapter_onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues
 Project-URL: Documentation, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki
 Project-URL: Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 Description-Content-Type: text/markdown
 
@@ -40,39 +42,45 @@
   <img alt="最新发行版" src="https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge">
   <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
 </div>
 
 # mysTool - 米游社辅助工具插件
 
 ## 📣 更新内容
+### 2023.7.28 - v1.2.0-beta.1
+- 增加对QQ频道的支持 #128
+  > 说明文档：[🔗QQGuild 适配器](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Installation#QQGuild-适配器)
+- 增加用户数据绑定关联功能（如QQ频道账号与QQ聊天账号的数据绑定）
+  > 说明文档：[🔗用户数据绑定关联](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-UserBind)
+- 增加原神便笺树脂提醒阈值的设置选项 #151 by @Joseandluue
+  > 说明文档：[🔗对绑定的某个米哈游账户进行设置](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-Setting#%E5%AF%B9%E7%BB%91%E5%AE%9A%E7%9A%84%E6%9F%90%E4%B8%AA%E7%B1%B3%E5%93%88%E6%B8%B8%E8%B4%A6%E6%88%B7%E8%BF%9B%E8%A1%8C%E8%AE%BE%E7%BD%AE)
+- 修复 `preference.override_device_and_salt` 关闭无效的问题
+
 ### 2023.7.23 - v1.1.0
 - 增加崩坏：星穹铁道的便笺功能 #140 #143 by @Joseandluue @RemiDre
     > 说明文档：[🔗星穹铁道实时便笺](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-StarRailStatus)
 - 修复每小时都发送便笺通知的Bug #135
 - 人机验证打码平台支持自定义JSON内容 #133
     > 说明文档：[🔗geetest_json](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Configuration-Preference#geetest_json)
 - 修复商品兑换API #110
 - 不在好友列表的用户数据在删除前将进行备份 #129
     > 备份目录：`data/nonebot_plugin_mystool/deletedUsers`
-- 防止因插件数据文件中默认存在 device_config, salt_config 而导致更新后默认配置被原配置覆盖的问题
-- 若需要修改 device_config 配置，修改后还设置插件数据文件中 preference.override_device_and_salt 为 true 以覆盖默认值
+- 防止因插件数据文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
+- 若需要修改 `device_config` 配置，修改后还设置插件数据文件中 `preference.override_device_and_salt` 为 true 以覆盖默认值
     > 说明文档：
     > - [🔗网络请求设备信息 `class DeviceConfig`](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Configuration-DeviceConfig)
     > - [🔗override_device_and_salt](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Configuration-Preference#override_device_and_salt)
+- 增加了是否使用多进程生成商品图片的配置项 `good_list_image_config`.`MULTI_PROCESS`，如果遇到生成图片失败可以尝试关闭该项
 - 在兑换开始后的一段时间内不断尝试兑换，直到成功 #110
 - 兑换开始后将不会延迟兑换，用户数据文件中 `preference.exchange_latency` 将作为同一线程下每个兑换请求之间的时间间隔 #110
 - 兑换请求日志内容增加了发送请求时的时间戳
 
-### 2023.6.23 - v1.0.1
-- 修复无法导出Cookies的问题
-- 修复因缺少参量质变仪数据而导致不断提醒的Bug
-- 修复账号设置中游戏签到开启/关闭状态实际对应的是米游币任务的Bug #121 by @xxtg666
-
 ## 功能和特性
 
+- 支持QQ聊天和QQ频道
 - 短信验证登录，免抓包获取 Cookie
 - 自动完成每日米游币任务
 - 自动进行游戏签到
 - 可制定米游币商品兑换计划，到点兑换（因加入了人机验证，成功率较低）
 - 可支持多个 QQ 账号，每个 QQ 账号可绑定多个米哈游账户
 - QQ 推送执行结果通知
 - 原神、崩坏：星穹铁道状态便笺通知
```

