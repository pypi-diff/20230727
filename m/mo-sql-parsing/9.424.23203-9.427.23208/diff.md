# Comparing `tmp/mo_sql_parsing-9.424.23203-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.427.23208-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38347 bytes, number of entries: 13
+Zip file size: 38408 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-18 01:32 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22382 b- defN 23-Jul-18 01:32 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10695 b- defN 23-Jul-18 01:32 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    34100 b- defN 23-Jul-22 13:56 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    34229 b- defN 23-Jul-27 21:40 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7357 b- defN 23-Jul-22 13:56 mo_sql_parsing/types.py
--rw-rw-rw-  2.0 fat    22995 b- defN 23-Jul-18 01:32 mo_sql_parsing/utils.py
+-rw-rw-rw-  2.0 fat    23118 b- defN 23-Jul-27 21:40 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2920 b- defN 23-Jul-18 01:32 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/RECORD
-13 files, 129507 bytes uncompressed, 36441 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/RECORD
+13 files, 129759 bytes uncompressed, 36502 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/LICENSE
+Filename: mo_sql_parsing-9.427.23208.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/METADATA
+Filename: mo_sql_parsing-9.427.23208.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/WHEEL
+Filename: mo_sql_parsing-9.427.23208.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.427.23208.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/zip-safe
+Filename: mo_sql_parsing-9.427.23208.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.424.23203.dist-info/RECORD
+Filename: mo_sql_parsing-9.427.23208.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -549,15 +549,15 @@
         #####################################################################
         # DML STATEMENTS
         #####################################################################
 
         # MySQL's index_type := Using + ( "BTREE" | "HASH" )
         index_type = Optional(assign("using", ident("index_type")))
 
-        index_column_names = LB + delimited_list(identifier("columns")) + RB
+        index_column_names = LB + delimited_list((identifier("value") + Optional(LB + int_num("length") + RB)) / to_index_part)("columns") + RB
 
         column_def_delete = assign("on delete", (keyword("cascade") | keyword("set null") | keyword("set default")),)
 
         table_def_foreign_key = FOREIGN_KEY + Optional(
             Optional(identifier("index_name"))
             + index_column_names
             + column_def_references
@@ -603,15 +603,19 @@
             )
             + Optional(AS.suppress() + infix_notation(query, [])("query"))
         )("create table")
 
         create_view = (
             keyword("create")
             + Optional(keyword("or") + flag("replace"))
-            + Optional(keyword("algorithm").suppress() + EQ + (keyword("merge") | keyword("temptable") | keyword("undefined"))("algorithm"))
+            + Optional(
+                keyword("algorithm").suppress()
+                + EQ
+                + (keyword("merge") | keyword("temptable") | keyword("undefined"))("algorithm")
+            )
             + temporary
             + VIEW.suppress()
             + Optional((keyword("if not exists") / False)("replace"))
             + identifier("name")
             + AS
             + query("query")
         )("create view")
```

## mo_sql_parsing/utils.py

```diff
@@ -307,14 +307,21 @@
 def to_trim_call(tokens):
     frum = tokens["from"]
     if not frum:
         return Call("trim", [tokens["chars"]], {"direction": tokens["direction"]})
     return Call("trim", [frum], {"characters": tokens["chars"], "direction": tokens["direction"]},)
 
 
+def to_index_part(tokens):
+    value = dict(tokens)
+    if len(value)==1:
+        return value['value']
+    return value
+
+
 def to_kwarg(tokens):
     return {k: v for k, v in [tuple(tokens)]}
 
 
 def to_literal(t):
     return {"literal": unliteral_field(t[0])}
```

## Comparing `mo_sql_parsing-9.424.23203.dist-info/LICENSE` & `mo_sql_parsing-9.427.23208.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.424.23203.dist-info/METADATA` & `mo_sql_parsing-9.427.23208.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.424.23203
+Version: 9.427.23208
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_sql_parsing-9.424.23203.dist-info/RECORD` & `mo_sql_parsing-9.427.23208.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=ZbsunSI2YPlPkveviGXQuv_YjCmofsrVOOu6qb500gM,2530
 mo_sql_parsing/formatting.py,sha256=Nzcrs6aWLQRK0hd8QvyPZ4hMF1onIhyvE2iBrtKF-Fw,22382
 mo_sql_parsing/keywords.py,sha256=nFTOQv7VOTDI4Ud3oSJh0-II9FGH4wWXmFRwZ5R3uzk,10695
-mo_sql_parsing/sql_parser.py,sha256=GY36sWfWai9Qg-s2D2GRQ668kDHlrP135Of-3TFNAAk,34100
+mo_sql_parsing/sql_parser.py,sha256=S6oZUKwMvYp8LTwFp4mYnK_0g4aAa1ySg5Kb8WeTRG8,34229
 mo_sql_parsing/types.py,sha256=tloEMsDgghBPm9O9MjyMLj8lUJ2ALTMdPEv3hU841HY,7357
-mo_sql_parsing/utils.py,sha256=au9Z9qebVGYikMj7sae1m7-cs1PRRNem80HVxmW6h30,22995
+mo_sql_parsing/utils.py,sha256=r5EAEgGlIINl3UPN18Hk7LS4pQzeA_GLytRP-CI79aE,23118
 mo_sql_parsing/windows.py,sha256=KelC9CZopR53tb0xAPxWsbxt59ieR_kNmM37FFcMjzE,2920
-mo_sql_parsing-9.424.23203.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.424.23203.dist-info/METADATA,sha256=F9oNO3-S39xqr_gUShAsA3yghsWMMuxSf5TT7pKsmTA,9345
-mo_sql_parsing-9.424.23203.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.424.23203.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.424.23203.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.424.23203.dist-info/RECORD,,
+mo_sql_parsing-9.427.23208.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.427.23208.dist-info/METADATA,sha256=legbgdTQiK0Ar9zieB3Br7cBPpxiie9APN-TH9hahzQ,9345
+mo_sql_parsing-9.427.23208.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.427.23208.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.427.23208.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.427.23208.dist-info/RECORD,,
```

