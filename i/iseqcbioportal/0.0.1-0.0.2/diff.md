# Comparing `tmp/iseqcbioportal-0.0.1.tar.gz` & `tmp/iseqcbioportal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iseqcbioportal-0.0.1.tar", last modified: Thu Jul 27 07:38:27 2023, max compression
+gzip compressed data, was "iseqcbioportal-0.0.2.tar", last modified: Thu Jul 27 14:31:44 2023, max compression
```

## Comparing `iseqcbioportal-0.0.1.tar` & `iseqcbioportal-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3078 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/.gitignore
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1067 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/LICENSE
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      868 2023-07-26 10:19:46.000000 iseqcbioportal-0.0.1/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/cbioportal/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/cbioportal/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1419 2023-07-25 16:07:49.000000 iseqcbioportal-0.0.1/cbioportal/create_cbioportal_database.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/cbioportal/test/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/cbioportal/test/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1034 2023-07-25 16:44:42.000000 iseqcbioportal-0.0.1/cbioportal/test/create_cbioportal_database_test.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1953 2023-07-25 16:51:36.000000 iseqcbioportal-0.0.1/cbioportal/vcf_annotate_cbioportal.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      719 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      156 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       77 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-07-27 07:38:27.000000 iseqcbioportal-0.0.1/iseqcbioportal.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      941 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       69 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 07:38:27.240926 iseqcbioportal-0.0.1/utils/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.1/utils/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2360 2023-07-25 16:06:15.000000 iseqcbioportal-0.0.1/utils/utils.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3078 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/.gitignore
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1067 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/LICENSE
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      868 2023-07-26 10:19:46.000000 iseqcbioportal-0.0.2/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/cbioportal/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/cbioportal/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1419 2023-07-27 14:30:28.000000 iseqcbioportal-0.0.2/cbioportal/create_cbioportal_database.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/cbioportal/test/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/cbioportal/test/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1034 2023-07-25 16:44:42.000000 iseqcbioportal-0.0.2/cbioportal/test/create_cbioportal_database_test.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2081 2023-07-27 14:30:48.000000 iseqcbioportal-0.0.2/cbioportal/vcf_annotate_cbioportal.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      719 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      156 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       90 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      957 2023-07-27 14:31:44.010106 iseqcbioportal-0.0.2/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       69 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/utils/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/utils/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2360 2023-07-27 14:30:10.000000 iseqcbioportal-0.0.2/utils/utils.py
```

### Comparing `iseqcbioportal-0.0.1/.gitignore` & `iseqcbioportal-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.1/LICENSE` & `iseqcbioportal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.1/PKG-INFO` & `iseqcbioportal-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqcbioportal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for creating database from cBioPortal and annotating VCF with information from this database
 Home-page: https://gitlab.com/intelliseq/iseqcbioportal
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqcbioportal-0.0.1/README.md` & `iseqcbioportal-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.1/cbioportal/create_cbioportal_database.py` & `iseqcbioportal-0.0.2/cbioportal/create_cbioportal_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from utils import utils
 from typing import List
 from typing import Dict
 from tqdm import tqdm
 
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 def create_cbioportal_database(all_studies: List[Dict]):
     engine = utils.create_sqlite_engine("cbioportal.db")
     for study in tqdm(all_studies):
         studyId = {
             "studyIds": [
```

### Comparing `iseqcbioportal-0.0.1/cbioportal/test/create_cbioportal_database_test.py` & `iseqcbioportal-0.0.2/cbioportal/test/create_cbioportal_database_test.py`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.1/cbioportal/vcf_annotate_cbioportal.py` & `iseqcbioportal-0.0.2/cbioportal/vcf_annotate_cbioportal.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import argparse
 import pandas as pd
 import sqlite3
 import pysam
 from utils import utils
 
 
+__version__ = '0.0.2'
+
+
 def annotate_vcf(record: pysam.libcbcf.VariantRecord, vcf: pysam.VariantFile, studies: list, database: sqlite3.Connection):
     gene_name = record.info.get("ISEQ_GENES_NAMES")[0]
     cases_for_gene = 0
     all_cases = 0
     for study_id in studies:
         df = pd.read_sql(f'''SELECT * FROM {study_id} 
             WHERE hugoGeneSymbol LIKE "{gene_name}"''' , database)
@@ -23,14 +26,15 @@
         record.info["ISEQ_CBIOPORTAL_FREQUENCY"] = str(frequency)
     vcf.write(record)          
 
 
 def main():
     parser = argparse.ArgumentParser(description='Annotate VCF with number of samples with one or more mutations \
                                      and percentage of samples with one or more mutations')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s {}'.format(__version__))
     parser.add_argument('--input-vcf', type=str, required=True, help='Input VCF to annotate')
     parser.add_argument('--studies', type=str, required=True, nargs='+', help='StudyIds')
     parser.add_argument('--output-vcf', type=str, required=True, help='Output annotated VCF')
     args = parser.parse_args()
 
     # connect to database
     database = utils.connect_to_database("cbioportal.db")
```

### Comparing `iseqcbioportal-0.0.1/iseqcbioportal.egg-info/PKG-INFO` & `iseqcbioportal-0.0.2/iseqcbioportal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqcbioportal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for creating database from cBioPortal and annotating VCF with information from this database
 Home-page: https://gitlab.com/intelliseq/iseqcbioportal
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqcbioportal-0.0.1/iseqcbioportal.egg-info/SOURCES.txt` & `iseqcbioportal-0.0.2/iseqcbioportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.1/setup.cfg` & `iseqcbioportal-0.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iseqcbioportal
-version = 0.0.1
+version = 0.0.2
 author = Mateusz Marynowski
 author_email = mateusz.marynowski@intelliseq.pl
 description = Package for creating database from cBioPortal and annotating VCF with information from this database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/intelliseq/iseqcbioportal
 classifiers = 
@@ -19,14 +19,15 @@
 python_requires = >=3.6
 install_requires = 
 	pandas >= 1.4.2
 	requests >= 2.28.1
 	SQLAlchemy >= 1.4.0
 	loguru >= 0.6.0
 	pysam >= 0.21.0
+	tqdm >= 4.64.1
 
 [options.packages.find]
 where = .
 
 [options.entry_points]
 console_scripts = 
 	create_cbioportal_database = cbioportal.create_cbioportal_database:main
```

### Comparing `iseqcbioportal-0.0.1/utils/utils.py` & `iseqcbioportal-0.0.2/utils/utils.py`

 * *Files identical despite different names*

