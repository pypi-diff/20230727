# Comparing `tmp/dwiqc-0.9.2-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.9.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 29603 bytes, number of entries: 25
+Zip file size: 29464 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      225 b- defN 23-Jul-05 14:23 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-27 14:42 dwiqc/__version__.py
--rw-r--r--  2.0 unx     1423 b- defN 23-Jul-27 14:16 dwiqc/browser/__init__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-27 17:51 dwiqc/__version__.py
+-rw-r--r--  2.0 unx     1352 b- defN 23-Jul-27 17:50 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 23-Jul-25 18:43 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6998 b- defN 23-Jul-24 15:35 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     3920 b- defN 23-Jul-27 14:41 dwiqc/cli/install_containers.py
--rw-r--r--  2.0 unx     6955 b- defN 23-Jul-25 18:43 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     3967 b- defN 23-Jul-27 17:50 dwiqc/cli/install_containers.py
+-rw-r--r--  2.0 unx     6788 b- defN 23-Jul-27 14:53 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     4237 b- defN 23-Jul-24 15:35 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      383 b- defN 23-Jul-13 14:56 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jul-05 14:23 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx     1029 b- defN 23-Jul-13 14:57 dwiqc/config/prequal.yaml
 -rw-r--r--  2.0 unx      634 b- defN 23-Jul-13 14:58 dwiqc/config/qsiprep.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jul-05 14:23 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jul-05 14:23 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    15862 b- defN 23-Jul-18 18:16 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4656 b- defN 23-Jul-05 14:23 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     8449 b- defN 23-Jul-20 14:45 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jul-05 14:23 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13087 b- defN 23-Jul-24 16:31 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     7186 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      460 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1969 b- defN 23-Jul-27 14:43 dwiqc-0.9.2.dist-info/RECORD
-25 files, 85607 bytes uncompressed, 26461 bytes compressed:  69.1%
+-rwxr-xr-x  2.0 unx     7186 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      460 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1969 b- defN 23-Jul-27 17:51 dwiqc-0.9.3.dist-info/RECORD
+25 files, 85416 bytes uncompressed, 26322 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -51,26 +51,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.9.2.data/scripts/dwiQC.py
+Filename: dwiqc-0.9.3.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.9.2.dist-info/LICENSE
+Filename: dwiqc-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.9.2.dist-info/METADATA
+Filename: dwiqc-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.9.2.dist-info/WHEEL
+Filename: dwiqc-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.9.2.dist-info/top_level.txt
+Filename: dwiqc-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.9.2.dist-info/RECORD
+Filename: dwiqc-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/browser/__init__.py

```diff
@@ -2,19 +2,18 @@
 import logging
 import subprocess
 from lxml import etree, html
 from pathlib import Path
 import mimetypes
 import os
 logger = logging.getLogger(__name__)
-home_dir = os.path.expanduser("~")
 
 
 def snapshot(url, saveto):
-	proc1 = f'{home_dir}/.config/dwiqc/containers/chromium.sif --no-sandbox --headless --print-to-pdf={saveto} {url}'
+	proc1 = f'chromium.sif --no-sandbox --headless --print-to-pdf={saveto} {url}'
 	output = subprocess.Popen(proc1, shell=True, stderr=subprocess.PIPE)
 	output.communicate()
 
 def imbed_images(infile, outfile=None):
     infile = Path(infile)
     if not outfile:
         outfile = infile.with_stem(f'{infile.stem}-imbedded_images')
```

## dwiqc/cli/install_containers.py

```diff
@@ -30,14 +30,16 @@
 
 symlink_location = os.path.join(home_dir, '.config/dwiqc/containers/')
 
 def do(args):
 
 	os.makedirs(args.install_location, exist_ok=True)
 
+	os.makedirs(symlink_location, exist_ok=True)
+
 	check_storage(args.install_location)
 
 	logger.info('installing chromium...')
 
 	### check if chromium already there
 
 	if os.path.isfile(f"{args.install_location}/chromium.sif"):
```

## dwiqc/cli/process.py

```diff
@@ -16,18 +16,14 @@
 from bids import BIDSLayout
 from dwiqc.xnat import Report
 import dwiqc.tasks.prequal as prequal
 import dwiqc.tasks.qsiprep as qsiprep
 import dwiqc.tasks.prequal_EQ as prequal_EQ
 import dwiqc.tasks.qsiprep_EQ as qsiprep_EQ
 import dwiqc.browser as browser
-sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
-from env_modules_python import module
-
-module('load', 'chromium.org/chromium/102.0.5005.115-ncf')
 
 
 logger = logging.getLogger(__name__)
 
 def do(args):
     if args.insecure:
         logger.warning('disabling ssl certificate verification')
@@ -68,15 +64,15 @@
         logger.error("No PA field map data found. Double check bids directory to verify. Exiting.")
         sys.exit()
 
     json_file = os.path.basename(layout.get(subject=args.sub, extension='.json', suffix='dwi', run=args.run, return_type='filename').pop())
 
     basename = os.path.splitext(json_file)[0]
    
-    #logger.debug('DWI raw: %s', raw)
+    logger.debug('DWI raw: %s', raw)
 
     os.system('mkdir -p $TMPDIR')
 
 
     # prequal job
     prequal_outdir = None
     if 'prequal' in args.sub_tasks:
```

## Comparing `dwiqc-0.9.2.data/scripts/dwiQC.py` & `dwiqc-0.9.3.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.9.2.dist-info/LICENSE` & `dwiqc-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.9.2.dist-info/RECORD` & `dwiqc-0.9.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=da-FBC_xqyFP9W4XmGavJfNav07fNpk1rtF4fXCw_6o,247
-dwiqc/browser/__init__.py,sha256=ZjDP9HeQSX3gbTqEXfhD1WPDymxZB04CbHfHviDFJmU,1423
+dwiqc/__version__.py,sha256=lHz2lconAeBkm2vIo6qFcGUS7v3iqHd7NH5EErWKJ0k,247
+dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
 dwiqc/cli/__init__.py,sha256=QD5zUAU1PHaJdE14htZyZCCUOYQ1rHHMtT2v8lBF8QE,94
 dwiqc/cli/get.py,sha256=Eu7VTB6Od_BrOMpTqS5EvFZ-NDPRsbD3FZ0-Q72E2XE,6998
-dwiqc/cli/install_containers.py,sha256=BoDgX_x_57559iLsNP6fJqR9RMqy_K9kfX_EnYXBVr4,3920
-dwiqc/cli/process.py,sha256=sKhQZp-1-aiMZpqQaDoxAStilQYPgaxc_aBuQg4mX0w,6955
+dwiqc/cli/install_containers.py,sha256=O9hPTBjnwdr1Q6wrHLNm7kPWSSoeIJBi9rMqOvpJcSA,3967
+dwiqc/cli/process.py,sha256=iNiuyklAmGNmhRZMpyi0D0KFoLgC-_yfcPUdocau-gE,6788
 dwiqc/cli/tandem.py,sha256=nn-EqvSLCy5X1Z66e1c9OZfff-ThiOOPQihl04WPXpY,4237
 dwiqc/config/__init__.py,sha256=X33iA2gj1lDc6fsIYPUcqvZUDV--IphhJY4JTNd-Yg0,383
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/config/prequal.yaml,sha256=tm6Jrb5aj7M2EqD87oXXG1VWryws44hn-uzRISeGNkM,1029
 dwiqc/config/qsiprep.yaml,sha256=QlGuIa2jAwNSWkv8CirhWVk50eRoIGVvieiUWGk9k-8,634
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=BZNfFuBglguxeYqozr-_crVTXFxeXc4I5Oms_nkZ-SA,15862
 dwiqc/tasks/prequal_EQ.py,sha256=hvs6qjRNoJXuCzdvP-9BnaZc4xwvI9LHSgmueRobt1Q,4656
 dwiqc/tasks/qsiprep.py,sha256=7rtKi6NHPN3kl2imSk12h5gW1DX0qmWVsL1ie9jkfJ4,8449
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=fjdic3dblSWMag4vOwCcgyHgD2pBcu7qICNrt7HBwVU,13087
-dwiqc-0.9.2.data/scripts/dwiQC.py,sha256=Nd-pDUAXJgqUOc7Olk6QD_u7zyxiO9gXzRzAWU1lY2c,7186
-dwiqc-0.9.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.9.2.dist-info/METADATA,sha256=18DbTYJAVBjdzEyIE72wstCs_qIyQByumlXCRTLIYf4,460
-dwiqc-0.9.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-dwiqc-0.9.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.9.2.dist-info/RECORD,,
+dwiqc-0.9.3.data/scripts/dwiQC.py,sha256=Nd-pDUAXJgqUOc7Olk6QD_u7zyxiO9gXzRzAWU1lY2c,7186
+dwiqc-0.9.3.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.9.3.dist-info/METADATA,sha256=g1lHZIKweDhGIyc15UKw_zIhDXLWYnLuNoqdMOSobp8,460
+dwiqc-0.9.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+dwiqc-0.9.3.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.9.3.dist-info/RECORD,,
```

