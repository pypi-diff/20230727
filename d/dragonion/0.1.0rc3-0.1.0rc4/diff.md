# Comparing `tmp/dragonion-0.1.0rc3-py3-none-any.whl.zip` & `tmp/dragonion-0.1.0rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37006 bytes, number of entries: 69
+Zip file size: 37008 bytes, number of entries: 69
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 dragonion/__init__.py
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 dragonion/__main__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dragonion/modules/cli/__init__.py
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 dragonion/modules/cli/main.py
 -rw-r--r--  2.0 unx       21 b- defN 80-Jan-01 00:00 dragonion/modules/tui/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/authentication/__init__.py
@@ -60,12 +60,12 @@
 -rw-r--r--  2.0 unx     2805 b- defN 80-Jan-01 00:00 dragonion/utils/core/dirs.py
 -rw-r--r--  2.0 unx      699 b- defN 80-Jan-01 00:00 dragonion/utils/core/emoji.py
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 dragonion/utils/onion/__init__.py
 -rw-r--r--  2.0 unx     1110 b- defN 80-Jan-01 00:00 dragonion/utils/onion/auth.py
 -rw-r--r--  2.0 unx     6796 b- defN 80-Jan-01 00:00 dragonion/utils/onion/onion.py
 -rw-r--r--  2.0 unx    10968 b- defN 80-Jan-01 00:00 dragonion/utils/onion/stem_process.py
 -rw-r--r--  2.0 unx     2365 b- defN 80-Jan-01 00:00 dragonion/utils/onion/tor_downloader.py
--rw-r--r--  2.0 unx     1631 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     7267 b- defN 16-Jan-01 00:00 dragonion-0.1.0rc3.dist-info/RECORD
-69 files, 71267 bytes uncompressed, 24760 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1631 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     7267 b- defN 16-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/RECORD
+69 files, 71267 bytes uncompressed, 24762 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -189,20 +189,20 @@
 
 Filename: dragonion/utils/onion/stem_process.py
 Comment: 
 
 Filename: dragonion/utils/onion/tor_downloader.py
 Comment: 
 
-Filename: dragonion-0.1.0rc3.dist-info/METADATA
+Filename: dragonion-0.1.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: dragonion-0.1.0rc3.dist-info/WHEEL
+Filename: dragonion-0.1.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: dragonion-0.1.0rc3.dist-info/entry_points.txt
+Filename: dragonion-0.1.0rc4.dist-info/entry_points.txt
 Comment: 
 
-Filename: dragonion-0.1.0rc3.dist-info/RECORD
+Filename: dragonion-0.1.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dragonion/utils/onion/auth.py

```diff
@@ -23,8 +23,8 @@
         return auth['host']
     elif auth_strings[0] and auth_strings[1]:
         with open(os.path.join(os.path.join(tor_data_directory_name, 'auth'),
                                'service.auth_private'), 'w') as f:
             f.write(f'{auth_strings[0]}:descriptor:'
                     f'x25519:{auth_strings[1]}')
 
-        return f'{auth_strings[1]}.onion'
+        return f'{auth_strings[0]}.onion'
```

## Comparing `dragonion-0.1.0rc3.dist-info/METADATA` & `dragonion-0.1.0rc4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonion
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: 
 Author: BarsTiger
 Author-email: zxcbarstiger@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `dragonion-0.1.0rc3.dist-info/RECORD` & `dragonion-0.1.0rc4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 dragonion/modules/tui/tui.py,sha256=rq0rJyHjxEQiSIxzG0LvJx-Jzlnx7zDoPVBg01bR3KI,2467
 dragonion/utils/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/utils/core/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/utils/core/const.py,sha256=OQT-J_OIgTZktbrjYk01HWn2ZRLzQzj0nodZObGTjuM,83
 dragonion/utils/core/dirs.py,sha256=M_7bjY6_Em8ICbfcNc-AZPhIz4s2t6KLBvBeURIz3wY,2805
 dragonion/utils/core/emoji.py,sha256=ojZx_hL50wBlpq6Zip-Y23c_q-ljrQKXtmscK4jyoY8,699
 dragonion/utils/onion/__init__.py,sha256=gQajsInd9Xh0QMplPYSpOVDs7f3HAajOqF2G1pg6TfQ,52
-dragonion/utils/onion/auth.py,sha256=OvEcCybb7hxikvkt7OgZSn1iG6RKx2cAWaiRFMRHi28,1110
+dragonion/utils/onion/auth.py,sha256=2762A-N1elA0G-JTxkknEwkmWY2UvGX7bGGRrxEheEw,1110
 dragonion/utils/onion/onion.py,sha256=OifJcBEZHZYmuWNw4Clu1qct2VTE471wnLzD9Jdc4Po,6796
 dragonion/utils/onion/stem_process.py,sha256=0QB6ErA1pO4I1aIPkyoRDqpTjcZQkCjHjbsao-cX7JY,10968
 dragonion/utils/onion/tor_downloader.py,sha256=XXJepwjwPvrwxvTA4dIPmmqYQLXaIk6SCs7po5ikpHA,2365
-dragonion-0.1.0rc3.dist-info/METADATA,sha256=ohf7ML0yvJ49lUCZ-1wkAEgFITStG-0SWsttBGlaZYo,1631
-dragonion-0.1.0rc3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-dragonion-0.1.0rc3.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
-dragonion-0.1.0rc3.dist-info/RECORD,,
+dragonion-0.1.0rc4.dist-info/METADATA,sha256=4mjzknXSJY55DHa_N3pyX1QYA6azkUao1J9UC-JedeE,1631
+dragonion-0.1.0rc4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+dragonion-0.1.0rc4.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
+dragonion-0.1.0rc4.dist-info/RECORD,,
```

