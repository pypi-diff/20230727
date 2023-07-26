# Comparing `tmp/oobabot_plugin-0.2.1.tar.gz` & `tmp/oobabot_plugin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot_plugin-0.2.1.tar", max compression
+gzip compressed data, was "oobabot_plugin-0.2.2.tar", max compression
```

## Comparing `oobabot_plugin-0.2.1.tar` & `oobabot_plugin-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-24 23:25:59.529104 oobabot_plugin-0.2.1/LICENSE
--rw-r--r--   0        0        0     1951 2023-05-24 23:25:59.529239 oobabot_plugin-0.2.1/README.md
--rw-r--r--   0        0        0     1892 2023-07-17 23:13:28.166029 oobabot_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      264 2023-07-17 23:13:28.166406 oobabot_plugin-0.2.1/src/oobabot_plugin/__init__.py
--rw-r--r--   0        0        0     7536 2023-06-24 09:50:54.210004 oobabot_plugin-0.2.1/src/oobabot_plugin/bootstrap.py
--rw-r--r--   0        0        0     7976 2023-07-12 11:59:27.606739 oobabot_plugin-0.2.1/src/oobabot_plugin/button_enablers.py
--rw-r--r--   0        0        0     9560 2023-07-07 10:24:51.240670 oobabot_plugin-0.2.1/src/oobabot_plugin/button_handlers.py
--rw-r--r--   0        0        0     3385 2023-07-12 10:54:51.062187 oobabot_plugin-0.2.1/src/oobabot_plugin/controller.py
--rw-r--r--   0        0        0     9903 2023-05-25 05:24:15.485352 oobabot_plugin-0.2.1/src/oobabot_plugin/input_handlers.py
--rw-r--r--   0        0        0     3305 2023-05-25 06:56:54.200392 oobabot_plugin-0.2.1/src/oobabot_plugin/install.py
--rw-r--r--   0        0        0      806 2023-05-24 23:25:59.534874 oobabot_plugin-0.2.1/src/oobabot_plugin/instructions.md
--rw-r--r--   0        0        0    16325 2023-07-12 11:58:29.964662 oobabot_plugin-0.2.1/src/oobabot_plugin/layout.py
--rw-r--r--   0        0        0     4100 2023-07-12 12:09:49.203841 oobabot_plugin-0.2.1/src/oobabot_plugin/oobabot_log.css
--rw-r--r--   0        0        0      498 2023-06-26 15:36:57.565953 oobabot_plugin-0.2.1/src/oobabot_plugin/oobabot_log.js
--rw-r--r--   0        0        0     1144 2023-06-24 06:51:19.539687 oobabot_plugin-0.2.1/src/oobabot_plugin/script.py
--rw-r--r--   0        0        0      783 2023-06-22 12:29:04.858021 oobabot_plugin-0.2.1/src/oobabot_plugin/server.py
--rw-r--r--   0        0        0     6740 2023-07-12 12:05:48.229050 oobabot_plugin-0.2.1/src/oobabot_plugin/strings.py
--rw-r--r--   0        0        0      211 2023-07-07 10:24:51.243788 oobabot_plugin-0.2.1/src/oobabot_plugin/transcript.md
--rw-r--r--   0        0        0     5702 2023-07-12 10:44:52.595621 oobabot_plugin-0.2.1/src/oobabot_plugin/transcript_view.py
--rw-r--r--   0        0        0     9034 2023-07-12 10:44:41.273374 oobabot_plugin-0.2.1/src/oobabot_plugin/worker.py
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 oobabot_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 23:25:59.529104 oobabot_plugin-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1951 2023-05-24 23:25:59.529239 oobabot_plugin-0.2.2/README.md
+-rw-r--r--   0        0        0     1892 2023-07-26 23:02:19.865081 oobabot_plugin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-07-26 23:02:27.139613 oobabot_plugin-0.2.2/src/oobabot_plugin/__init__.py
+-rw-r--r--   0        0        0     7536 2023-06-24 09:50:54.210004 oobabot_plugin-0.2.2/src/oobabot_plugin/bootstrap.py
+-rw-r--r--   0        0        0     7976 2023-07-12 11:59:27.606739 oobabot_plugin-0.2.2/src/oobabot_plugin/button_enablers.py
+-rw-r--r--   0        0        0     9560 2023-07-07 10:24:51.240670 oobabot_plugin-0.2.2/src/oobabot_plugin/button_handlers.py
+-rw-r--r--   0        0        0     3385 2023-07-12 10:54:51.062187 oobabot_plugin-0.2.2/src/oobabot_plugin/controller.py
+-rw-r--r--   0        0        0     9903 2023-05-25 05:24:15.485352 oobabot_plugin-0.2.2/src/oobabot_plugin/input_handlers.py
+-rw-r--r--   0        0        0     3305 2023-05-25 06:56:54.200392 oobabot_plugin-0.2.2/src/oobabot_plugin/install.py
+-rw-r--r--   0        0        0      806 2023-05-24 23:25:59.534874 oobabot_plugin-0.2.2/src/oobabot_plugin/instructions.md
+-rw-r--r--   0        0        0    16325 2023-07-12 11:58:29.964662 oobabot_plugin-0.2.2/src/oobabot_plugin/layout.py
+-rw-r--r--   0        0        0     4100 2023-07-12 12:09:49.203841 oobabot_plugin-0.2.2/src/oobabot_plugin/oobabot_log.css
+-rw-r--r--   0        0        0      498 2023-06-26 15:36:57.565953 oobabot_plugin-0.2.2/src/oobabot_plugin/oobabot_log.js
+-rw-r--r--   0        0        0     1144 2023-06-24 06:51:19.539687 oobabot_plugin-0.2.2/src/oobabot_plugin/script.py
+-rw-r--r--   0        0        0      783 2023-06-22 12:29:04.858021 oobabot_plugin-0.2.2/src/oobabot_plugin/server.py
+-rw-r--r--   0        0        0     7163 2023-07-26 22:53:23.177063 oobabot_plugin-0.2.2/src/oobabot_plugin/strings.py
+-rw-r--r--   0        0        0      211 2023-07-07 10:24:51.243788 oobabot_plugin-0.2.2/src/oobabot_plugin/transcript.md
+-rw-r--r--   0        0        0     5702 2023-07-12 10:44:52.595621 oobabot_plugin-0.2.2/src/oobabot_plugin/transcript_view.py
+-rw-r--r--   0        0        0     9034 2023-07-12 10:44:41.273374 oobabot_plugin-0.2.2/src/oobabot_plugin/worker.py
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 oobabot_plugin-0.2.2/PKG-INFO
```

### Comparing `oobabot_plugin-0.2.1/LICENSE` & `oobabot_plugin-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/README.md` & `oobabot_plugin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/pyproject.toml` & `oobabot_plugin-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oobabot-plugin"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot."
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot-plugin"
 
 [tool.poetry.dependencies]
```

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/bootstrap.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/bootstrap.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/button_enablers.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/button_enablers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/button_handlers.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/button_handlers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/controller.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/controller.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/input_handlers.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/input_handlers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/install.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/install.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/instructions.md` & `oobabot_plugin-0.2.2/src/oobabot_plugin/instructions.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/layout.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/layout.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/oobabot_log.css` & `oobabot_plugin-0.2.2/src/oobabot_plugin/oobabot_log.css`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/script.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/script.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/server.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/server.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/strings.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,129 +294,155 @@
 00001250: 6374 6572 732e 6170 7065 6e64 2866 696c  cters.append(fil
 00001260: 6570 6174 682e 7374 656d 290a 2020 2020  epath.stem).    
 00001270: 6368 6172 6163 7465 7273 2e73 6f72 7428  characters.sort(
 00001280: 290a 2020 2020 6368 6172 6163 7465 7273  ).    characters
 00001290: 2e69 6e73 6572 7428 302c 2043 4841 5241  .insert(0, CHARA
 000012a0: 4354 4552 5f4e 4f4e 4529 0a20 2020 2072  CTER_NONE).    r
 000012b0: 6574 7572 6e20 6368 6172 6163 7465 7273  eturn characters
-000012c0: 0a0a 0a64 6566 2072 6570 6169 725f 6c6f  ...def repair_lo
-000012d0: 6767 696e 6728 2920 2d3e 2074 7970 696e  gging() -> typin
-000012e0: 672e 4f70 7469 6f6e 616c 5b6c 6f67 6769  g.Optional[loggi
-000012f0: 6e67 2e4c 6f67 6765 725d 3a0a 2020 2020  ng.Logger]:.    
-00001300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001320: 2323 0a20 2020 2023 2073 6f2c 206c 6f67  ##.    # so, log
-00001330: 6769 6e67 5f63 6f6c 6f72 732e 7079 2c20  ging_colors.py, 
-00001340: 7261 7468 6572 2074 6861 6e20 7573 696e  rather than usin
-00001350: 6720 7468 6520 6c6f 6767 696e 6720 6d6f  g the logging mo
-00001360: 6475 6c65 2773 2062 7569 6c74 2d69 6e0a  dule's built-in.
-00001370: 2020 2020 2320 666f 726d 6174 7465 722c      # formatter,
-00001380: 2069 7320 6d6f 6e6b 6579 2d70 6174 6368   is monkey-patch
-00001390: 696e 6720 7468 6520 6c6f 6767 696e 6720  ing the logging 
-000013a0: 6d6f 6475 6c65 2773 2053 7472 6561 6d48  module's StreamH
-000013b0: 616e 646c 6572 2e65 6d69 742e 0a20 2020  andler.emit..   
-000013c0: 2023 2054 6869 7320 6973 2061 2070 726f   # This is a pro
-000013d0: 626c 656d 2066 6f72 2075 732c 2062 6563  blem for us, bec
-000013e0: 6175 7365 2077 6520 616c 736f 2075 7365  ause we also use
-000013f0: 2074 6865 206c 6f67 6769 6e67 206d 6f64   the logging mod
-00001400: 756c 652c 2062 7574 0a20 2020 2023 2064  ule, but.    # d
-00001410: 6f6e 2774 2077 616e 7420 414e 5349 2063  on't want ANSI c
-00001420: 6f6c 6f72 2063 6f64 6573 2073 686f 7769  olor codes showi
-00001430: 6e67 2075 7020 696e 2048 544d 4c2e 2020  ng up in HTML.  
-00001440: 5765 2061 6c73 6f20 646f 6e27 7420 7761  We also don't wa
-00001450: 6e74 0a20 2020 2023 2074 6f20 6272 6561  nt.    # to brea
-00001460: 6b20 7468 6569 7220 6c6f 6767 696e 672e  k their logging.
-00001470: 0a20 2020 2023 0a20 2020 2023 2053 6f2c  .    #.    # So,
-00001480: 2077 6527 7265 2067 6f69 6e67 2074 6f20   we're going to 
-00001490: 7361 7665 2074 6865 6972 206d 6f6e 6b65  save their monke
-000014a0: 792d 7061 7463 6865 6420 656d 6974 2c20  y-patched emit, 
-000014b0: 7265 6c6f 6164 2074 6865 206c 6f67 6769  reload the loggi
-000014c0: 6e67 0a20 2020 2023 206d 6f64 756c 652c  ng.    # module,
-000014d0: 2073 6176 6520 6f66 6620 7468 6520 2272   save off the "r
-000014e0: 6561 6c22 2065 6d69 742c 2074 6865 6e20  eal" emit, then 
-000014f0: 7265 2d61 7070 6c79 2074 6865 6972 206d  re-apply their m
-00001500: 6f6e 6b65 792d 7061 7463 682e 0a20 2020  onkey-patch..   
-00001510: 2023 0a20 2020 2023 2057 6520 6e65 6564   #.    # We need
-00001520: 2074 6f20 646f 2061 6c6c 2074 6869 7320   to do all this 
-00001530: 6265 666f 7265 2077 6520 6372 6561 7465  before we create
-00001540: 2074 6865 206f 6f62 6162 6f74 5f77 6f72   the oobabot_wor
-00001550: 6b65 722c 2073 6f20 7468 6174 0a20 2020  ker, so that.   
-00001560: 2023 2074 6865 206c 6f67 7320 6372 6561   # the logs crea
-00001570: 7465 6420 6475 7269 6e67 2073 7461 7274  ted during start
-00001580: 7570 2061 7265 2070 726f 7065 726c 7920  up are properly 
-00001590: 666f 726d 6174 7465 642e 0a0a 2020 2020  formatted...    
-000015a0: 2320 7361 7665 2074 6865 206d 6f6e 6b65  # save the monke
-000015b0: 792d 7061 7463 6865 6420 656d 6974 0a20  y-patched emit. 
-000015c0: 2020 2068 6163 6b65 645f 656d 6974 203d     hacked_emit =
-000015d0: 206c 6f67 6769 6e67 2e53 7472 6561 6d48   logging.StreamH
-000015e0: 616e 646c 6572 2e65 6d69 740a 0a20 2020  andler.emit..   
-000015f0: 2023 2072 656c 6f61 6420 7468 6520 6c6f   # reload the lo
-00001600: 6767 696e 6720 6d6f 6475 6c65 0a20 2020  gging module.   
-00001610: 2074 7279 3a0a 2020 2020 2020 2020 696d   try:.        im
-00001620: 706f 7274 6c69 622e 7265 6c6f 6164 286c  portlib.reload(l
-00001630: 6f67 6769 6e67 290a 2020 2020 6578 6365  ogging).    exce
-00001640: 7074 2049 6d70 6f72 7445 7272 6f72 2061  pt ImportError a
-00001650: 7320 6572 723a 0a20 2020 2020 2020 2070  s err:.        p
-00001660: 7269 6e74 2866 224f 6f62 6162 6f74 3a20  rint(f"Oobabot: 
-00001670: 4572 726f 7220 7265 6c6f 6164 696e 6720  Error reloading 
-00001680: 6c6f 6767 696e 6720 6d6f 6475 6c65 3a20  logging module: 
-00001690: 7b65 7272 7d22 2c20 6669 6c65 3d73 7973  {err}", file=sys
-000016a0: 2e73 7464 6572 7229 0a20 2020 2020 2020  .stderr).       
-000016b0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-000016c0: 2020 2320 6372 6561 7465 206f 7572 206c    # create our l
-000016d0: 6f67 6765 7220 6561 726c 790a 2020 2020  ogger early.    
-000016e0: 6f6f 6261 626f 742e 6661 6e63 795f 6c6f  oobabot.fancy_lo
-000016f0: 6767 6572 2e69 6e69 745f 6c6f 6767 696e  gger.init_loggin
-00001700: 6728 6c6f 6767 696e 672e 4445 4255 472c  g(logging.DEBUG,
-00001710: 2054 7275 6529 0a20 2020 206f 6f62 615f   True).    ooba_
-00001720: 6c6f 6767 6572 203d 206f 6f62 6162 6f74  logger = oobabot
-00001730: 2e66 616e 6379 5f6c 6f67 6765 722e 6765  .fancy_logger.ge
-00001740: 7428 290a 0a20 2020 2023 206d 616e 7561  t()..    # manua
-00001750: 6c6c 7920 6170 706c 7920 7468 6520 2263  lly apply the "c
-00001760: 6f72 7265 6374 2220 656d 6974 2074 6f20  orrect" emit to 
-00001770: 6561 6368 206f 6620 7468 6520 5374 7265  each of the Stre
-00001780: 616d 4861 6e64 6c65 7273 0a20 2020 2023  amHandlers.    #
-00001790: 2074 6861 7420 6661 6e63 795f 6c6f 6767   that fancy_logg
-000017a0: 6572 2063 7265 6174 6564 0a20 2020 2066  er created.    f
-000017b0: 6f72 2068 616e 646c 6572 2069 6e20 6f6f  or handler in oo
-000017c0: 6261 5f6c 6f67 6765 722e 6861 6e64 6c65  ba_logger.handle
-000017d0: 7273 3a0a 2020 2020 2020 2020 6966 2069  rs:.        if i
-000017e0: 7369 6e73 7461 6e63 6528 6861 6e64 6c65  sinstance(handle
-000017f0: 722c 206c 6f67 6769 6e67 2e53 7472 6561  r, logging.Strea
-00001800: 6d48 616e 646c 6572 293a 0a20 2020 2020  mHandler):.     
-00001810: 2020 2020 2020 2068 616e 646c 6572 2e65         handler.e
-00001820: 6d69 7420 3d20 7479 7065 732e 4d65 7468  mit = types.Meth
-00001830: 6f64 5479 7065 286c 6f67 6769 6e67 2e53  odType(logging.S
-00001840: 7472 6561 6d48 616e 646c 6572 2e65 6d69  treamHandler.emi
-00001850: 742c 2068 616e 646c 6572 290a 0a20 2020  t, handler)..   
-00001860: 206c 6f67 6769 6e67 2e53 7472 6561 6d48   logging.StreamH
-00001870: 616e 646c 6572 2e65 6d69 7420 3d20 6861  andler.emit = ha
-00001880: 636b 6564 5f65 6d69 740a 2020 2020 7265  cked_emit.    re
-00001890: 7475 726e 206f 6f62 615f 6c6f 6767 6572  turn ooba_logger
-000018a0: 0a0a 0a53 5441 5455 535f 5052 4546 4958  ...STATUS_PREFIX
-000018b0: 203d 2022 3c68 333e 4f6f 6261 626f 7420   = "<h3>Oobabot 
-000018c0: 5374 6174 7573 3c2f 6833 3e22 0a0a 0a64  Status</h3>"...d
-000018d0: 6566 2073 7461 7475 735f 6865 6164 696e  ef status_headin
-000018e0: 6728 7374 6174 7573 3a20 7374 7229 202d  g(status: str) -
-000018f0: 3e20 7374 723a 0a20 2020 2069 6620 7374  > str:.    if st
-00001900: 6174 7573 203d 3d20 2272 756e 6e69 6e67  atus == "running
-00001910: 223a 0a20 2020 2020 2020 2072 6574 7572  ":.        retur
-00001920: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-00001930: 5354 4154 5553 5f50 5245 4649 580a 2020  STATUS_PREFIX.  
-00001940: 2020 2020 2020 2020 2020 2b20 273c 6469            + '<di
-00001950: 7620 636c 6173 733d 226f 6f62 6162 6f74  v class="oobabot
-00001960: 5f73 7461 7475 7320 6f6f 6261 626f 745f  _status oobabot_
-00001970: 7374 6174 7573 5f72 756e 6e69 6e67 223e  status_running">
-00001980: 5275 6e6e 696e 673c 2f64 6976 3e27 0a20  Running</div>'. 
-00001990: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
-000019a0: 7374 6174 7573 203d 3d20 2273 746f 7070  status == "stopp
-000019b0: 6564 223a 0a20 2020 2020 2020 2072 6574  ed":.        ret
-000019c0: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
-000019d0: 2020 5354 4154 5553 5f50 5245 4649 580a    STATUS_PREFIX.
-000019e0: 2020 2020 2020 2020 2020 2020 2b20 273c              + '<
-000019f0: 6469 7620 636c 6173 733d 226f 6f62 6162  div class="oobab
-00001a00: 6f74 5f73 7461 7475 7320 6f6f 6261 626f  ot_status oobabo
-00001a10: 745f 7374 6174 7573 5f73 746f 7070 6564  t_status_stopped
-00001a20: 223e 5374 6f70 7065 643c 2f64 6976 3e27  ">Stopped</div>'
-00001a30: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
-00001a40: 6574 7572 6e20 5354 4154 5553 5f50 5245  eturn STATUS_PRE
-00001a50: 4649 580a                                FIX.
+000012c0: 0a0a 0a4f 5448 4552 5f48 4143 4b45 445f  ...OTHER_HACKED_
+000012d0: 4c4f 4747 494e 475f 4154 5452 4942 5554  LOGGING_ATTRIBUT
+000012e0: 4553 203d 205b 0a20 2020 2022 7761 726e  ES = [.    "warn
+000012f0: 696e 675f 6164 7669 6365 222c 0a20 2020  ing_advice",.   
+00001300: 2022 7761 726e 696e 675f 6f6e 6365 222c   "warning_once",
+00001310: 0a5d 0a0a 0a64 6566 2072 6570 6169 725f  .]...def repair_
+00001320: 6c6f 6767 696e 6728 2920 2d3e 2074 7970  logging() -> typ
+00001330: 696e 672e 4f70 7469 6f6e 616c 5b6c 6f67  ing.Optional[log
+00001340: 6769 6e67 2e4c 6f67 6765 725d 3a0a 2020  ging.Logger]:.  
+00001350: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+00001360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001370: 2323 2323 0a20 2020 2023 2073 6f2c 206c  ####.    # so, l
+00001380: 6f67 6769 6e67 5f63 6f6c 6f72 732e 7079  ogging_colors.py
+00001390: 2c20 7261 7468 6572 2074 6861 6e20 7573  , rather than us
+000013a0: 696e 6720 7468 6520 6c6f 6767 696e 6720  ing the logging 
+000013b0: 6d6f 6475 6c65 2773 2062 7569 6c74 2d69  module's built-i
+000013c0: 6e0a 2020 2020 2320 666f 726d 6174 7465  n.    # formatte
+000013d0: 722c 2069 7320 6d6f 6e6b 6579 2d70 6174  r, is monkey-pat
+000013e0: 6368 696e 6720 7468 6520 6c6f 6767 696e  ching the loggin
+000013f0: 6720 6d6f 6475 6c65 2773 2053 7472 6561  g module's Strea
+00001400: 6d48 616e 646c 6572 2e65 6d69 742e 0a20  mHandler.emit.. 
+00001410: 2020 2023 2054 6869 7320 6973 2061 2070     # This is a p
+00001420: 726f 626c 656d 2066 6f72 2075 732c 2062  roblem for us, b
+00001430: 6563 6175 7365 2077 6520 616c 736f 2075  ecause we also u
+00001440: 7365 2074 6865 206c 6f67 6769 6e67 206d  se the logging m
+00001450: 6f64 756c 652c 2062 7574 0a20 2020 2023  odule, but.    #
+00001460: 2064 6f6e 2774 2077 616e 7420 414e 5349   don't want ANSI
+00001470: 2063 6f6c 6f72 2063 6f64 6573 2073 686f   color codes sho
+00001480: 7769 6e67 2075 7020 696e 2048 544d 4c2e  wing up in HTML.
+00001490: 2020 5765 2061 6c73 6f20 646f 6e27 7420    We also don't 
+000014a0: 7761 6e74 0a20 2020 2023 2074 6f20 6272  want.    # to br
+000014b0: 6561 6b20 7468 6569 7220 6c6f 6767 696e  eak their loggin
+000014c0: 672e 0a20 2020 2023 0a20 2020 2023 2053  g..    #.    # S
+000014d0: 6f2c 2077 6527 7265 2067 6f69 6e67 2074  o, we're going t
+000014e0: 6f20 7361 7665 2074 6865 6972 206d 6f6e  o save their mon
+000014f0: 6b65 792d 7061 7463 6865 6420 656d 6974  key-patched emit
+00001500: 2c20 7265 6c6f 6164 2074 6865 206c 6f67  , reload the log
+00001510: 6769 6e67 0a20 2020 2023 206d 6f64 756c  ging.    # modul
+00001520: 652c 2073 6176 6520 6f66 6620 7468 6520  e, save off the 
+00001530: 2272 6561 6c22 2065 6d69 742c 2074 6865  "real" emit, the
+00001540: 6e20 7265 2d61 7070 6c79 2074 6865 6972  n re-apply their
+00001550: 206d 6f6e 6b65 792d 7061 7463 682e 0a20   monkey-patch.. 
+00001560: 2020 2023 0a20 2020 2023 2057 6520 6e65     #.    # We ne
+00001570: 6564 2074 6f20 646f 2061 6c6c 2074 6869  ed to do all thi
+00001580: 7320 6265 666f 7265 2077 6520 6372 6561  s before we crea
+00001590: 7465 2074 6865 206f 6f62 6162 6f74 5f77  te the oobabot_w
+000015a0: 6f72 6b65 722c 2073 6f20 7468 6174 0a20  orker, so that. 
+000015b0: 2020 2023 2074 6865 206c 6f67 7320 6372     # the logs cr
+000015c0: 6561 7465 6420 6475 7269 6e67 2073 7461  eated during sta
+000015d0: 7274 7570 2061 7265 2070 726f 7065 726c  rtup are properl
+000015e0: 7920 666f 726d 6174 7465 642e 0a0a 2020  y formatted...  
+000015f0: 2020 2320 7361 7665 2074 6865 206d 6f6e    # save the mon
+00001600: 6b65 792d 7061 7463 6865 6420 656d 6974  key-patched emit
+00001610: 0a20 2020 2068 6163 6b65 645f 656d 6974  .    hacked_emit
+00001620: 203d 206c 6f67 6769 6e67 2e53 7472 6561   = logging.Strea
+00001630: 6d48 616e 646c 6572 2e65 6d69 740a 2020  mHandler.emit.  
+00001640: 2020 7361 7665 645f 6861 636b 6564 5f61    saved_hacked_a
+00001650: 7474 7269 6275 7465 7320 3d20 7b7d 0a20  ttributes = {}. 
+00001660: 2020 2066 6f72 2061 7474 7220 696e 204f     for attr in O
+00001670: 5448 4552 5f48 4143 4b45 445f 4c4f 4747  THER_HACKED_LOGG
+00001680: 494e 475f 4154 5452 4942 5554 4553 3a0a  ING_ATTRIBUTES:.
+00001690: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+000016a0: 7472 286c 6f67 6769 6e67 2e4c 6f67 6765  tr(logging.Logge
+000016b0: 722c 2061 7474 7229 3a0a 2020 2020 2020  r, attr):.      
+000016c0: 2020 2020 2020 7361 7665 645f 6861 636b        saved_hack
+000016d0: 6564 5f61 7474 7269 6275 7465 735b 6174  ed_attributes[at
+000016e0: 7472 5d20 3d20 6765 7461 7474 7228 6c6f  tr] = getattr(lo
+000016f0: 6767 696e 672e 4c6f 6767 6572 2c20 6174  gging.Logger, at
+00001700: 7472 290a 0a20 2020 2023 2072 656c 6f61  tr)..    # reloa
+00001710: 6420 7468 6520 6c6f 6767 696e 6720 6d6f  d the logging mo
+00001720: 6475 6c65 0a20 2020 2074 7279 3a0a 2020  dule.    try:.  
+00001730: 2020 2020 2020 696d 706f 7274 6c69 622e        importlib.
+00001740: 7265 6c6f 6164 286c 6f67 6769 6e67 290a  reload(logging).
+00001750: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
+00001760: 7445 7272 6f72 2061 7320 6572 723a 0a20  tError as err:. 
+00001770: 2020 2020 2020 2070 7269 6e74 2866 224f         print(f"O
+00001780: 6f62 6162 6f74 3a20 4572 726f 7220 7265  obabot: Error re
+00001790: 6c6f 6164 696e 6720 6c6f 6767 696e 6720  loading logging 
+000017a0: 6d6f 6475 6c65 3a20 7b65 7272 7d22 2c20  module: {err}", 
+000017b0: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+000017c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000017d0: 4e6f 6e65 0a0a 2020 2020 2320 6372 6561  None..    # crea
+000017e0: 7465 206f 7572 206c 6f67 6765 7220 6561  te our logger ea
+000017f0: 726c 790a 2020 2020 6f6f 6261 626f 742e  rly.    oobabot.
+00001800: 6661 6e63 795f 6c6f 6767 6572 2e69 6e69  fancy_logger.ini
+00001810: 745f 6c6f 6767 696e 6728 6c6f 6767 696e  t_logging(loggin
+00001820: 672e 4445 4255 472c 2054 7275 6529 0a20  g.DEBUG, True). 
+00001830: 2020 206f 6f62 615f 6c6f 6767 6572 203d     ooba_logger =
+00001840: 206f 6f62 6162 6f74 2e66 616e 6379 5f6c   oobabot.fancy_l
+00001850: 6f67 6765 722e 6765 7428 290a 0a20 2020  ogger.get()..   
+00001860: 2023 206d 616e 7561 6c6c 7920 6170 706c   # manually appl
+00001870: 7920 7468 6520 2263 6f72 7265 6374 2220  y the "correct" 
+00001880: 656d 6974 2074 6f20 6561 6368 206f 6620  emit to each of 
+00001890: 7468 6520 5374 7265 616d 4861 6e64 6c65  the StreamHandle
+000018a0: 7273 0a20 2020 2023 2074 6861 7420 6661  rs.    # that fa
+000018b0: 6e63 795f 6c6f 6767 6572 2063 7265 6174  ncy_logger creat
+000018c0: 6564 0a20 2020 2066 6f72 2068 616e 646c  ed.    for handl
+000018d0: 6572 2069 6e20 6f6f 6261 5f6c 6f67 6765  er in ooba_logge
+000018e0: 722e 6861 6e64 6c65 7273 3a0a 2020 2020  r.handlers:.    
+000018f0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00001900: 6528 6861 6e64 6c65 722c 206c 6f67 6769  e(handler, loggi
+00001910: 6e67 2e53 7472 6561 6d48 616e 646c 6572  ng.StreamHandler
+00001920: 293a 0a20 2020 2020 2020 2020 2020 2068  ):.            h
+00001930: 616e 646c 6572 2e65 6d69 7420 3d20 7479  andler.emit = ty
+00001940: 7065 732e 4d65 7468 6f64 5479 7065 286c  pes.MethodType(l
+00001950: 6f67 6769 6e67 2e53 7472 6561 6d48 616e  ogging.StreamHan
+00001960: 646c 6572 2e65 6d69 742c 2068 616e 646c  dler.emit, handl
+00001970: 6572 290a 0a20 2020 206c 6f67 6769 6e67  er)..    logging
+00001980: 2e53 7472 6561 6d48 616e 646c 6572 2e65  .StreamHandler.e
+00001990: 6d69 7420 3d20 6861 636b 6564 5f65 6d69  mit = hacked_emi
+000019a0: 740a 2020 2020 2320 7265 7374 6f72 6520  t.    # restore 
+000019b0: 6f74 6865 7220 6861 636b 6564 2d6f 6e20  other hacked-on 
+000019c0: 6174 7472 6962 7574 6573 0a20 2020 2066  attributes.    f
+000019d0: 6f72 2061 7474 722c 2076 616c 7565 2069  or attr, value i
+000019e0: 6e20 7361 7665 645f 6861 636b 6564 5f61  n saved_hacked_a
+000019f0: 7474 7269 6275 7465 732e 6974 656d 7328  ttributes.items(
+00001a00: 293a 0a20 2020 2020 2020 2073 6574 6174  ):.        setat
+00001a10: 7472 286c 6f67 6769 6e67 2e4c 6f67 6765  tr(logging.Logge
+00001a20: 722c 2061 7474 722c 2076 616c 7565 290a  r, attr, value).
+00001a30: 0a20 2020 2072 6574 7572 6e20 6f6f 6261  .    return ooba
+00001a40: 5f6c 6f67 6765 720a 0a0a 5354 4154 5553  _logger...STATUS
+00001a50: 5f50 5245 4649 5820 3d20 223c 6833 3e4f  _PREFIX = "<h3>O
+00001a60: 6f62 6162 6f74 2053 7461 7475 733c 2f68  obabot Status</h
+00001a70: 333e 220a 0a0a 6465 6620 7374 6174 7573  3>"...def status
+00001a80: 5f68 6561 6469 6e67 2873 7461 7475 733a  _heading(status:
+00001a90: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+00001aa0: 2020 6966 2073 7461 7475 7320 3d3d 2022    if status == "
+00001ab0: 7275 6e6e 696e 6722 3a0a 2020 2020 2020  running":.      
+00001ac0: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
+00001ad0: 2020 2020 2020 2053 5441 5455 535f 5052         STATUS_PR
+00001ae0: 4546 4958 0a20 2020 2020 2020 2020 2020  EFIX.           
+00001af0: 202b 2027 3c64 6976 2063 6c61 7373 3d22   + '<div class="
+00001b00: 6f6f 6261 626f 745f 7374 6174 7573 206f  oobabot_status o
+00001b10: 6f62 6162 6f74 5f73 7461 7475 735f 7275  obabot_status_ru
+00001b20: 6e6e 696e 6722 3e52 756e 6e69 6e67 3c2f  nning">Running</
+00001b30: 6469 763e 270a 2020 2020 2020 2020 290a  div>'.        ).
+00001b40: 2020 2020 6966 2073 7461 7475 7320 3d3d      if status ==
+00001b50: 2022 7374 6f70 7065 6422 3a0a 2020 2020   "stopped":.    
+00001b60: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+00001b70: 2020 2020 2020 2020 2053 5441 5455 535f           STATUS_
+00001b80: 5052 4546 4958 0a20 2020 2020 2020 2020  PREFIX.         
+00001b90: 2020 202b 2027 3c64 6976 2063 6c61 7373     + '<div class
+00001ba0: 3d22 6f6f 6261 626f 745f 7374 6174 7573  ="oobabot_status
+00001bb0: 206f 6f62 6162 6f74 5f73 7461 7475 735f   oobabot_status_
+00001bc0: 7374 6f70 7065 6422 3e53 746f 7070 6564  stopped">Stopped
+00001bd0: 3c2f 6469 763e 270a 2020 2020 2020 2020  </div>'.        
+00001be0: 290a 2020 2020 7265 7475 726e 2053 5441  ).    return STA
+00001bf0: 5455 535f 5052 4546 4958 0a              TUS_PREFIX.
```

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/transcript_view.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/transcript_view.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/src/oobabot_plugin/worker.py` & `oobabot_plugin-0.2.2/src/oobabot_plugin/worker.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.1/PKG-INFO` & `oobabot_plugin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot-plugin
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot.
 Home-page: https://github.com/chrisrude/oobabot-plugin
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

