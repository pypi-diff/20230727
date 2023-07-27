# Comparing `tmp/lkfmt-0.2.1-py3-none-any.whl.zip` & `tmp/lkfmt-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7289 bytes, number of entries: 9
+Zip file size: 7318 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 lkfmt/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 80-Jan-01 00:00 lkfmt/__main__.py
 -rw-r--r--  2.0 unx     5807 b- defN 80-Jan-01 00:00 lkfmt/diff.py
--rw-r--r--  2.0 unx     6219 b- defN 80-Jan-01 00:00 lkfmt/formatter.py
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2075 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      670 b- defN 16-Jan-01 00:00 lkfmt-0.2.1.dist-info/RECORD
-9 files, 16805 bytes uncompressed, 6149 bytes compressed:  63.4%
+-rw-r--r--  2.0 unx     6389 b- defN 80-Jan-01 00:00 lkfmt/formatter.py
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 lkfmt-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2075 b- defN 80-Jan-01 00:00 lkfmt-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lkfmt-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 lkfmt-0.2.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      670 b- defN 16-Jan-01 00:00 lkfmt-0.2.2.dist-info/RECORD
+9 files, 16975 bytes uncompressed, 6178 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: lkfmt/diff.py
 Comment: 
 
 Filename: lkfmt/formatter.py
 Comment: 
 
-Filename: lkfmt-0.2.1.dist-info/LICENSE
+Filename: lkfmt-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: lkfmt-0.2.1.dist-info/METADATA
+Filename: lkfmt-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: lkfmt-0.2.1.dist-info/WHEEL
+Filename: lkfmt-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: lkfmt-0.2.1.dist-info/entry_points.txt
+Filename: lkfmt-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: lkfmt-0.2.1.dist-info/RECORD
+Filename: lkfmt-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lkfmt/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .diff import show_diff
 from .diff import stat_changes
 from .formatter import fmt_all
 from .formatter import fmt_one
 from .formatter import fmt_one as fmt_file
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

## lkfmt/formatter.py

```diff
@@ -160,41 +160,46 @@
     assert file.endswith(('.py', '.txt'))
     if chdir:
         os.chdir(os.path.dirname(os.path.abspath(file)))
 
     with open(file, 'r', encoding='utf-8') as f:
         code = origin_code = f.read()
 
+    if not fs.filename(file) == '__init__.py':
+        code = autoflake.fix_code(
+            code,
+            ignore_init_module_imports=True,
+            ignore_pass_after_docstring=False,
+            ignore_pass_statements=False,
+            remove_all_unused_imports=True,
+        )
     code = black.format_str(
         code,
         mode=black.Mode(
             line_length=80,
-            string_normalization=False,
-            magic_trailing_comma=False,
+            # magic_trailing_comma=False,
+            magic_trailing_comma=True,
             preview=True,
+            string_normalization=False,
         ),
     )
     code = isort.code(
         code,
         config=isort.Config(
             case_sensitive=True,
             force_single_line=True,
+            honor_noqa=True,
             line_length=80,
+            lines_after_imports=-1,
+            lines_between_sections=1,
             only_modified=True,
             profile='black',
+            reverse_relative=True,
         ),
     )
-    if not fs.filename(file) == '__init__.py':
-        # we don't strip any import in `__init__.py`.
-        code = autoflake.fix_code(
-            code,
-            remove_all_unused_imports=True,
-            ignore_pass_statements=False,
-            ignore_pass_after_docstring=False,
-        )
 
     if code == origin_code:
         print('[green dim]no code change[/]', ':rt')
         return code, (0, 0, 0)
 
     if inplace:
         with open(file, 'w', encoding='utf-8') as f:
```

## Comparing `lkfmt-0.2.1.dist-info/LICENSE` & `lkfmt-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lkfmt-0.2.1.dist-info/METADATA` & `lkfmt-0.2.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkfmt
-Version: 0.2.1
+Version: 0.2.2
 Summary: All-in-one Python code formattor which is tailored of `black` + `isort` + `autoflake` for myself taste.
 Home-page: https://github.com/likianta/lkfmt
 License: MIT
 Author: likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lkfmt-0.2.1.dist-info/RECORD` & `lkfmt-0.2.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-lkfmt/__init__.py,sha256=dxyryd7vVblPXpZHpWrIBILfo4iH7_Fy3l6to6pvvI0,187
+lkfmt/__init__.py,sha256=3NupqEqn4Oxwwugppn943SBnB4_8g5YdeVMTCc84i_Y,187
 lkfmt/__main__.py,sha256=xpk_lSdRLk0UEuDQZSJyN76Niobvog1w8AB_0cop238,641
 lkfmt/diff.py,sha256=AvCNkz2sUaS99SlyiW9zd4ILxxIF-j_8uAZnlY0P8U8,5807
-lkfmt/formatter.py,sha256=fFI8hSyk-9QlkNlB-lEVCqxq0tyLo-BZNnbtIhyN8ng,6219
-lkfmt-0.2.1.dist-info/LICENSE,sha256=bO1rHKUWDbdeAwBtNXIDn9xUV35nu8Wo_v29KNXwm2I,1068
-lkfmt-0.2.1.dist-info/METADATA,sha256=ZSVwTFUSP1Gru5HDqcaGZb5QRYnVwoIlET7_R1bQF-g,2075
-lkfmt-0.2.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-lkfmt-0.2.1.dist-info/entry_points.txt,sha256=q_mrR6vJjVomeNzdN7IwzqD4hJCmKpY0z68XPRVH2_A,50
-lkfmt-0.2.1.dist-info/RECORD,,
+lkfmt/formatter.py,sha256=2RrJ833Re4tFJB-lZZuzLAIKkiKEIlt-8oQg_jzXVPY,6389
+lkfmt-0.2.2.dist-info/LICENSE,sha256=bO1rHKUWDbdeAwBtNXIDn9xUV35nu8Wo_v29KNXwm2I,1068
+lkfmt-0.2.2.dist-info/METADATA,sha256=yz4AbRe-Xco-PlWxO974OVgmV1q8YQATA7NtbZrfVO4,2075
+lkfmt-0.2.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+lkfmt-0.2.2.dist-info/entry_points.txt,sha256=q_mrR6vJjVomeNzdN7IwzqD4hJCmKpY0z68XPRVH2_A,50
+lkfmt-0.2.2.dist-info/RECORD,,
```

