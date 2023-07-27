# Comparing `tmp/glypniro-0.1.1.tar.gz` & `tmp/glypniro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypniro-0.1.1.tar", max compression
+gzip compressed data, was "glypniro-0.1.2.tar", max compression
```

## Comparing `glypniro-0.1.1.tar` & `glypniro-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.1/glypniro/__init__.py
--rw-r--r--   0        0        0    14001 2023-07-21 20:06:56.672928 glypniro-0.1.1/glypniro/cli.py
--rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.1/glypniro/common.py
--rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.1/glypniro/reformat.py
--rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.1/glypniro/reformat_skyline.py
--rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.1/LICENSE
--rw-r--r--   0        0        0      672 2023-07-24 23:51:48.273671 glypniro-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.1/README.md
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.2/glypniro/__init__.py
+-rw-r--r--   0        0        0    14386 2023-07-27 01:34:47.027984 glypniro-0.1.2/glypniro/cli.py
+-rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.2/glypniro/common.py
+-rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.2/glypniro/reformat.py
+-rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.2/glypniro/reformat_skyline.py
+-rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.2/LICENSE
+-rw-r--r--   0        0        0      672 2023-07-27 01:37:24.969523 glypniro-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.2/README.md
+-rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.2/PKG-INFO
```

### Comparing `glypniro-0.1.1/glypniro/cli.py` & `glypniro-0.1.2/glypniro/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
                          "unique PSM selected for calculation of the data in the final output", is_flag=True)
 @click.option("--mode", "-m", help="Select the mode of operation. 0: Byonic only, 1: PD only, 2: Byonic and PD", type=int, default=2)
 @click.option("--custom-group", "-c", help="A tabulated text file with two columns, Glycans and Labels. Glycans must be the glycans appear in the result and labels is the custome label for them", type=click.Path(exists=True))
 def main(input_file, output, score_cutoff, trust_byonic, get_uniprot, parse_uniprot, debug, mode, custom_group):
     """
     Automated workflow for processing and combining Byonic and PD output
     """
+    print(input_file, output, score_cutoff, trust_byonic, get_uniprot, parse_uniprot, debug, mode, custom_group)
     ex = GlypnirO(trust_byonic=trust_byonic, get_uniprot=get_uniprot, debug=debug,
                   parse_uniprot=parse_uniprot)
     if mode == 1:
         for i, r in ex.add_batch_component(input_file, score_cutoff):
             print(r)
         ex.process_components()
         result = ex.analyze_components(relabel=custom_group)
@@ -87,15 +88,20 @@
 
         if ex.debug:
             for u in ex.unique_dict:
                 with pd.ExcelWriter(output + "_" + u + ".xlsx") as writer:
                     df = pd.DataFrame(ex.unique_dict[u])
                     df.to_excel(writer, index=False)
     elif mode == 2:
-        data = pd.read_csv(input_file, sep="\t", encoding="utf-8")
+        if input_file.endswith(".txt") or input_file.endswith(".tsv"):
+            data = pd.read_csv(input_file, sep="\t", encoding="utf-8")
+        elif input_file.endswith(".csv"):
+            data = pd.read_csv(input_file, encoding="utf-8")
+        elif input_file.endswith(".xlsx"):
+            data = pd.read_excel(input_file)
         data, sample_info = process_tmt_pd_byonic(data)
 
         ex.uniprot_parsed_data = data[["Master Protein Accessions", "Protein Descriptions"]].rename(
             columns={"Master Protein Accessions": "Entry", "Protein Descriptions": "Protein names"})
         component = GlypnirOComponent(data, mode=mode, trust_byonic=trust_byonic)
         component.process(mode=mode, tmt_info=sample_info, protein_column="Master Protein Accessions",
                           sequence_column="Annotated Sequence", glycans_column="Glycan composition",
```

### Comparing `glypniro-0.1.1/glypniro/common.py` & `glypniro-0.1.2/glypniro/common.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.1/glypniro/reformat.py` & `glypniro-0.1.2/glypniro/reformat.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.1/glypniro/reformat_skyline.py` & `glypniro-0.1.2/glypniro/reformat_skyline.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.1/LICENSE` & `glypniro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.1/pyproject.toml` & `glypniro-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glypniro"
-version = "0.1.1"
+version = "0.1.2"
 description = "A automated script for processing and combining Byonic and PD standard output."
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.11.1"
```

### Comparing `glypniro-0.1.1/README.md` & `glypniro-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.1/PKG-INFO` & `glypniro-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypniro
-Version: 0.1.1
+Version: 0.1.2
 Summary: A automated script for processing and combining Byonic and PD standard output.
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

