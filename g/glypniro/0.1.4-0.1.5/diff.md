# Comparing `tmp/glypniro-0.1.4.tar.gz` & `tmp/glypniro-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypniro-0.1.4.tar", max compression
+gzip compressed data, was "glypniro-0.1.5.tar", max compression
```

## Comparing `glypniro-0.1.4.tar` & `glypniro-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.4/glypniro/__init__.py
--rw-r--r--   0        0        0    14386 2023-07-27 01:40:55.473132 glypniro-0.1.4/glypniro/cli.py
--rw-r--r--   0        0        0    49506 2023-07-27 02:22:48.052311 glypniro-0.1.4/glypniro/common.py
--rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.4/glypniro/reformat.py
--rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.4/glypniro/reformat_skyline.py
--rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.4/LICENSE
--rw-r--r--   0        0        0      672 2023-07-27 02:22:54.750074 glypniro-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.4/README.md
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.5/glypniro/__init__.py
+-rw-r--r--   0        0        0    14386 2023-07-27 01:40:55.473132 glypniro-0.1.5/glypniro/cli.py
+-rw-r--r--   0        0        0    49511 2023-07-27 06:12:12.139164 glypniro-0.1.5/glypniro/common.py
+-rw-r--r--   0        0        0     6575 2023-07-27 03:38:03.430308 glypniro-0.1.5/glypniro/reformat.py
+-rw-r--r--   0        0        0     2648 2023-07-27 03:50:47.869319 glypniro-0.1.5/glypniro/reformat_skyline.py
+-rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.5/LICENSE
+-rw-r--r--   0        0        0      672 2023-07-27 06:12:21.730480 glypniro-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.5/README.md
+-rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.5/PKG-INFO
```

### Comparing `glypniro-0.1.4/glypniro/cli.py` & `glypniro-0.1.5/glypniro/cli.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.4/glypniro/common.py` & `glypniro-0.1.5/glypniro/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,15 +847,15 @@
                 not_in = pd.DataFrame(not_in, columns=["Entry", "Protein names"])
                 self.uniprot_parsed_data = pd.concat([self.uniprot_parsed_data[['Entry', 'Protein names']], not_in], ignore_index=True)
                 # print(self.uniprot_parsed_data)
         else:
             self.uniprot_parsed_data = self.uniprot_parsed_data.groupby(["Entry"]).head(1).reset_index().drop(["index"], axis=1)
 
         result_data = result_data.merge(self.uniprot_parsed_data, left_on="Protein", right_on="Entry")
-        result_data.drop("Entry", 1, inplace=True)
+        result_data.drop("Entry", axis=1, inplace=True)
 
         if self.trust_byonic:
             groups = result_data.groupby(by=["Protein", "Protein names",
                                              # "Isoform",
                                              "Position"])
         else:
             groups = result_data.groupby(by=["Protein", "Protein names",
```

### Comparing `glypniro-0.1.4/glypniro/reformat.py` & `glypniro-0.1.5/glypniro/reformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from sequal.sequence import Sequence
 from sequal.resources import proton
 import pathlib
 import click
 
 
 @click.command()
-@click.option("-b", "-byonic", type=click.Path(exists=True), help="Filepath to Byonic output xlsx file.")
-@click.option("-p", "-peakview", type=click.Path(exists=True), help="Filepath to PeakView peptide output in xlsx format")
-@click.option("-o", "-output", type=click.Path(exists=False), help="Filepath to output")
+@click.option("-b", "--byonic", type=click.Path(exists=True), help="Filepath to Byonic output xlsx file.")
+@click.option("-p", "--peakview", type=click.Path(exists=True), help="Filepath to PeakView peptide output in xlsx format")
+@click.option("-o", "--output", type=click.Path(exists=False), help="Filepath to output")
 def main(b, p, o):
     pathlib.Path(o).mkdir(parents=True, exist_ok=True)
     byonic = pd.read_excel(b, sheet_name="Spectra")
     peakview = pd.read_excel(p)
     result = []
     for i, _ in byonic.groupby(
             ["Peptide\n< ProteinMetrics Confidential >", "Glycans\nNHFAGNa", "Protein Name", "Starting\nposition",
```

### Comparing `glypniro-0.1.4/glypniro/reformat_skyline.py` & `glypniro-0.1.5/glypniro/reformat_skyline.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,50 +6,58 @@
 glycan_column = "Glycans\nNHFAGNa"
 peptide_column = "Peptide\n< ProteinMetrics Confidential >"
 scan_number_regex = re.compile(r"id=(\d+)")
 replicate_regex = re.compile(r"(\w+)(\d+)$")
 
 
 @click.command()
-@click.option("-b", "-byonic", type=click.Path(exists=True), help="Filepath to Byonic output xlsx file.")
-@click.option("-s", "-skyline", type=click.Path(exists=True), help="Filepath to Skyline peptide output in xlsx format")
-@click.option("-o", "-output", type=click.Path(exists=False), help="Filepath to output folder")
+@click.option("-b", type=click.Path(exists=True), help="Filepath to Byonic output xlsx file.")
+@click.option("-s", type=click.Path(exists=True), help="Filepath to Skyline peptide output in xlsx format")
+@click.option("-o", type=click.Path(), help="Filepath to output folder")
 def main(b, s, o):
     work = []
     df = pd.read_csv(s)
     byonic = pd.read_excel(b, sheet_name="Spectra")
     split_data = df["Peptide"].str.split("_", expand=True)
     df[peptide_column] = split_data[0]
     df[glycan_column] = split_data[1]
     df["z"] = split_data[2]
+    print(df["Glycans\nNHFAGNa"])
     byonic.drop([glycan_column, "z"], axis=1, inplace=True)
     df = df.merge(byonic, on=peptide_column)
+
     current_condition = ""
     current_replicate = ""
     # df["Replicate"] = df["Replicate"].astype(str)
     matches = df["Replicate"].str.extractall(replicate_regex).reset_index()
     # scan_number = df["Scan #"].str.extractall(scan_number_regex).reset_index()
     df["Condition id"] = matches[0]
     df["Replicate id"] = matches[1]
     df["Area"] = df["Normalized Area"]
     output_folder = o
     pathlib.Path(output_folder).mkdir(parents=True, exist_ok=True)
+
     for g, d in df.groupby(["Condition id", "Replicate id"]):
         pd_file = str(pathlib.Path(output_folder).joinpath("_".join(g) + ".txt"))
         byonic_file = str(pathlib.Path(output_folder).joinpath("_".join(g) + ".xlsx"))
         scan_pd = []
         scan_byonic = []
         for i in range(d.shape[0]):
             scan_pd.append(str(i))
             scan_byonic.append("id=" + str(i))
         with pd.ExcelWriter(byonic_file) as writer:
             d["Scan #"] = pd.Series(scan_byonic, index=d.index)
             d["First Scan"] = pd.Series(scan_pd, index=d.index)
-            d[["Protein Name", "Glycans\nNHFAGNa", "Peptide\n< ProteinMetrics Confidential >", "Score", "Scan #",
-               "Starting\nposition", "Calc.\nmass (M+H)"]].to_excel(writer, sheet_name="Spectra", index=False)
-            d[["First Scan", "Area"]].to_csv(pd_file, sep="\t", index=False)
+
+            new_df = d[["Protein Name", "Glycans\nNHFAGNa", "Peptide\n< ProteinMetrics Confidential >", "Score", "Scan #",
+               "Starting\nposition", "Calc.\nmass (M+H)"]]
+            new_df.to_excel(writer, sheet_name="Spectra", index=False)
+
+            new_df = d[["First Scan", "Area"]]
+            new_df.to_csv(pd_file, sep="\t", index=False)
+
             work.append([g[0], g[1], byonic_file, pd_file])
 
     work = pd.DataFrame(work, columns=["condition_id", "replicate_id", "filename", "area_filename"])
     with pd.ExcelWriter(str(pathlib.Path(output_folder).joinpath("work.xlsx"))) as writer:
         work.to_excel(writer, index=False)
```

### Comparing `glypniro-0.1.4/LICENSE` & `glypniro-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.4/pyproject.toml` & `glypniro-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glypniro"
-version = "0.1.4"
+version = "0.1.5"
 description = "A automated script for processing and combining Byonic and PD standard output."
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.11.1"
```

### Comparing `glypniro-0.1.4/README.md` & `glypniro-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.4/PKG-INFO` & `glypniro-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypniro
-Version: 0.1.4
+Version: 0.1.5
 Summary: A automated script for processing and combining Byonic and PD standard output.
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

