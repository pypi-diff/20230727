# Comparing `tmp/bioat-0.2.4.tar.gz` & `tmp/bioat-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.2.4.tar", max compression
+gzip compressed data, was "bioat-0.2.5.tar", max compression
```

## Comparing `bioat-0.2.4.tar` & `bioat-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,39 @@
--rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.2.4/LICENSE
--rw-r--r--   0        0        0      915 2023-05-26 06:22:16.000000 bioat-0.2.4/README.md
--rw-r--r--   0        0        0     1115 2023-07-14 11:21:41.646684 bioat-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      637 2023-06-23 18:19:23.000000 bioat-0.2.4/src/bioat/__init__.py
--rw-r--r--   0        0        0      451 2023-06-17 10:35:36.000000 bioat-0.2.4/src/bioat/__main__.py
--rw-r--r--   0        0        0      508 2023-05-26 06:02:39.000000 bioat-0.2.4/src/bioat/about.py
--rw-r--r--   0        0        0    13916 2023-06-17 12:05:22.000000 bioat-0.2.4/src/bioat/bamtools.py
--rw-r--r--   0        0        0      738 2023-06-17 09:21:50.000000 bioat-0.2.4/src/bioat/bedtools.py
--rw-r--r--   0        0        0     1833 2023-06-17 10:35:16.000000 bioat-0.2.4/src/bioat/cli.py
--rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.000000 bioat-0.2.4/src/bioat/detect_seq.py
--rw-r--r--   0        0        0      151 2023-06-23 18:19:23.000000 bioat-0.2.4/src/bioat/exceptions.py
--rw-r--r--   0        0        0    11024 2023-05-26 05:45:47.000000 bioat-0.2.4/src/bioat/fastxtools.py
--rw-r--r--   0        0        0      818 2023-03-13 04:16:15.000000 bioat-0.2.4/src/bioat/genome.py
--rw-r--r--   0        0        0     5940 2023-06-17 09:21:44.000000 bioat-0.2.4/src/bioat/hictools.py
--rw-r--r--   0        0        0        0 2023-04-01 12:21:31.000000 bioat-0.2.4/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0      158 2023-04-01 13:17:43.000000 bioat-0.2.4/src/bioat/lib/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1139 2023-04-08 13:50:28.000000 bioat-0.2.4/src/bioat/lib/__pycache__/_dev_tools.cpython-310.pyc
--rw-r--r--   0        0        0     4141 2023-04-13 16:28:19.000000 bioat-0.2.4/src/bioat/lib/__pycache__/libalignment.cpython-310.pyc
--rw-r--r--   0        0        0    60057 2023-05-11 15:11:40.000000 bioat-0.2.4/src/bioat/lib/__pycache__/libcircos.cpython-310.pyc
--rw-r--r--   0        0        0     4482 2023-07-14 09:34:57.159756 bioat-0.2.4/src/bioat/lib/__pycache__/libcolor.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-06-17 09:18:10.000000 bioat-0.2.4/src/bioat/lib/__pycache__/libcrispr.cpython-310.pyc
--rw-r--r--   0        0        0     1436 2023-05-26 06:06:23.000000 bioat-0.2.4/src/bioat/lib/__pycache__/libdataclasses.cpython-310.pyc
--rw-r--r--   0        0        0     7907 2023-04-13 16:44:42.000000 bioat-0.2.4/src/bioat/lib/__pycache__/libplot.cpython-310.pyc
--rw-r--r--   0        0        0      854 2023-04-08 13:49:32.000000 bioat-0.2.4/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     9873 2023-07-14 10:59:33.355659 bioat-0.2.4/src/bioat/lib/circos/example_data_barplot.csv
--rw-r--r--   0        0        0    30782 2023-07-14 10:59:33.354431 bioat-0.2.4/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
--rw-r--r--   0        0        0      427 2023-07-14 10:59:33.353754 bioat-0.2.4/src/bioat/lib/circos/example_data_chromosome_general.csv
--rw-r--r--   0        0        0     5143 2023-07-14 10:59:33.353243 bioat-0.2.4/src/bioat/lib/circos/example_data_links.csv
--rw-r--r--   0        0        0     9856 2023-07-14 10:59:33.356255 bioat-0.2.4/src/bioat/lib/circos/example_data_point.csv
--rw-r--r--   0        0        0     9107 2023-07-14 10:59:33.351197 bioat-0.2.4/src/bioat/lib/circos/example_data_rect_gradual.csv
--rw-r--r--   0        0        0      450 2023-07-14 10:59:33.355004 bioat-0.2.4/src/bioat/lib/circos/hg38/chromosome_length_hg38.csv
--rw-r--r--   0        0        0    31637 2023-07-14 10:59:33.351929 bioat-0.2.4/src/bioat/lib/circos/hg38/cytoBand_hg38.csv
--rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.2.4/src/bioat/lib/libalignment.py
--rw-r--r--   0        0        0    77331 2023-07-14 11:21:27.429046 bioat-0.2.4/src/bioat/lib/libcircos.py
--rw-r--r--   0        0        0     4460 2023-07-14 09:37:59.766340 bioat-0.2.4/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     6571 2023-06-17 09:16:08.000000 bioat-0.2.4/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0      793 2023-05-26 06:06:17.000000 bioat-0.2.4/src/bioat/lib/libdataclasses.py
--rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.000000 bioat-0.2.4/src/bioat/lib/libdetect_seq.py
--rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.000000 bioat-0.2.4/src/bioat/lib/libplot.py
--rw-r--r--   0        0        0      509 2023-05-11 14:37:34.000000 bioat-0.2.4/src/bioat/lib/libsnakemake.py
--rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.000000 bioat-0.2.4/src/bioat/logger.py
--rw-r--r--   0        0        0      717 2023-06-17 09:22:39.000000 bioat-0.2.4/src/bioat/mgitools.py
--rw-r--r--   0        0        0     5748 2023-05-26 05:47:35.000000 bioat-0.2.4/src/bioat/systemtools.py
--rw-r--r--   0        0        0     3280 2023-06-17 09:26:06.000000 bioat-0.2.4/src/bioat/tabletools.py
--rw-r--r--   0        0        0    81594 2023-06-23 18:19:23.000000 bioat-0.2.4/src/bioat/target_seq.py
--rw-r--r--   0        0        0      519 2023-07-14 11:21:36.653744 bioat-0.2.4/src/bioat/version.py
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 bioat-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.2.5/LICENSE
+-rw-r--r--   0        0        0      915 2023-05-26 06:22:16.476980 bioat-0.2.5/README.md
+-rw-r--r--   0        0        0     1115 2023-07-27 07:43:33.110979 bioat-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      637 2023-06-23 18:19:23.000000 bioat-0.2.5/src/bioat/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-17 10:35:36.080629 bioat-0.2.5/src/bioat/__main__.py
+-rw-r--r--   0        0        0      508 2023-05-26 06:02:39.222570 bioat-0.2.5/src/bioat/about.py
+-rw-r--r--   0        0        0    13916 2023-06-17 12:05:22.520338 bioat-0.2.5/src/bioat/bamtools.py
+-rw-r--r--   0        0        0      738 2023-06-17 09:21:50.061008 bioat-0.2.5/src/bioat/bedtools.py
+-rw-r--r--   0        0        0     1833 2023-06-17 10:35:16.669568 bioat-0.2.5/src/bioat/cli.py
+-rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.2.5/src/bioat/detect_seq.py
+-rw-r--r--   0        0        0      151 2023-06-23 18:19:23.000000 bioat-0.2.5/src/bioat/exceptions.py
+-rw-r--r--   0        0        0    11024 2023-05-26 05:45:47.350133 bioat-0.2.5/src/bioat/fastxtools.py
+-rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.2.5/src/bioat/genome.py
+-rw-r--r--   0        0        0     5940 2023-06-17 09:21:44.490936 bioat-0.2.5/src/bioat/hictools.py
+-rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.2.5/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.2.5/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     9873 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_barplot.csv
+-rw-r--r--   0        0        0    30782 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
+-rw-r--r--   0        0        0      427 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_chromosome_general.csv
+-rw-r--r--   0        0        0     5143 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_links.csv
+-rw-r--r--   0        0        0     9856 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_point.csv
+-rw-r--r--   0        0        0     9107 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/example_data_rect_gradual.csv
+-rw-r--r--   0        0        0      450 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/hg38/chromosome_length_hg38.csv
+-rw-r--r--   0        0        0    31637 2023-05-11 14:17:36.000000 bioat-0.2.5/src/bioat/lib/circos/hg38/cytoBand_hg38.csv
+-rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.2.5/src/bioat/lib/libalignment.py
+-rw-r--r--   0        0        0    77322 2023-07-27 07:39:03.827893 bioat-0.2.5/src/bioat/lib/libcircos.py
+-rw-r--r--   0        0        0     4460 2023-07-14 09:35:07.000000 bioat-0.2.5/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     6571 2023-06-17 09:16:08.912240 bioat-0.2.5/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0      787 2023-07-07 13:34:23.740347 bioat-0.2.5/src/bioat/lib/libdataclasses.py
+-rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.2.5/src/bioat/lib/libdetect_seq.py
+-rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.2.5/src/bioat/lib/libplot.py
+-rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.2.5/src/bioat/lib/libsnakemake.py
+-rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.2.5/src/bioat/logger.py
+-rw-r--r--   0        0        0      717 2023-06-17 09:22:39.495970 bioat-0.2.5/src/bioat/mgitools.py
+-rw-r--r--   0        0        0     5748 2023-05-26 05:47:35.184115 bioat-0.2.5/src/bioat/systemtools.py
+-rw-r--r--   0        0        0     3280 2023-06-17 09:26:06.543411 bioat-0.2.5/src/bioat/tabletools.py
+-rw-r--r--   0        0        0    81594 2023-06-23 18:19:23.000000 bioat-0.2.5/src/bioat/target_seq.py
+-rw-r--r--   0        0        0      519 2023-07-27 07:43:25.466844 bioat-0.2.5/src/bioat/version.py
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 bioat-0.2.5/PKG-INFO
```

### Comparing `bioat-0.2.4/LICENSE` & `bioat-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/README.md` & `bioat-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/pyproject.toml` & `bioat-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioat"
-version = "0.2.4"
+version = "0.2.5"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 homepage = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 # README file(s) are used as the package description
 readme = "README.md"
```

### Comparing `bioat-0.2.4/src/bioat/__init__.py` & `bioat-0.2.5/src/bioat/__init__.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/bamtools.py` & `bioat-0.2.5/src/bioat/bamtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/bedtools.py` & `bioat-0.2.5/src/bioat/bedtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/cli.py` & `bioat-0.2.5/src/bioat/cli.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/detect_seq.py` & `bioat-0.2.5/src/bioat/detect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/fastxtools.py` & `bioat-0.2.5/src/bioat/fastxtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/genome.py` & `bioat-0.2.5/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/hictools.py` & `bioat-0.2.5/src/bioat/hictools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/_dev_tools.py` & `bioat-0.2.5/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/example_data_barplot.csv` & `bioat-0.2.5/src/bioat/lib/circos/example_data_barplot.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/example_data_chromosome_cytoband.csv` & `bioat-0.2.5/src/bioat/lib/circos/example_data_chromosome_cytoband.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/example_data_links.csv` & `bioat-0.2.5/src/bioat/lib/circos/example_data_links.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/example_data_point.csv` & `bioat-0.2.5/src/bioat/lib/circos/example_data_point.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/example_data_rect_gradual.csv` & `bioat-0.2.5/src/bioat/lib/circos/example_data_rect_gradual.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/circos/hg38/cytoBand_hg38.csv` & `bioat-0.2.5/src/bioat/lib/circos/hg38/cytoBand_hg38.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/libalignment.py` & `bioat-0.2.5/src/bioat/lib/libalignment.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/libcircos.py` & `bioat-0.2.5/src/bioat/lib/libcircos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1772,15 +1772,15 @@
         self._garc_dict[tarc_id]._plot_highlight(self.ax, highlight_dict=highlight_dict)
 
 
 def table_hg38_chromosome_length():
     return pd.read_csv(os.path.join(DATAPATH, 'chromosome_length_hg38.csv'))
 
 def table_hg38_cytoband():
-    return pd.read_csv(os.path.join(DATAPATH, 'chromosome_length_hg38.csv'))
+    return pd.read_csv(os.path.join(DATAPATH, 'cytoBand_hg38.csv'))
 
 
 if __name__ == "__main__":
     pass
     """
     tree = next(Phylo.parse("../tutorial/circos/hmptree.xml", "phyloxml")) 
     col_positions = get_col_positions(tree)
```

### Comparing `bioat-0.2.4/src/bioat/lib/libcolor.py` & `bioat-0.2.5/src/bioat/lib/libcolor.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/libcrispr.py` & `bioat-0.2.5/src/bioat/lib/libcrispr.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/libdataclasses.py` & `bioat-0.2.5/src/bioat/lib/libdataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @dataclasses.dataclass
 class Bed:
     chromosome: str
     start: int
     end: int
     name: str
-    score: int | str
+    score: int
     strand: str
 
 
 @dataclasses.dataclass
 class Bam:
     pass
```

### Comparing `bioat-0.2.4/src/bioat/lib/libdetect_seq.py` & `bioat-0.2.5/src/bioat/lib/libdetect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/lib/libplot.py` & `bioat-0.2.5/src/bioat/lib/libplot.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/logger.py` & `bioat-0.2.5/src/bioat/logger.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/mgitools.py` & `bioat-0.2.5/src/bioat/mgitools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/systemtools.py` & `bioat-0.2.5/src/bioat/systemtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/tabletools.py` & `bioat-0.2.5/src/bioat/tabletools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/target_seq.py` & `bioat-0.2.5/src/bioat/target_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.4/src/bioat/version.py` & `bioat-0.2.5/src/bioat/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 import bioat
 import datetime
 import os
 
 project_toml: str = os.path.join(bioat.__path__[0], 'version.py')
 sec = os.path.getmtime(project_toml)
 __upgrade_date__ = datetime.date.fromtimestamp(sec)
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 __author__ = 'Hua-nan ZHAO @ Tsinghua University'
 __email__ = 'hermanzhaozzzz@gmail.com'
 __doc_format__ = "restructuredtext"
 __doc_address__ = "https://github.com/hermanzhaozzzz/bioat/tree/master/docs"
 __repo_address__ = "https://github.com/hermanzhaozzzz/bioat"
```

### Comparing `bioat-0.2.4/PKG-INFO` & `bioat-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.2.4
+Version: 0.2.5
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
 Requires-Python: >=3.8.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

