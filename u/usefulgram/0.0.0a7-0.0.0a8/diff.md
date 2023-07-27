# Comparing `tmp/usefulgram-0.0.0a7.tar.gz` & `tmp/usefulgram-0.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a7.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0a8.tar", max compression
```

## Comparing `usefulgram-0.0.0a7.tar` & `usefulgram-0.0.0a8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a7/LICENSE
--rw-r--r--   0        0        0      751 2023-07-27 00:55:19.909963 usefulgram-0.0.0a7/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a7/README.md
--rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a7/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a7/usefulgram/enums/__init__.py
--rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a7/usefulgram/enums/const.py
--rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a7/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a7/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a7/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a7/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a7/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a7/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0     3673 2023-07-27 00:54:59.805545 usefulgram-0.0.0a7/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a7/usefulgram/keyboard/buttons.py
--rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a7/usefulgram/keyboard/rows.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a7/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a7/usefulgram/lazy/editor.py
--rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a7/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a7/usefulgram/lazy/sender.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a7/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a7/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a7/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a7/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a7/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a7/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a7/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a8/LICENSE
+-rw-r--r--   0        0        0      751 2023-07-27 02:54:10.220194 usefulgram-0.0.0a8/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a8/README.md
+-rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a8/usefulgram/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a8/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a8/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a8/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a8/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a8/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a8/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a8/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a8/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0     3673 2023-07-27 00:54:59.805545 usefulgram-0.0.0a8/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a8/usefulgram/keyboard/buttons.py
+-rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a8/usefulgram/keyboard/rows.py
+-rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a8/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a8/usefulgram/lazy/editor.py
+-rw-r--r--   0        0        0     8253 2023-07-27 02:54:10.225180 usefulgram-0.0.0a8/usefulgram/lazy/lazy_editing.py
+-rw-r--r--   0        0        0     1756 2023-07-27 02:54:10.216965 usefulgram-0.0.0a8/usefulgram/lazy/sender.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a8/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a8/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a8/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a8/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a8/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a8/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a8/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a8/PKG-INFO
```

### Comparing `usefulgram-0.0.0a7/LICENSE` & `usefulgram-0.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/pyproject.toml` & `usefulgram-0.0.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a7"
+version = "0.0.0a8"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `usefulgram-0.0.0a7/README.md` & `usefulgram-0.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/exceptions/exceptions.py` & `usefulgram-0.0.0a8/usefulgram/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0a8/usefulgram/filters/database_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0a8/usefulgram/filters/parse_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/keyboard/builder.py` & `usefulgram-0.0.0a8/usefulgram/keyboard/builder.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/keyboard/buttons.py` & `usefulgram-0.0.0a8/usefulgram/keyboard/buttons.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/keyboard/rows.py` & `usefulgram-0.0.0a8/usefulgram/keyboard/rows.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/lazy/editor.py` & `usefulgram-0.0.0a8/usefulgram/lazy/editor.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/lazy/lazy_editing.py` & `usefulgram-0.0.0a8/usefulgram/lazy/lazy_editing.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,257 +263,254 @@
 00001060: 6f3a 204f 7074 696f 6e61 6c5b 4653 496e  o: Optional[FSIn
 00001070: 7075 7446 696c 655d 2c0d 0a20 2020 2020  putFile],..     
 00001080: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
 00001090: 6b75 703a 204f 7074 696f 6e61 6c5b 496e  kup: Optional[In
 000010a0: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
 000010b0: 7570 5d2c 0d0a 2020 2020 2020 2020 2020  up],..          
 000010c0: 2020 7061 7273 655f 6d6f 6465 3a20 556e    parse_mode: Un
-000010d0: 696f 6e5b 7374 722c 2055 4e53 4554 5f50  ion[str, UNSET_P
-000010e0: 4152 5345 5f4d 4f44 455d 2c0d 0a20 2020  ARSE_MODE],..   
-000010f0: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-00001100: 5f77 6562 5f70 6167 655f 7072 6576 6965  _web_page_previe
-00001110: 773a 2062 6f6f 6c2c 0d0a 2020 2020 2920  w: bool,..    ) 
-00001120: 2d3e 2055 6e69 6f6e 5b4d 6573 7361 6765  -> Union[Message
-00001130: 2c20 626f 6f6c 5d3a 0d0a 0d0a 2020 2020  , bool]:....    
-00001140: 2020 2020 6966 206e 6f74 2063 616e 5f65      if not can_e
-00001150: 6469 743a 0d0a 2020 2020 2020 2020 2020  dit:..          
-00001160: 2020 7465 7874 203d 204c 617a 7945 6469    text = LazyEdi
-00001170: 7469 6e67 2e5f 6765 745f 6d65 7373 6167  ting._get_messag
-00001180: 655f 7465 7874 2874 6578 742c 206d 6573  e_text(text, mes
-00001190: 7361 6765 3d6d 6573 7361 6765 290d 0a0d  sage=message)...
-000011a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000011b0: 7572 6e20 6177 6169 7420 4d65 7373 6167  urn await Messag
-000011c0: 6553 656e 6465 722e 7365 6e64 280d 0a20  eSender.send(.. 
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000011e0: 6f74 3d62 6f74 2c0d 0a20 2020 2020 2020  ot=bot,..       
-000011f0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00001200: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
-00001210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001220: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-00001230: 645f 6964 3d6d 6573 7361 6765 2e6d 6573  d_id=message.mes
-00001240: 7361 6765 5f74 6872 6561 645f 6964 2c0d  sage_thread_id,.
-00001250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001260: 2074 6578 743d 7465 7874 2c0d 0a20 2020   text=text,..   
-00001270: 2020 2020 2020 2020 2020 2020 2070 686f               pho
-00001280: 746f 3d70 686f 746f 2c0d 0a20 2020 2020  to=photo,..     
-00001290: 2020 2020 2020 2020 2020 2076 6964 656f             video
-000012a0: 3d76 6964 656f 2c0d 0a20 2020 2020 2020  =video,..       
-000012b0: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
-000012c0: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
-000012d0: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
-000012e0: 2020 2020 2070 6172 7365 5f6d 6f64 653d       parse_mode=
-000012f0: 7061 7273 655f 6d6f 6465 2c0d 0a20 2020  parse_mode,..   
-00001300: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00001310: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
-00001320: 6576 6965 773d 6469 7361 626c 655f 7765  eview=disable_we
-00001330: 625f 7061 6765 5f70 7265 7669 6577 0d0a  b_page_preview..
-00001340: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-00001350: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001360: 6177 6169 7420 4d65 7373 6167 6545 6469  await MessageEdi
-00001370: 746f 722e 6564 6974 280d 0a20 2020 2020  tor.edit(..     
-00001380: 2020 2020 2020 2062 6f74 3d62 6f74 2c0d         bot=bot,.
-00001390: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-000013a0: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
-000013b0: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
-000013c0: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
-000013d0: 7373 6167 652e 6d65 7373 6167 655f 6964  ssage.message_id
-000013e0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-000013f0: 6578 743d 7465 7874 2c0d 0a20 2020 2020  ext=text,..     
-00001400: 2020 2020 2020 2070 686f 746f 3d70 686f         photo=pho
-00001410: 746f 2c0d 0a20 2020 2020 2020 2020 2020  to,..           
-00001420: 2076 6964 656f 3d76 6964 656f 2c0d 0a20   video=video,.. 
-00001430: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00001440: 5f6d 6172 6b75 703d 7265 706c 795f 6d61  _markup=reply_ma
-00001450: 726b 7570 2c0d 0a20 2020 2020 2020 2020  rkup,..         
-00001460: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
-00001470: 7273 655f 6d6f 6465 2c0d 0a20 2020 2020  rse_mode,..     
-00001480: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
-00001490: 6562 5f70 6167 655f 7072 6576 6965 773d  eb_page_preview=
-000014a0: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
-000014b0: 5f70 7265 7669 6577 0d0a 2020 2020 2020  _preview..      
-000014c0: 2020 290d 0a0d 0a20 2020 2064 6566 205f    )....    def _
-000014d0: 6765 745f 6361 6e5f 6564 6974 5f73 7461  get_can_edit_sta
-000014e0: 7475 7328 0d0a 2020 2020 2020 2020 2020  tus(..          
-000014f0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00001500: 2020 2020 206d 6573 7361 6765 3a20 4d65       message: Me
-00001510: 7373 6167 652c 0d0a 2020 2020 2020 2020  ssage,..        
-00001520: 2020 2020 7068 6f74 6f3a 204f 7074 696f      photo: Optio
-00001530: 6e61 6c5b 4653 496e 7075 7446 696c 655d  nal[FSInputFile]
-00001540: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-00001550: 6964 656f 3a20 4f70 7469 6f6e 616c 5b46  ideo: Optional[F
-00001560: 5349 6e70 7574 4669 6c65 5d2c 0d0a 2020  SInputFile],..  
-00001570: 2020 2920 2d3e 2062 6f6f 6c3a 0d0a 0d0a    ) -> bool:....
-00001580: 2020 2020 2020 2020 6966 206d 6573 7361          if messa
-00001590: 6765 2069 7320 4e6f 6e65 3a0d 0a20 2020  ge is None:..   
-000015a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000015b0: 4661 6c73 650d 0a0d 0a20 2020 2020 2020  False....       
-000015c0: 2069 6620 6e6f 7420 7365 6c66 2e5f 6765   if not self._ge
-000015d0: 745f 626f 745f 616c 6c6f 775f 6564 6974  t_bot_allow_edit
-000015e0: 5f73 7461 7475 7328 0d0a 2020 2020 2020  _status(..      
-000015f0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00001600: 653d 6d65 7373 6167 652c 0d0a 2020 2020  e=message,..    
-00001610: 2020 2020 2020 2020 2020 2020 7068 6f74              phot
-00001620: 6f3d 7068 6f74 6f2c 0d0a 2020 2020 2020  o=photo,..      
-00001630: 2020 2020 2020 2020 2020 7669 6465 6f3d            video=
-00001640: 7669 6465 6f0d 0a20 2020 2020 2020 2029  video..        )
-00001650: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001660: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-00001670: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00001680: 7565 0d0a 0d0a 2020 2020 4073 7461 7469  ue....    @stati
-00001690: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
-000016a0: 205f 6765 745f 7374 6162 6c65 5f77 6169   _get_stable_wai
-000016b0: 745f 7469 6d65 286d 6573 7361 6765 3a20  t_time(message: 
-000016c0: 4d65 7373 6167 6529 202d 3e20 666c 6f61  Message) -> floa
-000016d0: 743a 0d0a 2020 2020 2020 2020 6966 206d  t:..        if m
-000016e0: 6573 7361 6765 2e65 6469 745f 6461 7465  essage.edit_date
-000016f0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-00001700: 7420 3d20 6461 7465 7469 6d65 2e66 726f  t = datetime.fro
-00001710: 6d74 696d 6573 7461 6d70 286d 6573 7361  mtimestamp(messa
-00001720: 6765 2e65 6469 745f 6461 7465 2c20 747a  ge.edit_date, tz
-00001730: 3d70 7974 7a2e 5554 4329 0d0a 0d0a 2020  =pytz.UTC)....  
-00001740: 2020 2020 2020 2020 2020 6465 6c74 6120            delta 
-00001750: 3d20 4c61 7a79 4564 6974 696e 672e 5f67  = LazyEditing._g
-00001760: 6574 5f74 696d 655f 6265 7477 6565 6e5f  et_time_between_
-00001770: 6375 7272 656e 745f 616e 645f 6d65 7373  current_and_mess
-00001780: 6167 6528 0d0a 2020 2020 2020 2020 2020  age(..          
-00001790: 2020 2020 2020 6d65 7373 6167 655f 6461        message_da
-000017a0: 7465 3d64 740d 0a20 2020 2020 2020 2020  te=dt..         
-000017b0: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
-000017c0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000017d0: 2064 656c 7461 203d 204c 617a 7945 6469   delta = LazyEdi
-000017e0: 7469 6e67 2e5f 6765 745f 7469 6d65 5f62  ting._get_time_b
-000017f0: 6574 7765 656e 5f63 7572 7265 6e74 5f61  etween_current_a
-00001800: 6e64 5f6d 6573 7361 6765 280d 0a20 2020  nd_message(..   
-00001810: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00001820: 7361 6765 5f64 6174 653d 6d65 7373 6167  sage_date=messag
-00001830: 652e 6461 7465 0d0a 2020 2020 2020 2020  e.date..        
-00001840: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-00001850: 2074 6f74 616c 5f73 6563 6f6e 6473 203d   total_seconds =
-00001860: 2064 656c 7461 2e74 6f74 616c 5f73 6563   delta.total_sec
-00001870: 6f6e 6473 2829 0d0a 0d0a 2020 2020 2020  onds()....      
-00001880: 2020 7761 6974 5f74 696d 6520 3d20 436f    wait_time = Co
-00001890: 6e73 742e 5354 4142 4c45 5f57 4149 545f  nst.STABLE_WAIT_
-000018a0: 5449 4d45 5f53 4543 4f4e 4453 202d 2074  TIME_SECONDS - t
-000018b0: 6f74 616c 5f73 6563 6f6e 6473 0d0a 2020  otal_seconds..  
-000018c0: 2020 2020 2020 7265 7475 726e 2072 6f75        return rou
-000018d0: 6e64 2877 6169 745f 7469 6d65 2c20 3329  nd(wait_time, 3)
-000018e0: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-000018f0: 6620 6564 6974 280d 0a20 2020 2020 2020  f edit(..       
-00001900: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00001910: 2020 2020 2020 2020 7465 7874 3a20 4f70          text: Op
-00001920: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00001930: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00001940: 2070 686f 746f 3a20 4f70 7469 6f6e 616c   photo: Optional
-00001950: 5b46 5349 6e70 7574 4669 6c65 5d20 3d20  [FSInputFile] = 
-00001960: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-00001970: 2020 2076 6964 656f 3a20 4f70 7469 6f6e     video: Option
-00001980: 616c 5b46 5349 6e70 7574 4669 6c65 5d20  al[FSInputFile] 
-00001990: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000019a0: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
-000019b0: 703a 204f 7074 696f 6e61 6c5b 496e 6c69  p: Optional[Inli
-000019c0: 6e65 4b65 7962 6f61 7264 4d61 726b 7570  neKeyboardMarkup
-000019d0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-000019e0: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
-000019f0: 653a 2055 6e69 6f6e 5b73 7472 2c20 554e  e: Union[str, UN
-00001a00: 5345 545f 5041 5253 455f 4d4f 4445 5d20  SET_PARSE_MODE] 
-00001a10: 3d20 554e 5345 545f 5041 5253 455f 4d4f  = UNSET_PARSE_MO
-00001a20: 4445 2c0d 0a20 2020 2020 2020 2020 2020  DE,..           
-00001a30: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
-00001a40: 655f 7072 6576 6965 773a 2062 6f6f 6c20  e_preview: bool 
-00001a50: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00001a60: 2020 2020 2020 616e 7377 6572 5f74 6578        answer_tex
-00001a70: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-00001a80: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00001a90: 2020 2020 2020 616e 7377 6572 5f73 686f        answer_sho
-00001aa0: 775f 616c 6572 743a 2062 6f6f 6c20 3d20  w_alert: bool = 
-00001ab0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00001ac0: 2020 2020 6175 746f 616e 7377 6572 3a20      autoanswer: 
-00001ad0: 626f 6f6c 203d 2054 7275 650d 0a20 2020  bool = True..   
-00001ae0: 2029 202d 3e20 556e 696f 6e5b 4d65 7373   ) -> Union[Mess
-00001af0: 6167 652c 2062 6f6f 6c5d 3a0d 0a0d 0a20  age, bool]:.... 
-00001b00: 2020 2020 2020 2063 616c 6c62 6163 6b20         callback 
-00001b10: 3d20 7365 6c66 2e63 616c 6c62 6163 6b0d  = self.callback.
-00001b20: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00001b30: 203d 2063 616c 6c62 6163 6b2e 6d65 7373   = callback.mess
-00001b40: 6167 650d 0a0d 0a20 2020 2020 2020 2069  age....        i
-00001b50: 6620 6d65 7373 6167 6520 6973 204e 6f6e  f message is Non
-00001b60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001b70: 6177 6169 7420 6361 6c6c 6261 636b 2e61  await callback.a
-00001b80: 6e73 7765 7228 224d 6573 7361 6765 2074  nswer("Message t
-00001b90: 6f6f 206f 6c64 2229 0d0a 0d0a 2020 2020  oo old")....    
-00001ba0: 2020 2020 2020 2020 7261 6973 6520 4d65          raise Me
-00001bb0: 7373 6167 6554 6f6f 4f6c 640d 0a0d 0a20  ssageTooOld.... 
-00001bc0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00001bd0: 7461 626c 653a 0d0a 2020 2020 2020 2020  table:..        
-00001be0: 2020 2020 6177 6169 7420 6173 796e 6369      await asynci
-00001bf0: 6f2e 736c 6565 7028 7365 6c66 2e5f 6765  o.sleep(self._ge
-00001c00: 745f 7374 6162 6c65 5f77 6169 745f 7469  t_stable_wait_ti
-00001c10: 6d65 286d 6573 7361 6765 2929 0d0a 0d0a  me(message))....
-00001c20: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00001c30: 656c 662e 5f67 6574 5f64 6174 615f 6368  elf._get_data_ch
-00001c40: 616e 6765 735f 7374 6174 7573 280d 0a20  anges_status(.. 
-00001c50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001c60: 6573 7361 6765 3d6d 6573 7361 6765 2c0d  essage=message,.
-00001c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c80: 2074 6578 743d 7465 7874 2c0d 0a20 2020   text=text,..   
-00001c90: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00001ca0: 6c79 5f6d 6172 6b75 703d 7265 706c 795f  ly_markup=reply_
-00001cb0: 6d61 726b 7570 2c0d 0a20 2020 2020 2020  markup,..       
-00001cc0: 2020 2020 2020 2020 2076 6964 656f 3d76           video=v
-00001cd0: 6964 656f 2c0d 0a20 2020 2020 2020 2020  ideo,..         
-00001ce0: 2020 2020 2020 2070 686f 746f 3d70 686f         photo=pho
-00001cf0: 746f 0d0a 2020 2020 2020 2020 293a 0d0a  to..        ):..
-00001d00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001d10: 726e 206d 6573 7361 6765 0d0a 0d0a 2020  rn message....  
-00001d20: 2020 2020 2020 6361 6e5f 6564 6974 203d        can_edit =
-00001d30: 2073 656c 662e 5f67 6574 5f63 616e 5f65   self._get_can_e
-00001d40: 6469 745f 7374 6174 7573 280d 0a20 2020  dit_status(..   
-00001d50: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00001d60: 3d6d 6573 7361 6765 2c0d 0a20 2020 2020  =message,..     
-00001d70: 2020 2020 2020 2070 686f 746f 3d70 686f         photo=pho
-00001d80: 746f 2c0d 0a20 2020 2020 2020 2020 2020  to,..           
-00001d90: 2076 6964 656f 3d76 6964 656f 2c0d 0a20   video=video,.. 
-00001da0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00001db0: 2020 2020 7265 7375 6c74 203d 2061 7761      result = awa
-00001dc0: 6974 2073 656c 662e 5f73 656e 645f 6f72  it self._send_or
-00001dd0: 5f65 6469 7428 0d0a 2020 2020 2020 2020  _edit(..        
-00001de0: 2020 2020 626f 743d 7365 6c66 2e62 6f74      bot=self.bot
-00001df0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00001e00: 616e 5f65 6469 743d 6361 6e5f 6564 6974  an_edit=can_edit
-00001e10: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00001e20: 6573 7361 6765 3d6d 6573 7361 6765 2c0d  essage=message,.
-00001e30: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00001e40: 743d 7465 7874 2c0d 0a20 2020 2020 2020  t=text,..       
-00001e50: 2020 2020 2070 686f 746f 3d70 686f 746f       photo=photo
-00001e60: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-00001e70: 6964 656f 3d76 6964 656f 2c0d 0a20 2020  ideo=video,..   
-00001e80: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
-00001e90: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
-00001ea0: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
-00001eb0: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
-00001ec0: 655f 6d6f 6465 2c0d 0a20 2020 2020 2020  e_mode,..       
-00001ed0: 2020 2020 2064 6973 6162 6c65 5f77 6562       disable_web
-00001ee0: 5f70 6167 655f 7072 6576 6965 773d 6469  _page_preview=di
-00001ef0: 7361 626c 655f 7765 625f 7061 6765 5f70  sable_web_page_p
-00001f00: 7265 7669 6577 2c0d 0a20 2020 2020 2020  review,..       
-00001f10: 2029 0d0a 0d0a 2020 2020 2020 2020 6177   )....        aw
-00001f20: 6169 7420 6173 796e 6369 6f2e 736c 6565  ait asyncio.slee
-00001f30: 7028 436f 6e73 742e 5345 434f 4e44 535f  p(Const.SECONDS_
-00001f40: 4245 5457 4545 4e5f 4f50 4552 4154 494f  BETWEEN_OPERATIO
-00001f50: 4e29 0d0a 0d0a 2020 2020 2020 2020 6177  N)....        aw
-00001f60: 6169 7420 7365 6c66 2e5f 6175 746f 5f63  ait self._auto_c
-00001f70: 616c 6c62 6163 6b5f 616e 7377 6572 280d  allback_answer(.
-00001f80: 0a20 2020 2020 2020 2020 2020 2062 6f74  .            bot
-00001f90: 3d73 656c 662e 626f 742c 0d0a 2020 2020  =self.bot,..    
-00001fa0: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
-00001fb0: 5f69 643d 6361 6c6c 6261 636b 2e69 642c  _id=callback.id,
-00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 6175  ..            au
-00001fd0: 746f 616e 7377 6572 3d61 7574 6f61 6e73  toanswer=autoans
-00001fe0: 7765 722c 0d0a 2020 2020 2020 2020 2020  wer,..          
-00001ff0: 2020 616e 7377 6572 5f74 6578 743d 616e    answer_text=an
-00002000: 7377 6572 5f74 6578 742c 0d0a 2020 2020  swer_text,..    
-00002010: 2020 2020 2020 2020 616e 7377 6572 5f73          answer_s
-00002020: 686f 775f 616c 6572 743d 616e 7377 6572  how_alert=answer
-00002030: 5f73 686f 775f 616c 6572 740d 0a20 2020  _show_alert..   
-00002040: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-00002050: 2020 7265 7475 726e 2072 6573 756c 740d    return result.
-00002060: 0a                                       .
+000010d0: 696f 6e5b 7374 725d 2c0d 0a20 2020 2020  ion[str],..     
+000010e0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+000010f0: 6562 5f70 6167 655f 7072 6576 6965 773a  eb_page_preview:
+00001100: 2062 6f6f 6c2c 0d0a 2020 2020 2920 2d3e   bool,..    ) ->
+00001110: 2055 6e69 6f6e 5b4d 6573 7361 6765 2c20   Union[Message, 
+00001120: 626f 6f6c 5d3a 0d0a 0d0a 2020 2020 2020  bool]:....      
+00001130: 2020 6966 206e 6f74 2063 616e 5f65 6469    if not can_edi
+00001140: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00001150: 7465 7874 203d 204c 617a 7945 6469 7469  text = LazyEditi
+00001160: 6e67 2e5f 6765 745f 6d65 7373 6167 655f  ng._get_message_
+00001170: 7465 7874 2874 6578 742c 206d 6573 7361  text(text, messa
+00001180: 6765 3d6d 6573 7361 6765 290d 0a0d 0a20  ge=message).... 
+00001190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000011a0: 6e20 6177 6169 7420 4d65 7373 6167 6553  n await MessageS
+000011b0: 656e 6465 722e 7365 6e64 280d 0a20 2020  ender.send(..   
+000011c0: 2020 2020 2020 2020 2020 2020 2062 6f74               bot
+000011d0: 3d62 6f74 2c0d 0a20 2020 2020 2020 2020  =bot,..         
+000011e0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
+000011f0: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
+00001200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001210: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+00001220: 6964 3d6d 6573 7361 6765 2e6d 6573 7361  id=message.messa
+00001230: 6765 5f74 6872 6561 645f 6964 2c0d 0a20  ge_thread_id,.. 
+00001240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001250: 6578 743d 7465 7874 2c0d 0a20 2020 2020  ext=text,..     
+00001260: 2020 2020 2020 2020 2020 2070 686f 746f             photo
+00001270: 3d70 686f 746f 2c0d 0a20 2020 2020 2020  =photo,..       
+00001280: 2020 2020 2020 2020 2076 6964 656f 3d76           video=v
+00001290: 6964 656f 2c0d 0a20 2020 2020 2020 2020  ideo,..         
+000012a0: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+000012b0: 6b75 703d 7265 706c 795f 6d61 726b 7570  kup=reply_markup
+000012c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000012d0: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
+000012e0: 7273 655f 6d6f 6465 2c0d 0a20 2020 2020  rse_mode,..     
+000012f0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+00001300: 6c65 5f77 6562 5f70 6167 655f 7072 6576  le_web_page_prev
+00001310: 6965 773d 6469 7361 626c 655f 7765 625f  iew=disable_web_
+00001320: 7061 6765 5f70 7265 7669 6577 0d0a 2020  page_preview..  
+00001330: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00001340: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00001350: 6169 7420 4d65 7373 6167 6545 6469 746f  ait MessageEdito
+00001360: 722e 6564 6974 280d 0a20 2020 2020 2020  r.edit(..       
+00001370: 2020 2020 2062 6f74 3d62 6f74 2c0d 0a20       bot=bot,.. 
+00001380: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00001390: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
+000013a0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+000013b0: 206d 6573 7361 6765 5f69 643d 6d65 7373   message_id=mess
+000013c0: 6167 652e 6d65 7373 6167 655f 6964 2c0d  age.message_id,.
+000013d0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+000013e0: 743d 7465 7874 2c0d 0a20 2020 2020 2020  t=text,..       
+000013f0: 2020 2020 2070 686f 746f 3d70 686f 746f       photo=photo
+00001400: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00001410: 6964 656f 3d76 6964 656f 2c0d 0a20 2020  ideo=video,..   
+00001420: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+00001430: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+00001440: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
+00001450: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
+00001460: 655f 6d6f 6465 2c0d 0a20 2020 2020 2020  e_mode,..       
+00001470: 2020 2020 2064 6973 6162 6c65 5f77 6562       disable_web
+00001480: 5f70 6167 655f 7072 6576 6965 773d 6469  _page_preview=di
+00001490: 7361 626c 655f 7765 625f 7061 6765 5f70  sable_web_page_p
+000014a0: 7265 7669 6577 0d0a 2020 2020 2020 2020  review..        
+000014b0: 290d 0a0d 0a20 2020 2064 6566 205f 6765  )....    def _ge
+000014c0: 745f 6361 6e5f 6564 6974 5f73 7461 7475  t_can_edit_statu
+000014d0: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+000014e0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+000014f0: 2020 206d 6573 7361 6765 3a20 4d65 7373     message: Mess
+00001500: 6167 652c 0d0a 2020 2020 2020 2020 2020  age,..          
+00001510: 2020 7068 6f74 6f3a 204f 7074 696f 6e61    photo: Optiona
+00001520: 6c5b 4653 496e 7075 7446 696c 655d 2c0d  l[FSInputFile],.
+00001530: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
+00001540: 656f 3a20 4f70 7469 6f6e 616c 5b46 5349  eo: Optional[FSI
+00001550: 6e70 7574 4669 6c65 5d2c 0d0a 2020 2020  nputFile],..    
+00001560: 2920 2d3e 2062 6f6f 6c3a 0d0a 0d0a 2020  ) -> bool:....  
+00001570: 2020 2020 2020 6966 206d 6573 7361 6765        if message
+00001580: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00001590: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000015a0: 6c73 650d 0a0d 0a20 2020 2020 2020 2069  lse....        i
+000015b0: 6620 6e6f 7420 7365 6c66 2e5f 6765 745f  f not self._get_
+000015c0: 626f 745f 616c 6c6f 775f 6564 6974 5f73  bot_allow_edit_s
+000015d0: 7461 7475 7328 0d0a 2020 2020 2020 2020  tatus(..        
+000015e0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+000015f0: 6d65 7373 6167 652c 0d0a 2020 2020 2020  message,..      
+00001600: 2020 2020 2020 2020 2020 7068 6f74 6f3d            photo=
+00001610: 7068 6f74 6f2c 0d0a 2020 2020 2020 2020  photo,..        
+00001620: 2020 2020 2020 2020 7669 6465 6f3d 7669          video=vi
+00001630: 6465 6f0d 0a20 2020 2020 2020 2029 3a0d  deo..        ):.
+00001640: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00001650: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+00001660: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00001670: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00001680: 6574 686f 640d 0a20 2020 2064 6566 205f  ethod..    def _
+00001690: 6765 745f 7374 6162 6c65 5f77 6169 745f  get_stable_wait_
+000016a0: 7469 6d65 286d 6573 7361 6765 3a20 4d65  time(message: Me
+000016b0: 7373 6167 6529 202d 3e20 666c 6f61 743a  ssage) -> float:
+000016c0: 0d0a 2020 2020 2020 2020 6966 206d 6573  ..        if mes
+000016d0: 7361 6765 2e65 6469 745f 6461 7465 3a0d  sage.edit_date:.
+000016e0: 0a20 2020 2020 2020 2020 2020 2064 7420  .            dt 
+000016f0: 3d20 6461 7465 7469 6d65 2e66 726f 6d74  = datetime.fromt
+00001700: 696d 6573 7461 6d70 286d 6573 7361 6765  imestamp(message
+00001710: 2e65 6469 745f 6461 7465 2c20 747a 3d70  .edit_date, tz=p
+00001720: 7974 7a2e 5554 4329 0d0a 0d0a 2020 2020  ytz.UTC)....    
+00001730: 2020 2020 2020 2020 6465 6c74 6120 3d20          delta = 
+00001740: 4c61 7a79 4564 6974 696e 672e 5f67 6574  LazyEditing._get
+00001750: 5f74 696d 655f 6265 7477 6565 6e5f 6375  _time_between_cu
+00001760: 7272 656e 745f 616e 645f 6d65 7373 6167  rrent_and_messag
+00001770: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+00001780: 2020 2020 6d65 7373 6167 655f 6461 7465      message_date
+00001790: 3d64 740d 0a20 2020 2020 2020 2020 2020  =dt..           
+000017a0: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
+000017b0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000017c0: 656c 7461 203d 204c 617a 7945 6469 7469  elta = LazyEditi
+000017d0: 6e67 2e5f 6765 745f 7469 6d65 5f62 6574  ng._get_time_bet
+000017e0: 7765 656e 5f63 7572 7265 6e74 5f61 6e64  ween_current_and
+000017f0: 5f6d 6573 7361 6765 280d 0a20 2020 2020  _message(..     
+00001800: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001810: 6765 5f64 6174 653d 6d65 7373 6167 652e  ge_date=message.
+00001820: 6461 7465 0d0a 2020 2020 2020 2020 2020  date..          
+00001830: 2020 290d 0a0d 0a20 2020 2020 2020 2074    )....        t
+00001840: 6f74 616c 5f73 6563 6f6e 6473 203d 2064  otal_seconds = d
+00001850: 656c 7461 2e74 6f74 616c 5f73 6563 6f6e  elta.total_secon
+00001860: 6473 2829 0d0a 0d0a 2020 2020 2020 2020  ds()....        
+00001870: 7761 6974 5f74 696d 6520 3d20 436f 6e73  wait_time = Cons
+00001880: 742e 5354 4142 4c45 5f57 4149 545f 5449  t.STABLE_WAIT_TI
+00001890: 4d45 5f53 4543 4f4e 4453 202d 2074 6f74  ME_SECONDS - tot
+000018a0: 616c 5f73 6563 6f6e 6473 0d0a 2020 2020  al_seconds..    
+000018b0: 2020 2020 7265 7475 726e 2072 6f75 6e64      return round
+000018c0: 2877 6169 745f 7469 6d65 2c20 3329 0d0a  (wait_time, 3)..
+000018d0: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+000018e0: 6564 6974 280d 0a20 2020 2020 2020 2020  edit(..         
+000018f0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+00001900: 2020 2020 2020 7465 7874 3a20 4f70 7469        text: Opti
+00001910: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00001920: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00001930: 686f 746f 3a20 4f70 7469 6f6e 616c 5b46  hoto: Optional[F
+00001940: 5349 6e70 7574 4669 6c65 5d20 3d20 4e6f  SInputFile] = No
+00001950: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00001960: 2076 6964 656f 3a20 4f70 7469 6f6e 616c   video: Optional
+00001970: 5b46 5349 6e70 7574 4669 6c65 5d20 3d20  [FSInputFile] = 
+00001980: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00001990: 2020 2072 6570 6c79 5f6d 6172 6b75 703a     reply_markup:
+000019a0: 204f 7074 696f 6e61 6c5b 496e 6c69 6e65   Optional[Inline
+000019b0: 4b65 7962 6f61 7264 4d61 726b 7570 5d20  KeyboardMarkup] 
+000019c0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+000019d0: 2020 2020 2070 6172 7365 5f6d 6f64 653a       parse_mode:
+000019e0: 2055 6e69 6f6e 5b73 7472 5d20 3d20 554e   Union[str] = UN
+000019f0: 5345 545f 5041 5253 455f 4d4f 4445 2c0d  SET_PARSE_MODE,.
+00001a00: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00001a10: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
+00001a20: 6576 6965 773a 2062 6f6f 6c20 3d20 4661  eview: bool = Fa
+00001a30: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00001a40: 2020 616e 7377 6572 5f74 6578 743a 204f    answer_text: O
+00001a50: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00001a60: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00001a70: 2020 616e 7377 6572 5f73 686f 775f 616c    answer_show_al
+00001a80: 6572 743a 2062 6f6f 6c20 3d20 4661 6c73  ert: bool = Fals
+00001a90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00001aa0: 6175 746f 616e 7377 6572 3a20 626f 6f6c  autoanswer: bool
+00001ab0: 203d 2054 7275 650d 0a20 2020 2029 202d   = True..    ) -
+00001ac0: 3e20 556e 696f 6e5b 4d65 7373 6167 652c  > Union[Message,
+00001ad0: 2062 6f6f 6c5d 3a0d 0a0d 0a20 2020 2020   bool]:....     
+00001ae0: 2020 2063 616c 6c62 6163 6b20 3d20 7365     callback = se
+00001af0: 6c66 2e63 616c 6c62 6163 6b0d 0a20 2020  lf.callback..   
+00001b00: 2020 2020 206d 6573 7361 6765 203d 2063       message = c
+00001b10: 616c 6c62 6163 6b2e 6d65 7373 6167 650d  allback.message.
+00001b20: 0a0d 0a20 2020 2020 2020 2069 6620 6d65  ...        if me
+00001b30: 7373 6167 6520 6973 204e 6f6e 653a 0d0a  ssage is None:..
+00001b40: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00001b50: 7420 6361 6c6c 6261 636b 2e61 6e73 7765  t callback.answe
+00001b60: 7228 224d 6573 7361 6765 2074 6f6f 206f  r("Message too o
+00001b70: 6c64 2229 0d0a 0d0a 2020 2020 2020 2020  ld")....        
+00001b80: 2020 2020 7261 6973 6520 4d65 7373 6167      raise Messag
+00001b90: 6554 6f6f 4f6c 640d 0a0d 0a20 2020 2020  eTooOld....     
+00001ba0: 2020 2069 6620 7365 6c66 2e73 7461 626c     if self.stabl
+00001bb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001bc0: 6177 6169 7420 6173 796e 6369 6f2e 736c  await asyncio.sl
+00001bd0: 6565 7028 7365 6c66 2e5f 6765 745f 7374  eep(self._get_st
+00001be0: 6162 6c65 5f77 6169 745f 7469 6d65 286d  able_wait_time(m
+00001bf0: 6573 7361 6765 2929 0d0a 0d0a 2020 2020  essage))....    
+00001c00: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00001c10: 5f67 6574 5f64 6174 615f 6368 616e 6765  _get_data_change
+00001c20: 735f 7374 6174 7573 280d 0a20 2020 2020  s_status(..     
+00001c30: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001c40: 6765 3d6d 6573 7361 6765 2c0d 0a20 2020  ge=message,..   
+00001c50: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+00001c60: 743d 7465 7874 2c0d 0a20 2020 2020 2020  t=text,..       
+00001c70: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+00001c80: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+00001c90: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
+00001ca0: 2020 2020 2076 6964 656f 3d76 6964 656f       video=video
+00001cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001cc0: 2020 2070 686f 746f 3d70 686f 746f 0d0a     photo=photo..
+00001cd0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+00001ce0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+00001cf0: 6573 7361 6765 0d0a 0d0a 2020 2020 2020  essage....      
+00001d00: 2020 6361 6e5f 6564 6974 203d 2073 656c    can_edit = sel
+00001d10: 662e 5f67 6574 5f63 616e 5f65 6469 745f  f._get_can_edit_
+00001d20: 7374 6174 7573 280d 0a20 2020 2020 2020  status(..       
+00001d30: 2020 2020 206d 6573 7361 6765 3d6d 6573       message=mes
+00001d40: 7361 6765 2c0d 0a20 2020 2020 2020 2020  sage,..         
+00001d50: 2020 2070 686f 746f 3d70 686f 746f 2c0d     photo=photo,.
+00001d60: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
+00001d70: 656f 3d76 6964 656f 2c0d 0a20 2020 2020  eo=video,..     
+00001d80: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00001d90: 7265 7375 6c74 203d 2061 7761 6974 2073  result = await s
+00001da0: 656c 662e 5f73 656e 645f 6f72 5f65 6469  elf._send_or_edi
+00001db0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00001dc0: 626f 743d 7365 6c66 2e62 6f74 2c0d 0a20  bot=self.bot,.. 
+00001dd0: 2020 2020 2020 2020 2020 2063 616e 5f65             can_e
+00001de0: 6469 743d 6361 6e5f 6564 6974 2c0d 0a20  dit=can_edit,.. 
+00001df0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001e00: 6765 3d6d 6573 7361 6765 2c0d 0a20 2020  ge=message,..   
+00001e10: 2020 2020 2020 2020 2074 6578 743d 7465           text=te
+00001e20: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+00001e30: 2070 686f 746f 3d70 686f 746f 2c0d 0a20   photo=photo,.. 
+00001e40: 2020 2020 2020 2020 2020 2076 6964 656f             video
+00001e50: 3d76 6964 656f 2c0d 0a20 2020 2020 2020  =video,..       
+00001e60: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
+00001e70: 703d 7265 706c 795f 6d61 726b 7570 2c0d  p=reply_markup,.
+00001e80: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00001e90: 7365 5f6d 6f64 653d 7061 7273 655f 6d6f  se_mode=parse_mo
+00001ea0: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
+00001eb0: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
+00001ec0: 655f 7072 6576 6965 773d 6469 7361 626c  e_preview=disabl
+00001ed0: 655f 7765 625f 7061 6765 5f70 7265 7669  e_web_page_previ
+00001ee0: 6577 2c0d 0a20 2020 2020 2020 2029 0d0a  ew,..        )..
+00001ef0: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00001f00: 6173 796e 6369 6f2e 736c 6565 7028 436f  asyncio.sleep(Co
+00001f10: 6e73 742e 5345 434f 4e44 535f 4245 5457  nst.SECONDS_BETW
+00001f20: 4545 4e5f 4f50 4552 4154 494f 4e29 0d0a  EEN_OPERATION)..
+00001f30: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00001f40: 7365 6c66 2e5f 6175 746f 5f63 616c 6c62  self._auto_callb
+00001f50: 6163 6b5f 616e 7377 6572 280d 0a20 2020  ack_answer(..   
+00001f60: 2020 2020 2020 2020 2062 6f74 3d73 656c           bot=sel
+00001f70: 662e 626f 742c 0d0a 2020 2020 2020 2020  f.bot,..        
+00001f80: 2020 2020 6361 6c6c 6261 636b 5f69 643d      callback_id=
+00001f90: 6361 6c6c 6261 636b 2e69 642c 0d0a 2020  callback.id,..  
+00001fa0: 2020 2020 2020 2020 2020 6175 746f 616e            autoan
+00001fb0: 7377 6572 3d61 7574 6f61 6e73 7765 722c  swer=autoanswer,
+00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+00001fd0: 7377 6572 5f74 6578 743d 616e 7377 6572  swer_text=answer
+00001fe0: 5f74 6578 742c 0d0a 2020 2020 2020 2020  _text,..        
+00001ff0: 2020 2020 616e 7377 6572 5f73 686f 775f      answer_show_
+00002000: 616c 6572 743d 616e 7377 6572 5f73 686f  alert=answer_sho
+00002010: 775f 616c 6572 740d 0a20 2020 2020 2020  w_alert..       
+00002020: 2029 0d0a 0d0a 2020 2020 2020 2020 7265   )....        re
+00002030: 7475 726e 2072 6573 756c 740d 0a         turn result..
```

### Comparing `usefulgram-0.0.0a7/usefulgram/lazy/sender.py` & `usefulgram-0.0.0a8/usefulgram/lazy/sender.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             bot: Bot,
             chat_id: int,
             text: Optional[str],
             message_thread_id: Optional[int] = None,
             photo: Optional[FSInputFile] = None,
             video: Optional[FSInputFile] = None,
             reply_markup: Optional[InlineKeyboardMarkup] = None,
-            parse_mode: Union[str, UNSET_PARSE_MODE] = UNSET_PARSE_MODE,
+            parse_mode: Union[str] = UNSET_PARSE_MODE,
             disable_web_page_preview: bool = False,
     ) -> Coroutine[Any, Any, Message]:
 
         if photo is not None:
             return bot.send_photo(
                 chat_id=chat_id,
                 message_thread_id=message_thread_id,
```

### Comparing `usefulgram-0.0.0a7/usefulgram/middlewares/stacker.py` & `usefulgram-0.0.0a8/usefulgram/middlewares/stacker.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0a8/usefulgram/middlewares/trottling.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/parsing/decode.py` & `usefulgram-0.0.0a8/usefulgram/parsing/decode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/usefulgram/parsing/encode.py` & `usefulgram-0.0.0a8/usefulgram/parsing/encode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a7/PKG-INFO` & `usefulgram-0.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulgram
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: Like aiogram but more easy
 Home-page: https://github.com/Sethis/usefulgram
 License: MIT
 Author: Alexandr Bortnik
 Author-email: sambonsttt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

